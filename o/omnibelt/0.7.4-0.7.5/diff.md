# Comparing `tmp/omnibelt-0.7.4.tar.gz` & `tmp/omnibelt-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnibelt-0.7.4.tar", last modified: Tue Apr  4 10:02:36 2023, max compression
+gzip compressed data, was "omnibelt-0.7.5.tar", last modified: Thu May 11 08:40:47 2023, max compression
```

## Comparing `omnibelt-0.7.4.tar` & `omnibelt-0.7.5.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        0 2023-04-04 10:02:36.952993 omnibelt-0.7.4/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)       31 2022-10-10 21:24:56.000000 omnibelt-0.7.4/.fig.yaml
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     1067 2022-10-10 21:24:56.000000 omnibelt-0.7.4/LICENSE
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      250 2023-04-04 10:02:36.946810 omnibelt-0.7.4/PKG-INFO
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      272 2022-10-10 21:24:56.000000 omnibelt-0.7.4/README.md
-drwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        0 2023-04-04 10:02:36.706779 omnibelt-0.7.4/omnibelt/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3140 2023-03-11 23:06:07.000000 omnibelt-0.7.4/omnibelt/__init__.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      565 2023-04-04 10:02:25.000000 omnibelt-0.7.4/omnibelt/_info.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    23793 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/basic_containers.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3378 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/containers.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3530 2023-04-04 10:01:24.000000 omnibelt-0.7.4/omnibelt/crafts.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     1684 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/errors.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    13797 2023-03-11 23:06:07.000000 omnibelt-0.7.4/omnibelt/exporting.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3748 2023-01-03 02:31:14.000000 omnibelt-0.7.4/omnibelt/exporting_common.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    16842 2022-10-25 23:11:34.000000 omnibelt-0.7.4/omnibelt/farming.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     8341 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/filesystem.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     2754 2023-01-03 02:31:14.000000 omnibelt-0.7.4/omnibelt/flow.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      334 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/hashing.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     4324 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/logging.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     5663 2023-01-03 02:31:14.000000 omnibelt-0.7.4/omnibelt/logic.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    35399 2023-01-03 02:31:14.000000 omnibelt-0.7.4/omnibelt/nodes.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     7801 2023-01-30 14:58:55.000000 omnibelt-0.7.4/omnibelt/operators.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    20294 2023-01-03 02:31:14.000000 omnibelt-0.7.4/omnibelt/ordered_set.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    18477 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/packing.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     2038 2022-10-27 18:12:45.000000 omnibelt-0.7.4/omnibelt/patterns.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3913 2023-01-30 14:58:55.000000 omnibelt-0.7.4/omnibelt/propagators.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    12961 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/pure_packing.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     8195 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/registries.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     8409 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/secure.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     4483 2023-01-03 02:31:14.000000 omnibelt-0.7.4/omnibelt/structured.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      264 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/timing.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     2054 2022-10-10 21:25:01.000000 omnibelt-0.7.4/omnibelt/transactions.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    43082 2023-01-30 14:58:55.000000 omnibelt-0.7.4/omnibelt/tricks.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     6536 2023-01-22 20:47:09.000000 omnibelt-0.7.4/omnibelt/typing.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      853 2023-03-26 15:25:59.000000 omnibelt-0.7.4/omnibelt/utils.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     1761 2022-10-17 21:06:18.000000 omnibelt-0.7.4/omnibelt/viz.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     6097 2023-01-16 22:53:08.000000 omnibelt-0.7.4/omnibelt/wrappers.py
-drwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        0 2023-04-04 10:02:36.910148 omnibelt-0.7.4/omnibelt.egg-info/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      250 2023-04-04 10:02:34.000000 omnibelt-0.7.4/omnibelt.egg-info/PKG-INFO
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      880 2023-04-04 10:02:34.000000 omnibelt-0.7.4/omnibelt.egg-info/SOURCES.txt
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        1 2023-04-04 10:02:34.000000 omnibelt-0.7.4/omnibelt.egg-info/dependency_links.txt
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        2 2020-06-29 21:05:59.000000 omnibelt-0.7.4/omnibelt.egg-info/not-zip-safe
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)       71 2023-04-04 10:02:34.000000 omnibelt-0.7.4/omnibelt.egg-info/requires.txt
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        9 2023-04-04 10:02:34.000000 omnibelt-0.7.4/omnibelt.egg-info/top_level.txt
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)       38 2023-04-04 10:02:36.954924 omnibelt-0.7.4/setup.cfg
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     1142 2022-10-10 21:25:01.000000 omnibelt-0.7.4/setup.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-11 08:40:47.544014 omnibelt-0.7.5/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1067 2020-09-28 09:56:44.000000 omnibelt-0.7.5/LICENSE
+-rw-r--r--   0 fleeb     (7343) is        (1040)      233 2023-05-11 08:40:47.541015 omnibelt-0.7.5/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)      272 2022-01-21 09:21:49.000000 omnibelt-0.7.5/README.md
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-11 08:40:47.429017 omnibelt-0.7.5/omnibelt/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3140 2023-03-05 18:25:46.000000 omnibelt-0.7.5/omnibelt/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      565 2023-05-11 08:40:39.000000 omnibelt-0.7.5/omnibelt/_info.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    23793 2021-08-09 09:34:56.000000 omnibelt-0.7.5/omnibelt/basic_containers.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3378 2021-10-13 13:02:21.000000 omnibelt-0.7.5/omnibelt/containers.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3530 2023-03-31 13:07:56.000000 omnibelt-0.7.5/omnibelt/crafts.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1684 2021-08-09 09:34:56.000000 omnibelt-0.7.5/omnibelt/errors.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    13797 2023-03-06 10:10:49.000000 omnibelt-0.7.5/omnibelt/exporting.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3748 2022-12-26 15:53:28.000000 omnibelt-0.7.5/omnibelt/exporting_common.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    16842 2022-10-26 09:57:16.000000 omnibelt-0.7.5/omnibelt/farming.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8341 2022-04-04 07:55:06.000000 omnibelt-0.7.5/omnibelt/filesystem.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2754 2022-12-28 18:59:48.000000 omnibelt-0.7.5/omnibelt/flow.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      334 2022-04-30 14:13:38.000000 omnibelt-0.7.5/omnibelt/hashing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4324 2022-04-18 10:19:57.000000 omnibelt-0.7.5/omnibelt/logging.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5663 2023-01-01 19:17:56.000000 omnibelt-0.7.5/omnibelt/logic.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    35399 2022-12-25 17:28:02.000000 omnibelt-0.7.5/omnibelt/nodes.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     7801 2023-02-20 09:22:06.000000 omnibelt-0.7.5/omnibelt/operators.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    20294 2022-12-20 16:32:10.000000 omnibelt-0.7.5/omnibelt/ordered_set.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    18477 2022-09-20 14:19:20.000000 omnibelt-0.7.5/omnibelt/packing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2038 2022-10-26 16:21:50.000000 omnibelt-0.7.5/omnibelt/patterns.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3913 2023-02-20 09:22:06.000000 omnibelt-0.7.5/omnibelt/propagators.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    12961 2021-08-09 09:34:56.000000 omnibelt-0.7.5/omnibelt/pure_packing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8378 2023-05-10 11:53:12.000000 omnibelt-0.7.5/omnibelt/registries.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8409 2022-04-04 07:55:06.000000 omnibelt-0.7.5/omnibelt/secure.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4483 2023-01-01 18:32:59.000000 omnibelt-0.7.5/omnibelt/structured.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      264 2021-01-14 22:27:58.000000 omnibelt-0.7.5/omnibelt/timing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2054 2021-08-09 09:34:56.000000 omnibelt-0.7.5/omnibelt/transactions.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    43082 2023-02-20 09:22:06.000000 omnibelt-0.7.5/omnibelt/tricks.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6536 2023-01-21 17:15:30.000000 omnibelt-0.7.5/omnibelt/typing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      853 2023-03-16 17:01:14.000000 omnibelt-0.7.5/omnibelt/utils.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1761 2022-10-17 14:37:13.000000 omnibelt-0.7.5/omnibelt/viz.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6097 2023-01-16 21:22:29.000000 omnibelt-0.7.5/omnibelt/wrappers.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-11 08:40:47.498014 omnibelt-0.7.5/omnibelt.egg-info/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      233 2023-05-11 08:40:45.000000 omnibelt-0.7.5/omnibelt.egg-info/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)      984 2023-05-11 08:40:46.000000 omnibelt-0.7.5/omnibelt.egg-info/SOURCES.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        1 2023-05-11 08:40:45.000000 omnibelt-0.7.5/omnibelt.egg-info/dependency_links.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        1 2020-09-28 09:57:04.000000 omnibelt-0.7.5/omnibelt.egg-info/not-zip-safe
+-rw-r--r--   0 fleeb     (7343) is        (1040)       71 2023-05-11 08:40:45.000000 omnibelt-0.7.5/omnibelt.egg-info/requires.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        9 2023-05-11 08:40:45.000000 omnibelt-0.7.5/omnibelt.egg-info/top_level.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)       38 2023-05-11 08:40:47.545015 omnibelt-0.7.5/setup.cfg
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1142 2021-08-09 09:34:56.000000 omnibelt-0.7.5/setup.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-11 08:40:47.535017 omnibelt-0.7.5/tests/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      883 2021-08-09 09:34:56.000000 omnibelt-0.7.5/tests/test_basics.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      666 2021-08-09 09:34:56.000000 omnibelt-0.7.5/tests/test_packing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      796 2021-08-09 09:34:56.000000 omnibelt-0.7.5/tests/test_secure.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      535 2021-08-09 09:34:56.000000 omnibelt-0.7.5/tests/test_transactions.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1018 2022-10-26 09:57:16.000000 omnibelt-0.7.5/tests/test_wrappers.py
```

### Comparing `omnibelt-0.7.4/LICENSE` & `omnibelt-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/__init__.py` & `omnibelt-0.7.5/omnibelt/__init__.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/_info.py` & `omnibelt-0.7.5/omnibelt/_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 name = 'omnibelt'
 long_name = 'omni-belt'
 
