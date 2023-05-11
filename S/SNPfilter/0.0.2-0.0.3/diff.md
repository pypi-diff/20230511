# Comparing `tmp/SNPfilter-0.0.2.tar.gz` & `tmp/SNPfilter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNPfilter-0.0.2.tar", last modified: Thu May 11 01:48:01 2023, max compression
+gzip compressed data, was "SNPfilter-0.0.3.tar", last modified: Thu May 11 05:55:54 2023, max compression
```

## Comparing `SNPfilter-0.0.2.tar` & `SNPfilter-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 01:48:01.000000 SNPfilter-0.0.2/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2023-05-02 03:30:38.000000 SNPfilter-0.0.2/LICENSE
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       19 2023-05-02 03:45:18.000000 SNPfilter-0.0.2/MANIFEST.in
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3965 2023-05-11 01:48:01.000000 SNPfilter-0.0.2/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3633 2023-05-07 03:58:28.000000 SNPfilter-0.0.2/README.md
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 01:48:01.000000 SNPfilter-0.0.2/SNPfilter.egg-info/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3965 2023-05-11 01:48:00.000000 SNPfilter-0.0.2/SNPfilter.egg-info/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      354 2023-05-11 01:48:01.000000 SNPfilter-0.0.2/SNPfilter.egg-info/SOURCES.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2023-05-11 01:48:00.000000 SNPfilter-0.0.2/SNPfilter.egg-info/dependency_links.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       49 2023-05-11 01:48:00.000000 SNPfilter-0.0.2/SNPfilter.egg-info/entry_points.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       31 2023-05-11 01:48:00.000000 SNPfilter-0.0.2/SNPfilter.egg-info/requires.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       10 2023-05-11 01:48:01.000000 SNPfilter-0.0.2/SNPfilter.egg-info/top_level.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2023-05-11 01:48:01.000000 SNPfilter-0.0.2/setup.cfg
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      756 2023-05-07 02:49:23.000000 SNPfilter-0.0.2/setup.py
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 01:48:01.000000 SNPfilter-0.0.2/snpfilter/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-02 03:35:02.000000 SNPfilter-0.0.2/snpfilter/__init__.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)    12774 2023-05-11 01:34:58.000000 SNPfilter-0.0.2/snpfilter/cli.py
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 01:48:01.000000 SNPfilter-0.0.2/snpfilter/scripts/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-07 03:02:58.000000 SNPfilter-0.0.2/snpfilter/scripts/__init__.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      605 2023-05-07 03:04:06.000000 SNPfilter-0.0.2/snpfilter/scripts/map.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      362 2023-05-11 01:46:46.000000 SNPfilter-0.0.2/snpfilter/versions.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2023-05-02 03:30:38.000000 SNPfilter-0.0.3/LICENSE
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       19 2023-05-02 03:45:18.000000 SNPfilter-0.0.3/MANIFEST.in
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3965 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3633 2023-05-07 03:58:28.000000 SNPfilter-0.0.3/README.md
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/SNPfilter.egg-info/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3965 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      354 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/SNPfilter.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       49 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/entry_points.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       31 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/requires.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       10 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/top_level.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/setup.cfg
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      756 2023-05-07 02:49:23.000000 SNPfilter-0.0.3/setup.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/snpfilter/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-02 03:35:02.000000 SNPfilter-0.0.3/snpfilter/__init__.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)    12776 2023-05-11 05:51:01.000000 SNPfilter-0.0.3/snpfilter/cli.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/snpfilter/scripts/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-07 03:02:58.000000 SNPfilter-0.0.3/snpfilter/scripts/__init__.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      605 2023-05-07 03:04:06.000000 SNPfilter-0.0.3/snpfilter/scripts/map.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      502 2023-05-11 05:51:59.000000 SNPfilter-0.0.3/snpfilter/versions.py
```

### Comparing `SNPfilter-0.0.2/LICENSE` & `SNPfilter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SNPfilter-0.0.2/PKG-INFO` & `SNPfilter-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPfilter
-Version: 0.0.2
+Version: 0.0.3
 Summary: A handy little tool for filtering SNPs.
 Home-page: https://github.com/SouthernCD/SNPfilter
 Author: Yuxing Xu
 Author-email: xuyuxing@mail.kib.ac.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

### Comparing `SNPfilter-0.0.2/README.md` & `SNPfilter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `SNPfilter-0.0.2/SNPfilter.egg-info/PKG-INFO` & `SNPfilter-0.0.3/SNPfilter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPfilter
-Version: 0.0.2
+Version: 0.0.3
 Summary: A handy little tool for filtering SNPs.
 Home-page: https://github.com/SouthernCD/SNPfilter
 Author: Yuxing Xu
 Author-email: xuyuxing@mail.kib.ac.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

### Comparing `SNPfilter-0.0.2/setup.py` & `SNPfilter-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `SNPfilter-0.0.2/snpfilter/cli.py` & `SNPfilter-0.0.3/snpfilter/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         parser_a.add_argument('R1', type=str,
                               help='fastq file 1')
         parser_a.add_argument('R2', type=str,
                               help='fastq file 2')
         parser_a.add_argument('-t', '--threads', type=int,
                               help='num of threads', default=8)
         parser_a.add_argument('-q', '--min-MQ', type=int,
-                              help='skip alignments with mapQ smaller than INT', default=0)
+                              help='skip alignments with mapQ smaller than INT', default=20)
         parser_a.add_argument('-Q', '--min-BQ', type=int,
-                              help='skip bases with baseQ/BAQ smaller than INT', default=0)
+                              help='skip bases with baseQ/BAQ smaller than INT', default=20)
         parser_a.set_defaults(func=prepare_main)
 
         # argparse for qcfilter
         parser_a = subparsers.add_parser('qcfilter',
                                          description='filtering snp from bcf file with min depth and min variant frequency\n')
 
         parser_a.add_argument('sample_id', type=str,
```

### Comparing `SNPfilter-0.0.2/snpfilter/scripts/map.py` & `SNPfilter-0.0.3/snpfilter/scripts/map.py`

 * *Files identical despite different names*

