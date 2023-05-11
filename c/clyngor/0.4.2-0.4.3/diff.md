# Comparing `tmp/clyngor-0.4.2.tar.gz` & `tmp/clyngor-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clyngor-0.4.2.tar", last modified: Thu Mar 31 11:10:56 2022, max compression
+gzip compressed data, was "clyngor-0.4.3.tar", last modified: Thu May 11 13:45:33 2023, max compression
```

## Comparing `clyngor-0.4.2.tar` & `clyngor-0.4.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-03-31 11:10:56.881117 clyngor-0.4.2/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    35149 2022-03-31 11:10:56.000000 clyngor-0.4.2/LICENCE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      129 2022-03-31 11:10:56.000000 clyngor-0.4.2/MANIFEST.in
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    17586 2022-03-31 11:10:56.881117 clyngor-0.4.2/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    16659 2022-03-31 11:10:56.000000 clyngor-0.4.2/README.mkd
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-03-31 11:10:56.881117 clyngor-0.4.2/clyngor/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2369 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      790 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/__main__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    13510 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/answers.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2835 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/as_pyasp.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2195 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/decoder.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      923 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/grounding.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1365 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/inline.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11562 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/parsing.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     7037 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/propagators.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11521 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/solving.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-03-31 11:10:56.881117 clyngor-0.4.2/clyngor/test/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      633 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/conftest.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2009 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/definitions.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    15074 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_answers.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8248 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_api.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2469 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_clingo_module.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3473 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_decoder.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1042 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_grounding.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    12459 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_parsing.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     5128 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_propagator_class.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1705 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_solving.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      594 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_stress.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2083 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_time_limit.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2310 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_upapi.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3386 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/test/test_utils.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3448 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/upapi.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    13301 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor/utils.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-03-31 11:10:56.881117 clyngor-0.4.2/clyngor.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    17586 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      902 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor.egg-info/not-zip-safe
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2022-03-31 11:10:56.000000 clyngor-0.4.2/clyngor.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1117 2022-03-31 11:10:56.881117 clyngor-0.4.2/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2022-03-31 11:10:56.000000 clyngor-0.4.2/setup.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1001)        0 2023-05-11 13:45:33.091288 clyngor-0.4.3/
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    35149 2023-05-11 13:45:32.000000 clyngor-0.4.3/LICENCE
+-rw-r--r--   0 lucas     (1000) lucas     (1001)      129 2023-05-11 13:45:32.000000 clyngor-0.4.3/MANIFEST.in
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    17586 2023-05-11 13:45:33.091288 clyngor-0.4.3/PKG-INFO
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    16659 2023-05-11 13:45:32.000000 clyngor-0.4.3/README.mkd
+drwxr-xr-x   0 lucas     (1000) lucas     (1001)        0 2023-05-11 13:45:33.087955 clyngor-0.4.3/clyngor/
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     2369 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/__init__.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)      790 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/__main__.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    13510 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/answers.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     2835 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/as_pyasp.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     2195 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/decoder.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)      923 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/grounding.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     1365 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/inline.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    11690 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/parsing.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     7037 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/propagators.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    11583 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/solving.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1001)        0 2023-05-11 13:45:33.091288 clyngor-0.4.3/clyngor/test/
+-rw-r--r--   0 lucas     (1000) lucas     (1001)        0 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/__init__.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)      633 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/conftest.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     2009 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/definitions.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    15074 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_answers.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     8942 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_api.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     2469 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_clingo_module.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     3473 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_decoder.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     1042 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_grounding.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    13096 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_parsing.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     5128 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_propagator_class.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     1705 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_solving.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)      594 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_stress.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     2083 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_time_limit.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     2310 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_upapi.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     3386 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/test/test_utils.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     3448 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/upapi.py
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    13301 2023-05-11 13:45:32.000000 clyngor-0.4.3/clyngor/utils.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1001)        0 2023-05-11 13:45:33.087955 clyngor-0.4.3/clyngor.egg-info/
+-rw-r--r--   0 lucas     (1000) lucas     (1001)    17586 2023-05-11 13:45:33.000000 clyngor-0.4.3/clyngor.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1000) lucas     (1001)      902 2023-05-11 13:45:33.000000 clyngor-0.4.3/clyngor.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1001)        1 2023-05-11 13:45:33.000000 clyngor-0.4.3/clyngor.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1001)        1 2023-05-11 13:45:33.000000 clyngor-0.4.3/clyngor.egg-info/not-zip-safe
+-rw-r--r--   0 lucas     (1000) lucas     (1001)       59 2023-05-11 13:45:33.000000 clyngor-0.4.3/clyngor.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1001)        8 2023-05-11 13:45:33.000000 clyngor-0.4.3/clyngor.egg-info/top_level.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1001)     1117 2023-05-11 13:45:33.091288 clyngor-0.4.3/setup.cfg
+-rw-r--r--   0 lucas     (1000) lucas     (1001)       38 2023-05-11 13:45:32.000000 clyngor-0.4.3/setup.py
```

### Comparing `clyngor-0.4.2/LICENCE` & `clyngor-0.4.3/LICENCE`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/PKG-INFO` & `clyngor-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clyngor
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python wrapper around Clingo/Answer Set Programming
 Home-page: https://github.com/aluriak/clyngor
 Author: Lucas Bourneuf
 Author-email: lucas.bourneuf@laposte.net
 License: GPLv3
 Keywords: Answer Set Programming,wrapper,clingo
 Platform: UNKNOWN
```

