# Comparing `tmp/ChildProject-0.1.0.tar.gz` & `tmp/ChildProject-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ChildProject/ChildProject/dist/.tmp-p5_nm356/ChildProject-0.1.0.tar", last modified: Mon Feb 20 15:20:21 2023, max compression
+gzip compressed data, was "/home/runner/work/ChildProject/ChildProject/dist/.tmp-ea3mva9p/ChildProject-0.1.1.tar", last modified: Thu May 11 09:39:35 2023, max compression
```

## Comparing `ChildProject-0.1.0.tar` & `ChildProject-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 15:20:21.000000 ChildProject-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject/
--rw-r--r--   0 runner    (1001) docker     (116)      116 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    70159 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/annotations.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    20403 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (116)    26958 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/converters.py
--rw-r--r--   0 runner    (1001) docker     (116)     9700 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject/pipelines/
--rw-r--r--   0 runner    (1001) docker     (116)      304 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5318 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (116)    10008 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/eafbuilder.py
--rw-r--r--   0 runner    (1001) docker     (116)    43331 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)    16388 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/metricsFunctions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1537 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)    14907 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/processors.py
--rw-r--r--   0 runner    (1001) docker     (116)    39571 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/samplers.py
--rw-r--r--   0 runner    (1001) docker     (116)    25384 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/pipelines/zooniverse.py
--rw-r--r--   0 runner    (1001) docker     (116)    30780 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/projects.py
--rw-r--r--   0 runner    (1001) docker     (116)     9628 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject/templates/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2753 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/templates/basic.etf
--rw-r--r--   0 runner    (1001) docker     (116)     3720 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/templates/basic.pfsx
--rw-r--r--   0 runner    (1001) docker     (116)     2844 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/templates/native.etf
--rw-r--r--   0 runner    (1001) docker     (116)     3753 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/templates/native.pfsx
--rw-r--r--   0 runner    (1001) docker     (116)     1903 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/templates/non-native.etf
--rw-r--r--   0 runner    (1001) docker     (116)     1931 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/templates/non-native.pfsx
--rw-r--r--   0 runner    (1001) docker     (116)    13192 2023-02-20 15:20:13.000000 ChildProject-0.1.0/ChildProject/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4942 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1354 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       60 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      310 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-20 15:20:21.000000 ChildProject-0.1.0/ChildProject.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2023-02-20 15:20:13.000000 ChildProject-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4942 2023-02-20 15:20:21.000000 ChildProject-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4341 2023-02-20 15:20:13.000000 ChildProject-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-20 15:20:21.000000 ChildProject-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2079 2023-02-20 15:20:13.000000 ChildProject-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 15:20:21.000000 ChildProject-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)    23543 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (116)     1835 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     2448 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (116)      560 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_documentation.py
--rw-r--r--   0 runner    (1001) docker     (116)     6263 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (116)     6940 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     1840 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (116)      866 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (116)     3626 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_reliability.py
--rw-r--r--   0 runner    (1001) docker     (116)     6030 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (116)     4648 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2418 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1690 2023-02-20 15:20:13.000000 ChildProject-0.1.0/tests/test_zooniverse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:39:35.000000 ChildProject-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73770 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/annotations.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20490 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26958 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9700 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5318 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10008 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/eafbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/fake_panoptes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42740 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17187 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/metricsFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14881 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39571 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40286 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/pipelines/zooniverse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35073 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/projects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9628 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/templates/basic.etf
+-rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/templates/basic.pfsx
+-rw-r--r--   0 runner    (1001) docker     (122)     2844 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/templates/native.etf
+-rw-r--r--   0 runner    (1001) docker     (122)     3753 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/templates/native.pfsx
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/templates/non-native.etf
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/templates/non-native.pfsx
+-rw-r--r--   0 runner    (1001) docker     (122)    13457 2023-05-11 09:39:19.000000 ChildProject-0.1.1/ChildProject/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4942 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-11 09:39:35.000000 ChildProject-0.1.1/ChildProject.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-11 09:39:19.000000 ChildProject-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4942 2023-05-11 09:39:35.000000 ChildProject-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4341 2023-05-11 09:39:19.000000 ChildProject-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 09:39:35.000000 ChildProject-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-05-11 09:39:19.000000 ChildProject-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:39:35.000000 ChildProject-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    26020 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6263 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8842 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2746 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_reliability.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6146 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5618 2023-05-11 09:39:19.000000 ChildProject-0.1.1/tests/test_zooniverse.py
```

### Comparing `ChildProject-0.1.0/ChildProject/annotations.py` & `ChildProject-0.1.1/ChildProject/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,20 +326,31 @@
             ovl_ranges = self.annotations[ovl_ranges][['set','annotation_filename']].values.tolist()
             errors.extend(
                 [
                     f"overlaps in the annotation index for the following [set, annotation_filename] list: {ovl_ranges}"
                 ]
             )
             
+        #check the index for bad range_onset range_offset
         ranges_invalid = self.annotations[(self.annotations['range_offset'] <= self.annotations['range_onset']) | (self.annotations['range_onset'] < 0)]
         if ranges_invalid.shape[0] > 0:
             errors.extend(
                 [f"annotation index does not verify range_offset > range_onset >= 0 for set <{line['set']}>, annotation filename <{line['annotation_filename']}>"
                   for line in ranges_invalid.to_dict(orient="records")]        
             )
+            
+        #if duration is in recordings.csv, check index for annotation segments overflowing recording duration
+        if self.project.recordings is not None and 'duration' in self.project.recordings.columns:
+            df = self.annotations.merge(self.project.recordings, how='left', on='recording_filename')
+            ranges_invalid = df[(df['range_offset'] > df['duration'])]
+            if ranges_invalid.shape[0] > 0:
+                errors.extend(
+                    [f"annotation index has an offset higher than recorded duration of the audio <{line['set']}>, annotation filename <{line['annotation_filename']}>"
+                      for line in ranges_invalid.to_dict(orient="records")]        
+                )
         
         warnings += self._check_for_outdated_merged_sets()
 
         return errors, warnings
 
     def validate_annotation(self, annotation: dict) -> Tuple[List[str], List[str]]:
         print(
@@ -599,30 +610,37 @@
         :param new_tiers: List of EAF tiers names. If specified, the corresponding EAF tiers will be imported.
         :type new_tiers: list[str], optional
         :param overwrite_existing: choose if lines with the same set and annotation_filename should be overwritten
         :type overwrite_existing: bool, optional
         :return: dataframe of imported annotations, as in :ref:`format-annotations`.
         :rtype: pd.DataFrame
         """
-        input_processed= input.copy()
-        
-        input_processed["range_onset"] = input_processed["range_onset"].astype(np.int64)
-        input_processed["range_offset"] = input_processed["range_offset"].astype(np.int64)
+        input_processed= input.copy().reset_index()
         
-        assert (input_processed["range_offset"] > input_processed["range_onset"]).all(), "range_offset must be greater than range_onset"
-        assert (input_processed["range_onset"] >= 0).all(), "range_onset must be greater or equal to 0"
-
         required_columns = {
             c.name
             for c in AnnotationManager.INDEX_COLUMNS
             if c.required and not c.generated
         }
 
         assert_dataframe("input", input_processed)
         assert_columns_presence("input", input_processed, required_columns)
+        
+        input_processed["range_onset"] = input_processed["range_onset"].astype(np.int64)
+        input_processed["range_offset"] = input_processed["range_offset"].astype(np.int64)
+        
+        assert (input_processed["range_offset"] > input_processed["range_onset"]).all(), "range_offset must be greater than range_onset"
+        assert (input_processed["range_onset"] >= 0).all(), "range_onset must be greater or equal to 0"
+        if "duration" in self.project.recordings.columns:
+            assert (input_processed["range_offset"] <= input_processed.merge(self.project.recordings,
+                                                                            how='left',
+                                                                            on='recording_filename',
+                                                                            validate='m:1'
+                                                                            ).reset_index()["duration"]
+            ).all(), "range_offset must be smaller than the duration of the recording"
 
         missing_recordings = input_processed[
             ~input_processed["recording_filename"].isin(
                 self.project.recordings["recording_filename"]
             )
         ]
         missing_recordings = missing_recordings["recording_filename"]
@@ -681,15 +699,15 @@
         else:
             errors = None
 
         self.read()
         self.annotations = pd.concat([self.annotations, imported], sort=False)
         #at this point, 2 lines with same set and annotation_filename can happen if specified overwrite,
         # dropping duplicates remove the first importation and keeps the more recent one
-        self.annotations = self.annotations.sort_values('imported_at').drop_duplicates(subset=["set","annotation_filename"], keep='last')
+        self.annotations = self.annotations.sort_values('imported_at').drop_duplicates(subset=["set","recording_filename","range_onset","range_offset"], keep='last')
         self.write()
         
         sets = set(input_processed['set'].unique())
         outdated_sets = self._check_for_outdated_merged_sets(sets= sets)
         for warning in outdated_sets:
             print("warning: {}".format(warning))
 
@@ -786,15 +804,21 @@
         current_path = os.path.join(self.project.path, "annotations", annotation_set)
         new_path = os.path.join(self.project.path, "annotations", new_set)
 
         if not os.path.exists(current_path):
             raise Exception("'{}' does not exists, aborting".format(current_path))
 
         if os.path.exists(new_path):
-            raise Exception("'{}' already exists, aborting".format(new_path))
+            if os.path.exists(os.path.join(new_path, 'raw')):
+                raise Exception("raw folder '{}' already exists, aborting".format(os.path.join(new_path, 'raw')))
+            if os.path.exists(os.path.join(new_path, 'converted')):
+                raise Exception("converted folder '{}' already exists, aborting".format(os.path.join(new_path, 'converted')))
+                
+        if (self.annotations[self.annotations["set"] == new_set].shape[0] > 0): 
+            raise Exception("'{}' set already exists in the index".format(new_set))
 
         if (
             self.annotations[self.annotations["set"] == annotation_set].shape[0] == 0
             and not ignore_errors
             and not recursive
         ):
             raise Exception(
@@ -827,14 +851,27 @@
                 os.path.join(current_path, "converted"),
                 os.path.join(new_path, "converted"),
             )
 
         self.annotations.loc[
             (self.annotations["set"] == annotation_set), "set"
         ] = new_set
+                
+        #find the merged from lines that should be updated and update them
+        if 'merged_from' in self.annotations.columns:
+            merged_from = self.annotations['merged_from'].astype(str).str.split(',')
+            matches = [False if not isinstance(s, list) else annotation_set in s for s in merged_from.values.tolist()]
+            
+            def update_mf(old_list, old, new):
+                res = set(old_list)
+                res.discard(old)
+                res.add(new)
+                return ','.join(res)
+            
+            self.annotations.loc[matches, 'merged_from'] = merged_from[matches].apply(partial(update_mf, old=annotation_set,new=new_set))
         self.write()
 
     def merge_annotations(
         self, left_columns, right_columns, columns, output_set, input, skip_existing: bool = False
     ):
         """From 2 DataFrames listing the annotation indexes to merge together (those indexes should come from
         the intersection of the left_set and right_set indexes), the listing of the columns
@@ -1384,33 +1421,55 @@
                 if missing_data == "warn":
                     print(f"warning: {error_message}")
                 else:
                     raise Exception(error_message)
 
         return pd.concat(stack) if len(stack) else pd.DataFrame()
 
-    def get_within_time_range(
-        self, annotations: pd.DataFrame, interval : TimeInterval, errors="raise"
+    def get_within_time_range(self,
+        annotations: pd.DataFrame,
+        interval : TimeInterval = None,
+        start_time: str = None,
+        end_time: str = None,
     ):
         """Clip all input annotations within a given HH:MM:SS clock-time range.
         Those that do not intersect the input time range at all are filtered out.
 
         :param annotations: DataFrame of input annotations to filter. The only columns that are required are: ``recording_filename``, ``range_onset``, and ``range_offset``.
         :type annotations: pd.DataFrame
         :param interval: Interval of hours to consider, contains the start hour and end hour
         :type interval: TimeInterval
-        :param errors: how to deal with invalid start_time values for the recordings. Takes the same values as ``pandas.to_datetime``.
-        :type errors: str
+        :param start_time: start_time to use in a HH:MM format, only used if interval is None, replaces the first value of interval
+        :type start_time: str
+        :param end_time: end_time to use in a HH:MM format, only used if interval is None, replaces the second value of interval
+        :type end_time: str
         :return: a DataFrame of annotations; \
         For each row, ``range_onset`` and ``range_offset`` are clipped within the desired clock-time range. \
         The clock-time corresponding to the onset and offset of each annotation \
         is stored in two newly created columns named ``range_onset_time`` and ``range_offset_time``. \
         If the input annotation exceeds 24 hours, one row per matching interval is returned. \
         :rtype: pd.DataFrame
         """
+        assert interval is not None or (start_time and end_time), "you must pass an interval or a start_time and end_time"
+        
+        if interval is None:
+            try:
+                start_dt = datetime.datetime.strptime(start_time, "%H:%M")
+            except:
+                raise ValueError(
+                    f"invalid value for start_time ('{start_time}'); should have HH:MM format instead"
+                )
+    
+            try:
+                end_dt = datetime.datetime.strptime(end_time, "%H:%M")
+            except:
+                raise ValueError(
+                    f"invalid value for end_time ('{end_time}'); should have HH:MM format instead"
+                )
+            interval = TimeInterval(start_dt,end_dt)
 
         assert_dataframe("annotations", annotations)
         assert_columns_presence(
             "annotations",
             annotations,
             {"recording_filename", "range_onset", "range_offset"},
         )
```

### Comparing `ChildProject-0.1.0/ChildProject/cmdline.py` & `ChildProject-0.1.1/ChildProject/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,15 +491,16 @@
         arg("--force", help="overwrite if column exists", action="store_true"),
     ]
 )
 def compute_durations(args):
     """creates a 'duration' column into metadata/recordings. duration is in ms"""
     project = ChildProject(args.source)
 
