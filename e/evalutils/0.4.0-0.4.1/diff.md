# Comparing `tmp/evalutils-0.4.0.tar.gz` & `tmp/evalutils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalutils-0.4.0.tar", max compression
+gzip compressed data, was "evalutils-0.4.1.tar", max compression
```

## Comparing `evalutils-0.4.0.tar` & `evalutils-0.4.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1086 2023-03-03 15:24:15.028576 evalutils-0.4.0/LICENSE
--rw-r--r--   0        0        0     1512 2023-03-03 15:24:15.028576 evalutils-0.4.0/README.md
--rw-r--r--   0        0        0      356 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/__init__.py
--rw-r--r--   0        0        0       82 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/__main__.py
--rw-r--r--   0        0        0     3938 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/annotations.py
--rw-r--r--   0        0        0     6632 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/cli.py
--rw-r--r--   0        0        0    23270 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/evalutils.py
--rw-r--r--   0        0        0      195 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/exceptions.py
--rw-r--r--   0        0        0     4108 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/io.py
--rw-r--r--   0        0        0    10237 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/roc.py
--rw-r--r--   0        0        0     3827 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/scorers.py
--rw-r--r--   0        0        0    29369 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/stats.py
--rw-r--r--   0        0        0        0 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/__init__.py
--rw-r--r--   0        0        0      414 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/hooks/__init__.py
--rw-r--r--   0        0        0     2124 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/hooks/post_gen_project.py
--rw-r--r--   0        0        0      340 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/hooks/pre_gen_project.py
--rw-r--r--   0        0        0       21 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/.dockerignore
--rw-r--r--   0        0        0       94 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitattributes.j2
--rw-r--r--   0        0        0      555 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1190 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitignore
--rw-r--r--   0        0        0      965 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/Dockerfile
--rw-r--r--   0        0        0      354 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/README.md
--rw-r--r--   0        0        0      466 2023-03-03 15:24:15.028576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
--rw-r--r--   0        0        0   372164 2023-03-03 15:24:15.032576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
--rw-r--r--   0        0        0      336 2023-03-03 15:24:15.032576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_classification.json
--rw-r--r--   0        0        0     1849 2023-03-03 15:24:15.032576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_detection.json
--rw-r--r--   0        0        0      418 2023-03-03 15:24:15.032576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_segmentation.json
--rwxr-xr-x   0        0        0      137 2023-03-03 15:24:15.032576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/build.sh
--rw-r--r--   0        0        0     4438 2023-03-03 15:24:15.032576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation.py.j2
--rw-r--r--   0        0        0      408 2023-03-03 15:24:15.032576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
--rw-r--r--   0        0        0   529641 2023-03-03 15:24:15.036576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
--rw-r--r--   0        0        0      397 2023-03-03 15:24:15.036576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.mhd
--rw-r--r--   0        0        0   414098 2023-03-03 15:24:15.036576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw
--rw-r--r--   0        0        0      358 2023-03-03 15:24:15.036576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/detection-submission.csv
--rw-r--r--   0        0        0       52 2023-03-03 15:24:15.036576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/submission.csv
--rwxr-xr-x   0        0        0      134 2023-03-03 15:24:15.036576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/export.sh
--rw-r--r--   0        0        0      415 2023-03-03 15:24:15.036576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
--rw-r--r--   0        0        0  1014889 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
--rw-r--r--   0        0        0      403 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.mhd
--rw-r--r--   0        0        0   806220 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw
--rw-r--r--   0        0        0      154 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/detection-reference.csv
--rw-r--r--   0        0        0       52 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/reference.csv
--rw-r--r--   0        0        0     2691 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/process.py.j2
--rw-r--r--   0        0        0      106 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/requirements.in
--rwxr-xr-x   0        0        0     2122 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/test.sh
--rw-r--r--   0        0        0     1240 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/utils.py
--rw-r--r--   0        0        0     4408 2023-03-03 15:24:15.040576 evalutils-0.4.0/evalutils/validators.py
--rw-r--r--   0        0        0     2110 2023-03-03 15:24:15.040576 evalutils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2630 1970-01-01 00:00:00.000000 evalutils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-11 08:32:51.617926 evalutils-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1512 2023-05-11 08:32:51.617926 evalutils-0.4.1/README.md
+-rw-r--r--   0        0        0      356 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/__main__.py
+-rw-r--r--   0        0        0     3938 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/annotations.py
+-rw-r--r--   0        0        0     6632 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/cli.py
+-rw-r--r--   0        0        0    23270 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/evalutils.py
+-rw-r--r--   0        0        0      195 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/exceptions.py
+-rw-r--r--   0        0        0     4094 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/io.py
+-rw-r--r--   0        0        0    10237 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/roc.py
+-rw-r--r--   0        0        0     3827 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/scorers.py
+-rw-r--r--   0        0        0    29369 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/stats.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/__init__.py
+-rw-r--r--   0        0        0      414 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/hooks/__init__.py
+-rw-r--r--   0        0        0     2124 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      340 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0       21 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.dockerignore
+-rw-r--r--   0        0        0       94 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitattributes.j2
+-rw-r--r--   0        0        0      555 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1190 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitignore
+-rw-r--r--   0        0        0      965 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/Dockerfile
+-rw-r--r--   0        0        0      354 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/README.md
+-rw-r--r--   0        0        0      466 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
+-rw-r--r--   0        0        0   372164 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
+-rw-r--r--   0        0        0      336 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_classification.json
+-rw-r--r--   0        0        0     1849 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_detection.json
+-rw-r--r--   0        0        0      418 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_segmentation.json
+-rwxr-xr-x   0        0        0      137 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/build.sh
+-rw-r--r--   0        0        0     4438 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation.py.j2
+-rw-r--r--   0        0        0      408 2023-05-11 08:32:51.621927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
+-rw-r--r--   0        0        0   529641 2023-05-11 08:32:51.621927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
+-rw-r--r--   0        0        0      397 2023-05-11 08:32:51.621927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.mhd
+-rw-r--r--   0        0        0   414098 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw
+-rw-r--r--   0        0        0      358 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/detection-submission.csv
+-rw-r--r--   0        0        0       52 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/submission.csv
+-rwxr-xr-x   0        0        0      134 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/export.sh
+-rw-r--r--   0        0        0      415 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
+-rw-r--r--   0        0        0  1014889 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
+-rw-r--r--   0        0        0      403 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.mhd
+-rw-r--r--   0        0        0   806220 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw
+-rw-r--r--   0        0        0      154 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/detection-reference.csv
+-rw-r--r--   0        0        0       52 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/reference.csv
+-rw-r--r--   0        0        0     2691 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/process.py.j2
+-rw-r--r--   0        0        0      106 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/requirements.in
+-rwxr-xr-x   0        0        0     2122 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/test.sh
+-rw-r--r--   0        0        0     1240 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/utils.py
+-rw-r--r--   0        0        0     4408 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/validators.py
+-rw-r--r--   0        0        0     2115 2023-05-11 08:32:51.625927 evalutils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 evalutils-0.4.1/PKG-INFO
```

### Comparing `evalutils-0.4.0/LICENSE` & `evalutils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/README.md` & `evalutils-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/annotations.py` & `evalutils-0.4.1/evalutils/annotations.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/cli.py` & `evalutils-0.4.1/evalutils/cli.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/evalutils.py` & `evalutils-0.4.1/evalutils/evalutils.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/io.py` & `evalutils-0.4.1/evalutils/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         raise NotImplementedError
 
 
 class ImageIOLoader(ImageLoader):
     @staticmethod
     def load_image(fname):
         with open(fname, "rb") as f:
