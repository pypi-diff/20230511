# Comparing `tmp/madai-0.2.1.tar.gz` & `tmp/madai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madai-0.2.1.tar", max compression
+gzip compressed data, was "madai-0.2.2.tar", max compression
```

## Comparing `madai-0.2.1.tar` & `madai-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      758 2023-05-09 10:01:02.650782 madai-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.2.1/madai/__init__.py
--rw-r--r--   0        0        0     4803 2023-05-09 11:56:53.481861 madai-0.2.1/madai/chi2.py
--rw-r--r--   0        0        0      143 2023-05-09 09:53:01.108847 madai-0.2.1/madai/cli.py
--rw-r--r--   0        0        0     2762 2023-05-09 12:52:19.338144 madai-0.2.1/madai/spearman.py
--rw-r--r--   0        0        0     1492 2023-05-09 09:18:16.958076 madai-0.2.1/madai/utils.py
--rw-r--r--   0        0        0      574 2023-05-09 12:52:27.318302 madai-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 madai-0.2.1/setup.py
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 madai-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      758 2023-05-09 10:01:02.650782 madai-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.2.2/madai/__init__.py
+-rw-r--r--   0        0        0     4803 2023-05-09 11:56:53.481861 madai-0.2.2/madai/chi2.py
+-rw-r--r--   0        0        0      143 2023-05-09 09:53:01.108847 madai-0.2.2/madai/cli.py
+-rw-r--r--   0        0        0     2777 2023-05-09 13:45:53.611636 madai-0.2.2/madai/spearman.py
+-rw-r--r--   0        0        0     1492 2023-05-09 09:18:16.958076 madai-0.2.2/madai/utils.py
+-rw-r--r--   0        0        0      574 2023-05-11 08:56:15.842412 madai-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 madai-0.2.2/setup.py
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 madai-0.2.2/PKG-INFO
```

### Comparing `madai-0.2.1/README.md` & `madai-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `madai-0.2.1/madai/chi2.py` & `madai-0.2.2/madai/chi2.py`

 * *Files identical despite different names*

### Comparing `madai-0.2.1/madai/spearman.py` & `madai-0.2.2/madai/spearman.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     a_ranked_words = [w for w, _ in Counter(a_words).most_common(top_n_words)]
     b_ranked_words = [w for w, _ in Counter(b_words).most_common(top_n_words)]
 
     assert isinstance(a_ranked_words[0], str)
     assert isinstance(b_ranked_words[0], str)
 
     d = spearmanr(a_ranked_words, b_ranked_words)[0]
+    d = abs(d)
 
     return d
 
 
 def sim_corpus(a: Corpus, b: Corpus, top_n_words: int) -> float:
     return sim(a.sample_words(), b.sample_words(), top_n_words)
```

### Comparing `madai-0.2.1/madai/utils.py` & `madai-0.2.2/madai/utils.py`

 * *Files identical despite different names*

### Comparing `madai-0.2.1/pyproject.toml` & `madai-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "madai"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["sobamchan <oh.sore.sore.soutarou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 scipy = "^1.10.1"
```

### Comparing `madai-0.2.1/setup.py` & `madai-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'typer==0.7.0']
 
 entry_points = \
 {'console_scripts': ['madai = madai.cli:app']}
 
 setup_kwargs = {
     'name': 'madai',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': '',
     'long_description': '# madai\n\nCompute difference between two corpus by using chi2.\nImplementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).\n\nI am not fully sure if this implementation is perfectly follow this paper.\nFeel free to make issues to point out some problems if you find.\n\n## Installation\n\n```\npip install madai\n```\n\n## Usage\n\nmadai implements two ways of computing similarity between two corpus, chi2 and spearman.\nUse spearman when two corpus are different in size.\n\nTwo target corpus need to be text files, each line containing one document/sentence.\n\n```\nmadai chi2 /path/to/corpus/a /path/to/corpus/b\n\n# or\n\nmadai spearman /path/to/corpus/a /path/to/corpus/b\n```\n\nTo view parameters, run,\n```\nmadai --help\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `madai-0.2.1/PKG-INFO` & `madai-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madai
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

