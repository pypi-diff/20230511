# Comparing `tmp/datacompy-0.8.4.tar.gz` & `tmp/datacompy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacompy-0.8.4.tar", last modified: Wed Jan  4 18:18:04 2023, max compression
+gzip compressed data, was "datacompy-0.9.0.tar", last modified: Thu May 11 17:32:51 2023, max compression
```

## Comparing `datacompy-0.8.4.tar` & `datacompy-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 18:18:04.563284 datacompy-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-04 18:17:39.000000 datacompy-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-04 18:17:39.000000 datacompy-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-01-04 18:18:04.563284 datacompy-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-01-04 18:17:39.000000 datacompy-0.8.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 18:18:04.563284 datacompy-0.8.4/datacompy/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-01-04 18:17:39.000000 datacompy-0.8.4/datacompy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32736 2023-01-04 18:17:39.000000 datacompy-0.8.4/datacompy/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    34871 2023-01-04 18:17:39.000000 datacompy-0.8.4/datacompy/sparkcompare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 18:18:04.563284 datacompy-0.8.4/datacompy/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-04 18:17:39.000000 datacompy-0.8.4/datacompy/templates/column_comparison.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-04 18:17:39.000000 datacompy-0.8.4/datacompy/templates/column_summary.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-04 18:17:39.000000 datacompy-0.8.4/datacompy/templates/fav_column_summary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-04 18:17:39.000000 datacompy-0.8.4/datacompy/templates/header.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-04 18:17:39.000000 datacompy-0.8.4/datacompy/templates/row_summary.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 18:18:04.563284 datacompy-0.8.4/datacompy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-01-04 18:18:04.000000 datacompy-0.8.4/datacompy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-01-04 18:18:04.000000 datacompy-0.8.4/datacompy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 18:18:04.000000 datacompy-0.8.4/datacompy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 18:18:00.000000 datacompy-0.8.4/datacompy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-04 18:18:04.000000 datacompy-0.8.4/datacompy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-04 18:18:04.000000 datacompy-0.8.4/datacompy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-04 18:17:39.000000 datacompy-0.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-01-04 18:18:04.563284 datacompy-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-04 18:17:39.000000 datacompy-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:32:51.344617 datacompy-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 17:32:16.000000 datacompy-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 17:32:16.000000 datacompy-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-11 17:32:51.344617 datacompy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-11 17:32:16.000000 datacompy-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:32:51.340617 datacompy-0.9.0/datacompy/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-11 17:32:16.000000 datacompy-0.9.0/datacompy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32231 2023-05-11 17:32:16.000000 datacompy-0.9.0/datacompy/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34994 2023-05-11 17:32:16.000000 datacompy-0.9.0/datacompy/sparkcompare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:32:51.344617 datacompy-0.9.0/datacompy/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-11 17:32:16.000000 datacompy-0.9.0/datacompy/templates/column_comparison.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 17:32:16.000000 datacompy-0.9.0/datacompy/templates/column_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-11 17:32:16.000000 datacompy-0.9.0/datacompy/templates/fav_column_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 17:32:16.000000 datacompy-0.9.0/datacompy/templates/header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-11 17:32:16.000000 datacompy-0.9.0/datacompy/templates/row_summary.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:32:51.344617 datacompy-0.9.0/datacompy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-11 17:32:51.000000 datacompy-0.9.0/datacompy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-11 17:32:51.000000 datacompy-0.9.0/datacompy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:32:51.000000 datacompy-0.9.0/datacompy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:32:20.000000 datacompy-0.9.0/datacompy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-11 17:32:51.000000 datacompy-0.9.0/datacompy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 17:32:51.000000 datacompy-0.9.0/datacompy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-11 17:32:16.000000 datacompy-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-11 17:32:51.344617 datacompy-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-11 17:32:16.000000 datacompy-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:32:51.344617 datacompy-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    48222 2023-05-11 17:32:16.000000 datacompy-0.9.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68504 2023-05-11 17:32:16.000000 datacompy-0.9.0/tests/test_sparkcompare.py
```

### Comparing `datacompy-0.8.4/LICENSE` & `datacompy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datacompy-0.8.4/PKG-INFO` & `datacompy-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacompy
-Version: 0.8.4
+Version: 0.9.0
 Summary: Dataframe comparison in Python
 Home-page: https://github.com/capitalone/datacompy
 Author: Ian Robertson, Dan Coates, Faisal Dosani
 Author-email: faisal.dosani@capitalone.com
 Maintainer: Faisal Dosani
 Maintainer-email: faisal.dosani@capitalone.com
 License: Apache Software License
@@ -13,15 +13,14 @@
 Project-URL: Source Code, https://github.com/capitalone/datacompy
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: spark
 Provides-Extra: docs
 Provides-Extra: tests
