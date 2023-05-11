# Comparing `tmp/pymince-2.6.0.tar.gz` & `tmp/pymince-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymince-2.6.0.tar", last modified: Mon Apr 17 09:52:29 2023, max compression
+gzip compressed data, was "pymince-2.7.0.tar", last modified: Thu May 11 08:41:55 2023, max compression
```

## Comparing `pymince-2.6.0.tar` & `pymince-2.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:29.263609 pymince-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-17 09:52:11.000000 pymince-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37583 2023-04-17 09:52:29.263609 pymince-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36760 2023-04-17 09:52:11.000000 pymince-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:29.259609 pymince-2.6.0/pymince/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/std.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:29.263609 pymince-2.6.0/pymince.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37583 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-17 09:52:11.000000 pymince-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:52:29.263609 pymince-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 09:52:11.000000 pymince-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:41:55.426123 pymince-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 08:41:37.000000 pymince-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-05-11 08:41:55.426123 pymince-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37200 2023-05-11 08:41:37.000000 pymince-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:41:55.426123 pymince-2.7.0/pymince/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:41:55.426123 pymince-2.7.0/pymince.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-11 08:41:37.000000 pymince-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:41:55.426123 pymince-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-11 08:41:37.000000 pymince-2.7.0/setup.py
```

### Comparing `pymince-2.6.0/LICENSE` & `pymince-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/PKG-INFO` & `pymince-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymince
-Version: 2.6.0
+Version: 2.7.0
 Summary: Python shredded utilities
 Home-page: https://github.com/rmoralespp/pymince
 Author: rmoralespp
 Author-email: rmoralespp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -55,15 +55,15 @@
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -798,14 +798,17 @@
 ```
 ##### partition
 ```
 partition(predicate, iterable)
 
 Split the iterable into two lists, based on the boolean return-value
 of the predicate.
+- (1): items that have predicate(item) == False.
+- (2): items that have predicate(item) == True.
+
 
 Examples:
     from pymince.iterator import partition
 
     is_odd = lambda x: x % 2 != 0
     even_items, odd_items = partition(is_odd, range(10))  # ([0, 2, 4, 6, 8], [1, 3, 5, 7, 9])
 ```
@@ -955,21 +958,33 @@
 ##### idump_into
 ```
 idump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump an iterable incrementally into a JSON file
 using the "utf-8" encoding.
 The result will always be an array with the elements of the iterable.
+*** Useful to reduce memory consumption ***
 
 Examples:
     from pymince.json import idump_into
 
     it = iter([{"key": "foo"}, {"key": "bar"}])
     dump_into("foo.json", it)
 ```
+##### idump_lines
+```
+idump_lines(iterable, **dumps_kwargs)
+
+Generator yielding string lines that form a JSON array
+with the serialized elements of given iterable.
+*** Useful to reduce memory consumption ***
+
+:param iterable: Iterable[dict]
+:rtype: Iterable[str]
+```
 ##### load_from
 ```
 load_from(filename, encoding='utf-8')
 
 Load JSON from a file using "utf-8" encoding.
 
 Examples:
```

### Comparing `pymince-2.6.0/README.md` & `pymince-2.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -775,14 +775,17 @@
 ```
 ##### partition
 ```
 partition(predicate, iterable)
 
 Split the iterable into two lists, based on the boolean return-value
 of the predicate.
+- (1): items that have predicate(item) == False.
+- (2): items that have predicate(item) == True.
+
 
 Examples:
     from pymince.iterator import partition
 
     is_odd = lambda x: x % 2 != 0
     even_items, odd_items = partition(is_odd, range(10))  # ([0, 2, 4, 6, 8], [1, 3, 5, 7, 9])
 ```
@@ -932,21 +935,33 @@
 ##### idump_into
 ```
 idump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump an iterable incrementally into a JSON file
 using the "utf-8" encoding.
 The result will always be an array with the elements of the iterable.
+*** Useful to reduce memory consumption ***
 
 Examples:
     from pymince.json import idump_into
 
     it = iter([{"key": "foo"}, {"key": "bar"}])
     dump_into("foo.json", it)
 ```
+##### idump_lines
+```
+idump_lines(iterable, **dumps_kwargs)
+
+Generator yielding string lines that form a JSON array
+with the serialized elements of given iterable.
+*** Useful to reduce memory consumption ***
+
+:param iterable: Iterable[dict]
+:rtype: Iterable[str]
+```
 ##### load_from
 ```
 load_from(filename, encoding='utf-8')
 
 Load JSON from a file using "utf-8" encoding.
 
 Examples:
```

### Comparing `pymince-2.6.0/pymince/algorithm.py` & `pymince-2.7.0/pymince/algorithm.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/boolean.py` & `pymince-2.7.0/pymince/boolean.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/dates.py` & `pymince-2.7.0/pymince/dates.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/dictionary.py` & `pymince-2.7.0/pymince/dictionary.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/file.py` & `pymince-2.7.0/pymince/file.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/functional.py` & `pymince-2.7.0/pymince/functional.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/iterator.py` & `pymince-2.7.0/pymince/iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,17 @@
     return next(it, empty) is not empty and next(it, empty) is empty
 
 
 def partition(predicate, iterable):
     """
     Split the iterable into two lists, based on the boolean return-value
     of the predicate.
+    - (1): items that have predicate(item) == False.
+    - (2): items that have predicate(item) == True.
+
 
     Examples:
         from pymince.iterator import partition
 
         is_odd = lambda x: x % 2 != 0
         even_items, odd_items = partition(is_odd, range(10))  # ([0, 2, 4, 6, 8], [1, 3, 5, 7, 9])
     """
