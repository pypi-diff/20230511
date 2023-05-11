# Comparing `tmp/mypy-boto3-support-1.26.35.tar.gz` & `tmp/mypy-boto3-support-1.26.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-support-1.26.35.tar", last modified: Wed Dec 21 21:23:14 2022, max compression
+gzip compressed data, was "mypy-boto3-support-1.26.61.tar", last modified: Tue Jan 31 20:49:59 2023, max compression
```

## Comparing `mypy-boto3-support-1.26.35.tar` & `mypy-boto3-support-1.26.61.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 21:23:14.735104 mypy-boto3-support-1.26.35/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2022-12-21 21:23:14.735104 mypy-boto3-support-1.26.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 21:23:14.735104 mypy-boto3-support-1.26.35/mypy_boto3_support/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2022-12-21 21:22:59.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/mypy_boto3_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 21:23:14.735104 mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2022-12-21 21:23:14.000000 mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2022-12-21 21:23:14.000000 mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 21:23:14.000000 mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 21:23:14.000000 mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-21 21:23:14.000000 mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-21 21:23:14.000000 mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 21:23:14.735104 mypy-boto3-support-1.26.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2022-12-21 21:22:58.000000 mypy-boto3-support-1.26.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:59.050196 mypy-boto3-support-1.26.61/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-01-31 20:49:59.050196 mypy-boto3-support-1.26.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:59.038196 mypy-boto3-support-1.26.61/mypy_boto3_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:59.050196 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:59.050196 mypy-boto3-support-1.26.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/setup.py
```

### Comparing `mypy-boto3-support-1.26.35/LICENSE` & `mypy-boto3-support-1.26.61/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/PKG-INFO` & `mypy-boto3-support-1.26.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.26.35
-Summary: Type annotations for boto3.Support 1.26.35 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.61
+Summary: Type annotations for boto3.Support 1.26.61 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.26.35](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-support-1.26.35/README.md` & `mypy-boto3-support-1.26.61/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.26.35](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/__init__.py` & `mypy-boto3-support-1.26.61/mypy_boto3_support/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/__init__.pyi` & `mypy-boto3-support-1.26.61/mypy_boto3_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/__main__.py` & `mypy-boto3-support-1.26.61/mypy_boto3_support/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Support 1.26.35\nVersion:         1.26.35\nBuilder version:"
-        " 7.12.0\nDocs:           "
+        "Type annotations for boto3.Support 1.26.61\nVersion:         1.26.61\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.35")
+    print("1.26.61")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/client.py` & `mypy-boto3-support-1.26.61/mypy_boto3_support/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/client.pyi` & `mypy-boto3-support-1.26.61/mypy_boto3_support/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/literals.py` & `mypy-boto3-support-1.26.61/mypy_boto3_support/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,24 +71,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -196,14 +198,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/literals.pyi` & `mypy-boto3-support-1.26.61/mypy_boto3_support/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -69,24 +69,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -194,14 +196,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/paginator.py` & `mypy-boto3-support-1.26.61/mypy_boto3_support/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/paginator.pyi` & `mypy-boto3-support-1.26.61/mypy_boto3_support/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/type_defs.py` & `mypy-boto3-support-1.26.61/mypy_boto3_support/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support/type_defs.pyi` & `mypy-boto3-support-1.26.61/mypy_boto3_support/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/PKG-INFO` & `mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.26.35
-Summary: Type annotations for boto3.Support 1.26.35 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.61
+Summary: Type annotations for boto3.Support 1.26.61 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.26.35](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-support-1.26.35/mypy_boto3_support.egg-info/SOURCES.txt` & `mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.35/setup.py` & `mypy-boto3-support-1.26.61/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-support",
-    version="1.26.35",
+    version="1.26.61",
     packages=["mypy_boto3_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Support 1.26.35 service generated with mypy-boto3-builder"
-        " 7.12.0"
+        "Type annotations for boto3.Support 1.26.61 service generated with mypy-boto3-builder"
+        " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