### Comparing `clyngor-0.4.2/README.mkd` & `clyngor-0.4.3/README.mkd`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/__init__.py` & `clyngor-0.4.3/clyngor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 CLINGO_BIN_PATH = 'clingo'
-__version__ = '0.4.2'
+__version__ = '0.4.3'
 
 from clyngor.utils import ASPSyntaxError, ASPWarning, parse_clingo_output, clingo_value_to_python, with_clingo_bin, opt_models_from_clyngor_answers, answer_set_to_str, answer_set_from_str
 from clyngor.answers import Answers, ClingoAnswers
 from clyngor.solving import solve, clingo_version, command
 from clyngor.grounding import solve_from_grounded, grounded_program
 from clyngor.inline import ASP
 from clyngor.decoder import decode
```

### Comparing `clyngor-0.4.2/clyngor/__main__.py` & `clyngor-0.4.3/clyngor/__main__.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/answers.py` & `clyngor-0.4.3/clyngor/answers.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/as_pyasp.py` & `clyngor-0.4.3/clyngor/as_pyasp.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/decoder.py` & `clyngor-0.4.3/clyngor/decoder.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/grounding.py` & `clyngor-0.4.3/clyngor/grounding.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/inline.py` & `clyngor-0.4.3/clyngor/inline.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/parsing.py` & `clyngor-0.4.3/clyngor/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,20 +191,21 @@
                   under type 'progression' as a string.
 
     In any case, tuple ('answer', termset) will be returned
     with termset a string containing the raw data.
 
     """
     ASW_FLAG, OPT_FLAG, OPT_FOUND, PROGRESS = 'Answer: ', 'Optimization: ', 'OPTIMUM FOUND', 'Progression :'
+    UNSAT = 'UNSATISFIABLE'
     output = iter(output.splitlines() if isinstance(output, str) else output)
 
     # get the first lines
     line = next(output)
     infos = []
-    while not line.startswith(ASW_FLAG):
+    while not line.startswith(ASW_FLAG) and not line.startswith(UNSAT):
         infos.append(line)
         try:
             line = next(output)
         except StopIteration:
             return
 
     # first answer begins
@@ -214,14 +215,16 @@
             yield 'answer', next(output)
         elif line.startswith(OPT_FLAG) and yield_opti:
             yield 'optimization', tuple(map(int, line[len(OPT_FLAG):].strip().split()))
         elif line.startswith(OPT_FOUND) and yield_opti:
             yield 'optimum found', True
         elif line.startswith(PROGRESS) and yield_prgs:
             yield 'progression', line[len(PROGRESS):].strip()
+        elif line.startswith(UNSAT):
+            yield 'unsat', True
         elif not line.strip():  # empty line: statistics are beginning
             if not yield_stats: break  # stats are the last part of the output
             stats = {}
             for line in output:
                 sep = line.find(':')
                 key, value = line[:sep], line[sep+1:]
                 stats[key.strip()] = value.strip()
```

### Comparing `clyngor-0.4.2/clyngor/propagators.py` & `clyngor-0.4.3/clyngor/propagators.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/solving.py` & `clyngor-0.4.3/clyngor/solving.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,16 @@
             answer = payload
         elif ptype == 'optimum found':
             optimum_found = payload
         elif ptype == 'optimization':
             optimization = payload
         elif ptype == 'statistics':
             statistics.update(payload)
+        elif ptype == 'unsat':
+            pass  # don't care
         elif ptype == 'info':
             pass  # don't care
         else:
             assert ptype in parse_clasp_output.out_types, 'solving.parse_clasp_output yields an unexpected type ' + repr(ptype)
     if answer is not None:  # if no optimization, probably one miss
         assert answer_number is not None, answer_number
         yield answer, optimization, optimum_found, answer_number
```

### Comparing `clyngor-0.4.2/clyngor/test/conftest.py` & `clyngor-0.4.3/clyngor/test/conftest.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/definitions.py` & `clyngor-0.4.3/clyngor/test/definitions.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_answers.py` & `clyngor-0.4.3/clyngor/test/test_answers.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_api.py` & `clyngor-0.4.3/clyngor/test/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,41 +142,41 @@
 
 
 @run_with_clingo_binary_only
 def test_syntax_error():
     assert not clyngor.have_clingo_module()
     with pytest.raises(clyngor.ASPSyntaxError) as excinfo:
         tuple(clyngor.solve((), inline='invalid', force_tempfile=True))
-    assert excinfo.value.filename.startswith('/tmp/tmp')
+    assert excinfo.value.filename.startswith(tempfile.gettempdir())
     assert excinfo.value.lineno == 2
     assert excinfo.value.offset == 1
     assert excinfo.value.payload['char_end'] == 2
-    assert excinfo.value.msg.startswith('unexpected EOF in file /tmp/tmp')
+    assert excinfo.value.msg.startswith(f'unexpected EOF in file {tempfile.gettempdir()}')
     assert excinfo.value.msg.endswith(' at line 2 and column 1-2')
 
 
 @run_with_clingo_binary_only
 def test_syntax_error_semicolon():
     with pytest.raises(clyngor.ASPSyntaxError) as excinfo:
         tuple(clyngor.solve((), inline='color(X,red):- ;int(X,"adult").', force_tempfile=True))
-    assert excinfo.value.filename.startswith('/tmp/tmp')
+    assert excinfo.value.filename.startswith(tempfile.gettempdir())
     assert excinfo.value.lineno == 1
     assert excinfo.value.offset == 16
-    assert excinfo.value.msg.startswith('unexpected ; in file /tmp/tmp')
+    assert excinfo.value.msg.startswith(f'unexpected ; in file {tempfile.gettempdir()}')
     assert excinfo.value.msg.endswith(' at line 1 and column 16-17')
 
 
 @run_with_clingo_binary_only
 def test_syntax_error_brace():
     with pytest.raises(clyngor.ASPSyntaxError) as excinfo:
         tuple(clyngor.solve((), inline='color(X,red):- {{}}.', force_tempfile=True))
-    assert excinfo.value.filename.startswith('/tmp/tmp')
+    assert excinfo.value.filename.startswith(tempfile.gettempdir())
     assert excinfo.value.lineno == 1
     assert excinfo.value.offset == 17
-    assert excinfo.value.msg.startswith('unexpected { in file /tmp/tmp')
+    assert excinfo.value.msg.startswith(f'unexpected {{ in file {tempfile.gettempdir()}')
     assert excinfo.value.msg.endswith(' at line 1 and column 17-18')
 
 
 @run_with_clingo_binary_only
 def test_syntax_error_brace_with_stdin():
     with pytest.raises(clyngor.ASPSyntaxError) as excinfo:
         tuple(clyngor.solve((), inline='color(X,red):- {{}}.'))
@@ -190,15 +190,15 @@
 @run_with_clingo_binary_only
 def test_undefined_warning():
     assert not clyngor.have_clingo_module()
     with pytest.raises(clyngor.ASPWarning) as excinfo:
         tuple(clyngor.solve((), inline='b:- c.', error_on_warning=True, force_tempfile=True))
     assert excinfo.value.atom == 'c'
     assert len(excinfo.value.args) == 1
-    start = "atom 'c' does not occur in any rule head in file /tmp/tmp"
+    start = f"atom 'c' does not occur in any rule head in file {tempfile.gettempdir()}"
     assert excinfo.value.args[0].startswith(start)
     assert excinfo.value.args[0].endswith(" at line 1 and column 5-6")
 
     # NB: the following should NOT raise any error (default value)
     tuple(clyngor.solve((), inline='b:- c.', error_on_warning=False))
     tuple(clyngor.solve((), inline='b:- c.'))
 
@@ -215,7 +215,35 @@
     #show -r/1.
     """
     models = clyngor.solve(inline=CODE)
     model = next(models, None)
     assert next(models, None) is None
     print(model)
     assert model == {('-r', (1,)), ('-r', (2,))}
