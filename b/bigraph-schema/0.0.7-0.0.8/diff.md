# Comparing `tmp/bigraph-schema-0.0.7.tar.gz` & `tmp/bigraph-schema-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigraph-schema-0.0.7.tar", last modified: Fri May  5 23:02:52 2023, max compression
+gzip compressed data, was "bigraph-schema-0.0.8.tar", last modified: Wed May 10 21:58:21 2023, max compression
```

## Comparing `bigraph-schema-0.0.7.tar` & `bigraph-schema-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      378 2023-04-24 01:31:10.000000 bigraph-schema-0.0.7/README.md
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/bigraph_schema/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      106 2023-04-19 21:19:48.000000 bigraph-schema-0.0.7/bigraph_schema/__init__.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.7/bigraph_schema/parse.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      919 2023-04-20 03:53:50.000000 bigraph-schema-0.0.7/bigraph_schema/protocol.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18894 2023-05-05 23:00:46.000000 bigraph-schema-0.0.7/bigraph_schema/registry.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    19757 2023-05-05 23:00:52.000000 bigraph-schema-0.0.7/bigraph_schema/schema.py
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/bigraph_schema.egg-info/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      337 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       25 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/requires.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/top_level.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/setup.cfg
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1327 2023-05-05 23:02:36.000000 bigraph-schema-0.0.7/setup.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      378 2023-04-24 01:31:10.000000 bigraph-schema-0.0.8/README.md
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/bigraph_schema/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      120 2023-05-09 21:20:11.000000 bigraph-schema-0.0.8/bigraph_schema/__init__.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.8/bigraph_schema/parse.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      919 2023-04-20 03:53:50.000000 bigraph-schema-0.0.8/bigraph_schema/protocol.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    22067 2023-05-10 21:40:16.000000 bigraph-schema-0.0.8/bigraph_schema/registry.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18418 2023-05-10 21:39:51.000000 bigraph-schema-0.0.8/bigraph_schema/schema.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/bigraph_schema.egg-info/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      337 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       25 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/requires.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/top_level.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/setup.cfg
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1327 2023-05-10 21:57:59.000000 bigraph-schema-0.0.8/setup.py
```

### Comparing `bigraph-schema-0.0.7/PKG-INFO` & `bigraph-schema-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.7
+Version: 0.0.8
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.7/bigraph_schema/parse.py` & `bigraph-schema-0.0.8/bigraph_schema/parse.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.7/bigraph_schema/protocol.py` & `bigraph-schema-0.0.8/bigraph_schema/protocol.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.7/bigraph_schema/registry.py` & `bigraph-schema-0.0.8/bigraph_schema/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 import random
 import pytest
 from typing import Any
 
 from bigraph_schema.parse import parse_type_parameters
 
+NONE_SYMBOL = ''
+
 required_schema_keys = (
     '_default',
     '_apply',
     '_serialize',
     '_deserialize',
 )
 
@@ -203,14 +205,16 @@
 
         return result
 
 
     def substitute_type(self, schema):
         if isinstance(schema, str):
             schema = self.access(schema)
+            if schema is None:
+                raise Exception(f'trying to substitute a type that is unrecognized {schema}')
         elif '_type' in schema:
             type_key = schema['_type']
             type_schema = copy.deepcopy(self.access(type_key))
             schema = deep_merge(type_schema, schema)
 
         return schema
 
@@ -240,16 +244,21 @@
 
         if '_default' in schema:
             if not '_deserialize' in schema:
                 raise Exception(
                     f'asking for default for {type_key} but no deserialize in {schema}')
             deserialize = deserialize_registry.access(
                 schema['_deserialize'])
-            default = deserialize(
-                schema['_default'])
+            if '_type_parameters' in schema:
+                default = deserialize(
+                    schema['_default'],
+                    schema['_type_parameters'])
+            else:
+                default = deserialize(
+                    schema['_default'])
         else:
             default = {}
             for key, subschema in schema.items():
                 if key not in type_schema_keys:
                     default[key] = self.generate_default(subschema)
 
         return default
@@ -308,39 +317,73 @@
 registry_registry.register('_type', type_registry)
 registry_registry.register('_apply', apply_registry)
 registry_registry.register('_divide', divide_registry)
 registry_registry.register('_serialize', serialize_registry)
 registry_registry.register('_deserialize', deserialize_registry)
 
 