-version = '0.7.4'
+version = '0.7.5'
 url = 'https://github.com/felixludos/omni-belt'
 
 description = 'Universal python utilities'
 
 author = 'Felix Leeb'
 author_email = 'felixludos.info@gmail.com'
```

### Comparing `omnibelt-0.7.4/omnibelt/basic_containers.py` & `omnibelt-0.7.5/omnibelt/basic_containers.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/containers.py` & `omnibelt-0.7.5/omnibelt/containers.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/crafts.py` & `omnibelt-0.7.5/omnibelt/crafts.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/errors.py` & `omnibelt-0.7.5/omnibelt/errors.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/exporting.py` & `omnibelt-0.7.5/omnibelt/exporting.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/exporting_common.py` & `omnibelt-0.7.5/omnibelt/exporting_common.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/farming.py` & `omnibelt-0.7.5/omnibelt/farming.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/filesystem.py` & `omnibelt-0.7.5/omnibelt/filesystem.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/flow.py` & `omnibelt-0.7.5/omnibelt/flow.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/logging.py` & `omnibelt-0.7.5/omnibelt/logging.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/logic.py` & `omnibelt-0.7.5/omnibelt/logic.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/nodes.py` & `omnibelt-0.7.5/omnibelt/nodes.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/operators.py` & `omnibelt-0.7.5/omnibelt/operators.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/ordered_set.py` & `omnibelt-0.7.5/omnibelt/ordered_set.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/packing.py` & `omnibelt-0.7.5/omnibelt/packing.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/patterns.py` & `omnibelt-0.7.5/omnibelt/patterns.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/propagators.py` & `omnibelt-0.7.5/omnibelt/propagators.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/pure_packing.py` & `omnibelt-0.7.5/omnibelt/pure_packing.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/registries.py` & `omnibelt-0.7.5/omnibelt/registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,18 @@
 	def _get_sister_entry_key(cls, key, value):
 		assert isinstance(value, cls.entry_cls)
 		if key == getattr(value, cls._key_name):
 			return getattr(value, cls._sister_key_name)
 		return getattr(value, cls._key_name)
 
 
