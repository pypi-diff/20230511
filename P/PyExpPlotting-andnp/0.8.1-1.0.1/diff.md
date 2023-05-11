# Comparing `tmp/PyExpPlotting-andnp-0.8.1.tar.gz` & `tmp/PyExpPlotting-andnp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyExpPlotting-andnp-0.8.1.tar", last modified: Thu Apr 21 16:16:44 2022, max compression
+gzip compressed data, was "PyExpPlotting-andnp-1.0.1.tar", last modified: Thu May 11 18:49:37 2023, max compression
```

## Comparing `PyExpPlotting-andnp-0.8.1.tar` & `PyExpPlotting-andnp-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 16:16:44.895104 PyExpPlotting-andnp-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-04-21 16:16:44.895104 PyExpPlotting-andnp-0.8.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 16:16:44.891104 PyExpPlotting-andnp-0.8.1/PyExpPlotting/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     6689 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting/distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting/learning_curves.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting/matplot.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting/sensitivity_curves.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 16:16:44.895104 PyExpPlotting-andnp-0.8.1/PyExpPlotting_andnp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-04-21 16:16:44.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting_andnp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-04-21 16:16:44.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting_andnp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 16:16:44.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting_andnp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-04-21 16:16:44.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting_andnp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-21 16:16:44.000000 PyExpPlotting-andnp-0.8.1/PyExpPlotting_andnp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-04-21 16:14:49.000000 PyExpPlotting-andnp-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-04-21 16:16:38.000000 PyExpPlotting-andnp-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-04-21 16:16:44.895104 PyExpPlotting-andnp-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-04-21 16:16:38.000000 PyExpPlotting-andnp-0.8.1/setup.py
+-rw-r--r--   0        0        0        1 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/colors.py
+-rw-r--r--   0        0        0     1148 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/defaults.py
+-rw-r--r--   0        0        0     6689 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/distributions.py
+-rw-r--r--   0        0        0     2604 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/learning_curves.py
+-rw-r--r--   0        0        0     2393 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/matplot.py
+-rw-r--r--   0        0        0        0 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/py.typed
+-rw-r--r--   0        0        0     3125 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/sensitivity_curves.py
+-rw-r--r--   0        0        0      842 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/PyExpPlotting/tools.py
+-rw-r--r--   0        0        0      107 2023-05-11 18:48:56.546692 PyExpPlotting-andnp-1.0.1/README.md
+-rw-r--r--   0        0        0      825 2023-05-11 18:49:35.102435 PyExpPlotting-andnp-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1362 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/distribution.py
+-rw-r--r--   0        0        0      635 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/experiments/example/CartPole/QLearning.json
+-rw-r--r--   0        0        0      653 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/experiments/example/CartPole/QRC.json
+-rw-r--r--   0        0        0      664 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/experiments/example/CartPole/SBEED.json
+-rw-r--r--   0        0        0      635 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/experiments/example/MountainCar/QLearning.json
+-rw-r--r--   0        0        0      653 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/experiments/example/MountainCar/QRC.json
+-rw-r--r--   0        0        0      664 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/experiments/example/MountainCar/SBEED.json
+-rw-r--r--   0        0        0     1034 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/experiments/example/learning_curve.py
+-rw-r--r--   0        0        0     1005 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/learning_curve.py
+-rw-r--r--   0        0        0     1010 2023-05-11 18:48:56.550691 PyExpPlotting-andnp-1.0.1/tests/sensitivity_curve.py
+-rw-r--r--   0        0        0      304 1970-01-01 00:00:00.000000 PyExpPlotting-andnp-1.0.1/PKG-INFO
```

### Comparing `PyExpPlotting-andnp-0.8.1/PyExpPlotting/defaults.py` & `PyExpPlotting-andnp-1.0.1/PyExpPlotting/defaults.py`

 * *Files identical despite different names*

### Comparing `PyExpPlotting-andnp-0.8.1/PyExpPlotting/distributions.py` & `PyExpPlotting-andnp-1.0.1/PyExpPlotting/distributions.py`

 * *Files identical despite different names*

### Comparing `PyExpPlotting-andnp-0.8.1/PyExpPlotting/matplot.py` & `PyExpPlotting-andnp-1.0.1/PyExpPlotting/matplot.py`

 * *Files identical despite different names*