-    perform_validation(project, require_success=True, ignore_recordings=True)
+    #accumulate to false b/c we don't want to write confidential info into recordings.csv
+    perform_validation(project, require_success=True, ignore_recordings=True, accumulate=False)
 
     if "duration" in project.recordings.columns:
         if not args.force:
             print("duration exists, aborting")
             return
 
         project.recordings.drop(columns=["duration"], inplace=True)
@@ -509,18 +510,18 @@
     recordings = project.recordings.merge(
         durations[durations["recording_filename"] != "NA"],
         how="left",
         left_on="recording_filename",
         right_on="recording_filename",
     )
     recordings["duration"].fillna(0, inplace=True)
-    recordings["duration"] = recordings["duration"].astype(int)
-    recordings.to_csv(
-        os.path.join(project.path, "metadata/recordings.csv"), index=False
-    )
+    recordings["duration"] = recordings["duration"].astype("Int64")
+    
+    project.recordings = recordings.copy()
+    project.write_recordings()
     
 @subcommand(
     [
         arg("source", help="project path"),
         arg("audio1", help="name of the first audio file as it is indexed in recordings.csv in column <recording_filename>"),
         arg("audio2", help="name of the second audio file as it is indexed in recordings.csv in column <recording_filename>"),
         arg("--profile", help="which audio profile to use", default=""),
```

### Comparing `ChildProject-0.1.0/ChildProject/converters.py` & `ChildProject-0.1.1/ChildProject/converters.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/metrics.py` & `ChildProject-0.1.1/ChildProject/metrics.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/pipelines/anonymize.py` & `ChildProject-0.1.1/ChildProject/pipelines/anonymize.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/pipelines/eafbuilder.py` & `ChildProject-0.1.1/ChildProject/pipelines/eafbuilder.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/pipelines/metrics.py` & `ChildProject-0.1.1/ChildProject/pipelines/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,20 +226,17 @@
                 if index.shape[0]:
                     duration_set = (
                             index["range_offset"] - index["range_onset"]
                         ).sum()
                 else : duration_set = 0
                 row[1]["duration_{}".format(line["set"])] = duration_set
                 prev_set = curr_set            
-
-            if 'name' in line and not pd.isnull(line["name"]) and line["name"]: #the 'name' column exists and its value is not NaN or ''  => use the name given by the user
-                row[1][line["name"]] = line["callable"](annotations, duration_set, **line.drop(['callable', 'set','name'],errors='ignore').dropna().to_dict())[1]
-            else : # use the default name of the metric function
-                name, value = line["callable"](annotations, duration_set, **line.drop(['callable', 'set','name'],errors='ignore').dropna().to_dict())
-                row[1][name] = value
+                
+            name, value = line["callable"](annotations, duration_set, **line.drop(['callable', 'set'],errors='ignore').dropna().to_dict())
+            row[1][name] = value
         
         return row[1]
                 
     
     def extract(self):
         """from the initiated self.metrics, compute each row metrics (handles threading)
         Once the Metrics class is initialized, call this function to extract the metrics and populate self.metrics
@@ -356,18 +353,15 @@
             
         #this loop is for the purpose of checking for name duplicates in the metrics
         #we do a dry run on the first line with no annotations bc impractical to check in multiprocessing
         df = pd.DataFrame()
         duration_set = 0
         names = set()
         for i, line in self.metrics_list.iterrows():
-            if 'name' in line and not pd.isnull(line["name"]) and line["name"]: 
-                name = line["name"]
-            else : # use the default name of the metric function
-                name, value = line["callable"](df, duration_set, **line.drop(['callable', 'set','name'],errors='ignore').dropna().to_dict())
+            name, value = line["callable"](df, duration_set, **line.drop(['callable', 'set'],errors='ignore').dropna().to_dict())
                 
             if name in names:
                 raise ValueError('the metric name <{}> is used multiple times, make sure it is unique'.format(name))
             else:
                 names.add(name)
             
         #checking that columns added by the user are unique (e.g. date_iso may be different when extract by child_id), replace with NA if they are not
```

### Comparing `ChildProject-0.1.0/ChildProject/pipelines/metricsFunctions.py` & `ChildProject-0.1.1/ChildProject/pipelines/metricsFunctions.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,35 +12,48 @@
      - duration which is the duration of audio annotated in milliseconds
      - kwargs, whatever keyword parameter you chose to pass to the function (except 'name', 'callable', 'set' which can not be used). This will need to be given with the list of metrics when called
  - Wrap you function with the 'metricFunction' decorator to make it callable by the pipeline, read metricFunction help for more info
 """
 
 #error message in case of missing columns in annotations
 MISSING_COLUMNS = 'The given set <{}> does not have the required column <{}> for computing the {} metric'
+
+RESERVED = {'set','name','callable'} #arguments reserved usage. use other keyword labels.
     
-def metricFunction(args: set, columns: set, emptyValue = 0, name : str = None):
+def metricFunction(args: set, columns: set, emptyValue = 0, default_name : str = None):
     """Decorator for all metrics functions to make them ready to be called by the pipeline.
     
-    :param args: set of required keyword arguments for that function, raise ValueError if were not given
+    :param args: set of required keyword arguments for that function, raise ValueError if were not given \
+    you cannot use keywords [name, callale, set] as they are reserved
     :type args: set
     :param columns: set of required columns in the dataframe given, missing columns raise ValueError
     :type columns: set
     :param name: default name to use for the metric in the resulting dataframe. Every keyword argument found in the name will be replaced by its value (e.g. 'voc_speaker_ph' uses kwarg 'speaker' so if speaker = 'CHI', name will be 'voc_chi_ph'). if no name is given, the __name__ of the function is used
     :type name: str
     :param emptyValue: value to return when annotations are empty but the unit was annotated (e.g. 0 for counts like voc_speaker_ph , None for proportions like lp_n)
     :return: new function to substitute the metric function
     :rtype: Callable
     """
     def decorator(function):
+        for a in args:
+            if a in RESERVED: raise ValueError('Error when defining {} with required argument {}, you cannot use reserved keywords {}, change your required argument name'.format(function.__name__,a,RESERVED))
         @functools.wraps(function)
         def new_func(annotations: pd.DataFrame, duration: int, **kwargs):
             for arg in args:
                 if arg not in kwargs : raise ValueError('{} metric needs an argument <{}>'.format(function.__name__,arg))
-            metric_name = name
-            if not name : metric_name = function.__name__
+            #if a name is explicitly given, use it
+            if 'name' in kwargs and not pd.isnull(kwargs['name']) and kwargs['name']:
+                metric_name = kwargs['name']
+            #else if a default name for the function exists, use the function name
+            elif default_name:
+                metric_name = default_name
+            #else, no name was found, use the name of the function
+            else:
+                metric_name = function.__name__
+            
             metric_name_replaced = metric_name
             #metric_name is the basename used to designate this metric (voc_speaker_ph), metric_name_replaced replaces the values of kwargs
             #found in the name by their values, giving the metric name for that instance only (voc_chi_ph)
             for arg in kwargs:
                 metric_name_replaced = re.sub(arg , str(kwargs[arg]).lower(),metric_name_replaced)
             if annotations.shape[0]:
                 missing_columns = columns - set(annotations.columns)
```

### Comparing `ChildProject-0.1.0/ChildProject/pipelines/pipeline.py` & `ChildProject-0.1.1/ChildProject/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/pipelines/processors.py` & `ChildProject-0.1.1/ChildProject/pipelines/processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.recordings = Pipeline.recordings_from_list(recordings)
 
         self.input_profile = input_profile
 
         if self.input_profile:
             input_path = os.path.join(
                 self.project.path,
-                ChildProject.projects.ChildProject.CONVERTED_RECORDINGS,
+                ChildProject.projects.CONVERTED_RECORDINGS,
                 self.input_profile,
             )
 
             assert os.path.exists(
                 input_path
             ), f"provided input profile {input_profile} does not exist"
 
@@ -50,15 +50,15 @@
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         pipelines[cls.SUBCOMMAND] = cls
 
     def output_directory(self):
         return os.path.join(
             self.project.path,
-            ChildProject.projects.ChildProject.CONVERTED_RECORDINGS,
+            ChildProject.projects.CONVERTED_RECORDINGS,
             self.name,
         )
 
     def read_metadata(self):
         path = os.path.join(self.output_directory(), "recordings.csv")
 
         if os.path.exists(path):
```

### Comparing `ChildProject-0.1.0/ChildProject/pipelines/samplers.py` & `ChildProject-0.1.1/ChildProject/pipelines/samplers.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/pipelines/zooniverse.py` & `ChildProject-0.1.1/ChildProject/pipelines/zooniverse.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,30 +7,36 @@
 import os
 import pandas as pd
 import shutil
 import subprocess
 import sys
 import array
 import traceback
+import signal
+import re
+
 from typing import List
 from yaml import dump
 
+from functools import partial
+
 import matplotlib.pyplot as plt
 from matplotlib.ticker import ScalarFormatter
 from numpy import log10
 
 from pydub import AudioSegment
 from pydub.utils import get_array_type
 
 from parselmouth import Sound
 from parselmouth import SpectralAnalysisWindowShape
 
 import ChildProject
 from ChildProject.pipelines.pipeline import Pipeline
 from ChildProject.tables import assert_dataframe, assert_columns_presence
+from ChildProject.utils import retry_func
 
 from typing import Tuple
 
 import time
 
 
 def pad_interval(
@@ -258,14 +264,15 @@
             for key in parameters
             if key not in ["self", "kwargs"]
         ]
         parameters.extend([{key: kwargs[key]} for key in kwargs])
 
         self.destination = destination
         self.project = ChildProject.projects.ChildProject(path)
+        self.project.read()
 
         self.chunks_length = int(chunks_length)
         self.chunks_min_amount = int(chunks_min_amount)
         self.spectro = spectrogram
         self.profile = profile
 
         threads = int(threads)
@@ -308,16 +315,18 @@
                     "png": c.getbasename("png") if self.spectro else "NA",
                     "date_extracted": datetime.datetime.now().strftime(
                         "%Y-%m-%d %H:%M:%S"
                     ),
                     "uploaded": False,
                     "project_id": "",
                     "subject_set": "",
+                    "subject_set_id": pd.NA,
                     "zooniverse_id": 0,
                     "keyword": keyword,
+                    "dataset": self.project.experiment
                 }
                 for c in self.chunks
             ]
         )
 
         # shuffle chunks so that they can't be joined back together
         # based on Zooniverse subject IDs