-            with get_reader(f, mode="i", as_gray=True) as r:
+            with get_reader(f, mode="i") as r:
                 return r.get_data(0)
 
     @staticmethod
     def hash_image(image):
         return hash(image.tobytes())
```

### Comparing `evalutils-0.4.0/evalutils/roc.py` & `evalutils-0.4.1/evalutils/roc.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/scorers.py` & `evalutils-0.4.1/evalutils/scorers.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/stats.py` & `evalutils-0.4.1/evalutils/stats.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/hooks/post_gen_project.py` & `evalutils-0.4.1/evalutils/templates/container/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/.github/workflows/ci.yml` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitignore` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/Dockerfile` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/Dockerfile`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_detection.json` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_detection.json`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation.py.j2` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation.py.j2`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/process.py.j2` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/process.py.j2`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/templates/container/{{ cookiecutter.package_name }}/test.sh` & `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/test.sh`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/utils.py` & `evalutils-0.4.1/evalutils/utils.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/evalutils/validators.py` & `evalutils-0.4.1/evalutils/validators.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.0/pyproject.toml` & `evalutils-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evalutils"
-version = "0.4.0"
+version = "0.4.1"
 description = "evalutils helps users create extensions for grand-challenge.org"
 authors = ["James Meakin <evalutils@jmsmkn.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/comic/evalutils"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -24,15 +24,15 @@
 # and https://github.com/python-poetry/poetry/issues/2453
 SimpleITK = ">=2.0,!=2.1.1.1"
 cookiecutter = "*"
 click = "*"
 scipy = "*"
 scikit-learn = "*"
 numpy = ">=1.22"
-pandas = ">=1.3"
+pandas = ">=1.3,<2.0"
 pip-tools = ">=6"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-xdist = "*"
 pytest-randomly = "*"
 pytest-cov = "*"
```

### Comparing `evalutils-0.4.0/PKG-INFO` & `evalutils-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalutils
-Version: 0.4.0
+Version: 0.4.1
 Summary: evalutils helps users create extensions for grand-challenge.org
 Home-page: https://github.com/comic/evalutils
 License: MIT
 Author: James Meakin
 Author-email: evalutils@jmsmkn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SimpleITK (>=2.0,!=2.1.1.1)
 Requires-Dist: click
 Requires-Dist: cookiecutter
 Requires-Dist: imageio[tifffile]
 Requires-Dist: numpy (>=1.22)
-Requires-Dist: pandas (>=1.3)
+Requires-Dist: pandas (>=1.3,<2.0)
 Requires-Dist: pip-tools (>=6)
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Project-URL: Repository, https://github.com/comic/evalutils
 Description-Content-Type: text/markdown
 
 # evalutils
```