+
+
+def test_unsatisfiable():
+    "Should return an empty answers set"
+    CODE = """
+    p(1).
+    q(1).
+
+    :- p(X), q(X).
+    """
+    models = clyngor.solve(inline=CODE, stats=False)
+    model = next(models, None)
+    assert model is None
+    assert len(models.statistics) == 4
+
+
+def test_unsatisfiable_statistics():
+    "Should return an empty answers set but provide the statistics"
+    CODE = """
+    p(1).
+    q(1).
+
+    :- p(X), q(X).
+    """
+    models = clyngor.solve(inline=CODE, stats=True)
+    model = next(models, None)
+    assert model is None
+    assert len(models.statistics) > 4
```

### Comparing `clyngor-0.4.2/clyngor/test/test_clingo_module.py` & `clyngor-0.4.3/clyngor/test/test_clingo_module.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_decoder.py` & `clyngor-0.4.3/clyngor/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_grounding.py` & `clyngor-0.4.3/clyngor/test/test_grounding.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_parsing.py` & `clyngor-0.4.3/clyngor/test/test_parsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,17 +247,38 @@
     # ensure that all data has been found
     assert next(expected_answer, None) is None
     assert next(expected_optimization, None) is None
 
 
 def test_unsat():
     parsed = Parser().parse_clasp_output(OUTCLASP_UNSATISFIABLE.splitlines())