@@ -347,30 +356,38 @@
         chunks: str,
         project_id: int,
         set_name: str,
         zooniverse_login="",
         zooniverse_pwd="",
         amount: int = 1000,
         ignore_errors: bool = False,
+        record_orphan: bool = False,
+        test_endpoint: bool = False,
         **kwargs
     ):
         """Uploads ``amount`` audio chunks from the CSV dataframe `chunks` to a zooniverse project.
 
         :param chunks: path to the chunk CSV dataframe
         :type chunks: [type]
         :param project_id: zooniverse project id
         :type project_id: int
         :param set_name: name of the subject set
         :type set_name: str
         :param zooniverse_login: zooniverse login. If not specified, the program attempts to get it from the environment variable ``ZOONIVERSE_LOGIN`` instead, defaults to ''
         :type zooniverse_login: str, optional
         :param zooniverse_pwd: zooniverse password. If not specified, the program attempts to get it from the environment variable ``ZOONIVERSE_PWD`` instead, defaults to ''
         :type zooniverse_pwd: str, optional
-        :param amount: amount of chunks to upload, defaults to 0
+        :param amount: amount of chunks to upload, defaults to 1000
         :type amount: int, optional
+        :param ignore_errors: carry on with the upload even if a clip fails, the csv will be updated accordingly, single clip errors are ignored but errors that will repeat (e.g. maximum number of subjects uploaded) will still exit
+        :type ignore_errors: bool, optional
+        :param record_orphan: when true, chunks that are correctly uploaded but not linked to a subject set (orphan) have their line updated with the subject id, project id and Uploaded flag at True, but subject_set empty. link_orphan_subjects can be used to reattempt it. If false, the chunk is considered not uploaded.   
+        :type record_orphan: bool, optional
+        :param test_endpoint: run this command for tests, operations with zooniverse arefaked and considered succesfull
+        :type test_endpoint: bool, optional
         """
 
         self.chunks_file = chunks
         self.get_credentials(zooniverse_login, zooniverse_pwd)
 
         metadata_location = os.path.join(self.chunks_file)
         try:
@@ -383,100 +400,351 @@
         assert_dataframe("chunks", self.chunks)
         assert_columns_presence(
             "chunks",
             self.chunks,
             {"recording_filename", "onset", "offset", "uploaded", "mp3"},
         )
         
-        from panoptes_client import Panoptes, Project, Subject, SubjectSet
+        if test_endpoint:
+            from ChildProject.pipelines.fake_panoptes import Panoptes, Project, Subject, SubjectSet, PanoptesAPIException, reset_tests, TEST_MAX_SUBJECT
+            reset_tests()
+            if test_endpoint == 2: Subject.max_subjects = TEST_MAX_SUBJECT
+        else:
+            from panoptes_client import Panoptes, Project, Subject, SubjectSet
+            from panoptes_client.panoptes import PanoptesAPIException
+
 
         Panoptes.connect(username=self.zooniverse_login, password=self.zooniverse_pwd)
         zooniverse_project = Project(project_id)
 
-        subjects_metadata = []
-        uploaded = 0
-
+        self.subjects_metadata = []
+    
         subject_set = None
 
         for ss in zooniverse_project.links.subject_sets:
             if ss.display_name == set_name:
                 subject_set = ss
 
         if subject_set is None:
             subject_set = SubjectSet()
             subject_set.links.project = zooniverse_project
             subject_set.display_name = set_name
             subject_set.save()
 
-        subjects = []
-
         chunks_to_upload = self.chunks[self.chunks["uploaded"] == False].head(amount)
         chunks_to_upload = chunks_to_upload.to_dict(orient="index")
 
         if len(chunks_to_upload) == 0:
             print("nothing left to upload.")
             return
+        
+        self.orphan_chunks = []
+    
+        #handling sigterm and sigint to write to a csv file before exiting to keep track of what was done
+        #this is hard to test on a controlled environment, for now, manual testing is required
+        original_sigint_handler = signal.getsignal(signal.SIGINT)
+        original_sigterm_handler = signal.getsignal(signal.SIGTERM)
+        signal.signal(signal.SIGINT, partial(self.exit_upload, rec_orphan=record_orphan, sub_set=set_name))
+        signal.signal(signal.SIGTERM, partial(self.exit_upload, rec_orphan=record_orphan, sub_set=set_name))
+        
+        max_subjects_error = re.compile('User has uploaded \d+ subjects of \d+ maximum')
 
         for chunk_index in chunks_to_upload:
             chunk = chunks_to_upload[chunk_index]
 
             print(
                 "uploading chunk {} ({},{})".format(
                     chunk["recording_filename"], chunk["onset"], chunk["offset"]
                 )
             )
 
-            subject = Subject()
-            subject.links.project = zooniverse_project
-            subject.add_location(
-                os.path.join(os.path.dirname(self.chunks_file), "chunks", chunk["mp3"])
-            )
-            subject.metadata["date_extracted"] = chunk["date_extracted"]
-
             try:
+                #we take the mp3 file as the is the format supported by zooniverse
+                subject = Subject()
+                subject.links.project = zooniverse_project
+                subject.add_location(
+                    os.path.join(os.path.dirname(self.chunks_file), "chunks", chunk["mp3"])
+                )
+                subject.metadata["date_extracted"] = chunk["date_extracted"]
+                subject.metadata["dataset"] = chunk["dataset"] if 'dataset' in chunk.keys() else pd.NA
+                subject.metadata["filename"] = chunk["mp3"]
+
                 subject.save()
             except Exception as e:
                 print(
                     "failed to save chunk {}. an exception has occured:\n{}".format(
                         chunk_index, str(e)
                     )
                 )
                 print(traceback.format_exc())
 
+                if ignore_errors and not re.fullmatch(max_subjects_error, str(e)):
+                    continue
+                else:
+                    print("subject upload halting here.")
+                    break
+                
+            try: 
+                retry_func(subject_set.add, PanoptesAPIException, 3, subjects=subject)              
+            except PanoptesAPIException as e:
+                print(
+                    "failed to add subject {} to subject_set {}. an exception has occured:\n{}".format(
+                        chunk_index, subject_set.display_name, str(e)
+                    )
+                )
+                print(traceback.format_exc())
+                
+                chunk["index"] = chunk_index
+                chunk["zooniverse_id"] = str(subject.id)
+                chunk["project_id"] = str(project_id)
+                chunk["subject_set"] = ""
+                chunk['subject_set_id'] = pd.NA
+                chunk["uploaded"] = True
+                self.orphan_chunks.append(chunk)
+                
                 if ignore_errors:
                     continue
                 else:
                     print("subject upload halting here.")
                     break
 
-            subjects.append(subject)
-
             chunk["index"] = chunk_index
             chunk["zooniverse_id"] = str(subject.id)
             chunk["project_id"] = str(project_id)
             chunk["subject_set"] = str(subject_set.display_name)
+            chunk["subject_set_id"] = str(subject_set.id)
             chunk["uploaded"] = True
-            subjects_metadata.append(chunk)
+            self.subjects_metadata.append(chunk)
 
-        if len(subjects) == 0:
+        if len(self.subjects_metadata) + len(self.orphan_chunks) == 0:
             return
 
-        subject_set.add(subjects)
+        if len(self.subjects_metadata) : self.chunks.update(pd.DataFrame(self.subjects_metadata).set_index("index"))
+        
+        if record_orphan and len(self.orphan_chunks): 
+            self.chunks.update(pd.DataFrame(self.orphan_chunks).set_index("index"))
 
-        self.chunks.update(pd.DataFrame(subjects_metadata).set_index("index"))
+            print("WARNING: {} chunks were uploaded but not linked to the subject set {}. To attempt to relink them, try link_orphan_subjects".format(len(self.orphan_chunks), subject_set.display_name))
 
         self.chunks.to_csv(self.chunks_file)
