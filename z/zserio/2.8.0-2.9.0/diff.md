# Comparing `tmp/zserio-2.8.0.tar.gz` & `tmp/zserio-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zserio-2.8.0.tar", last modified: Fri Oct 14 14:51:26 2022, max compression
+gzip compressed data, was "zserio-2.9.0.tar", last modified: Fri Dec  2 12:51:14 2022, max compression
```

## Comparing `zserio-2.8.0.tar` & `zserio-2.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       21 2022-06-01 07:10:15.000000 zserio-2.8.0/MANIFEST.in
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     2867 2022-10-14 14:51:26.664862 zserio-2.8.0/PKG-INFO
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     2102 2022-06-01 07:10:15.000000 zserio-2.8.0/README.md
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       38 2022-10-14 14:51:26.664862 zserio-2.8.0/setup.cfg
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     4910 2022-06-01 07:10:15.000000 zserio-2.8.0/setup.py
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/src/
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)      119 2022-06-01 07:10:15.000000 zserio-2.8.0/src/mypy.ini
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     2057 2022-06-01 07:10:15.000000 zserio-2.8.0/src/pylintrc.txt
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/src/zserio/
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)      139 2022-06-01 07:10:15.000000 zserio-2.8.0/src/zserio/__init__.py
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)      512 2022-06-01 07:10:15.000000 zserio-2.8.0/src/zserio/__main__.py
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     5458 2022-06-01 07:10:15.000000 zserio-2.8.0/src/zserio/compiler.py
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-06-01 07:10:15.000000 zserio-2.8.0/src/zserio/py.typed
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/test/
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     7107 2022-06-01 07:10:15.000000 zserio-2.8.0/test/test_compiler.py
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/test/zs/
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/test/zs/default_package/
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       43 2022-06-01 07:10:15.000000 zserio-2.8.0/test/zs/default_package/structure_default.zs
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/test/zs/main_zs_with_path/
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/test/zs/main_zs_with_path/company/
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/test/zs/main_zs_with_path/company/main/
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       86 2022-06-01 07:10:15.000000 zserio-2.8.0/test/zs/main_zs_with_path/company/main/structure_with_path.zs
-drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-10-14 14:51:26.664862 zserio-2.8.0/test/zs/main_zs_without_path/
--rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       76 2022-06-01 07:10:15.000000 zserio-2.8.0/test/zs/main_zs_without_path/structure_without_path.zs
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       21 2022-06-01 07:10:15.000000 zserio-2.9.0/MANIFEST.in
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     2867 2022-12-02 12:51:14.073781 zserio-2.9.0/PKG-INFO
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     2102 2022-06-01 07:10:15.000000 zserio-2.9.0/README.md
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       38 2022-12-02 12:51:14.073781 zserio-2.9.0/setup.cfg
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     4910 2022-06-01 07:10:15.000000 zserio-2.9.0/setup.py
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/src/
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)      119 2022-06-01 07:10:15.000000 zserio-2.9.0/src/mypy.ini
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     2057 2022-06-01 07:10:15.000000 zserio-2.9.0/src/pylintrc.txt
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/src/zserio/
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)      139 2022-06-01 07:10:15.000000 zserio-2.9.0/src/zserio/__init__.py
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)      512 2022-06-01 07:10:15.000000 zserio-2.9.0/src/zserio/__main__.py
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     5556 2022-11-10 08:51:03.000000 zserio-2.9.0/src/zserio/compiler.py
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-06-01 07:10:15.000000 zserio-2.9.0/src/zserio/py.typed
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/test/
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)     7107 2022-06-01 07:10:15.000000 zserio-2.9.0/test/test_compiler.py
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/test/zs/
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/test/zs/default_package/
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       43 2022-06-01 07:10:15.000000 zserio-2.9.0/test/zs/default_package/structure_default.zs
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/test/zs/main_zs_with_path/
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/test/zs/main_zs_with_path/company/
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/test/zs/main_zs_with_path/company/main/
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       86 2022-06-01 07:10:15.000000 zserio-2.9.0/test/zs/main_zs_with_path/company/main/structure_with_path.zs
+drwxrwxr-x   0 mrozloznik  (1000) mrozloznik  (1000)        0 2022-12-02 12:51:14.073781 zserio-2.9.0/test/zs/main_zs_without_path/
+-rw-rw-r--   0 mrozloznik  (1000) mrozloznik  (1000)       76 2022-06-01 07:10:15.000000 zserio-2.9.0/test/zs/main_zs_without_path/structure_without_path.zs
```

### Comparing `zserio-2.8.0/PKG-INFO` & `zserio-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zserio
-Version: 2.8.0
+Version: 2.9.0
 Summary: Zserio runtime with compiler.
 Home-page: https://github.com/ndsev/zserio-pypi
 Author: Navigation Data Standard e.V.
 Author-email: support@nds-association.org
 License: BSD-3 Clause
 Description: Zserio PyPi package contains Zserio compiler and Zserio Python runtime. Zserio is serialization framework
         available at [GitHub](http://zserio.org).
```

### Comparing `zserio-2.8.0/README.md` & `zserio-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `zserio-2.8.0/setup.py` & `zserio-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `zserio-2.8.0/src/pylintrc.txt` & `zserio-2.9.0/src/pylintrc.txt`

 * *Files identical despite different names*

### Comparing `zserio-2.8.0/src/zserio/__main__.py` & `zserio-2.9.0/src/zserio/__main__.py`

 * *Files identical despite different names*

### Comparing `zserio-2.8.0/src/zserio/compiler.py` & `zserio-2.9.0/src/zserio/compiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,16 +28,17 @@
 
     java_executable = _find_java_executable()
     zserio_command = [java_executable, "-cp", ZSERIO_JAR_FILE, "zserio.tools.ZserioToolPython"]
     zserio_command[len(zserio_command):] = cmd_args
 
     return subprocess.run(zserio_command, capture_output = capture_output, check = check_exit_code, text = True)
 
-def generate(main_zs_file: str, *, is_default_package: bool = False, zs_dir: str = None, gen_dir: str = None,
-             top_level_package: str = None, extra_args: typing.List[str] = None) -> typing.Any:
+def generate(main_zs_file: str, *, is_default_package: bool = False, zs_dir: typing.Optional[str] = None,
+             gen_dir: typing.Optional[str] = None, top_level_package: typing.Optional[str] = None,
+             extra_args: typing.Optional[typing.List[str]] = None) -> typing.Any:
     """
     Generates Python sources by running zserio compiler.
 
     The generated Python package API will be automatically imported and returned as a result.
 
     The generated Python package will be as well automatically added to the pythonpath.
 
@@ -101,15 +102,15 @@
         java_executable = shutil.which("java")
         if not java_executable:
             raise JavaNotFoundException("compiler: Java not found (checked ${JAVA_HOME} and ${PATH})")
 
     return java_executable
 
 def _import_api_module(main_zs_file: str, is_default_package: bool, python_dir: str,
-                       top_level_package: str = None) -> typing.Any:
+                       top_level_package: typing.Optional[str] = None) -> typing.Any:
     abs_python_dir = os.path.abspath(python_dir)
     sys.path.append(abs_python_dir)
 
     api_module_path = "api"
     if not is_default_package:
         # we need to find out the first left most part of path
         if top_level_package is not None:
```

### Comparing `zserio-2.8.0/test/test_compiler.py` & `zserio-2.9.0/test/test_compiler.py`

 * *Files identical despite different names*