```

### Comparing `datacompy-0.8.4/README.rst` & `datacompy-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,20 @@
 
 
 .. _spark-detail:
 
 Spark Detail
 ============
 
+.. important::
+
+    With version ``v0.9.0`` SparkCompare now uses Null Safe (``<=>``) comparisons
+
+..
+
 DataComPy's ``SparkCompare`` class will join two dataframes either on a list of join
 columns. It has the capability to map column names that may be different in each
 dataframe, including in the join columns. You are responsible for creating the
 dataframes from any source which Spark can handle and specifying a unique join
 key. If there are duplicates in either dataframe by join key, the match process
 will remove the duplicates before joining (and tell you how many duplicates were
 found).
```

### Comparing `datacompy-0.8.4/datacompy/__init__.py` & `datacompy-0.9.0/datacompy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.8.4"
+__version__ = "0.9.0"
 
 from datacompy.core import *
 from datacompy.sparkcompare import NUMERIC_SPARK_TYPES, SparkCompare
```

### Comparing `datacompy-0.8.4/datacompy/core.py` & `datacompy-0.9.0/datacompy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,26 +157,26 @@
         index : str
             The "index" of the dataframe - df1 or df2.
         cast_column_names_lower: bool, optional
             Boolean indicator that controls of column names will be cast into lower case
         """
         dataframe = getattr(self, index)
         if not isinstance(dataframe, pd.DataFrame):
-            raise TypeError("{} must be a pandas DataFrame".format(index))
+            raise TypeError(f"{index} must be a pandas DataFrame")
 
         if cast_column_names_lower:
             dataframe.columns = [str(col).lower() for col in dataframe.columns]
         else:
             dataframe.columns = [str(col) for col in dataframe.columns]
         # Check if join_columns are present in the dataframe
         if not set(self.join_columns).issubset(set(dataframe.columns)):
-            raise ValueError("{} must have all columns from join_columns".format(index))
+            raise ValueError(f"{index} must have all columns from join_columns")
 
         if len(set(dataframe.columns)) < len(dataframe.columns):
-            raise ValueError("{} must have unique column names".format(index))
+            raise ValueError(f"{index} must have unique column names")
 
         if self.on_index:
             if dataframe.index.duplicated().sum() > 0:
                 self._any_dupes = True
         else:
             if len(dataframe.drop_duplicates(subset=self.join_columns)) < len(
                 dataframe
@@ -192,30 +192,26 @@
         """
         LOG.debug("Checking equality")
         if self.df1.equals(self.df2):
             LOG.info("df1 Pandas.DataFrame.equals df2")
         else:
             LOG.info("df1 does not Pandas.DataFrame.equals df2")
         LOG.info(
-            "Number of columns in common: {}".format(len(self.intersect_columns()))
+            f"Number of columns in common: {len(self.intersect_columns())}"
         )
         LOG.debug("Checking column overlap")
         for col in self.df1_unq_columns():
-            LOG.info("Column in df1 and not in df2: {}".format(col))
+            LOG.info(f"Column in df1 and not in df2: {col}")
         LOG.info(
-            "Number of columns in df1 and not in df2: {}".format(
-                len(self.df1_unq_columns())
-            )
+            f"Number of columns in df1 and not in df2: {len(self.df1_unq_columns())}"
         )
         for col in self.df2_unq_columns():
-            LOG.info("Column in df2 and not in df1: {}".format(col))
+            LOG.info(f"Column in df2 and not in df1: {col}")
         LOG.info(
-            "Number of columns in df2 and not in df1: {}".format(
-                len(self.df2_unq_columns())
-            )
+            f"Number of columns in df2 and not in df1: {len(self.df2_unq_columns())}"
         )
         LOG.debug("Merging dataframes")
         self._dataframe_merge(ignore_spaces)
         self._intersect_compare(ignore_spaces, ignore_case)
         if self.matches():
             LOG.info("df1 matches df2")
         else:
@@ -302,26 +298,24 @@
 
         LOG.debug("Selecting df2 unique rows")
         self.df2_unq_rows = outer_join[outer_join["_merge"] == "right_only"][
             df2_cols
         ].copy()
         self.df2_unq_rows.columns = self.df2.columns
         LOG.info(
-            "Number of rows in df1 and not in df2: {}".format(len(self.df1_unq_rows))
+            f"Number of rows in df1 and not in df2: {len(self.df1_unq_rows)}"
         )
         LOG.info(
-            "Number of rows in df2 and not in df1: {}".format(len(self.df2_unq_rows))
+            f"Number of rows in df2 and not in df1: {len(self.df2_unq_rows)}"
         )
 
         LOG.debug("Selecting intersecting rows")
         self.intersect_rows = outer_join[outer_join["_merge"] == "both"].copy()
         LOG.info(
-            "Number of rows in df1 and df2 (not necessarily equal): {}".format(
-                len(self.intersect_rows)
-            )
+            "Number of rows in df1 and df2 (not necessarily equal): {len(self.intersect_rows)}"
         )
 
     def _intersect_compare(self, ignore_spaces, ignore_case):
         """Run the comparison on the intersect dataframe
 
         This loops through all columns that are shared between df1 and df2, and
         creates a column column_match which is True for matches, False
@@ -357,17 +351,15 @@
                 ).sum()
 
             if row_cnt > 0:
                 match_rate = float(match_cnt) / row_cnt
             else:
                 match_rate = 0
             LOG.info(
-                "{}: {} / {} ({:.2%}) match".format(
-                    column, match_cnt, row_cnt, match_rate
-                )
+                f"{column}: {match_cnt} / {row_cnt} ({match_rate:.2%}) match"
             )
 
             self.column_stats.append(
                 {
                     "column": column,
                     "match_column": col_match,
                     "match_cnt": match_cnt,
@@ -515,22 +507,20 @@
                     self.ignore_spaces,
                     self.ignore_case,
                 )
 
                 if not ignore_matching_cols or (
                     ignore_matching_cols and not col_comparison.all()
                 ):
-                    LOG.debug("Adding column {} to the result.".format(orig_col_name))
+                    LOG.debug(f"Adding column {orig_col_name} to the result.")
                     match_list.append(col)
                     return_list.extend([orig_col_name + "_df1", orig_col_name + "_df2"])
                 elif ignore_matching_cols:
                     LOG.debug(
-                        "Column {} is equal in df1 and df2. It will not be added to the result.".format(
-                            orig_col_name
-                        )
+                        f"Column {orig_col_name} is equal in df1 and df2. It will not be added to the result."
                     )
 
         mm_bool = self.intersect_rows[match_list].all(axis="columns")
         return self.intersect_rows[~mm_bool][self.join_columns + return_list]
 
     def report(self, sample_count=10, column_count=10, html_file=None):
         """Returns a string representation of a report.  The representation can