+        
+        signal.signal(signal.SIGINT, original_sigint_handler)
+        signal.signal(signal.SIGTERM, original_sigterm_handler)
+        
+    def exit_upload(self, *args, rec_orphan, sub_set):
+        if len(self.subjects_metadata) + len(self.orphan_chunks) != 0:
+            if len(self.subjects_metadata) : self.chunks.update(pd.DataFrame(self.subjects_metadata).set_index("index"))
+            
+            if rec_orphan and len(self.orphan_chunks): 
+                self.chunks.update(pd.DataFrame(self.orphan_chunks).set_index("index"))
+                print("WARNING: {} chunks were uploaded but not linked to the subject set {}. To attempt to relink them, try link_orphan_subjects".format(len(self.orphan_chunks), sub_set))
+                
+            self.chunks.to_csv(self.chunks_file)
+            
+        print("Signal interruption {}, exited gracefully".format(args[0]))
+        sys.exit(0)
+        
+        
+    def link_orphan_subjects(
+        self,
+        chunks: str,
+        project_id: int,
+        set_name: str,
+        zooniverse_login="",
+        zooniverse_pwd="",
+        ignore_errors: bool = False,       
+        test_endpoint: bool = False,
+        **kwargs
+    ):
+        """Attempts to link subjects that have been uploaded but not linked to a subject set in zooniverse
+        from the CSV dataframe `chunks` to a zooniverse project (Attempts are made on chunks that have a zooniverse_id,
+        a project_id and uploaded at True but no subject_set )
+
+        :param chunks: path to the chunk CSV dataframe
+        :type chunks: [type]
+        :param project_id: zooniverse project id
+        :type project_id: int
+        :param set_name: name of the subject set
+        :type set_name: str
+        :param zooniverse_login: zooniverse login. If not specified, the program attempts to get it from the environment variable ``ZOONIVERSE_LOGIN`` instead, defaults to ''
+        :type zooniverse_login: str, optional
+        :param zooniverse_pwd: zooniverse password. If not specified, the program attempts to get it from the environment variable ``ZOONIVERSE_PWD`` instead, defaults to ''
+        :type zooniverse_pwd: str, optional
+        :param amount: amount of chunks to upload, defaults to 0
+        :type amount: int, optional
+        :param ignore_errors: carry on with the upload even if a clip fails, the csv will be updated accordingly
+        :type ignore_errors: bool, optional
+        :param test_endpoint: run this command for tests, operations with zooniverse arefaked and considered succesfull
+        :type test_endpoint: bool, optional
+        """
+        
+        self.chunks_file = chunks
+        self.get_credentials(zooniverse_login, zooniverse_pwd)
+
+        metadata_location = os.path.join(self.chunks_file)
+        try:
+            self.chunks = pd.read_csv(metadata_location, index_col="index")
+        except:
+            raise Exception(
+                "cannot read chunk metadata from {}.".format(metadata_location)
+            )
+
+        assert_dataframe("chunks", self.chunks)
+        assert_columns_presence(
+            "chunks",
+            self.chunks,
+            {"recording_filename", "onset", "offset", "uploaded", "mp3", "zooniverse_id", "project_id", "subject_set"},
+        )
+        
+        if test_endpoint:
+            from ChildProject.pipelines.fake_panoptes import Panoptes, Project, Subject, SubjectSet, PanoptesAPIException, reset_tests
+            reset_tests() 
+        else:
+            from panoptes_client import Panoptes, Project, Subject, SubjectSet
+            from panoptes_client.panoptes import PanoptesAPIException
+
+        Panoptes.connect(username=self.zooniverse_login, password=self.zooniverse_pwd)
+        zooniverse_project = Project(project_id)
+
+        subjects_metadata = []
+
+        subject_set = None
+
+        for ss in zooniverse_project.links.subject_sets:
+            if ss.display_name == set_name:
+                subject_set = ss
+
+        if subject_set is None:
+            subject_set = SubjectSet()
+            subject_set.links.project = zooniverse_project
+            subject_set.display_name = set_name
+            subject_set.save()
+
+        # select chunks that are uploaded, have an id and project but no set
+        chunks_to_link = self.chunks[(self.chunks["uploaded"] == True) &
+                                      (~self.chunks['zooniverse_id'].isnull()) &
+                                      (~self.chunks['project_id'].isnull()) &
+                                      (self.chunks['subject_set'].isnull())]
+        chunks_to_link = chunks_to_link.to_dict(orient="index")
+
+        if len(chunks_to_link) == 0:
+            print("no orphan chunks to link.")
+            return
+
+        for chunk_index in chunks_to_link:
+            chunk = chunks_to_link[chunk_index]
+
+            print(
+                "linking chunk {} ({},{})".format(
+                    chunk["recording_filename"], chunk["onset"], chunk["offset"]
+                )
+            )
+
+            try:
+                subject = Subject.find(chunk['zooniverse_id'])
+                
+            except Exception as e:
+                print(
+                    "Could not find subject {}. an exception has occured:\n{}".format(
+                        chunk['zooniverse_id'], str(e)
+                    )
+                )
+                print(traceback.format_exc())
+
+                if ignore_errors:
+                    continue
+                else:
+                    print("subject linking halting here.")
+                    break
+                
+            try: 
+                retry_func(subject_set.add, PanoptesAPIException, 3, subjects=subject)                
+            except PanoptesAPIException as e:
+                print(
+                    "failed to add subject {} to subject_set {}. an exception has occured:\n{}".format(
+                        chunk_index, subject_set.display_name, str(e)
+                    )
+                )
+                print(traceback.format_exc())
+                
+                if ignore_errors and str(e):
+                    continue
+                else:
+                    print("subject upload halting here.")
+                    break
+
+            chunk["index"] = chunk_index
+            chunk["subject_set"] = str(subject_set.display_name)
+            chunk["subject_set_id"] = str(subject_set.id)
+            subjects_metadata.append(chunk)
+
+        if len(subjects_metadata):
+            tmp = pd.DataFrame(subjects_metadata)
+            print(tmp.columns)
+            print(tmp)
+            self.chunks.update(pd.DataFrame(subjects_metadata).set_index("index"))
+
+            self.chunks.to_csv(self.chunks_file)
+            
+        print("linked {}/{} subjects".format(len(subjects_metadata),len(chunks_to_link)))
+        
+    def reset_orphan_subjects(
+        self,
+        chunks: str,
+        **kwargs
+    ):
+        """Look for orphan subjects and considers them to be not uploaded, This is to be done either if the oprhan
+        subjects were deleted from zooniverse or if they are not usable anymore. The next upload will try to push 
+        them to zooniverse as new subjects.
+
+        :param chunks: path to the chunk CSV dataframe
+        :type chunks: [type]
+        """
+        
+        self.chunks_file = chunks
+
+        metadata_location = os.path.join(self.chunks_file)
+        try:
+            self.chunks = pd.read_csv(metadata_location, index_col="index")
+        except:
+            raise Exception(
+                "cannot read chunk metadata from {}.".format(metadata_location)
+            )
+
+        assert_dataframe("chunks", self.chunks)
+        assert_columns_presence(
+            "chunks",
+            self.chunks,
+            {"recording_filename", "onset", "offset", "uploaded", "mp3", "zooniverse_id", "project_id", "subject_set"},
+        )
+
+        # select chunks that are uploaded, have an id and project but no set
+        selection = ((self.chunks["uploaded"] == True) &
+                      (~self.chunks['zooniverse_id'].isnull()) &
+                      (~self.chunks['project_id'].isnull()) &
+                      (self.chunks['subject_set'].isnull()))
+
+        self.chunks.loc[selection , ['uploaded','zooniverse_id','project_id']] = (False, "", "") 
+
+        nb_reset = selection[selection == True]
+        if nb_reset.shape[0]:
+            self.chunks.to_csv(self.chunks_file)
+            
+            print("reset {} orphan subjects".format(nb_reset))
+        else:
+            print("no orphan subject to reset".format(nb_reset))
 
     def retrieve_classifications(
         self,
         destination: str,
         project_id: int,
         zooniverse_login: str = "",
         zooniverse_pwd: str = "",
         chunks: List[str] = [],
+        test_endpoint: bool = False,
         **kwargs
     ):
 
         """Retrieve classifications from Zooniverse as a CSV dataframe.
         They will be matched with the original chunks metadata if the path one 
         or more chunk metadata files is provided.
 
@@ -489,15 +757,20 @@
         :param zooniverse_pwd: zooniverse password. If not specified, the program attempts to get it from the environment variable ``ZOONIVERSE_PWD`` instead, defaults to ''
         :type zooniverse_pwd: str, optional
         :param chunks: the list of chunk metadata files to match the classifications to. If provided, only the classifications that have a match will be returned.
         :type chunks: List[str], optional
         """
         self.get_credentials(zooniverse_login, zooniverse_pwd)
 
-        from panoptes_client import Panoptes, Project, Classification
+        # if used in tests, use the fake functions
+        if test_endpoint:
+            from ChildProject.pipelines.fake_panoptes import Panoptes, Project, Classification
+        else:
+            from panoptes_client import Panoptes, Project, Classification
+            
         Panoptes.connect(username=self.zooniverse_login, password=self.zooniverse_pwd)
         project = Project(project_id)
 
         answers_translation_table = []
         for workflow in project.links.workflows:
             workflow_id = workflow.id
             for task_id in workflow.tasks:
@@ -556,21 +829,26 @@
         classifications.set_index("id").to_csv(destination)
 
     def run(self, action, **kwargs):
         if action == "extract-chunks":
             return self.extract_chunks(**kwargs)
         elif action == "upload-chunks":
             return self.upload_chunks(**kwargs)
+        elif action == "link-orphan-subjects":
+            return self.link_orphan_subjects(**kwargs)
+        elif action == "reset-orphan-subjects":
+            return self.reset_orphan_subjects(**kwargs)
         elif action == "retrieve-classifications":
             return self.retrieve_classifications(**kwargs)
 
     @staticmethod
     def setup_parser(parser):
         subparsers = parser.add_subparsers(help="action", dest="action")
 
+        """extract chunks parser"""
         parser_extraction = subparsers.add_parser(
             "extract-chunks",
             help="extract chunks to <destination>, and exports the metadata inside of this directory",
         )
         parser_extraction.add_argument("path", help="path to the dataset")
         parser_extraction.add_argument(
             "--keyword", help="export keyword", required=True
@@ -601,15 +879,17 @@
             "--profile",
             help="Recording profile to extract the audio clips from. If not specified, raw recordings will be used",
             default="",
         )
         parser_extraction.add_argument(
             "--threads", help="how many threads to run on", default=0, type=int
         )
-
+        
+        
+        """upload subjects parser"""
         parser_upload = subparsers.add_parser(
             "upload-chunks", help="upload chunks and updates chunk state"
         )
         parser_upload.add_argument(
             "--chunks", help="path to the chunk CSV dataframe", required=True
         )
         parser_upload.add_argument(
@@ -636,15 +916,61 @@
             default="",
         )
         parser_upload.add_argument(
             "--ignore-errors",
             help="keep uploading even when a subject fails to upload for some reason",
             action="store_true",
         )
-
+        parser_upload.add_argument(
+            "--record-orphan",
+            help="list correctly create subjects as uploaded even if linking to a subject set failed",
+            action="store_true",
+        )
+        
+        
+        """linking orphan subjects parser"""
+        parser_link_subjects = subparsers.add_parser(
+            "link-orphan-subjects", help="upload chunks and updates chunk state"
+        )
+        parser_link_subjects.add_argument(
+            "--chunks", help="path to the chunk CSV dataframe", required=True
+        )
+        parser_link_subjects.add_argument(
+            "--project-id", help="zooniverse project id", required=True, type=int
+        )
+        parser_link_subjects.add_argument(
+            "--set-name", help="subject set display name", required=True
+        )
+        parser_link_subjects.add_argument(
+            "--zooniverse-login",
+            help="zooniverse login. If not specified, the program attempts to get it from the environment variable ZOONIVERSE_LOGIN instead",
+            default="",
+        )
+        parser_link_subjects.add_argument(
+            "--zooniverse-pwd",
+            help="zooniverse password. If not specified, the program attempts to get it from the environment variable ZOONIVERSE_PWD instead",
+            default="",
+        )
+        parser_link_subjects.add_argument(
+            "--ignore-errors",
+            help="keep uploading even when a subject fails to upload for some reason",
+            action="store_true",
+        )
+        
+        
+        """reset orphan subjects parser"""
+        parser_reset_orphan = subparsers.add_parser(
+            "reset-orphan-subjects", help="upload chunks and updates chunk state"
+        )
+        parser_reset_orphan.add_argument(
+            "--chunks", help="path to the chunk CSV dataframe", required=True
+        )
+        
+        
+        """retrieve classifications parser"""
         parser_retrieve = subparsers.add_parser(
             "retrieve-classifications",
             help="retrieve classifications and save them as <destination>",
         )
         parser_retrieve.add_argument(
             "--destination", help="output CSV dataframe destination", required=True
         )
```

### Comparing `ChildProject-0.1.0/ChildProject/projects.py` & `ChildProject-0.1.1/ChildProject/projects.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,26 +12,37 @@
     IndexColumn,
     is_boolean,
     assert_dataframe,
     assert_columns_presence,
 )
 from .utils import get_audio_duration, path_is_parent
 
+RAW_RECORDINGS = os.path.normpath("recordings/raw")
+CONVERTED_RECORDINGS = os.path.normpath("recordings/converted")
+STANDARD_SAMPLE_RATE = 16000
+STANDARD_PROFILE = 'standard' # profile that is expected to contain the standardized audios (16kHz). The existence and sampling rates of this profile are checked when <validating this profile> or <validating without profile and the raw recordings are not 16kHz>.
+
+METADATA_FOLDER = 'metadata'
+CHILDREN_CSV = 'children.csv'
+RECORDINGS_CSV = 'recordings.csv'
+
+PROJECT_FOLDERS = ["recordings", "annotations", "metadata", "doc", "scripts"]
+
 
 class ChildProject:
     """ChildProject instance
     This class is a representation of a ChildProject dataset
 
     Constructor parameters:
 
     :param path: path to the root of the dataset.
     :type path: str
     :param enforce_dtypes: enforce dtypes on children/recordings dataframes, defaults to False
     :type enforce_dtypes: bool, optional
-    :param ignore_discarded: ignore entries such that discard=1, defaults to False
+    :param ignore_discarded: ignore entries such that discard=1, defaults to True
     :type ignore_discarded: bool, optional
     
     Attributes:
     :param path: path to the root of the dataset.
     :type path: str
     :param recordings: pandas dataframe representation of this dataset metadata/recordings.csv 
     :type recordings: class:`pd.DataFrame`
@@ -253,26 +264,22 @@
         IndexColumn(name="values", description="a summary of authorized values"),
         IndexColumn(name="scope", description="which group of users has access to it"),
         IndexColumn(
             name="annotation_set",
             description="for annotations: which set(s) contain this variable",
         ),
     ]
-
-    RAW_RECORDINGS = os.path.normpath("recordings/raw")
-    CONVERTED_RECORDINGS = os.path.normpath("recordings/converted")
-    STANDARD_SAMPLE_RATE = 16000
-    STANDARD_PROFILE = 'standard' # profile that is expected to contain the standardized audios (16kHz). The existence and sampling rates of this profile are checked when <validating this profile> or <validating without profile and the raw recordings are not 16kHz>.
-
-    PROJECT_FOLDERS = ["recordings", "annotations", "metadata", "doc", "scripts"]
+    
+    REC_COL_REF = {c.name: c for c in RECORDINGS_COLUMNS}
 
     def __init__(
-        self, path: str, enforce_dtypes: bool = False, ignore_discarded: bool = False
+        self, path: str, enforce_dtypes: bool = False, ignore_discarded: bool = True
     ):
         self.path = path
+        self.experiment = None
         self.enforce_dtypes = enforce_dtypes
         self.ignore_discarded = ignore_discarded
 
         self.errors = []
         self.warnings = []
         self.children = None
         self.recordings = None
@@ -286,15 +293,15 @@
         self,
         table: str,
         df: pd.DataFrame,
         columns: list,
         merge_column: str,
         verbose=False,
     ) -> pd.DataFrame:
-        md_path = os.path.join(self.path, "metadata", table)
+        md_path = os.path.join(self.path, METADATA_FOLDER, table)
 
         if not os.path.exists(md_path):
             return df
 
         md = pd.DataFrame(
             [
                 {"path": f, "basename": os.path.basename(f)}
@@ -350,73 +357,130 @@
                     dataframe, how="left", left_on=merge_column, right_on=merge_column
                 )
                 .set_index("line")
             )
 
         return df
 
-    def read(self, verbose=False):
-        """Read the metadata
+    def read(self, verbose=False, accumulate=True):
+        """Read the metadata from the project and stores it in recordings and children attributes
+        
+        :param verbose: read with additional output
+        :type verbose: bool
+        :param accumulate: add metadata from subfolders (usually confidential metadata)
+        :type accumulate: bool
         """
         self.ct = IndexTable(
             "children",
-            os.path.join(self.path, "metadata","children.csv"),
+            os.path.join(self.path, METADATA_FOLDER,CHILDREN_CSV),
             self.CHILDREN_COLUMNS,
             enforce_dtypes=self.enforce_dtypes,
         )
         self.rt = IndexTable(
             "recordings",
-            os.path.join(self.path, "metadata","recordings.csv"),
+            os.path.join(self.path, METADATA_FOLDER,RECORDINGS_CSV),
             self.RECORDINGS_COLUMNS,
             enforce_dtypes=self.enforce_dtypes,
         )
 
         self.children = self.ct.read()
         self.recordings = self.rt.read()
 
         # accumulate additional metadata (optional)