+def apply_update(schema, state, update):
+    # expects an expanded schema
+
+    if '_apply' in schema:
+        apply_function = apply_registry.access(schema['_apply'])
+        if '_type_parameters' in schema:
+            state = apply_function(state, update, schema['_type_parameters'])
+        else:
+            state = apply_function(state, update)
+    elif isinstance(update, dict):
+        for key, branch in update.items():
+            if key not in schema:
+                raise Exception(f'trying to update a key that is not in the schema {key} for state:\n{state}\nwith schema:\n{schema}')
+            else:
+                subupdate = apply_update(
+                    schema[key],
+                    state[key],
+                    branch
+                )
+
+                state[key] = subupdate
+    else:
+        schema = type_registry.expand_schema(schema)
+        state = apply_update(schema, state, update)
+
+    return state
+
+
+def apply(schema, initial, update):
+    expanded = type_registry.expand(schema)
+    state = copy.deepcopy(initial)
+    return apply_update(expanded, initial, update)
+
+
 def accumulate(current, update):
     return current + update
 
 def concatenate(current, update):
     return current + update
 
-def divide_float(value, _):
+def divide_float(value):
     half = value / 2.0
     return (half, half)
 
 # support function types for registrys?
 # def divide_int(value: int, _) -> tuple[int, int]:
-def divide_int(value, _):
+def divide_int(value):
     half = value // 2
     other_half = half
     if value % 2 == 1:
         other_half += 1
     return half, other_half
 
 
 # class DivideRegistry(Registry):
     
 
 # def divide_longest(dimensions: Dimension) -> Tuple[Dimension, Dimension]:
-def divide_longest(dimensions, _):
+def divide_longest(dimensions):
     # any way to declare the required keys for this function in the registry?
     # find a way to ask a function what type its domain and codomain are
 
     width = dimensions['width']
     height = dimensions['height']
     
     if width > height:
@@ -386,39 +429,77 @@
 
 
 def replace(old_value, new_value):
     return new_value
 
 
 # TODO: make these work
-def serialize_dict(value):
+def serialize_dict(value, type_parameters):
     return value
 
 
-def deserialize_dict(value):
+def deserialize_dict(value, type_parameters):
     return value
 
 
+def maybe_apply(current, update, type_parameters):
+    if current is None or update is None:
+        return update
+    else:
+        maybe_type = type_registry.access(parameters[0])
+        return apply_update(maybe_type, current, update)
+
+
+def maybe_divide(value, type_parameters):
+    if value is None:
+        return [None, None]
+    else:
+        pass
+
+
+def maybe_serialize(value, type_parameters):
+    if value is None:
+        return NONE_SYMBOL
+    else:
+        maybe_type = type_registry.access(parameters[0])
+        return serialize(maybe_type, value)
+
+
+def maybe_deserialize(encoded, type_parameters):
+    if encoded == NONE_SYMBOL:
+        return None
+    else:
+        maybe_type = type_registry.access(parameters[0])
+        return deserialize(maybe_type, encoded)
+
+
 # validate the function registered is of the right type?
 apply_registry.register('accumulate', accumulate)
 apply_registry.register('concatenate', concatenate)
 apply_registry.register('replace', replace)
 apply_registry.register('merge', deep_merge)
+apply_registry.register('maybe_apply', maybe_apply)
+
 divide_registry.register('divide_float', divide_float)
 divide_registry.register('divide_int', divide_int)
 divide_registry.register('divide_longest', divide_longest)
 divide_registry.register('divide_list', divide_list)
 divide_registry.register('divide_dict', divide_dict)
+divide_registry.register('maybe_divide', maybe_divide)
+
 serialize_registry.register('str', str)
 serialize_registry.register('serialize_dict', serialize_dict)
+serialize_registry.register('maybe_serialize', maybe_serialize)
+
 deserialize_registry.register('float', float)
 deserialize_registry.register('int', int)
 deserialize_registry.register('str', str)
 deserialize_registry.register('eval', eval)
 deserialize_registry.register('deserialize_dict', deserialize_dict)