```

### Comparing `pymince-2.6.0/pymince/json.py` & `pymince-2.7.0/pymince/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,50 +109,58 @@
             yield from reader
 
     with open(csv_path, encoding=encoding, newline="") as csv_f:
         # The official csv doc recommends opening the file with newline='' on all platforms to disable
         # universal newlines translation.
 
         data = itertools.islice(read(), start, stop)
-        pool = tuple(data)
+        idump_into(json_path, data, encoding=encoding, **kwargs)
 
-    dump_into(json_path, pool, encoding=encoding, **kwargs)
+
+def idump_lines(iterable, **dumps_kwargs):
+    """
+    Generator yielding string lines that form a JSON array
+    with the serialized elements of given iterable.
+    *** Useful to reduce memory consumption ***
+
+    :param iterable: Iterable[dict]
+    :rtype: Iterable[str]
+    """
+
+    it = iter(iterable)
+    encode = functools.partial(dumps, **dumps_kwargs)
+    indent = dumps_kwargs.get("indent")
+    prefix = " " * indent if indent else ""
+    yield "[\n"
+    obj = next(it, None)
+    if obj is not None:
+        yield textwrap.indent(encode(obj), prefix)
+    for obj in it:
+        yield ",\n"
+        yield textwrap.indent(encode(obj), prefix)
+    yield "\n"
+    yield "]"
 
 
 def idump_into(filename, iterable, encoding=ENCODING, **kwargs):
     """
     Dump an iterable incrementally into a JSON file
     using the "utf-8" encoding.
     The result will always be an array with the elements of the iterable.
+    *** Useful to reduce memory consumption ***
 
     Examples:
         from pymince.json import idump_into
 
         it = iter([{"key": "foo"}, {"key": "bar"}])
         dump_into("foo.json", it)
     """
 
-    def worker(items):
-        encode = functools.partial(dumps, **kwargs)
-        indent = kwargs.get("indent")
-        prefix = " " * indent if indent else ""
-        yield "[\n"
-        obj = next(items, None)
-        if obj is not None:
-            yield textwrap.indent(encode(obj), prefix)
-        for obj in items:
-            yield ",\n"
-            yield textwrap.indent(encode(obj), prefix)
-
-        yield "\n"
-        yield "]"
-
-    it = iter(iterable)
     with open(filename, mode="w", encoding=encoding) as f:
-        f.writelines(worker(it))
+        f.writelines(idump_lines(iterable, **kwargs))
 
 
 class JSONEncoder(json.JSONEncoder):
     """
     JSON encoder that handles additional types compared
     to `json.JSONEncoder`
```

### Comparing `pymince-2.6.0/pymince/logging.py` & `pymince-2.7.0/pymince/logging.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/std.py` & `pymince-2.7.0/pymince/std.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/text.py` & `pymince-2.7.0/pymince/text.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/warnings.py` & `pymince-2.7.0/pymince/warnings.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince/xml.py` & `pymince-2.7.0/pymince/xml.py`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/pymince.egg-info/PKG-INFO` & `pymince-2.7.0/pymince.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymince
-Version: 2.6.0
+Version: 2.7.0
 Summary: Python shredded utilities
 Home-page: https://github.com/rmoralespp/pymince
 Author: rmoralespp
 Author-email: rmoralespp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -55,15 +55,15 @@
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -798,14 +798,17 @@
 ```
 ##### partition
 ```
 partition(predicate, iterable)
 
 Split the iterable into two lists, based on the boolean return-value
 of the predicate.
+- (1): items that have predicate(item) == False.
+- (2): items that have predicate(item) == True.
+
 
 Examples:
     from pymince.iterator import partition
 
     is_odd = lambda x: x % 2 != 0
     even_items, odd_items = partition(is_odd, range(10))  # ([0, 2, 4, 6, 8], [1, 3, 5, 7, 9])
 ```
@@ -955,21 +958,33 @@
 ##### idump_into
 ```
 idump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump an iterable incrementally into a JSON file
 using the "utf-8" encoding.
 The result will always be an array with the elements of the iterable.
+*** Useful to reduce memory consumption ***
 
 Examples:
     from pymince.json import idump_into
 
     it = iter([{"key": "foo"}, {"key": "bar"}])
     dump_into("foo.json", it)
 ```
+##### idump_lines
+```
+idump_lines(iterable, **dumps_kwargs)
+
+Generator yielding string lines that form a JSON array
+with the serialized elements of given iterable.
+*** Useful to reduce memory consumption ***
+
+:param iterable: Iterable[dict]
+:rtype: Iterable[str]
+```
 ##### load_from
 ```
 load_from(filename, encoding='utf-8')
 
 Load JSON from a file using "utf-8" encoding.
 
 Examples:
```

### Comparing `pymince-2.6.0/pyproject.toml` & `pymince-2.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymince-2.6.0/setup.py` & `pymince-2.7.0/setup.py`

 * *Files identical despite different names*