-        self.ct.df = self.accumulate_metadata(
-            "children", self.children, self.CHILDREN_COLUMNS, "child_id", verbose
-        )
-        self.rt.df = self.accumulate_metadata(
-            "recordings",
-            self.recordings,
-            self.RECORDINGS_COLUMNS,
-            "recording_filename",
-            verbose,
-        )
+        if accumulate:
+            self.ct.df = self.accumulate_metadata(
+                "children", self.children, self.CHILDREN_COLUMNS, "child_id", verbose
+            )
+            self.rt.df = self.accumulate_metadata(
+                "recordings",
+                self.recordings,
+                self.RECORDINGS_COLUMNS,
+                "recording_filename",
+                verbose,
+            )
 
         if self.ignore_discarded and "discard" in self.ct.df:
-            self.ct.df = self.ct.df[self.ct.df["discard"].astype(str) == "1"]
+            self.ct.df['discard'] = self.ct.df["discard"].apply(np.nan_to_num).astype(int, errors='ignore')
+            self.ct.df = self.ct.df[self.ct.df["discard"].astype(str) != "1"]
 
         if self.ignore_discarded and "discard" in self.rt.df:
-            self.rt.df = self.rt.df[self.rt.df["discard"].astype(str) == "1"]
+            self.rt.df['discard'] = self.rt.df["discard"].apply(np.nan_to_num).astype(int, errors='ignore')
+            self.rt.df = self.rt.df[self.rt.df["discard"].astype(str) != "1"]
 
         self.children = self.ct.df
         self.recordings = self.rt.df
+        
+        exp = self.children.iloc[0]['experiment']
+        exp_values = set(self.children['experiment'].unique()).union(set(self.recordings['experiment'].unique()))
+        if len(exp_values) > 1:
+            raise ValueError(f"Column <experiment> must be unique across the dataset, in both children.csv and recordings.csv , {len(exp_values)} different values were found: {exp_values}")
+        self.experiment = exp
+        
+    def write_recordings(self, keep_discarded: bool = True, keep_original_columns: bool = True):
+        """
+        Write self.recordings to the recordings csv file of the dataset.
+        !! if `read()` was done with `accumulate` , you may write confidential information in recordings.csv !!
+        
+        :param keep_discarded: if True, the lines in the csv that are discarded by the dataset are kept when writing. defaults to True (when False, discarded lines disappear from the dataset)
+        :type keep_discarded: bool, optional
+        :param keep_original_columns: if True, deleting columns in the recordings dataframe will not result in them disappearing from the csv file (if false, only the current columns are kept)
+        :type keep_original_columns: bool, optional
+        :return: dataframe that was written to the csv file
+        :rtype: pandas.DataFrame
+        """
+        if self.recordings is None:
+            #logger to add (can not write recordings file as recordings is not initialized)
+            return None
+        #get the file as reference point
+        current_csv = pd.read_csv(os.path.join(self.path, METADATA_FOLDER,RECORDINGS_CSV))
+        
+        if 'discard' in current_csv.columns and keep_discarded:
+            # put the discard column into a usable form
+            current_csv['discard'] = current_csv['discard'].apply(np.nan_to_num).astype(int, errors='ignore')
+            # keep the discarded lines somewhere
+            discarded_recs = current_csv[current_csv['discard'].astype(str) == "1"]
+            
+            recs_to_write = pd.concat([self.recordings,discarded_recs])
+            recs_to_write = recs_to_write.astype(self.recordings.dtypes.to_dict())
+        else:
+            recs_to_write = self.recordings
+            
+        if keep_original_columns:
+            columns = current_csv.columns
+            for new in self.recordings.columns:
+                if new not in columns : columns = columns.append(pd.Index([new]))
+        else:
+            columns = self.recordings.columns
+            
+        recs_to_write.sort_index().to_csv(os.path.join(self.path, METADATA_FOLDER, RECORDINGS_CSV),columns = columns,index=False)
+        return recs_to_write
 
-    def validate(self, ignore_recordings: bool = False, profile: str = None) -> tuple:
+    def validate(self, ignore_recordings: bool = False, profile: str = None, accumulate: bool = True) -> tuple:
         """Validate a dataset, returning all errors and warnings.
 
         :param ignore_recordings: if True, no errors will be returned for missing recordings.
         :type ignore_recordings: bool, optional
+        :param profile: profile of recordings to use
+        :type profile: str, optional
+        :param accumulate: use accumulated metadata (usually confidential metadata if present)
+        :type accumualte: bool, optional
         :return: A tuple containing the list of errors, and the list of warnings.
         :rtype: a tuple of two lists
         """
         self.errors = []
         self.warnings = []
 
         directories = [d for d in os.listdir(self.path) if os.path.isdir(self.path)]
 
         for rd in self.REQUIRED_DIRECTORIES:
             if rd not in directories:
                 self.errors.append("missing directory {}.".format(rd))
 
         # check tables
-        self.read(verbose=True)
+        self.read(verbose=True, accumulate=accumulate)
 
         errors, warnings = self.ct.validate()
         self.errors += errors
         self.warnings += warnings
 
         errors, warnings = self.rt.validate()
         self.errors += errors
@@ -442,42 +506,42 @@
 
                     try:
                         path = self.get_recording_path(raw_filename, profile)
                     except:
                         if profile:
                             profile_metadata = os.path.join(
                                 self.path,
-                                self.CONVERTED_RECORDINGS,
+                                CONVERTED_RECORDINGS,
                                 profile,
-                                "recordings.csv",
+                                RECORDINGS_CSV,
                             )
                             self.errors.append(
                                 f"failed to recover the path for recording '{raw_filename}' and profile '{profile}'. Does the profile exist? Does {profile_metadata} exist?"
                             )
                         continue
 
                     if os.path.exists(path):
                         if not profile:
                             info = mediainfo(path)
-                            if int(info['sample_rate']) != self.STANDARD_SAMPLE_RATE:
+                            if int(info['sample_rate']) != STANDARD_SAMPLE_RATE:
                                 try:
-                                    std_path = self.get_recording_path(raw_filename, self.STANDARD_PROFILE)
+                                    std_path = self.get_recording_path(raw_filename, STANDARD_PROFILE)
                                     if os.path.exists(std_path):
                                         std_info = mediainfo(std_path)
-                                        if 'sample_rate' in std_info and int(std_info['sample_rate']) != self.STANDARD_SAMPLE_RATE:
-                                            self.warnings.append(f"converted version of recording '{raw_filename}' at '{std_path}' has unexpected sampling rate {std_info['sample_rate']}Hz when {self.STANDARD_SAMPLE_RATE}Hz is expected for profile {self.STANDARD_PROFILE}")
+                                        if 'sample_rate' in std_info and int(std_info['sample_rate']) != STANDARD_SAMPLE_RATE:
+                                            self.warnings.append(f"converted version of recording '{raw_filename}' at '{std_path}' has unexpected sampling rate {std_info['sample_rate']}Hz when {STANDARD_SAMPLE_RATE}Hz is expected for profile {STANDARD_PROFILE}")
                                     else:
-                                        self.warnings.append(f"recording '{raw_filename}' at '{path}' has a non standard sampling rate {info['sample_rate']}Hz and no converted version found in the standard profile at {std_path}. The file content may not be downloaded. you can create the missing standard converted audios with 'child-project process {self.path} {self.STANDARD_PROFILE} basic --format=wav --sampling={self.STANDARD_SAMPLE_RATE} --codec=pcm_s16le --skip-existing'")
+                                        self.warnings.append(f"recording '{raw_filename}' at '{path}' has a non standard sampling rate {info['sample_rate']}Hz and no converted version found in the standard profile at {std_path}. The file content may not be downloaded. you can create the missing standard converted audios with 'child-project process {self.path} {STANDARD_PROFILE} basic --format=wav --sampling={STANDARD_SAMPLE_RATE} --codec=pcm_s16le --skip-existing'")
                                 except:
-                                    profile_metadata = os.path.join(self.path,self.CONVERTED_RECORDINGS,self.STANDARD_PROFILE,"recordings.csv",)
-                                    self.warnings.append(f"recording '{raw_filename}' at '{path}' has a non standard sampling rate of {info['sample_rate']}Hz and no standard conversion in profile {self.STANDARD_PROFILE} was found. Does the standard profile exist? Does {profile_metadata} exist? you can create the standard profile with 'child-project process {self.path} {self.STANDARD_PROFILE} basic --format=wav --sampling={self.STANDARD_SAMPLE_RATE} --codec=pcm_s16le --skip-existing'")
-                        elif profile == self.STANDARD_PROFILE:
+                                    profile_metadata = os.path.join(self.path,CONVERTED_RECORDINGS,STANDARD_PROFILE,RECORDINGS_CSV,)
+                                    self.warnings.append(f"recording '{raw_filename}' at '{path}' has a non standard sampling rate of {info['sample_rate']}Hz and no standard conversion in profile {STANDARD_PROFILE} was found. Does the standard profile exist? Does {profile_metadata} exist? you can create the standard profile with 'child-project process {self.path} {STANDARD_PROFILE} basic --format=wav --sampling={STANDARD_SAMPLE_RATE} --codec=pcm_s16le --skip-existing'")
+                        elif profile == STANDARD_PROFILE:
                             info = mediainfo(path)
-                            if 'sample_rate' in info and int(info['sample_rate']) != self.STANDARD_SAMPLE_RATE:
-                                self.warnings.append(f"recording '{raw_filename}' at '{path}' has unexpected sampling rate {info['sample_rate']}Hz when {self.STANDARD_SAMPLE_RATE}Hz is expected for profile {self.STANDARD_PROFILE}")
+                            if 'sample_rate' in info and int(info['sample_rate']) != STANDARD_SAMPLE_RATE:
+                                self.warnings.append(f"recording '{raw_filename}' at '{path}' has unexpected sampling rate {info['sample_rate']}Hz when {STANDARD_SAMPLE_RATE}Hz is expected for profile {STANDARD_PROFILE}")
                         continue
 
                     message = f"cannot find recording '{raw_filename}' at '{path}'"
                     if column_attr.required:
                         self.errors.append(message)
                     else:
                         self.warnings.append(message)