+deserialize_registry.register('maybe_deserialize', maybe_deserialize)
 
 # if super type is re-registered, propagate changes to subtypes (?)
 
 # remove shape types
 type_library = {
     # abstract number type
     'number': {
@@ -459,15 +540,15 @@
         '_serialize': 'str',
         '_deserialize': 'eval',
         '_divide': 'divide_list',
         '_type_parameters': ['A'],
         '_description': 'general list type (or sublists)'
     },
 
-    'hash': {
+    'tree': {
         '_default': '{}',
         '_apply': 'merge',
         '_serialize': 'str',
         '_deserialize': 'eval',
         '_divide': 'divide_dict',
         '_type_parameters': ['A'],
         '_description': 'mapping from str to some type (or nested dicts)'
@@ -479,17 +560,27 @@
         '_serialize': 'serialize_dict',
         '_deserialize': 'deserialize_dict',
         '_divide': 'divide_dict',
         '_type_parameters': ['key', 'value'],
         '_description': 'mapping from keys of any type to values of any type'
     },
 
+    'maybe': {
+        '_default': 'None',
+        '_apply': 'maybe_apply',
+        '_serialize': 'maybe_serialize',
+        '_deserialize': 'maybe_deserialize',
+        '_divide': 'maybe_divide',
+        '_type_parameters': ['value'],
+        '_description': 'type to represent values that could be empty'
+    },
+
     'edge': {
         'wires': {
-            '_type': 'hash[list[string]]'
+            '_type': 'tree[list[string]]'
         },
     },
 
     # 'process': {
     #     'process': {'_type': 'process instance'},
     #     'config': {'_type': 'dict'},
     #     '_super': 'edge',
@@ -645,12 +736,34 @@
     with pytest.raises(Exception) as e:
         type_registry.register('int', type_library['string'])
 
     type_registry.register('int', type_library['string'], force=True)
     type_registry.register('int', type_library['int'], force=True)
 
 
+def test_apply_update():
+    schema = {'_type': 'cube'}
+    state = {
+        'width': 11,
+        'height': 13,
+        'depth': 44,
+    }
+    update = {
+        'depth': -5
+    }
+
+    new_state = apply(
+        schema,
+        state,
+        update
+    )
+
+    assert new_state['width'] == 11
+    assert new_state['depth'] == 39
+
+
 if __name__ == '__main__':
     test_cube()
     test_generate_default()
     test_expand_schema()
     test_reregister_type()
+    test_apply_update()
```

### Comparing `bigraph-schema-0.0.7/bigraph_schema/schema.py` & `bigraph-schema-0.0.8/bigraph_schema/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import pprint
-from bigraph_schema.registry import registry_registry, type_schema_keys, optional_schema_keys, type_library, deep_merge, test_cube
+from bigraph_schema.registry import registry_registry, type_schema_keys, optional_schema_keys, type_library, deep_merge, test_cube, apply_update, apply
 
 
 type_registry = registry_registry.access('_type')
 apply_registry = registry_registry.access('_apply')
 serialize_registry = registry_registry.access('_serialize')
 deserialize_registry = registry_registry.access('_deserialize')
 
@@ -235,44 +235,14 @@
 
 def fill(schema, state=None):
     if state is not None:
         state = copy.deepcopy(state)
     return fill_state(schema, state=state)
 
 
-def apply_update(schema, state, update):
-    # expects an expanded schema
-
-    if '_apply' in schema:
-        apply_function = apply_registry.access(schema['_apply'])
-        state = apply_function(state, update)
-    elif isinstance(update, dict):
-        for key, branch in update.items():
-            if key not in schema:
-                raise Exception(f'trying to update a key that is not in the schema {key} for state:\n{state}\nwith schema:\n{schema}')
-            else:
-                subupdate = apply_update(
-                    schema[key],
-                    state[key],
-                    branch
-                )
-
-                state[key] = subupdate
-    else:
-        raise Exception(f'trying to apply an update that is unrecognized {update} for state:\n{state}\nwith schema:\n{schema}')
-
-    return state
-
-
-def apply(schema, initial, update):
-    expanded = type_registry.expand(schema)
-    state = copy.deepcopy(initial)
-    return apply_update(expanded, initial, update)
-
-
 def link_place(place, link):
     pass
 
 
 def compose(a, b):
     pass
 
@@ -736,47 +706,17 @@
                 'e0.1': 'v4',
                 'e0.2': ('v4', 'v5')}}}    
 
     result = link_place(placegraph, hypergraph)
     # assert result == merged
 
 
-def test_apply_update():
-    schema = {'_type': 'cube'}
-    state = {
-        'width': 11,
-        'height': 13,
-        'depth': 44,
-    }
-    update = {
-        'depth': -5
-    }
-
-    new_state = apply(
-        schema,
-        state,
-        update
-    )
-
-    assert new_state['width'] == 11
-    assert new_state['depth'] == 39
-
-
 if __name__ == '__main__':
     test_cube()
     test_validate_schema()
     test_fill_int()
     test_fill_cube()
     test_establish_path()
     test_fill_in_missing_nodes()
     test_expected_schema()
-    test_apply_update()
-
-
-
-
-
-
-
-
```

### Comparing `bigraph-schema-0.0.7/bigraph_schema.egg-info/PKG-INFO` & `bigraph-schema-0.0.8/bigraph_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.7
+Version: 0.0.8
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.7/setup.py` & `bigraph-schema-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
 
 
 setup(
```