@@ -608,16 +598,16 @@
         any_mismatch = False
         for column in self.column_stats:
             if not column["all_match"]:
                 any_mismatch = True
                 match_stats.append(
                     {
                         "Column": column["column"],
-                        "{} dtype".format(self.df1_name): column["dtype1"],
-                        "{} dtype".format(self.df2_name): column["dtype2"],
+                        f"{self.df1_name} dtype": column["dtype1"],
+                        f"{self.df2_name} dtype": column["dtype2"],
                         "# Unequal": column["unequal_cnt"],
                         "Max Diff": column["max_diff"],
                         "# Null Diff": column["null_diff"],
                     }
                 )
                 if column["unequal_cnt"] > 0:
                     match_sample.append(
@@ -632,16 +622,16 @@
             report += "\n"
             df_match_stats = pd.DataFrame(match_stats)
             df_match_stats.sort_values("Column", inplace=True)
             # Have to specify again for sorting
             report += df_match_stats[
                 [
                     "Column",
-                    "{} dtype".format(self.df1_name),
-                    "{} dtype".format(self.df2_name),
+                    f"{self.df1_name} dtype",
+                    f"{self.df2_name} dtype",
                     "# Unequal",
                     "Max Diff",
                     "# Null Diff",
                 ]
             ].to_string()
             report += "\n\n"
 
@@ -650,33 +640,25 @@
                 report += "-------------------------------\n"
                 report += "\n"
                 for sample in match_sample:
                     report += sample.to_string()
                     report += "\n\n"
 
         if min(sample_count, self.df1_unq_rows.shape[0]) > 0:
-            report += "Sample Rows Only in {} (First {} Columns)\n".format(
-                self.df1_name, column_count
-            )
-            report += "---------------------------------------{}\n".format(
-                "-" * len(self.df1_name)
-            )
+            report += f"Sample Rows Only in {self.df1_name} (First {column_count} Columns)\n"
+            report += f"---------------------------------------{'-' * len(self.df1_name)}\n"
             report += "\n"
             columns = self.df1_unq_rows.columns[:column_count]
             unq_count = min(sample_count, self.df1_unq_rows.shape[0])
             report += self.df1_unq_rows.sample(unq_count)[columns].to_string()
             report += "\n\n"
 
         if min(sample_count, self.df2_unq_rows.shape[0]) > 0:
-            report += "Sample Rows Only in {} (First {} Columns)\n".format(
-                self.df2_name, column_count
-            )
-            report += "---------------------------------------{}\n".format(
-                "-" * len(self.df2_name)
-            )
+            report += f"Sample Rows Only in {self.df2_name} (First {column_count} Columns)\n"
+            report += f"---------------------------------------{'-' * len(self.df2_name)}\n"
             report += "\n"
             columns = self.df2_unq_rows.columns[:column_count]
             unq_count = min(sample_count, self.df2_unq_rows.shape[0])
             report += self.df2_unq_rows.sample(unq_count)[columns].to_string()
             report += "\n\n"
 
         if html_file:
@@ -855,15 +837,15 @@
     Returns
     -------
     str
         String column name that looks like '_temp_x' for some integer x
     """
     i = 0
     while True:
-        temp_column = "_temp_{}".format(i)
+        temp_column = f"_temp_{i}"
         unique = True
         for dataframe in dataframes:
             if temp_column in dataframe.columns:
                 i += 1
                 unique = False
         if unique:
             return temp_column
@@ -905,15 +887,15 @@
     -------
     Pandas.Series
         The ID column that's unique in each group.
     """
     default_value = "DATACOMPY_NULL"
     if dataframe[join_columns].isnull().any().any():
         if (dataframe[join_columns] == default_value).any().any():
-            raise ValueError("{} was found in your join columns".format(default_value))
+            raise ValueError(f"{default_value} was found in your join columns")
         return (
             dataframe[join_columns]
             .astype(str)
             .fillna(default_value)
             .groupby(join_columns)
             .cumcount()
         )
```

### Comparing `datacompy-0.8.4/datacompy/sparkcompare.py` & `datacompy-0.9.0/datacompy/sparkcompare.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,17 @@
 
     Returns
     -------
     bool
         True if both data types are comparable
     """
 
-    return type1 == type2 or (type1 in NUMERIC_SPARK_TYPES and type2 in NUMERIC_SPARK_TYPES)
+    return type1 == type2 or (
+        type1 in NUMERIC_SPARK_TYPES and type2 in NUMERIC_SPARK_TYPES
+    )
 
 
 class SparkCompare:
     """Comparison class used to compare two Spark Dataframes.
 
     Extends the ``Compare`` functionality to the wide world of Spark and
     out-of-memory data.
@@ -214,15 +216,17 @@
         return set(self.base_df.columns) & set(self.compare_df.columns)
 
     @property
     def columns_compared(self):
         """list[str]: Get columns to be compared in both dataframes (all
         columns in both excluding the join key(s)"""
         return [
-            column for column in list(self.columns_in_both) if column not in self._join_column_names
+            column
+            for column in list(self.columns_in_both)
+            if column not in self._join_column_names
         ]
 
     @property
     def columns_only_base(self):
         """set[str]: Get columns that are unique to the base dataframe"""
         return set(self.base_df.columns) - set(self.compare_df.columns)
 
@@ -265,90 +269,87 @@
     def _get_compare_rows(self):
         """Get the rows only from compare data frame"""
         return self.compare_df.select(self._join_column_names).subtract(
             self.base_df.select(self._join_column_names)
         )
 
     def _print_columns_summary(self, myfile):
-        """ Prints the column summary details"""
+        """Prints the column summary details"""
         print("\n****** Column Summary ******", file=myfile)
         print(
-            "Number of columns in common with matching schemas: {}".format(
-                len(self._columns_with_matching_schema())
-            ),
+            f"Number of columns in common with matching schemas: {len(self._columns_with_matching_schema())}",
             file=myfile,
         )
         print(
-            "Number of columns in common with schema differences: {}".format(
-                len(self._columns_with_schemadiff())
-            ),
+            f"Number of columns in common with schema differences: {len(self._columns_with_schemadiff())}",
             file=myfile,
         )
         print(
-            "Number of columns in base but not compare: {}".format(len(self.columns_only_base)),
+            f"Number of columns in base but not compare: {len(self.columns_only_base)}",
             file=myfile,
         )
         print(
-            "Number of columns in compare but not base: {}".format(len(self.columns_only_compare)),
+            f"Number of columns in compare but not base: {len(self.columns_only_compare)}",
             file=myfile,
         )
 
     def _print_only_columns(self, base_or_compare, myfile):
         """Prints the columns and data types only in either the base or compare datasets"""
 
         if base_or_compare.upper() == "BASE":
             columns = self.columns_only_base
             df = self.base_df
         elif base_or_compare.upper() == "COMPARE":
             columns = self.columns_only_compare
             df = self.compare_df
         else:
             raise ValueError(
-                'base_or_compare must be BASE or COMPARE, but was "{}"'.format(base_or_compare)
+                f'base_or_compare must be BASE or COMPARE, but was "{base_or_compare}"'
             )
 
         # If there are no columns only in this dataframe, don't display this section
         if not columns:
             return
 
         max_length = max([len(col) for col in columns] + [11])
-        format_pattern = "{{:{max}s}}".format(max=max_length)
+        format_pattern = f"{{:{max_length}s}}"
 
-        print("\n****** Columns In {} Only ******".format(base_or_compare.title()), file=myfile)
+        print(f"\n****** Columns In {base_or_compare.title()} Only ******", file=myfile)
         print((format_pattern + "  Dtype").format("Column Name"), file=myfile)
         print("-" * max_length + "  -------------", file=myfile)
 
         for column in columns:
             col_type = df.select(column).dtypes[0][1]
             print((format_pattern + "  {:13s}").format(column, col_type), file=myfile)
 
     def _columns_with_matching_schema(self):
-        """ This function will identify the columns which has matching schema"""
+        """This function will identify the columns which has matching schema"""
         col_schema_match = {}
         base_columns_dict = dict(self.base_df.dtypes)
         compare_columns_dict = dict(self.compare_df.dtypes)
 
         for base_row, base_type in base_columns_dict.items():
             if base_row in compare_columns_dict:
                 if base_type in compare_columns_dict.get(base_row):
                     col_schema_match[base_row] = compare_columns_dict.get(base_row)
 
         return col_schema_match
 
     def _columns_with_schemadiff(self):
-        """ This function will identify the columns which has different schema"""
+        """This function will identify the columns which has different schema"""
         col_schema_diff = {}
         base_columns_dict = dict(self.base_df.dtypes)
         compare_columns_dict = dict(self.compare_df.dtypes)
 
         for base_row, base_type in base_columns_dict.items():
             if base_row in compare_columns_dict:
                 if base_type not in compare_columns_dict.get(base_row):
                     col_schema_diff[base_row] = dict(
-                        base_type=base_type, compare_type=compare_columns_dict.get(base_row)
+                        base_type=base_type,
+                        compare_type=compare_columns_dict.get(base_row),
                     )
         return col_schema_diff
 
     @property
     def rows_both_mismatch(self):
         """pyspark.sql.DataFrame: Returns all rows in both dataframes that have mismatches"""
         if self._all_rows_mismatched is None:
@@ -368,15 +369,15 @@
     def rows_only_base(self):
         """pyspark.sql.DataFrame: Returns rows only in the base dataframe"""
         if not self._rows_only_base:
             base_rows = self._get_unq_base_rows()
             base_rows.createOrReplaceTempView("baseRows")
             self.base_df.createOrReplaceTempView("baseTable")
             join_condition = " AND ".join(
-                ["A." + name + "=B." + name for name in self._join_column_names]
+                ["A." + name + "<=>B." + name for name in self._join_column_names]
             )
             sql_query = "select A.* from baseTable as A, baseRows as B where {}".format(
                 join_condition
             )
             self._rows_only_base = self.spark.sql(sql_query)
 
             if self.cache_intermediates:
@@ -388,18 +389,20 @@
     def rows_only_compare(self):
         """pyspark.sql.DataFrame: Returns rows only in the compare dataframe"""
         if not self._rows_only_compare:
             compare_rows = self._get_compare_rows()
             compare_rows.createOrReplaceTempView("compareRows")
             self.compare_df.createOrReplaceTempView("compareTable")
             where_condition = " AND ".join(
-                ["A." + name + "=B." + name for name in self._join_column_names]
+                ["A." + name + "<=>B." + name for name in self._join_column_names]
             )
-            sql_query = "select A.* from compareTable as A, compareRows as B where {}".format(
-                where_condition
+            sql_query = (
+                "select A.* from compareTable as A, compareRows as B where {}".format(
+                    where_condition
+                )
             )
             self._rows_only_compare = self.spark.sql(sql_query)
 
             if self.cache_intermediates:
                 self._rows_only_compare.cache().count()
 
         return self._rows_only_compare
@@ -439,27 +442,35 @@
 
     def _merge_dataframes(self):
         """Merges the two dataframes and creates self._all_matched_rows and self._all_rows_mismatched."""
         full_joined_dataframe = self._get_or_create_joined_dataframe()
         full_joined_dataframe.createOrReplaceTempView("full_matched_table")
 
         select_statement = self._generate_select_statement(False)
-        select_query = """SELECT {} FROM full_matched_table A""".format(select_statement)
+        select_query = """SELECT {} FROM full_matched_table A""".format(
+            select_statement
+        )
 
-        self._all_matched_rows = self.spark.sql(select_query).orderBy(self._join_column_names)
+        self._all_matched_rows = self.spark.sql(select_query).orderBy(
+            self._join_column_names
+        )
         self._all_matched_rows.createOrReplaceTempView("matched_table")
 
-        where_cond = " OR ".join(["A." + name + "_match= False" for name in self.columns_compared])
+        where_cond = " OR ".join(
+            ["A." + name + "_match= False" for name in self.columns_compared]
+        )
         mismatch_query = """SELECT * FROM matched_table A WHERE {}""".format(where_cond)
-        self._all_rows_mismatched = self.spark.sql(mismatch_query).orderBy(self._join_column_names)
+        self._all_rows_mismatched = self.spark.sql(mismatch_query).orderBy(
+            self._join_column_names
+        )
 
     def _get_or_create_joined_dataframe(self):
         if self._joined_dataframe is None:
             join_condition = " AND ".join(
-                ["A." + name + "=B." + name for name in self._join_column_names]
+                ["A." + name + "<=>B." + name for name in self._join_column_names]
             )
             select_statement = self._generate_select_statement(match_data=True)
 
             self.base_df.createOrReplaceTempView("base_table")
             self.compare_df.createOrReplaceTempView("compare_table")
 
             join_query = r"""
@@ -475,68 +486,81 @@
                 self._joined_dataframe.cache()
                 self._common_row_count = self._joined_dataframe.count()
 
         return self._joined_dataframe
 
     def _print_num_of_rows_with_column_equality(self, myfile):
         # match_dataframe contains columns from both dataframes with flag to indicate if columns matched
-        match_dataframe = self._get_or_create_joined_dataframe().select(*self.columns_compared)
+        match_dataframe = self._get_or_create_joined_dataframe().select(
+            *self.columns_compared
+        )
         match_dataframe.createOrReplaceTempView("matched_df")
 
         where_cond = " AND ".join(
-            ["A." + name + "=" + str(MatchType.MATCH.value) for name in self.columns_compared]
+            [
+                "A." + name + "=" + str(MatchType.MATCH.value)
+                for name in self.columns_compared
+            ]
         )
-        match_query = r"""SELECT count(*) AS row_count FROM matched_df A WHERE {}""".format(
-            where_cond
+        match_query = (
+            r"""SELECT count(*) AS row_count FROM matched_df A WHERE {}""".format(
+                where_cond
+            )
         )
         all_rows_matched = self.spark.sql(match_query)
         matched_rows = all_rows_matched.head()[0]
 
         print("\n****** Row Comparison ******", file=myfile)
         print(
-            "Number of rows with some columns unequal: {}".format(
-                self.common_row_count - matched_rows
-            ),
+            f"Number of rows with some columns unequal: {self.common_row_count - matched_rows}",
             file=myfile,
         )
-        print("Number of rows with all columns equal: {}".format(matched_rows), file=myfile)
+        print(f"Number of rows with all columns equal: {matched_rows}", file=myfile)
 
     def _populate_columns_match_dict(self):
         """
         side effects:
             columns_match_dict assigned to { column -> match_type_counts }
                 where:
                     column (string): Name of a column that exists in both the base and comparison columns
                     match_type_counts (list of int with size = len(MatchType)): The number of each match type seen for this column (in order of the MatchType enum values)
 
         returns: None
         """
 
-        match_dataframe = self._get_or_create_joined_dataframe().select(*self.columns_compared)
+        match_dataframe = self._get_or_create_joined_dataframe().select(
+            *self.columns_compared
+        )
 
         def helper(c):
             # Create a predicate for each match type, comparing column values to the match type value
             predicates = [F.col(c) == k.value for k in MatchType]
             # Create a tuple(number of match types found for each match type in this column)
-            return F.struct([F.lit(F.sum(pred.cast("integer"))) for pred in predicates]).alias(c)
+            return F.struct(
+                [F.lit(F.sum(pred.cast("integer"))) for pred in predicates]
+            ).alias(c)
 
         # For each column, create a single tuple. This tuple's values correspond to the number of times
         # each match type appears in that column
-        match_data = match_dataframe.agg(*[helper(col) for col in self.columns_compared]).collect()
+        match_data = match_dataframe.agg(
+            *[helper(col) for col in self.columns_compared]
+        ).collect()
         match_data = match_data[0]
 
         for c in self.columns_compared:
             self.columns_match_dict[c] = match_data[c]
 
     def _create_select_statement(self, name):
         if self._known_differences:
             match_type_comparison = ""
             for k in MatchType:
-                match_type_comparison += " WHEN (A.{name}={match_value}) THEN '{match_name}'".format(
-                    name=name, match_value=str(k.value), match_name=k.name
+                match_type_comparison += (
+                    " WHEN (A.{name}={match_value}) THEN '{match_name}'".format(
+                        name=name, match_value=str(k.value), match_name=k.name
+                    )
                 )
             return "A.{name}_base, A.{name}_compare, (CASE WHEN (A.{name}={match_failure}) THEN False ELSE True END) AS {name}_match, (CASE {match_type_comparison} ELSE 'UNDEFINED' END) AS {name}_match_type ".format(
                 name=name,
                 match_failure=MatchType.MISMATCH.value,
                 match_type_comparison=match_type_comparison,
             )
         else:
@@ -601,35 +625,29 @@
     def _print_row_summary(self, myfile):
         base_df_cnt = self.base_df.count()
         compare_df_cnt = self.compare_df.count()
         base_df_with_dup_cnt = self._original_base_df.count()
         compare_df_with_dup_cnt = self._original_compare_df.count()
 
         print("\n****** Row Summary ******", file=myfile)
-        print("Number of rows in common: {}".format(self.common_row_count), file=myfile)
+        print(f"Number of rows in common: {self.common_row_count}", file=myfile)
         print(
-            "Number of rows in base but not compare: {}".format(
-                base_df_cnt - self.common_row_count
-            ),
+            f"Number of rows in base but not compare: {base_df_cnt - self.common_row_count}",
             file=myfile,
         )
         print(
-            "Number of rows in compare but not base: {}".format(
-                compare_df_cnt - self.common_row_count
-            ),
+            f"Number of rows in compare but not base: {compare_df_cnt - self.common_row_count}",
             file=myfile,
         )
         print(
-            "Number of duplicate rows found in base: {}".format(base_df_with_dup_cnt - base_df_cnt),
+            f"Number of duplicate rows found in base: {base_df_with_dup_cnt - base_df_cnt}",
             file=myfile,
         )
         print(
-            "Number of duplicate rows found in compare: {}".format(
-                compare_df_with_dup_cnt - compare_df_cnt
-            ),
+            f"Number of duplicate rows found in compare: {compare_df_with_dup_cnt - compare_df_cnt}",
             file=myfile,
         )
 
     def _print_schema_diff_details(self, myfile):
         schema_diff_dict = self._columns_with_schemadiff()
 
         if not schema_diff_dict:  # If there are no differences, don't print the section
@@ -649,24 +667,30 @@
         print(
             (format_pattern + "  Base Dtype     Compare Dtype").format(
                 "Base Column Name", "Compare Column Name"
             ),
             file=myfile,
         )
         print(
-            "-" * base_name_max + "  " + "-" * compare_name_max + "  -------------  -------------",
+            "-" * base_name_max
+            + "  "
+            + "-" * compare_name_max
+            + "  -------------  -------------",
             file=myfile,
         )
 
         for base_column, types in schema_diff_dict.items():
             compare_column = self._base_to_compare_name(base_column)
 
             print(
                 (format_pattern + "  {:13s}  {:13s}").format(
-                    base_column, compare_column, types["base_type"], types["compare_type"]
+                    base_column,
+                    compare_column,
+                    types["base_type"],
+                    types["compare_type"],
                 ),
                 file=myfile,
             )
 
     def _base_to_compare_name(self, base_name):
         """Translates a column name in the base dataframe to its counterpart in the
         compare dataframe, if they are different."""
@@ -701,65 +725,58 @@
         base_types = {x[0]: x[1] for x in self.base_df.dtypes}
         compare_types = {x[0]: x[1] for x in self.compare_df.dtypes}
 
         print("\n****** Column Comparison ******", file=myfile)
 
         if self._known_differences:
             print(
-                "Number of columns compared with unexpected differences in some values: {}".format(
-                    len(columns_with_mismatches)
-                ),
+                f"Number of columns compared with unexpected differences in some values: {len(columns_with_mismatches)}",
                 file=myfile,
             )
             print(
-                "Number of columns compared with all values equal but known differences found: {}".format(
-                    len(self.columns_compared)
-                    - len(columns_with_mismatches)
-                    - len(columns_fully_matching)
-                ),
+                f"Number of columns compared with all values equal but known differences found: {len(self.columns_compared) - len(columns_with_mismatches) - len(columns_fully_matching)}",
                 file=myfile,
             )
             print(
-                "Number of columns compared with all values completely equal: {}".format(
-                    len(columns_fully_matching)
-                ),
+                f"Number of columns compared with all values completely equal: {len(columns_fully_matching)}",
                 file=myfile,
             )
         else:
             print(
-                "Number of columns compared with some values unequal: {}".format(
-                    len(columns_with_mismatches)
-                ),
+                f"Number of columns compared with some values unequal: {len(columns_with_mismatches)}",
                 file=myfile,
             )
             print(
-                "Number of columns compared with all values equal: {}".format(
-                    len(columns_fully_matching)
-                ),
+                f"Number of columns compared with all values equal: {len(columns_fully_matching)}",
                 file=myfile,
             )
 
         # If all columns matched, don't print columns with unequal values
         if (not self.show_all_columns) and (
             len(columns_fully_matching) == len(self.columns_compared)
         ):
             return
 
         # if show_all_columns is set, set column name length maximum to max of ALL columns(with minimum)
         if self.show_all_columns:
             base_name_max = max([len(key) for key in self.columns_match_dict] + [16])
             compare_name_max = max(
-                [len(self._base_to_compare_name(key)) for key in self.columns_match_dict] + [19]
+                [
+                    len(self._base_to_compare_name(key))
+                    for key in self.columns_match_dict
+                ]
+                + [19]
             )
 
         # For columns with any differences, what are the longest base and compare column name lengths (with minimums)?
         else:
             base_name_max = max([len(key) for key in columns_with_any_diffs] + [16])
             compare_name_max = max(
-                [len(self._base_to_compare_name(key)) for key in columns_with_any_diffs] + [19]
+                [len(self._base_to_compare_name(key)) for key in columns_with_any_diffs]
+                + [19]
             )
 
         """ list of (header, condition, width, align)
                 where
                     header (String) : output header for a column
                     condition (Bool): true if this header should be displayed
                     width (Int)     : width of the column
@@ -786,17 +803,22 @@
 
         format_pattern = (" " * padding).join(
             [
                 ("{:" + (">" if h[3] else "") + str(h[2]) + "}")
                 for h in headers_columns_unequal_valid
             ]
         )
-        print(format_pattern.format(*[h[0] for h in headers_columns_unequal_valid]), file=myfile)
         print(
-            format_pattern.format(*["-" * len(h[0]) for h in headers_columns_unequal_valid]),
+            format_pattern.format(*[h[0] for h in headers_columns_unequal_valid]),
+            file=myfile,
+        )
+        print(
+            format_pattern.format(
+                *["-" * len(h[0]) for h in headers_columns_unequal_valid]
+            ),
             file=myfile,
         )
 
         for column_name, column_values in sorted(
             self.columns_match_dict.items(), key=lambda i: i[0]
         ):
             num_matches = column_values[MatchType.MATCH.value]
@@ -816,15 +838,16 @@
                     compare_types.get(column_name),
                     str(num_matches),
                     str(num_mismatches),
                 ]
                 if self.match_rates:
                     match_rate = 100 * (
                         1
-                        - (column_values[MatchType.MISMATCH.value] + 0.0) / self.common_row_count
+                        - (column_values[MatchType.MISMATCH.value] + 0.0)
+                        / self.common_row_count
                         + 0.0
                     )
                     output_row.append("{:02.5f}".format(match_rate))
                 if num_known_diffs is not None:
                     output_row.insert(len(output_row) - 1, str(num_known_diffs))
                 print(format_pattern.format(*output_row), file=myfile)
```

### Comparing `datacompy-0.8.4/datacompy.egg-info/PKG-INFO` & `datacompy-0.9.0/datacompy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacompy
-Version: 0.8.4
+Version: 0.9.0
 Summary: Dataframe comparison in Python
 Home-page: https://github.com/capitalone/datacompy
 Author: Ian Robertson, Dan Coates, Faisal Dosani
 Author-email: faisal.dosani@capitalone.com
 Maintainer: Faisal Dosani
 Maintainer-email: faisal.dosani@capitalone.com
 License: Apache Software License
@@ -13,15 +13,14 @@
 Project-URL: Source Code, https://github.com/capitalone/datacompy
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: spark
 Provides-Extra: docs
 Provides-Extra: tests
```

### Comparing `datacompy-0.8.4/datacompy.egg-info/SOURCES.txt` & `datacompy-0.9.0/datacompy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,10 @@
 datacompy.egg-info/not-zip-safe
 datacompy.egg-info/requires.txt
 datacompy.egg-info/top_level.txt
 datacompy/templates/column_comparison.txt
 datacompy/templates/column_summary.txt
 datacompy/templates/fav_column_summary.txt
 datacompy/templates/header.txt
-datacompy/templates/row_summary.txt
+datacompy/templates/row_summary.txt
+tests/test_core.py
+tests/test_sparkcompare.py
```

### Comparing `datacompy-0.8.4/setup.cfg` & `datacompy-0.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -7,38 +7,37 @@
 author = Ian Robertson, Dan Coates, Faisal Dosani
 author_email = faisal.dosani@capitalone.com
 license = Apache Software License
 maintainer = Faisal Dosani
 maintainer_email = faisal.dosani@capitalone.com
 url = https://github.com/capitalone/datacompy
 python_requires = 
-	>=3.7.0
+	>=3.8.0
 project_urls = 
 	Documentation = https://capitalone.github.io/datacompy/
 	Bug Tracker = https://github.com/capitalone/datacompy/issues
 	Source Code = https://github.com/capitalone/datacompy
 classifiers = 
 	Intended Audience :: Developers
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	pandas<=1.5.2,>=0.25.0
-	numpy<=1.24.1,>=1.11.3
+	pandas<=1.5.3,>=0.25.0
+	numpy<=1.24.2,>=1.22.0
 	ordered-set<=4.1.0,>=4.0.2
 
 [options.package_data]
 * = templates/*
 
 [options.extras_require]
 spark =
```