@@ -509,20 +573,20 @@
         files = [
             self.recordings[c.name].tolist()
             for c in self.RECORDINGS_COLUMNS
             if c.filename and c.name in self.recordings.columns
         ]
 
         indexed_files = [
-            os.path.abspath(os.path.join(self.path, self.RAW_RECORDINGS, str(f)))
+            os.path.abspath(os.path.join(self.path, RAW_RECORDINGS, str(f)))
             for f in pd.core.common.flatten(files)
         ]
 
         recordings_files = glob.glob(
-            os.path.join(os.path.normcase(self.path), self.RAW_RECORDINGS, "**/*.*"), recursive=True
+            os.path.join(os.path.normcase(self.path), RAW_RECORDINGS, "**/*.*"), recursive=True
         )
 
         for rf in recordings_files:
             if len(os.path.splitext(rf)) > 1 and os.path.splitext(rf)[1] in [
                 ".csv",
                 ".xls",
                 ".xlsx",
@@ -551,18 +615,18 @@
                 profile, recording_filename
             )
 
             if converted_filename is None:
                 return None
 
             return os.path.join(
-                os.path.normcase(self.path), self.CONVERTED_RECORDINGS, profile, os.path.normpath(converted_filename),
+                os.path.normcase(self.path), CONVERTED_RECORDINGS, profile, os.path.normpath(converted_filename),
             )
         else:
-            return os.path.join(os.path.normcase(self.path), self.RAW_RECORDINGS, os.path.normpath(recording_filename))
+            return os.path.join(os.path.normcase(self.path), RAW_RECORDINGS, os.path.normpath(recording_filename))
 
     def get_converted_recording_filename(
         self, profile: str, recording_filename: str
     ) -> str:
         """retrieve the converted filename of a recording under a given ``profile``,
         from its original filename.
 
@@ -577,15 +641,15 @@
         key = (profile, recording_filename)
 
         if key in self.converted_recordings_hashtable:
             return self.converted_recordings_hashtable[key]
 
         converted_recordings = pd.read_csv(
             os.path.join(
-                self.path, self.CONVERTED_RECORDINGS, profile, "recordings.csv"
+                self.path, CONVERTED_RECORDINGS, profile, RECORDINGS_CSV
             )
         )
         converted_recordings.dropna(subset=["converted_filename"], inplace=True)
 
         self.converted_recordings_hashtable.update(
             {
                 (profile, original): converted
@@ -602,17 +666,17 @@
             return None
 
     def recording_from_path(self, path: str, profile: str = None) -> str:
         if profile:
             raise NotImplementedError(
                 "cannot recover recording from the path to a converted media yet"
             )
-            # media_path = os.path.join(self.path, self.CONVERTED_RECORDINGS, profile)
+            # media_path = os.path.join(self.path, CONVERTED_RECORDINGS, profile)
         else:
-            media_path = os.path.join(self.path, self.RAW_RECORDINGS)
+            media_path = os.path.join(self.path, RAW_RECORDINGS)
 
         if not path_is_parent(media_path, path):
             return None
 
         recording = os.path.relpath(path, media_path)
 
         return recording
@@ -647,15 +711,15 @@
                 _recordings["recording_filename"].isin(recordings)
             ]
             
             if _recordings.shape[0] < len(recordings):
                 recs = pd.Series(recordings)
                 missing_recs = recs[~recs.isin(self.recordings['recording_filename'])].tolist()
                 #self.recordings[~self.recordings['recording_filename'].isin(recordings)]['recording_filename'].tolist()
-                raise ValueError("recordings {} were not found in the dataset index. Check the names and make sure they exist in '{}'".format(missing_recs,os.path.join('metadata','recordings.csv')))
+                raise ValueError("recordings {} were not found in the dataset index. Check the names and make sure they exist in '{}'".format(missing_recs,os.path.join(METADATA_FOLDER,RECORDINGS_CSV)))
                 
 
         return _recordings
 
     def compute_recordings_duration(self, profile: str = None) -> pd.DataFrame:
         """compute recordings duration
 
@@ -673,15 +737,18 @@
         )
         recordings["duration"].fillna(0, inplace=True)
         recordings["duration"] = (recordings["duration"] * 1000).astype(np.int64)
 
         return recordings
 
     def compute_ages(
-        self, recordings: pd.DataFrame = None, children: pd.DataFrame = None
+        self,
+        recordings: pd.DataFrame = None,
+        children: pd.DataFrame = None,
+        age_format: str = 'months',
     ) -> pd.Series:
         """Compute the age of the subject child for each recording (in months, as a float)
         and return it as a pandas Series object.
 
         Example:
 
         >>> from ChildProject.projects import ChildProject
@@ -694,22 +761,39 @@
         2            1  2020-04-20  3.613963
         3            1  2020-04-21  3.646817
 
         :param recordings: custom recordings DataFrame (see :ref:`format-metadata`), otherwise use all project recordings, defaults to None
         :type recordings: pd.DataFrame, optional
         :param children: custom children DataFrame (see :ref:`format-metadata`), otherwise use all project children data, defaults to None
         :type children: pd.DataFrame, optional
+        :param age_format: format to use for the output date default is months, choose between ['months','days','weeks', 'years']
+        :type age_format: str, optional
         """
 
         def date_is_valid(date: str, fmt: str):
             try:
                 datetime.datetime.strptime(date, fmt)
             except:
                 return False
             return True
+        
+        def date_fmt(dt,fmt='months'):
+            if dt:
+                if fmt == 'months':
+                    return dt.days / (365.25 / 12)
+                elif fmt == 'days':
+                    return dt.days
+                elif fmt == 'weeks':
+                    return dt.days / 7
+                elif fmt == 'years':
+                    return dt.days / 365.25
+                else:
+                    raise ValueError('unknown format for age : {}'.format(fmt))
+            else:
+                return None
 
         if recordings is None:
             recordings = self.recordings.copy()
 
         if children is None:
             children = self.children.copy()
 
@@ -738,15 +822,15 @@
                 if (
                     date_is_valid(r["child_dob"], "%Y-%m-%d")
                     and date_is_valid(r["date_iso"], "%Y-%m-%d")
                 )
                 else None,
                 axis=1,
             )
-            .apply(lambda dt: dt.days / (365.25 / 12) if dt else None)
+            .apply(partial(date_fmt,fmt=age_format))
         )
 
         return age
 
     def read_documentation(self) -> pd.DataFrame:
         docs = ["children", "recordings", "annotations"]
```

### Comparing `ChildProject-0.1.0/ChildProject/tables.py` & `ChildProject-0.1.1/ChildProject/tables.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/templates/basic.etf` & `ChildProject-0.1.1/ChildProject/templates/basic.etf`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/templates/basic.pfsx` & `ChildProject-0.1.1/ChildProject/templates/basic.pfsx`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/templates/native.etf` & `ChildProject-0.1.1/ChildProject/templates/native.etf`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/templates/native.pfsx` & `ChildProject-0.1.1/ChildProject/templates/native.pfsx`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/templates/non-native.etf` & `ChildProject-0.1.1/ChildProject/templates/non-native.etf`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/templates/non-native.pfsx` & `ChildProject-0.1.1/ChildProject/templates/non-native.pfsx`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/ChildProject/utils.py` & `ChildProject-0.1.1/ChildProject/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,23 @@
         self.stop = stop
 
     def length(self):
         return self.stop - self.start
 
     def __repr__(self):
         return "Segment([{}, {}])".format(self.start, self.stop)
+                
+def retry_func( func : callable , excep: Exception, tries : int = 3, **kwargs):
+    for i in range(tries):
+        try:
+            func(**kwargs)
+            return
+        except excep as e:
+            if i == tries - 1:
+                raise e
 
 
 def intersect_ranges(xs, ys):
     # Try to get the first range in each iterator:
     try:
         x, y = next(xs), next(ys)
     except StopIteration:
```

### Comparing `ChildProject-0.1.0/ChildProject.egg-info/PKG-INFO` & `ChildProject-0.1.1/ChildProject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChildProject
-Version: 0.1.0
+Version: 0.1.1
 Summary: LAAC@LSCP
 Home-page: https://github.com/LAAC-LSCP/ChildProject
 Author: Lucas Gautheron
 Author-email: lucas.gautheron@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ChildProject-0.1.0/ChildProject.egg-info/SOURCES.txt` & `ChildProject-0.1.1/ChildProject.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ChildProject.egg-info/entry_points.txt
 ChildProject.egg-info/not-zip-safe
 ChildProject.egg-info/requires.txt
 ChildProject.egg-info/top_level.txt
 ChildProject/pipelines/__init__.py
 ChildProject/pipelines/anonymize.py
 ChildProject/pipelines/eafbuilder.py
+ChildProject/pipelines/fake_panoptes.py
 ChildProject/pipelines/metrics.py
 ChildProject/pipelines/metricsFunctions.py
 ChildProject/pipelines/pipeline.py
 ChildProject/pipelines/processors.py
 ChildProject/pipelines/samplers.py
 ChildProject/pipelines/zooniverse.py
 ChildProject/templates/__init__.py
