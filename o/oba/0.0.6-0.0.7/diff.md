# Comparing `tmp/oba-0.0.6.tar.gz` & `tmp/oba-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oba-0.0.6.tar", last modified: Mon Oct 31 05:43:26 2022, max compression
+gzip compressed data, was "oba-0.0.7.tar", last modified: Thu May 11 10:18:50 2023, max compression
```

## Comparing `oba-0.0.6.tar` & `oba-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2022-10-31 05:43:26.361726 oba-0.0.6/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      665 2022-10-31 05:43:26.361629 oba-0.0.6/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      380 2022-10-21 09:44:26.000000 oba-0.0.6/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2022-10-31 05:43:26.361101 oba-0.0.6/oba/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       59 2022-10-21 09:44:26.000000 oba-0.0.6/oba/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1985 2022-10-31 05:43:17.000000 oba-0.0.6/oba/oba.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2022-10-31 05:43:26.361491 oba-0.0.6/oba.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      665 2022-10-31 05:43:26.000000 oba-0.0.6/oba.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      153 2022-10-31 05:43:26.000000 oba-0.0.6/oba.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2022-10-31 05:43:26.000000 oba-0.0.6/oba.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        4 2022-10-31 05:43:26.000000 oba-0.0.6/oba.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2022-10-31 05:43:26.361756 oba-0.0.6/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      609 2022-10-31 05:43:21.000000 oba-0.0.6/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-11 10:18:50.680847 oba-0.0.7/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1068 2022-11-07 04:42:30.000000 oba-0.0.7/LICENSE
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      798 2023-05-11 10:18:50.680743 oba-0.0.7/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      491 2022-11-07 04:37:13.000000 oba-0.0.7/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-11 10:18:50.680043 oba-0.0.7/oba/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       59 2022-10-21 09:44:26.000000 oba-0.0.7/oba/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     2320 2023-05-11 10:00:56.000000 oba-0.0.7/oba/oba.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-11 10:18:50.680588 oba-0.0.7/oba.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      798 2023-05-11 10:18:50.000000 oba-0.0.7/oba.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      161 2023-05-11 10:18:50.000000 oba-0.0.7/oba.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-05-11 10:18:50.000000 oba-0.0.7/oba.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        4 2023-05-11 10:18:50.000000 oba-0.0.7/oba.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-05-11 10:18:50.680884 oba-0.0.7/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      609 2023-05-11 10:18:39.000000 oba-0.0.7/setup.py
```

### Comparing `oba-0.0.6/oba/oba.py` & `oba-0.0.7/oba/oba.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from collections.abc import Iterable
+
+
 class NoneObj:
     __obj = dict()
 
     @staticmethod
     def raw(o: 'NoneObj'):
         return object.__getattribute__(o, '__path')
 
@@ -24,51 +27,58 @@
     def __setattr__(self, key, value):
         return
 
     def __bool__(self):
         return False
 
     def __str__(self):
-        raise ValueError(f'NoneObj ({NoneObj.raw(self)})')
+        raise ValueError(f'Path {NoneObj.raw(self)} not exists')
     
     
 class Obj:
     @staticmethod
     def iterable(obj):
-        types = [list, dict, tuple]
-        for t in types:
-            if isinstance(obj, t):
-                return True
-        return False
+        return isinstance(obj, Iterable)
 
     @staticmethod
     def raw(o: 'Obj'):
         if isinstance(o, Obj):
             return object.__getattribute__(o, '__obj')
         return o
 
-    def __init__(self, obj):
+    def __init__(self, obj=None):
+        if obj is None:
+            obj = {}
+        assert Obj.iterable(obj), TypeError('Obj input should be iterable')
         object.__setattr__(self, '__obj', obj)
 
     def __getitem__(self, item):
+        item = item.split('.', maxsplit=1)
+
         obj = Obj.raw(self)
         try:
-            obj = obj.__getitem__(item)
+            obj = obj.__getitem__(item[0])
         except Exception:
-            return NoneObj(f'{item}')
+            return NoneObj(f'{item[0]}')
         if Obj.iterable(obj):
-            return Obj(obj)
+            obj = Obj(obj)
+        if len(item) > 1:
+            obj = obj[item[1]]
         return obj
 
-    def __getattr__(self, item):
+    def __getattr__(self, item: str):
         return self[item]
 
-    def __setitem__(self, key, value):
-        obj = Obj.raw(self)
-        obj[key] = value
+    def __setitem__(self, key: str, value):
+        key = key.split('.', maxsplit=1)
+        if len(key) == 1:
+            obj = Obj.raw(self)
+            obj[key[0]] = value
+        else:
+            self[key[0]][key[1]] = value
 
     def __setattr__(self, key, value):
         self[key] = value
 
     def __contains__(self, item):
         obj = Obj.raw(self)
         return item in obj
@@ -81,10 +91,9 @@
             yield item
 
     def __len__(self):
         return len(Obj.raw(self))
 
 
 if __name__ == '__main__':
-    o = Obj({'m': 5})
-    print(o.m)
-    print(o.a.b[0].x)
+    o = Obj({'a': {'b': {'c': {'d': 1}}}})
+    print(o['a']['b.c']['e.f.g'])
```

### Comparing `oba-0.0.6/setup.py` & `oba-0.0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='oba',
-    version='0.0.6',
+    version='0.0.7',
     keywords=['dict', 'object'],
     description='make iter object easy to access (item to attr)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/Oba',
     author='Jyonn Liu',
```

