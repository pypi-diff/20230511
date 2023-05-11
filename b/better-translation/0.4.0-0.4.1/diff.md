# Comparing `tmp/better-translation-0.4.0.tar.gz` & `tmp/better-translation-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better-translation-0.4.0.tar", last modified: Thu May 11 12:00:43 2023, max compression
+gzip compressed data, was "better-translation-0.4.1.tar", last modified: Thu May 11 12:23:18 2023, max compression
```

## Comparing `better-translation-0.4.0.tar` & `better-translation-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:00:43.910112 better-translation-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 12:00:39.000000 better-translation-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.906112 better-translation-0.4.0/better_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/better_translation/_babel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/_babel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/_babel/lazy_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/better_translation/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/better_translation/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/django/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/better_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:00:43.000000 better-translation-0.4.0/better_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 12:00:43.000000 better-translation-0.4.0/better_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:00:43.000000 better-translation-0.4.0/better_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 12:00:43.000000 better-translation-0.4.0/better_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-11 12:00:39.000000 better-translation-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:00:43.910112 better-translation-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 12:00:41.000000 better-translation-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:18.897700 better-translation-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:23:18.897700 better-translation-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 12:23:13.000000 better-translation-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:18.897700 better-translation-0.4.1/better_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:18.897700 better-translation-0.4.1/better_translation/_babel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/_babel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/_babel/lazy_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:18.897700 better-translation-0.4.1/better_translation/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:18.897700 better-translation-0.4.1/better_translation/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/integrations/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/integrations/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/integrations/django/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 12:23:13.000000 better-translation-0.4.1/better_translation/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:23:18.897700 better-translation-0.4.1/better_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:23:18.000000 better-translation-0.4.1/better_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 12:23:18.000000 better-translation-0.4.1/better_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:23:18.000000 better-translation-0.4.1/better_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 12:23:18.000000 better-translation-0.4.1/better_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-11 12:23:13.000000 better-translation-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:23:18.897700 better-translation-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 12:23:17.000000 better-translation-0.4.1/setup.py
```

### Comparing `better-translation-0.4.0/better_translation/_babel/lazy_proxy.py` & `better-translation-0.4.1/better_translation/_babel/lazy_proxy.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.0/better_translation/extractor.py` & `better-translation-0.4.1/better_translation/extractor.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.0/better_translation/integrations/django/admin.py` & `better-translation-0.4.1/better_translation/integrations/django/admin.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.0/better_translation/integrations/django/models.py` & `better-translation-0.4.1/better_translation/integrations/django/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     context = models.CharField(
         max_length=1024,
         default="",
         blank=True,
     )
     has_plural = models.BooleanField(verbose_name="Has plural", default=False)
     is_used = models.BooleanField(verbose_name="Is used", default=True)
+    is_dynamic = models.BooleanField(verbose_name="Is dynamic", default=False)
 
     translations: models.QuerySet[BaseTranslation]
     """A QuerySet of translations for this message."""
 
     def __str__(self) -> str:
         return f"Message: {self.id}"
```

### Comparing `better-translation-0.4.0/better_translation/integrations/django/storage.py` & `better-translation-0.4.1/better_translation/integrations/django/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     def _get_storage_message(message: BaseMessage) -> StorageMessage:
         return StorageMessage(
             id=message.id,
             default=message.default,
             default_plural=message.default_plural,
             context=message.context,
             has_plural=message.has_plural,
+            is_dynamic=message.is_dynamic,
             translations={
                 translation.locale: StorageTranslation(
                     singular=translation.singular,
                     plural=translation.singular,
                 )
                 for translation in message.translations.all()
             },
@@ -132,8 +133,9 @@
     ) -> BaseMessage:
         return self.message_model(
             id=storage_message.id,
             default=storage_message.default,
             default_plural=storage_message.default_plural,
             context=storage_message.context,
             has_plural=storage_message.has_plural,
+            is_dynamic=storage_message.is_dynamic,
         )
```

### Comparing `better-translation-0.4.0/better_translation/provider.py` & `better-translation-0.4.1/better_translation/provider.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.0/better_translation/storage.py` & `better-translation-0.4.1/better_translation/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 class StorageMessage:
     id: MessageID
     default: TranslatedText
     default_plural: TranslatedText
     context: str
     has_plural: bool
     translations: Mapping[Locale, StorageTranslation]
+    is_dynamic: bool = False
 
 
 @dataclass(slots=True)
 class StorageTranslation:
     singular: TranslatedText
     plural: TranslatedText
```

### Comparing `better-translation-0.4.0/better_translation/translator.py` & `better-translation-0.4.1/better_translation/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         message = StorageMessage(
             id=message_id,
             default=default,
             default_plural=default_plural,
             translations={},
             context="",
             has_plural=False,
+            is_dynamic=True,
         )
 
         _ = asyncio.create_task(
             self.storage.add_messages(
                 messages=(message,),
             ),
         )
```

### Comparing `better-translation-0.4.0/better_translation.egg-info/SOURCES.txt` & `better-translation-0.4.1/better_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.0/pyproject.toml` & `better-translation-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.0/setup.py` & `better-translation-0.4.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 _version = (
-    "0.4.0"  # Version will be replaced by the CD pipeline
+    "0.4.1"  # Version will be replaced by the CD pipeline
 )
 VERSION = "0.0.0" if _version.startswith("{{") else _version
 
 
 def get_readme() -> str:
     readme = Path("README.md")
     return readme.read_text(encoding="utf-8")
```

