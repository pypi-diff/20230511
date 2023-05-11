# Comparing `tmp/crispr_shrinkage-0.1.8.tar.gz` & `tmp/crispr_shrinkage-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_shrinkage-0.1.8.tar", max compression
+gzip compressed data, was "crispr_shrinkage-0.1.9.tar", max compression
```

## Comparing `crispr_shrinkage-0.1.8.tar` & `crispr_shrinkage-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      155 2023-02-07 18:39:21.267575 crispr_shrinkage-0.1.8/crispr_shrinkage/__init__.py
--rw-r--r--   0        0        0    30930 2023-02-18 01:00:46.653143 crispr_shrinkage-0.1.8/crispr_shrinkage/framework/__pycache__/CrisprShrinkage.cpython-38.pyc
--rw-r--r--   0        0        0    76155 2023-02-22 04:02:25.365034 crispr_shrinkage-0.1.8/crispr_shrinkage/framework/CrisprShrinkage.py
--rw-r--r--   0        0        0      512 2023-02-22 04:07:51.062372 crispr_shrinkage-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-03 19:55:55.031074 crispr_shrinkage-0.1.8/README.md
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 crispr_shrinkage-0.1.8/setup.py
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 crispr_shrinkage-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      155 2023-02-07 18:39:21.267575 crispr_shrinkage-0.1.9/crispr_shrinkage/__init__.py
+-rw-r--r--   0        0        0    30930 2023-02-18 01:00:46.653143 crispr_shrinkage-0.1.9/crispr_shrinkage/framework/__pycache__/CrisprShrinkage.cpython-38.pyc
+-rw-r--r--   0        0        0    76300 2023-02-22 14:58:10.979673 crispr_shrinkage-0.1.9/crispr_shrinkage/framework/CrisprShrinkage.py
+-rw-r--r--   0        0        0      512 2023-02-22 14:58:24.204044 crispr_shrinkage-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-03 19:55:55.031074 crispr_shrinkage-0.1.9/README.md
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 crispr_shrinkage-0.1.9/setup.py
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 crispr_shrinkage-0.1.9/PKG-INFO
```

### Comparing `crispr_shrinkage-0.1.8/crispr_shrinkage/framework/__pycache__/CrisprShrinkage.cpython-38.pyc` & `crispr_shrinkage-0.1.9/crispr_shrinkage/framework/__pycache__/CrisprShrinkage.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `crispr_shrinkage-0.1.8/crispr_shrinkage/framework/CrisprShrinkage.py` & `crispr_shrinkage-0.1.9/crispr_shrinkage/framework/CrisprShrinkage.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,20 +206,21 @@
     replicate_indices: List[int]) -> Tuple[List[float], List[float]]:
     
     imputation_posterior_alpha = (singleton_imputation_prior_strength*negative_control_guide_pop1_total_normalized_counts_reps[replicate_indices]) 
     
     imputation_posterior_beta = (singleton_imputation_prior_strength*negative_control_guide_pop2_total_normalized_counts_reps[replicate_indices])
 
     max_imputation_posterior = 5000 # Setting this max, since calculating the KL divergence of a very high posterior value will result in a precision error
-    if max(imputation_posterior_alpha,imputation_posterior_beta) > max_imputation_posterior:
-        print("Downscaling posterior: {}, {}".format(imputation_posterior_alpha,imputation_posterior_beta))
-        if imputation_posterior_alpha > imputation_posterior_beta:
-            downscale_factor = max_imputation_posterior/imputation_posterior_alpha
-            imputation_posterior_alpha = imputation_posterior_alpha * downscale_factor
-            imputation_posterior_beta = imputation_posterior_beta * downscale_factor
+    for rep_i in range(replicate_indices):
+        if max(imputation_posterior_alpha[rep_i],imputation_posterior_beta[rep_i]) > max_imputation_posterior:
+            print("Downscaling posterior: {}, {}".format(imputation_posterior_alpha[rep_i],imputation_posterior_beta[rep_i]))
+            if imputation_posterior_alpha[rep_i] > imputation_posterior_beta[rep_i]:
+                downscale_factor = max_imputation_posterior/imputation_posterior_alpha[rep_i]
+                imputation_posterior_alpha[rep_i] = imputation_posterior_alpha[rep_i] * downscale_factor
+                imputation_posterior_beta[rep_i] = imputation_posterior_beta[rep_i] * downscale_factor
 
 
 
     return imputation_posterior_alpha, imputation_posterior_beta
 
 def perform_neighboorhood_score_imputation(each_guide: Guide, 
     experiment_guide_sets: ExperimentGuideSets,
```

### Comparing `crispr_shrinkage-0.1.8/pyproject.toml` & `crispr_shrinkage-0.1.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crispr_shrinkage"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Basheer Becerra <bbecerra@fas.harvard.edu>"]
 readme = "README.md"
 packages = [{include = "crispr_shrinkage"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `crispr_shrinkage-0.1.8/setup.py` & `crispr_shrinkage-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'crispr-shrinkage',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '',
     'author': 'Basheer Becerra',
     'author_email': 'bbecerra@fas.harvard.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `crispr_shrinkage-0.1.8/PKG-INFO` & `crispr_shrinkage-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crispr-shrinkage
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Basheer Becerra
 Author-email: bbecerra@fas.harvard.edu
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