+    current = next(parsed, None)
+    assert current is not None
+    l_type, model = current
+    assert l_type == 'unsat' and model is True
     assert next(parsed, None) is None
 
 
+def test_unsat_stats():
+    parsed = Parser().parse_clasp_output(OUTCLASP_UNSATISFIABLE.splitlines(), yield_stats=True)
+    stats = {
+        'Models': '0',
+        'Calls': '1',
+        'Time': '0.001s (Solving: 0.00s 1st Model: 0.00s Unsat: 0.00s)',
+        'CPU Time': '0.000s'
+    }
+
+    for type, model in parsed:
+        assert type in ('unsat', 'statistics')
+        if type == 'unsat':
+            assert model is True
+        elif type == 'statistics':
+            assert model == stats
+
+
 def test_multithread_with_progression():
     parsed = Parser().parse_clasp_output(CLINGO_OUTPUT_MULTITHREADING_WITH_PROGRESS.splitlines(),
                                          yield_prgs=True)
     expected_answer = iter((
         (('a', ()),),
         (('b', ()),),
     ))
```

### Comparing `clyngor-0.4.2/clyngor/test/test_propagator_class.py` & `clyngor-0.4.3/clyngor/test/test_propagator_class.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_solving.py` & `clyngor-0.4.3/clyngor/test/test_solving.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_stress.py` & `clyngor-0.4.3/clyngor/test/test_stress.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_time_limit.py` & `clyngor-0.4.3/clyngor/test/test_time_limit.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_upapi.py` & `clyngor-0.4.3/clyngor/test/test_upapi.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/test/test_utils.py` & `clyngor-0.4.3/clyngor/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/upapi.py` & `clyngor-0.4.3/clyngor/upapi.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor/utils.py` & `clyngor-0.4.3/clyngor/utils.py`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/clyngor.egg-info/PKG-INFO` & `clyngor-0.4.3/clyngor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clyngor
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python wrapper around Clingo/Answer Set Programming
 Home-page: https://github.com/aluriak/clyngor
 Author: Lucas Bourneuf
 Author-email: lucas.bourneuf@laposte.net
 License: GPLv3
 Keywords: Answer Set Programming,wrapper,clingo
 Platform: UNKNOWN
```

### Comparing `clyngor-0.4.2/clyngor.egg-info/SOURCES.txt` & `clyngor-0.4.3/clyngor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clyngor-0.4.2/setup.cfg` & `clyngor-0.4.3/setup.cfg`

 * *Files identical despite different names*

