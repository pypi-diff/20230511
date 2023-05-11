# Comparing `tmp/dummy_kinematics-0.0.7a3.tar.gz` & `tmp/dummy_kinematics-0.0.8.tar.gz`

## Comparing `dummy_kinematics-0.0.7a3.tar` & `dummy_kinematics-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/PKG-INFO
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/test2.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/__about__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/__init__.py
--rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/chart_element.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/config.py
--rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/data_converter.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/descriptors.py
--rw-r--r--   0        0        0    54622 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/dummy_iso_config.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/json_file_helper.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/logger_helper.py
--rw-r--r--   0        0        0    20807 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/ppt_factory.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/ppt_insert_helper.py
--rw-r--r--   0        0        0    15270 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/unitils.py
--rw-r--r--   0        0        0   252577 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/dummy_kinematics/default/default_template.pptx
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/LICENSE.txt
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/README.md
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/pyproject.toml
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a3/PKG-INFO
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/test2.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/__about__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/__init__.py
+-rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/chart_element.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/config.py
+-rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/data_converter.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/descriptors.py
+-rw-r--r--   0        0        0    54622 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/dummy_iso_config.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/json_file_helper.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/logger_helper.py
+-rw-r--r--   0        0        0    20807 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/ppt_factory.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/ppt_insert_helper.py
+-rw-r--r--   0        0        0    15270 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/unitils.py
+-rw-r--r--   0        0        0   252577 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/default/default_template.pptx
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/README.md
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/PKG-INFO
```

### Comparing `dummy_kinematics-0.0.7a3/PKG-INFO` & `dummy_kinematics-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy-kinematics
-Version: 0.0.7a3
+Version: 0.0.8
 Project-URL: Documentation, https://github.com/unknown/dummy-kinematics#readme
 Project-URL: Issues, https://github.com/unknown/dummy-kinematics/issues
 Project-URL: Source, https://github.com/unknown/dummy-kinematics
 Author-email: xiaochai <1219295581@qq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dummy_kinematics-0.0.7a3/test2.py` & `dummy_kinematics-0.0.8/test2.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/chart_element.py` & `dummy_kinematics-0.0.8/dummy_kinematics/chart_element.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/data_converter.py` & `dummy_kinematics-0.0.8/dummy_kinematics/data_converter.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/descriptors.py` & `dummy_kinematics-0.0.8/dummy_kinematics/descriptors.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/dummy_iso_config.py` & `dummy_kinematics-0.0.8/dummy_kinematics/dummy_iso_config.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/logger_helper.py` & `dummy_kinematics-0.0.8/dummy_kinematics/logger_helper.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/ppt_factory.py` & `dummy_kinematics-0.0.8/dummy_kinematics/ppt_factory.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/ppt_insert_helper.py` & `dummy_kinematics-0.0.8/dummy_kinematics/ppt_insert_helper.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/unitils.py` & `dummy_kinematics-0.0.8/dummy_kinematics/unitils.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/dummy_kinematics/default/default_template.pptx` & `dummy_kinematics-0.0.8/dummy_kinematics/default/default_template.pptx`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/README.md` & `dummy_kinematics-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.7a3/pyproject.toml` & `dummy_kinematics-0.0.8/pyproject.toml`

 * *Files identical despite different names*