-	def get_value(self, key):
-		return getattr(self.find(key), self._sister_key_name)
+	def get_value(self, key, default=unspecified_argument):
+		if default is unspecified_argument:
+			return getattr(self.find(key), self._sister_key_name)
+		return getattr(self.find(key), self._sister_key_name, default)
 
 
 	def update(self, other, sync=True):
 		if sync:
 			self._sister_registry_object.update({self._get_sister_entry_key(k, v): v
 			                                     for k, v in other.items()}, sync=False)
 		return super().update(other, sync=False)
@@ -257,16 +259,16 @@
 
 class Class_Registry(Entry_Double_Registry, sister_component='cls'):
 
 	def __init_subclass__(cls, sister_component='cls', components=[], required=[]):
 		super().__init_subclass__(primary_component='name', sister_component=sister_component,
 		                          components=components, required=required)
 
-	def get_class(self, key):
-		return self.get_value(key)
+	def get_class(self, key, default=unspecified_argument):
+		return self.get_value(key, default=default)
 
 	class DecoratorBase(Entry_Double_Registry.DecoratorBase):
 		def _register(self, val, name=None, **params):
 			if name is None:
 				name = val.__name__
 			return super()._register(val, name=name, **params)
```

### Comparing `omnibelt-0.7.4/omnibelt/secure.py` & `omnibelt-0.7.5/omnibelt/secure.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/structured.py` & `omnibelt-0.7.5/omnibelt/structured.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/transactions.py` & `omnibelt-0.7.5/omnibelt/transactions.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/tricks.py` & `omnibelt-0.7.5/omnibelt/tricks.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/typing.py` & `omnibelt-0.7.5/omnibelt/typing.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/utils.py` & `omnibelt-0.7.5/omnibelt/utils.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/viz.py` & `omnibelt-0.7.5/omnibelt/viz.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt/wrappers.py` & `omnibelt-0.7.5/omnibelt/wrappers.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.7.4/omnibelt.egg-info/SOURCES.txt` & `omnibelt-0.7.5/omnibelt.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.fig.yaml
 LICENSE
 README.md
 setup.py
 omnibelt/__init__.py
 omnibelt/_info.py
 omnibelt/basic_containers.py
 omnibelt/containers.py
@@ -34,8 +33,13 @@
 omnibelt/viz.py
 omnibelt/wrappers.py
 omnibelt.egg-info/PKG-INFO
 omnibelt.egg-info/SOURCES.txt
 omnibelt.egg-info/dependency_links.txt
 omnibelt.egg-info/not-zip-safe
 omnibelt.egg-info/requires.txt
-omnibelt.egg-info/top_level.txt
+omnibelt.egg-info/top_level.txt
+tests/test_basics.py
+tests/test_packing.py
+tests/test_secure.py
+tests/test_transactions.py
+tests/test_wrappers.py
```

### Comparing `omnibelt-0.7.4/setup.py` & `omnibelt-0.7.5/setup.py`

 * *Files identical despite different names*

