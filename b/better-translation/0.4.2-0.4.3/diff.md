# Comparing `tmp/better-translation-0.4.2.tar.gz` & `tmp/better-translation-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better-translation-0.4.2.tar", last modified: Thu May 11 12:31:33 2023, max compression
+gzip compressed data, was "better-translation-0.4.3.tar", last modified: Thu May 11 16:45:01 2023, max compression
```

## Comparing `better-translation-0.4.2.tar` & `better-translation-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:33.719207 better-translation-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:31:33.719207 better-translation-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 12:31:25.000000 better-translation-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:33.715206 better-translation-0.4.2/better_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:33.719207 better-translation-0.4.2/better_translation/_babel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/_babel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/_babel/lazy_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:33.719207 better-translation-0.4.2/better_translation/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:33.719207 better-translation-0.4.2/better_translation/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/integrations/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/integrations/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/integrations/django/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 12:31:25.000000 better-translation-0.4.2/better_translation/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:33.715206 better-translation-0.4.2/better_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:31:33.000000 better-translation-0.4.2/better_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 12:31:33.000000 better-translation-0.4.2/better_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:31:33.000000 better-translation-0.4.2/better_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 12:31:33.000000 better-translation-0.4.2/better_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-11 12:31:25.000000 better-translation-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:31:33.719207 better-translation-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 12:31:31.000000 better-translation-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.171024 better-translation-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 16:45:01.171024 better-translation-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 16:44:56.000000 better-translation-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.167024 better-translation-0.4.3/better_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.167024 better-translation-0.4.3/better_translation/_babel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/_babel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/_babel/lazy_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.167024 better-translation-0.4.3/better_translation/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.171024 better-translation-0.4.3/better_translation/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/django/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.167024 better-translation-0.4.3/better_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 16:45:01.000000 better-translation-0.4.3/better_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 16:45:01.000000 better-translation-0.4.3/better_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:45:01.000000 better-translation-0.4.3/better_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 16:45:01.000000 better-translation-0.4.3/better_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-11 16:44:56.000000 better-translation-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:45:01.171024 better-translation-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 16:44:59.000000 better-translation-0.4.3/setup.py
```

### Comparing `better-translation-0.4.2/better_translation/_babel/lazy_proxy.py` & `better-translation-0.4.3/better_translation/_babel/lazy_proxy.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/better_translation/extractor.py` & `better-translation-0.4.3/better_translation/extractor.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/better_translation/integrations/django/admin.py` & `better-translation-0.4.3/better_translation/integrations/django/admin.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/better_translation/integrations/django/models.py` & `better-translation-0.4.3/better_translation/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/better_translation/integrations/django/storage.py` & `better-translation-0.4.3/better_translation/integrations/django/storage.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/better_translation/provider.py` & `better-translation-0.4.3/better_translation/provider.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/better_translation/storage.py` & `better-translation-0.4.3/better_translation/storage.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/better_translation/translator.py` & `better-translation-0.4.3/better_translation/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 if TYPE_CHECKING:
     from better_translation.storage import IStorage
     from better_translation.types import (
         Locale,
         MessageID,
         TranslatedText,
     )
-
+from asgiref.sync import async_to_sync
 
 logger = logging.getLogger(__name__)
 
 
 class ITranslator(ABC):
     @abstractmethod
     def translate(  # noqa: PLR0913
@@ -125,19 +125,22 @@
             default_plural=default_plural,
             translations={},
             context="",
             has_plural=False,
             is_dynamic=True,
         )
 
-        _ = asyncio.create_task(
-            self.storage.add_messages(
-                messages=(message,),
-            ),
-        )
+        try:
+            _ = asyncio.create_task(
+                self.storage.add_messages(
+                    messages=(message,),
+                ),
+            )
+        except RuntimeError:
+            async_to_sync(self.storage.add_messages)(messages=(message,))
 
         return message
 
     def _get_singular_or_plural(
         self,
         n: int,
         singular: TranslatedText,
```

### Comparing `better-translation-0.4.2/better_translation.egg-info/SOURCES.txt` & `better-translation-0.4.3/better_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/pyproject.toml` & `better-translation-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.2/setup.py` & `better-translation-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 _version = (
-    "0.4.2"  # Version will be replaced by the CD pipeline
+    "0.4.3"  # Version will be replaced by the CD pipeline
 )
 VERSION = "0.0.0" if _version.startswith("{{") else _version
 
 
 def get_readme() -> str:
     readme = Path("README.md")
     return readme.read_text(encoding="utf-8")
```

