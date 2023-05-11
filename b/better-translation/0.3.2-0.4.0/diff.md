# Comparing `tmp/better-translation-0.3.2.tar.gz` & `tmp/better-translation-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better-translation-0.3.2.tar", last modified: Fri Apr 14 17:50:04 2023, max compression
+gzip compressed data, was "better-translation-0.4.0.tar", last modified: Thu May 11 12:00:43 2023, max compression
```

## Comparing `better-translation-0.3.2.tar` & `better-translation-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 17:50:04.147652 better-translation-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 17:50:01.000000 better-translation-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation/_babel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/_babel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/_babel/lazy_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/django/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 17:50:04.000000 better-translation-0.3.2/better_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-14 17:50:04.000000 better-translation-0.3.2/better_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:50:04.000000 better-translation-0.3.2/better_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 17:50:04.000000 better-translation-0.3.2/better_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-14 17:50:01.000000 better-translation-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:50:04.147652 better-translation-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 17:50:03.000000 better-translation-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:00:43.910112 better-translation-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 12:00:39.000000 better-translation-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.906112 better-translation-0.4.0/better_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/better_translation/_babel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/_babel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/_babel/lazy_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/better_translation/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/better_translation/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/integrations/django/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 12:00:39.000000 better-translation-0.4.0/better_translation/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:00:43.910112 better-translation-0.4.0/better_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:00:43.000000 better-translation-0.4.0/better_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 12:00:43.000000 better-translation-0.4.0/better_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:00:43.000000 better-translation-0.4.0/better_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 12:00:43.000000 better-translation-0.4.0/better_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-11 12:00:39.000000 better-translation-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:00:43.910112 better-translation-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 12:00:41.000000 better-translation-0.4.0/setup.py
```

### Comparing `better-translation-0.3.2/better_translation/_babel/lazy_proxy.py` & `better-translation-0.4.0/better_translation/_babel/lazy_proxy.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.2/better_translation/extractor.py` & `better-translation-0.4.0/better_translation/extractor.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.2/better_translation/integrations/django/admin.py` & `better-translation-0.4.0/better_translation/integrations/django/admin.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.2/better_translation/integrations/django/models.py` & `better-translation-0.4.0/better_translation/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.2/better_translation/integrations/django/storage.py` & `better-translation-0.4.0/better_translation/integrations/django/storage.py`

 * *Files 23% similar despite different names*

```diff
@@ -70,20 +70,48 @@
 
             logger.info("Adding message '%s' to the storage", message)
             self.storage[message.id] = message
             messages_to_create.add(self._get_message_model(message))
 
         await self.message_model.objects.abulk_create(messages_to_create)
 
-    async def add_messages_from_dirs(self, *dirs: Path) -> None:
+    async def add_messages_from_dirs(
+        self,
+        *dirs: Path,
+        update_messages_usage: bool = False,
+    ) -> list[StorageMessage]:
         messages: list[StorageMessage] = []
         for directory_path in dirs:
             messages.extend(self._extract_messages_from_dir(directory_path))
 
         await self.add_messages(messages)
+        if update_messages_usage:
+            await self.update_messages_usage(messages)
+
+        return messages
+
+    async def update_messages_usage(
+        self,
+        messages: Sequence[StorageMessage],
+    ) -> None:
+        logger.info("Finding unused messages...")
+
+        messages_ids = {message.id for message in messages}
+        unused_message_number = await self.message_model.objects.exclude(
+            id__in=messages_ids,
+        ).aupdate(is_used=False)
+
+        await self.message_model.objects.filter(
+            id__in=messages_ids,
+        ).aupdate(is_used=True)
+
+        logger.info(
+            "Found %s unused messages",
+            unused_message_number,
+        )
 
     @staticmethod
     def _get_storage_message(message: BaseMessage) -> StorageMessage:
         return StorageMessage(
             id=message.id,
             default=message.default,
             default_plural=message.default_plural,
```

### Comparing `better-translation-0.3.2/better_translation/provider.py` & `better-translation-0.4.0/better_translation/provider.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.2/better_translation/storage.py` & `better-translation-0.4.0/better_translation/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     async def add_messages(self, messages: Sequence[StorageMessage]) -> None:
         """Add new messages to the storage.
 
         Ignores messages that are already in the storage.
         """
 
     @abstractmethod
-    async def add_messages_from_dirs(self, *dirs: Path) -> None:
+    async def add_messages_from_dirs(self, *dirs: Path) -> list[StorageMessage]:
         """Add new messages to the storage from the given directories."""
 
 
 @dataclass(slots=True)
 class BaseStorage(IStorage, ABC):
     storage: dict[MessageID, StorageMessage] = field(
         default_factory=dict,
```

### Comparing `better-translation-0.3.2/better_translation/translator.py` & `better-translation-0.4.0/better_translation/translator.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.2/better_translation.egg-info/SOURCES.txt` & `better-translation-0.4.0/better_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.2/pyproject.toml` & `better-translation-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.2/setup.py` & `better-translation-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 _version = (
-    "0.3.2"  # Version will be replaced by the CD pipeline
+    "0.4.0"  # Version will be replaced by the CD pipeline
 )
 VERSION = "0.0.0" if _version.startswith("{{") else _version
 
 
 def get_readme() -> str:
     readme = Path("README.md")
     return readme.read_text(encoding="utf-8")
```