```

### Comparing `ChildProject-0.1.0/LICENSE` & `ChildProject-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/PKG-INFO` & `ChildProject-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChildProject
-Version: 0.1.0
+Version: 0.1.1
 Summary: LAAC@LSCP
 Home-page: https://github.com/LAAC-LSCP/ChildProject
 Author: Lucas Gautheron
 Author-email: lucas.gautheron@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ChildProject-0.1.0/README.md` & `ChildProject-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/setup.py` & `ChildProject-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 DIRECTORY = os.path.dirname(__file__)
 README = open(os.path.join(DIRECTORY, "README.md")).read()
 
 requires = {
     "core": ["pandas>=1.1.0,<=1.5.0", "jinja2", "numpy>=1.16.5", "datalad"],
     "annotations": ["lxml", "pympi-ling", "pylangacq", "python-dateutil>=2.8.1"],
     "metrics": ['pyannote.metrics; python_version >= "3.7.0"', "nltk", "scikit-learn", "GitPython"],
-    "audio": ["librosa", "pydub", "pysoundfile"],
+    "audio": ["librosa", "pydub", "soundfile"],
     "samplers": ["PyYAML"],
     "zooniverse": ["panoptes-client", "praat-parselmouth"],
     "eaf-builder": ["importlib-resources"],
     "constraints": [
         "click==7.1.1",
         "requests==2.25.0",
         "chardet<4,>=3.0.2",
```

### Comparing `ChildProject-0.1.0/tests/test_annotations.py` & `ChildProject-0.1.1/tests/test_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,33 @@
 
 DATA = os.path.join('tests', 'data')
 TRUTH = os.path.join('tests', 'truth')
 
 
 @pytest.fixture(scope="function")
 def project(request):
-    if not os.path.exists("output/annotations"):
-        shutil.copytree(src="examples/valid_raw_data", dst="output/annotations")
+    if os.path.exists("output/annotations"):
+#        shutil.copytree(src="examples/valid_raw_data", dst="output/annotations")
+        shutil.rmtree("output/annotations")
+    shutil.copytree(src="examples/valid_raw_data", dst="output/annotations")
       
     if os.path.isfile("output/annotations/metadata/annotations.csv"):
         os.remove("output/annotations/metadata/annotations.csv")
     for raw_annotation in glob.glob("output/annotations/annotations/*/converted"):
         shutil.rmtree(raw_annotation)
 
     project = ChildProject("output/annotations")
+    
     yield project
-
+    
+@pytest.fixture(scope="function")
+def am(request, project):
+    am= AnnotationManager(project)
+    project.recordings['duration'] = [100000000, 2000000] #force longer durations to allow for imports
+    yield am
 
 def test_csv():
     converted = CsvConverter().convert("tests/data/csv.csv").fillna("NA")
     truth = pd.read_csv("tests/truth/csv.csv").fillna("NA")
 
     pd.testing.assert_frame_equal(
         standardize_dataframe(converted, converted.columns),
@@ -146,16 +154,15 @@
     input_annotations.iloc[nline, input_annotations.columns.get_loc(column)] = value
     
     print(input_annotations[['range_onset','range_offset']])
     
     with pytest.raises(exception, match=error):
         am.import_annotations(input_annotations)
 
-def test_import(project):
-    am = AnnotationManager(project)
+def test_import(project, am):
 
     input_annotations = pd.read_csv("examples/valid_raw_data/annotations/input.csv")
     am.import_annotations(input_annotations)
     am.read()
 
     assert (
         am.annotations.shape[0] == input_annotations.shape[0]
@@ -200,17 +207,17 @@
  
 # test how the importation handles already existing files and overlaps in importation
 @pytest.mark.parametrize("input_file,ow,rimported,rerrors,exception", 
                          [("input_invalid.csv", False,None,None,ValueError),
                          ("input_reimport.csv", False,"imp_reimport_no_ow.csv","err_reimport_no_ow.csv",None),
                          ("input_reimport.csv", True,"imp_reimport_ow.csv",None,None),
                          ("input_importoverlaps.csv", False,"imp_overlap.csv","err_overlap.csv",None),
+                         ("input_import_duration_overflow.csv", False,None,None,AssertionError),
                          ])
-def test_multiple_imports(project, input_file, ow, rimported, rerrors, exception):
-    am = AnnotationManager(project)
+def test_multiple_imports(project, am, input_file, ow, rimported, rerrors, exception):
     
     input_file = os.path.join(DATA,input_file)
     
     input_annotations = pd.read_csv("examples/valid_raw_data/annotations/input.csv")
     
     am.import_annotations(input_annotations)
     am.read()
@@ -241,16 +248,14 @@
             #errors.to_csv(rerrors, index=False)
             rerrors = pd.read_csv(rerrors)
             pd.testing.assert_frame_equal(rerrors.reset_index(drop=True),
                                           errors.drop(['imported_at','package_version'],axis=1).reset_index(drop=True),
                                           check_like=True,
                                           check_dtype=False)
             
-        #raise Exception()
-            
         am.read()
         assert all(
             [
                 os.path.exists(
                     os.path.join(
                         project.path,
                         "annotations",
@@ -260,22 +265,25 @@
                     )
                 )
                 for a in am.annotations.to_dict(orient="records")
             ]
         ), "some annotations are missing"
         
         errors, warnings = am.validate()
+        print(errors)
+        print(warnings)
         assert len(errors) == 0 and len(warnings) == 0, "malformed annotations detected"
         
         errors, warnings = am.read()
+        print(errors)
+        print(warnings)
         assert len(errors) == 0 and len(warnings) == 0, "malformed annotation indexes detected"
 
 
-def test_intersect(project):
-    am = AnnotationManager(project)
+def test_intersect(project, am):
 
     input_annotations = pd.read_csv("examples/valid_raw_data/annotations/intersect.csv")
     am.import_annotations(input_annotations)
 
     intersection = AnnotationManager.intersection(
         am.annotations[am.annotations["set"].isin(["textgrid", "vtc_rttm"])]
     ).convert_dtypes()
@@ -301,16 +309,15 @@
         standardize_dataframe(
             pd.read_csv("tests/truth/intersect_b.csv"), columns
         ).convert_dtypes(),
         check_dtype=False,
     )
 
 
-def test_within_ranges(project):
-    am = AnnotationManager(project)
+def test_within_ranges(project, am):
 
     annotations = [
         {
             "recording_filename": "sound.wav",
             "set": "matching",
             "range_onset": onset,
             "range_offset": onset + 500,
@@ -348,30 +355,29 @@
             exception_caught = True
 
     assert (
         exception_caught
     ), "get_within_ranges should raise an exception when annotations do not fully cover the required ranges"
 
 
-def test_merge(project):
-    am = AnnotationManager(project)
+def test_merge(project, am):
 
     input_annotations = pd.read_csv("examples/valid_raw_data/annotations/input.csv")
     input_annotations = input_annotations[
-        input_annotations["set"].isin(["vtc_rttm", "alice"])
+        input_annotations["set"].isin(["vtc_rttm", "alice/output"])
     ]
     print(input_annotations)
     am.import_annotations(input_annotations)
     am.read()
 
     print(am.annotations)
     am.read()
     am.merge_sets(
         left_set="vtc_rttm",
-        right_set="alice",
+        right_set="alice/output",
         left_columns=["speaker_type"],
         right_columns=["phonemes", "syllables", "words"],
         output_set="alice_vtc",
         full_set_merge = False,
         recording_filter = {'sound.wav'}
     )
     am.read()
@@ -380,15 +386,15 @@
     assert anns.shape[0] == 1
     assert anns.iloc[0]['recording_filename'] == 'sound.wav'
     
     time.sleep(2) #sleeping for 2 seconds to have different 'imported_at' values so that can make sure both merge did fine
     
     am.merge_sets(
         left_set="vtc_rttm",
-        right_set="alice",
+        right_set="alice/output",
         left_columns=["speaker_type"],
         right_columns=["phonemes", "syllables", "words"],
         output_set="alice_vtc",
         full_set_merge = False,
         skip_existing = True
     )
     am.read()
@@ -405,29 +411,28 @@
 
     adult_segments = (
         segments[segments["speaker_type"].isin(["FEM", "MAL"])]
         .sort_values(["segment_onset", "segment_offset"])
         .reset_index(drop=True)
     )
     alice = (
-        am.get_segments(am.annotations[am.annotations["set"] == "alice"])
+        am.get_segments(am.annotations[am.annotations["set"] == "alice/output"])
         .sort_values(["segment_onset", "segment_offset"])
         .reset_index(drop=True)
     )
 
     pd.testing.assert_frame_equal(
         adult_segments[["phonemes", "syllables", "words"]],
         alice[["phonemes", "syllables", "words"]],
     )
     
     
 
 
-def test_clipping(project):
-    am = AnnotationManager(project)
+def test_clipping(project,am):
 
     input_annotations = pd.read_csv("examples/valid_raw_data/annotations/input.csv")
     input_annotations = input_annotations[input_annotations["recording_filename"] == "sound.wav"]
     am.import_annotations(input_annotations[input_annotations["set"] == "vtc_rttm"])
     am.read()
 
     start = 1981000
@@ -440,40 +445,46 @@
         and segments["segment_offset"].between(start, stop).all()
     ), "segments not properly clipped"
     assert segments.shape[0] == 2, "got {} segments, expected 2".format(
         segments.shape[0]
     )
 
 
-def test_within_time_range(project):
+def test_within_time_range(project,am):
     from ChildProject.utils import TimeInterval
-    am = AnnotationManager(project)
+    
     am.project.recordings = pd.read_csv("tests/data/time_range_recordings.csv")
 
     annotations = pd.read_csv("tests/data/time_range_annotations.csv")
     matches = am.get_within_time_range(annotations, TimeInterval(datetime.datetime(1900,1,1,9,0),datetime.datetime(1900,1,1,20,0)))
 
     truth = pd.read_csv("tests/truth/time_range.csv")
 
     pd.testing.assert_frame_equal(
         standardize_dataframe(matches, truth.columns),
         standardize_dataframe(truth, truth.columns),
     )
+    
+    matches = am.get_within_time_range(annotations, start_time="09:00", end_time="20:00")
+    
+    pd.testing.assert_frame_equal(
+        standardize_dataframe(matches, truth.columns),
+        standardize_dataframe(truth, truth.columns),
+    )
 
     exception_caught = False
     try:
         matches = am.get_within_time_range(annotations, "9am", "8pm")
     except ValueError as e:
         exception_caught = True
 
     assert exception_caught, "no exception was thrown despite invalid times"
 
 
-def test_segments_timestamps(project):
-    am = AnnotationManager(project)
+def test_segments_timestamps(project,am):
 
     segments = pd.DataFrame(
         [
             {
                 "recording_filename": "sound.wav",
                 "segment_onset": 3600 * 1000,
                 "segment_offset": 3600 * 1000 + 1000,
@@ -495,31 +506,75 @@
     )
 
     pd.testing.assert_frame_equal(
         standardize_dataframe(segments, truth.columns),
         standardize_dataframe(truth, truth.columns),
     )
 
-
-def test_rename(project):
-    am = AnnotationManager(project)
+#old set, new set, error to expect, mf = add a merged from column to index, index= add a fictional index line
+@pytest.mark.parametrize("old,new,error,mf,index", 
+                         [("textgrid", 'vtc_rttm',Exception,False,False),
+                          ("invented", 'renamed',Exception,False,False),
+                          ("textgrid", 'renamed',None,False,False),
+                          ("textgrid", 'alice',None,False,False), #in subdomain of alice/output
+                          ("textgrid", 'invented',Exception,False,True),
+                          ("textgrid", 'renamed',None,True,False),
+                         ])
+def test_rename(project,am,old, new, error, mf, index):
 
     input_annotations = pd.read_csv("examples/valid_raw_data/annotations/input.csv")
-    am.import_annotations(input_annotations[input_annotations["set"] == "textgrid"])
+    if mf:
+        am.import_annotations(input_annotations)
+    else:
+        am.import_annotations(input_annotations[input_annotations['set'] == old])
     am.read()
+    
+    if mf:
+        mdf = pd.read_csv("examples/valid_raw_data/annotations/merged_from.csv")
+        am.annotations['merged_from'] = mdf['merged_from']
+        am.write()
+        
+        wanted_list = am.annotations.sort_values(['set','recording_filename','range_onset','range_offset'])['merged_from'].astype(str).str.split(',').values.tolist()
+        i=0
+        while i < len(wanted_list):
+            j=0
+            while j < len(wanted_list[i]):
+                if wanted_list[i][j] == old: wanted_list[i][j] = new
+                j+=1
+            i+=1
+    if index:
+        add = pd.read_csv("examples/valid_raw_data/annotations/input.csv").head(1)
+        add['set'] = new
+        am.annotations = pd.concat([am.annotations, add])
+        am.write()
+    
     tg_count = am.annotations[am.annotations["set"] == "textgrid"].shape[0]
 
-    am.rename_set("textgrid", "renamed")
-    am.read()
-
-    errors, warnings = am.validate()
-    assert len(errors) == 0 and len(warnings) == 0, "malformed annotations detected"
-
-    assert am.annotations[am.annotations["set"] == "textgrid"].shape[0] == 0
-    assert am.annotations[am.annotations["set"] == "renamed"].shape[0] == tg_count
+    if error:
+        print(am.annotations[am.annotations["set"] == new].shape[0])
+        with pytest.raises(error):
+            am.rename_set(old, new)
+    else:
+        am.rename_set(old, new)
+        am.read()
+    
+        errors, warnings = am.validate()
+        assert len(errors) == 0 and len(warnings) == 0, "malformed annotations detected"
+    
+        assert am.annotations[am.annotations["set"] == old].shape[0] == 0
+        assert am.annotations[am.annotations["set"] == new].shape[0] == tg_count
+        
+        if mf:
+            result = am.annotations.sort_values(['set','recording_filename','range_onset','range_offset'])['merged_from'].astype(str).str.split(',').values.tolist()
+            i = 0
+            print(wanted_list)
+            print(result)
+            while i < len(wanted_list):
+                assert sorted(wanted_list[i]) == sorted(result[i])
+                i+= 1
 
 
 def custom_function(filename):
     from ChildProject.converters import VtcConverter
 
     df = pd.read_csv(
         filename,
@@ -557,16 +612,15 @@
         ],
         axis=1,
         inplace=True,
     )
     return df
 
 
-def test_custom_importation(project):
-    am = AnnotationManager(project)
+def test_custom_importation(project, am):
     input = pd.DataFrame(
         [
             {
                 "set": "vtc_rttm",
                 "range_onset": 0,
                 "range_offset": 4000,
                 "recording_filename": "sound.wav",
@@ -580,16 +634,15 @@
     am.import_annotations(input, import_function=custom_function)
     am.read()
 
     errors, warnings = am.validate()
     assert len(errors) == 0
 
 
-def test_set_from_path(project):
-    am = AnnotationManager(project)
+def test_set_from_path(project,am):
 
     assert am.set_from_path(os.path.join(project.path, "annotations/set")) == "set"
     assert am.set_from_path(os.path.join(project.path, "annotations/set/")) == "set"
     assert (
         am.set_from_path(os.path.join(project.path, "annotations/set/subset"))
         == "set/subset"
     )
```

### Comparing `ChildProject-0.1.0/tests/test_cli.py` & `ChildProject-0.1.1/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def test_import_annotations():
     stdout, stderr, exit_code = cli(
         [
             "child-project",
             "import-annotations",
             "examples/valid_raw_data",
             "--annotations",
-            "examples/valid_raw_data/annotations/input.csv",
+            "examples/valid_raw_data/annotations/input_short.csv",
         ]
     )
     assert exit_code == 0
 
 def test_compute_durations():
     stdout, stderr, exit_code = cli(
         [
```

### Comparing `ChildProject-0.1.0/tests/test_convert.py` & `ChildProject-0.1.1/tests/test_convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ChildProject.projects import ChildProject
+from ChildProject.projects import ChildProject, CONVERTED_RECORDINGS
 from ChildProject.pipelines.processors import AudioProcessingPipeline
 import numpy as np
 import os
 import pandas as pd
 import pytest
 import shutil
 
@@ -30,26 +30,26 @@
     recordings = project.recordings
     converted_recordings = pd.read_csv(processed)
 
     assert np.isclose(
         8000, project.compute_recordings_duration()["duration"].sum()
     ), "audio duration equals expected value"
     assert os.path.exists(
-        os.path.join(project.path, ChildProject.CONVERTED_RECORDINGS, "test")
+        os.path.join(project.path, CONVERTED_RECORDINGS, "test")
     ), "missing processed recordings folder"
     assert (
         recordings.shape[0] == converted_recordings.shape[0]
     ), "conversion table is incomplete"
     assert all(
         converted_recordings["success"].tolist()
     ), "not all recordings were successfully processed"
     assert all(
         [
             os.path.exists(
-                os.path.join(project.path, ChildProject.CONVERTED_RECORDINGS, "test", f)
+                os.path.join(project.path, CONVERTED_RECORDINGS, "test", f)
             )
             for f in converted_recordings["converted_filename"].tolist()
         ]
     ), "recording files are missing"
 
 
 def test_vetting(project):
```

### Comparing `ChildProject-0.1.0/tests/test_documentation.py` & `ChildProject-0.1.1/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/tests/test_eaf.py` & `ChildProject-0.1.1/tests/test_eaf.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/tests/test_metrics.py` & `ChildProject-0.1.1/tests/test_metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,47 @@
 import pytest
 import shutil
 
 from ChildProject.projects import ChildProject
 from ChildProject.annotations import AnnotationManager
 from ChildProject.pipelines.metrics import Metrics, LenaMetrics, AclewMetrics, CustomMetrics, MetricsSpecificationPipeline
 
+from ChildProject.pipelines.metricsFunctions import metricFunction, RESERVED
+
 
 def fake_vocs(data, filename):
     return data
 
 
 @pytest.fixture(scope="function")
 def project(request):
     if not os.path.exists("output/metrics"):
         shutil.copytree(src="examples/valid_raw_data", dst="output/metrics")
 
     project = ChildProject("output/metrics")
     project.read()
 
     yield project
-
+    
+@pytest.fixture(scope="function")
+def am(request, project):
+    am= AnnotationManager(project)
+    project.recordings['duration'] = [100000000, 2000000] #force longer durations to allow for imports
+    yield am    
+    
+#decorating functions with reserved kwargs should fail
+@pytest.mark.parametrize("error", [ValueError, ])
+def test_decorator(error):
+    for reserved in RESERVED:
+        
+        with pytest.raises(error):
+            
+            @metricFunction({reserved},{})
+            def fake_function(annotations, duration, **kwargs):
+                return 0
 
 def test_failures(project):
     exception_caught = False
     try:
         aclew = AclewMetrics(project, vtc="unknown")
     except ValueError as e:
         exception_caught = True
@@ -54,20 +72,60 @@
         m = Metrics(project, lm,  segments="unknown")
     except ValueError as e:
         exception_caught = True
 
     assert (
         exception_caught == True
     ), "Metrics failed to throw an exception despite having the segments argument and by having a value different than 'recording_filename'"
+           
+@pytest.mark.parametrize("error,col_change,new_value",
+                         [(ValueError, 'name', 'voc_mal_ph_its'),
+                          (ValueError, 'name', 'voc_fem_ph_its'),
+                          (ValueError, 'speaker', 'FEM'),
+                          (None,None,None),
+                          ])
+def test_metrics(project, am, error, col_change, new_value):
+    
+    data = pd.read_csv("tests/data/lena_its.csv")
+
+    am.import_annotations(
+        pd.DataFrame(
+            [
+                {
+                    "set": "custom_its",
+                    "raw_filename": "file.its",
+                    "time_seek": 0,
+                    "recording_filename": "sound.wav",
+                    "range_onset": 0,
+                    "range_offset": 100000000,
+                    "format": "its",
+                }
+            ]
+        ),
+        import_function=partial(fake_vocs, data),
+    )
+        
+    parameters=pd.read_csv("tests/data/list_metrics.csv")
+    
+    if error:
+        with pytest.raises(error):
+            parameters.iloc[0,parameters.columns.get_loc(col_change)] = new_value
+            mm = Metrics(project, parameters)
+    else:       
+        mm = Metrics(project, parameters)
+        mm.extract()
+    
+        truth = pd.read_csv("tests/truth/custom_metrics.csv")
+    
+        pd.testing.assert_frame_equal(mm.metrics, truth, check_like=True)
 
 
-def test_aclew(project):
+def test_aclew(project, am):
     data = pd.read_csv("tests/data/aclew.csv")
 
-    am = AnnotationManager(project)
     am.import_annotations(
         pd.DataFrame(
             [
                 {
                     "set": set,
                     "raw_filename": "file.rttm",
                     "time_seek": 0,
@@ -85,18 +143,17 @@
     aclew = AclewMetrics(project, by="child_id", rec_cols='date_iso', child_cols='experiment,child_dob',vtc='aclew_vtc',alice='aclew_alice',vcm='aclew_vcm')
     aclew.extract()
 
     truth = pd.read_csv("tests/truth/aclew_metrics.csv")
 
     pd.testing.assert_frame_equal(aclew.metrics, truth, check_like=True)
 
-def test_lena(project):
+def test_lena(project, am):
     data = pd.read_csv("tests/data/lena_its.csv")
 
-    am = AnnotationManager(project)
     am.import_annotations(
         pd.DataFrame(
             [
                 {
                     "set": "lena_its",
                     "raw_filename": "file.its",
                     "time_seek": 0,
@@ -113,16 +170,15 @@
     lena = LenaMetrics(project, set="lena_its", period='1h', from_time='10:00:00' , to_time= '16:00:00')
     lena.extract()
 
     truth = pd.read_csv("tests/truth/lena_metrics.csv")
 
     pd.testing.assert_frame_equal(lena.metrics, truth, check_like=True)
 
-def test_custom(project):
-    am = AnnotationManager(project)
+def test_custom(project, am):
     
     data = pd.read_csv("tests/data/lena_its.csv")
 
     am.import_annotations(
         pd.DataFrame(
             [
                 {
@@ -136,25 +192,25 @@
                 }
             ]
         ),
         import_function=partial(fake_vocs, data),
     )
         
     parameters="tests/data/list_metrics.csv"
+    
     cmm = CustomMetrics(project, parameters)
     cmm.extract()
 
     truth = pd.read_csv("tests/truth/custom_metrics.csv")
 
     pd.testing.assert_frame_equal(cmm.metrics, truth, check_like=True)
     
-def test_metrics_segments(project):
+def test_metrics_segments(project, am):
     data = pd.read_csv("tests/data/aclew.csv")
 
-    am = AnnotationManager(project)
     am.import_annotations(
         pd.DataFrame(
             [
                 {
                     "set": set,
                     "raw_filename": "file.rttm",
                     "time_seek": 0,
@@ -180,18 +236,17 @@
     metrics = Metrics(project, metrics_list=lm, by="segments", rec_cols='date_iso', child_cols='experiment,child_dob',segments='tests/data/segments.csv')
     metrics.extract()
 
     truth = pd.read_csv("tests/truth/segments_metrics.csv")
 
     pd.testing.assert_frame_equal(metrics.metrics, truth, check_like=True)
 
-def test_specs(project):
+def test_specs(project, am):
     data = pd.read_csv("tests/data/lena_its.csv")
     
-    am = AnnotationManager(project)
     am.import_annotations(
         pd.DataFrame(
             [
                 {
                     "set": "specs_its",
                     "raw_filename": "file.its",
                     "time_seek": 0,
```

### Comparing `ChildProject-0.1.0/tests/test_pipelines.py` & `ChildProject-0.1.1/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/tests/test_reliability.py` & `ChildProject-0.1.1/tests/test_reliability.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/tests/test_samplers.py` & `ChildProject-0.1.1/tests/test_samplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
                 "speaker_type": ["FEM", "CHI"][i % 2],
             }
             for i in range(conversation["vocs"])
         ]
     segments = pd.DataFrame(segments)
 
     am = AnnotationManager(project)
+    project.recordings['duration'] = 3600 * 1000 * 1000 #forcefully extend the audio duration to accept import here
     am.import_annotations(
         pd.DataFrame(
             [
                 {
                     "set": "conv",
                     "raw_filename": "file.rttm",
                     "time_seek": 0,
```

### Comparing `ChildProject-0.1.0/tests/test_utils.py` & `ChildProject-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.0/tests/test_validation.py` & `ChildProject-0.1.1/tests/test_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def test_valid_project():
     path = os.path.normpath("examples/valid_raw_data")
     project = ChildProject(path)
     errors, warnings = project.validate()
 
     assert len(errors) == 0, "valid input validation failed (expected to pass)"
-    assert len(warnings) == 3, "expected 1 warning, got {}".format(len(warnings))
+    assert len(warnings) == 4, "expected 3 warnings, got {}".format(len(warnings))
 
 
 def test_invalid_project():
     project = ChildProject("examples/invalid_raw_data")
     errors, warnings = project.validate()
     
     am = AnnotationManager(project)
@@ -22,16 +22,17 @@
 
     expected_errors = [
         os.path.normpath("examples/invalid_raw_data/metadata/children.csv")+ ": child_id '1' appears 2 times in lines [2,3], should appear once",
         "cannot find recording 'test_1_20200918.mp3' at "+os.path.normpath("'examples/invalid_raw_data/recordings/raw/test_1_20200918.mp3'"),
         os.path.normpath("examples/invalid_raw_data/metadata/recordings.csv")+ ": 'USB' is not a permitted value for column 'recording_device_type' on line 2, should be any of [lena,usb,olympus,babylogger,unknown]",
         "Age at recording is negative in recordings on line 3 (-15.4 months). Check date_iso for that recording and child_dob for the corresponding child.",
         "duplicate reference to annotations/vtc_rttm/converted/sound_1980000_1990000.csv (appears 2 times)",
-        "overlaps in the annotation index for the following [set, annotation_filename] list: [['textgrid', 'sound_0_10000.csv'], ['textgrid', 'sound_0_300000.csv'], ['textgrid', 'sound_0_40000000.csv'], ['vtc_rttm', 'sound_1980000_1990000.csv'], ['vtc_rttm', 'sound_1980000_1990000.csv']]",
+        "overlaps in the annotation index for the following [set, annotation_filename] list: [['textgrid', 'sound_0_10000.csv'], ['textgrid', 'sound_0_300000.csv'], ['vtc_rttm', 'sound_1980000_1990000.csv'], ['vtc_rttm', 'sound_1980000_1990000.csv']]",
         "annotation index does not verify range_offset > range_onset >= 0 for set <ranges>, annotation filename <sound_0_300000.csv>",
+        "annotation index has an offset higher than recorded duration of the audio <textgrid>, annotation filename <sound_0_40000000.csv>",
     ]
 
     expected_warnings = [
         os.path.normpath("examples/invalid_raw_data/metadata/recordings.csv")+ ": '2' does not pass callable test for column 'noisy_setting' on line 2",
         "file '"+ os.path.normpath("examples/invalid_raw_data/recordings/raw/test_1_2020091.mp3")+"' not indexed.",
     ]
     assert sorted(expected_errors) == sorted(
```

