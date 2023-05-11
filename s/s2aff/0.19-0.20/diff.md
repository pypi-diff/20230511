# Comparing `tmp/s2aff-0.19.tar.gz` & `tmp/s2aff-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.19.tar", last modified: Mon May  8 20:08:31 2023, max compression
+gzip compressed data, was "s2aff-0.20.tar", last modified: Thu May 11 17:55:27 2023, max compression
```

## Comparing `s2aff-0.19.tar` & `s2aff-0.20.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:08:31.751998 s2aff-0.19/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.19/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-08 20:08:31.751773 s2aff-0.19/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.19/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:08:31.745027 s2aff-0.19/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.19/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.19/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.19/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:08:31.745208 s2aff-0.19/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.19/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:08:31.747808 s2aff-0.19/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8094 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-08 19:52:35.000000 s2aff-0.19/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:08:31.749474 s2aff-0.19/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-08 19:46:34.000000 s2aff-0.19/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:08:31.748852 s2aff-0.19/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-08 20:08:31.000000 s2aff-0.19/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-08 20:08:31.000000 s2aff-0.19/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-08 20:08:31.000000 s2aff-0.19/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-08 20:08:31.000000 s2aff-0.19/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-08 20:08:31.000000 s2aff-0.19/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:08:31.751437 s2aff-0.19/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.19/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-08 19:46:34.000000 s2aff-0.19/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-08 19:46:34.000000 s2aff-0.19/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-08 19:46:34.000000 s2aff-0.19/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.19/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.19/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.19/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-08 20:08:31.752087 s2aff-0.19/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.19/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.378123 s2aff-0.20/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.20/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-11 17:55:27.377929 s2aff-0.20/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.20/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.371046 s2aff-0.20/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.20/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.20/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.20/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.371387 s2aff-0.20/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.20/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.374363 s2aff-0.20/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8094 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-08 19:52:35.000000 s2aff-0.20/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.20/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.375984 s2aff-0.20/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.375352 s2aff-0.20/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-11 17:55:26.000000 s2aff-0.20/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-11 17:55:27.000000 s2aff-0.20/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-11 17:55:26.000000 s2aff-0.20/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-11 17:55:27.000000 s2aff-0.20/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-11 17:55:27.000000 s2aff-0.20/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.377629 s2aff-0.20/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.20/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-11 17:55:27.378220 s2aff-0.20/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-11 17:55:21.000000 s2aff-0.20/setup.py
```

### Comparing `s2aff-0.19/LICENSE` & `s2aff-0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/README.md` & `s2aff-0.20/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/data/combine_gold.py` & `s2aff-0.20/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/data/download_latest_ror.py` & `s2aff-0.20/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/__init__.py` & `s2aff-0.20/s2aff/__init__.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/consts.py` & `s2aff-0.20/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/data.py` & `s2aff-0.20/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/features.py` & `s2aff-0.20/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/file_cache.py` & `s2aff-0.20/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/lightgbm_helpers.py` & `s2aff-0.20/s2aff/lightgbm_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         label_gain_max=1000,
         eval_at="1,2,3,4,5,100",
         n_estimators=5000,
         hyperopt_evals=25,
         device="cpu",
         tree_learner="data",
         random_seed=0,
-        threads=10,
+        threads=16,
         feval=None,
     ):
 
         super().__init__()
 
         if learning_task == "classification":
             assert metric in {"binary", "multiclass", "multiclassova"}
```

### Comparing `s2aff-0.19/s2aff/model.py` & `s2aff-0.20/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/ror.py` & `s2aff-0.20/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/text.py` & `s2aff-0.20/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/timo/integration_test.py` & `s2aff-0.20/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff/timo/interface.py` & `s2aff-0.20/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/s2aff.egg-info/SOURCES.txt` & `s2aff-0.20/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.20/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.20/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/scripts/generate_lightgbm_training_data.py` & `s2aff-0.20/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/scripts/train_lightgbm_reranker.py` & `s2aff-0.20/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/scripts/train_ner_model.py` & `s2aff-0.20/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/scripts/update_openalex_works_counts.py` & `s2aff-0.20/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.19/setup.py` & `s2aff-0.20/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.19",
+    version="0.20",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

