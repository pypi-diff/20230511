# Comparing `tmp/deltadask-0.1.0.tar.gz` & `tmp/deltadask-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltadask-0.1.0.tar", max compression
+gzip compressed data, was "deltadask-0.2.0.tar", max compression
```

## Comparing `deltadask-0.1.0.tar` & `deltadask-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     2682 2022-11-24 16:35:47.147019 deltadask-0.1.0/README.md
--rw-r--r--   0        0        0      592 2022-11-24 16:35:47.147276 deltadask-0.1.0/deltadask/__init__.py
--rw-r--r--   0        0        0      410 2022-11-24 16:35:47.151553 deltadask-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3387 2022-11-24 16:36:05.427266 deltadask-0.1.0/setup.py
--rw-r--r--   0        0        0     3048 2022-11-24 16:36:05.427454 deltadask-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3431 2023-05-11 14:53:47.948488 deltadask-0.2.0/README.md
+-rw-r--r--   0        0        0      895 2023-05-11 14:53:47.948686 deltadask-0.2.0/deltadask/__init__.py
+-rw-r--r--   0        0        0      430 2023-05-11 14:53:47.950744 deltadask-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3955 1970-01-01 00:00:00.000000 deltadask-0.2.0/PKG-INFO
```

### Comparing `deltadask-0.1.0/README.md` & `deltadask-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 ```python
 import deltadask
 
 ddf = deltadask.read_delta("path/to/delta/table")
 ```
 
+It's a lot more efficient for Dask to read a Delta table compared to a Parquet data lake.  Parquet tables are of course faster than CSV tables [as explained in this video](https://www.youtube.com/watch?v=9LYYOdIwQXg).  Delta tables are the next big performance improvement for Dask users.
+
 ## Basic usage
 
 Suppose you have a Delta table with the following three versions.
 
 ![Delta table with version](https://github.com/MrPowers/deltadask/blob/main/images/delta-table-with-versions.png)
 
 Here's how to read the latest version of the Delta table:
@@ -38,49 +40,55 @@
 ```
 
 ```
    id
 0   0
 1   1
 2   2
-3   4
-4   5
+0   4
+1   5
 ```
 
 Delta Lake makes it easy to time travel between different versions of a Delta table with Dask.
 
-See this notebook for a full working example with an environment so you can replicate this on your machine.
+See [this notebook](https://github.com/MrPowers/deltadask/blob/main/notebooks/deltadask-demo.ipynb) for a full working example with an environment so you can replicate this on your machine.
 
 ## Why Delta Lake is better than Parquet for Dask
 
 A Delta table stores data in Parquet files and metadata in a trasaction log.  The metadata includes the schema and location of the files.
 
 ![Delta table architecture](https://github.com/MrPowers/deltadask/blob/main/images/delta-table.png)
 
 A Dask Parquet data lake can be stored in two different ways.
 
 1. Parquet files with a single metadata file
 2. Parquet files without a metadata file
 
-Parquet files with a single metadata file are limited because a single file has scaling limitations.
+Parquet files with a single metadata file is bad because of scaling limitations.
+
+Parquet files without a metadata file require expensive file listing / Parquet footer queries to build the overall metadata statistics for the data lake.  It's a lot faster to fetch this information from the Delta transaction log.
+
+Delta Lake is better because the transaction log is scalable and can be queried must faster than a data lake.
 
-Parquet files without a metadata file are limited because they require a relatively expensive file listing operation followed by calls to build the overall metadata statistics for the data lake.
+## How to make reads faster
 
-Delta Lake is better because the transaction log is scalable and can be queried a lot faster than an expensive file listing operation.
+You can make Delta Lake queries faster by using column projection and predicate pushdown filtering.  These tactics allow you to send less data to the cluster.
 
 Here's an example of how to query a Delta table with Dask and take advantage of column pruning and predicate pushdown filtering:
 
 ```python
 ddf = deltadask.read_delta(
     "path/to/delta/table", 
-    columns=["col1"], filters=[[('col1', '==', 0)]])
+    columns=["col1"], # column pruning
+    filters=[[('col1', '==', 0)]] # predicate pushdown
+)
 ```
 
-## Why this library is really easy to build
+This query only sends `col1` to the cluster and none of the other columns (column projection).
 
-Reading a Delta Lake into a Dask DataFrame is ridiculously easy, thanks to [delta-rs](https://github.com/delta-io/delta-rs/).
+This query also uses the transaction log to idenfity files that at least contain some data with `col1` equal to zero.  If a file contains no matching data, then it won't be read.  Depending on how the data is organized, a lot of files can be skipped.  You can skip the number of files even more by partitioning or Z ORDERING the data.
 
-Reading Delta Lakes is also really fast and efficient.  You can get a list of the files from the transaction log which is a lot faster than a file listing operation.
+## How this library is built
 
-You can also skip entire files based on column metadata stored in the transaction log.  Skipping data allows for huge performance improvements.
+The [delta-rs](https://github.com/delta-io/delta-rs/) library makes it really easy to build the deltadask connector.
 
-Here's how to read a Delta Lake into a Dask DataFrame with this library:
+All the transaction log parsing logic is handled by delta-rs.  You can just plug into the APIs to easily build the Dask connector.
```

