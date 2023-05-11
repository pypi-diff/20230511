# Comparing `tmp/ross-rotordynamics-1.4.0.tar.gz` & `tmp/ross-rotordynamics-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ross/ross/dist/.tmp-hnobonsc/ross-rotordynamics-1.4.0.tar", last modified: Thu Apr 20 18:44:52 2023, max compression
+gzip compressed data, was "/home/runner/work/ross/ross/dist/.tmp-p8x5s_pj/ross-rotordynamics-1.4.1.tar", last modified: Thu May 11 18:21:04 2023, max compression
```

## Comparing `ross-rotordynamics-1.4.0.tar` & `ross-rotordynamics-1.4.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-20 18:44:37.000000 ross-rotordynamics-1.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 18:44:37.000000 ross-rotordynamics-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-20 18:44:37.000000 ross-rotordynamics-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63592 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/bearing_seal_element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross/defects/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/abs_defect.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/crack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/integrate_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    34531 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/misalignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16371 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/rubbing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/disk_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113322 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/cylindrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    33197 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    16708 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/new_units.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/point_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)   160210 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/results.py
--rw-r--r--   0 runner    (1001) docker     (123)   142548 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/rotor_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    78702 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/shaft_element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross/stochastic/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18629 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_bearing_seal_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_disk_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_point_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    82816 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_results_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    31534 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_rotor_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_shaft_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66395 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/bearing_seal_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/defects/abs_defect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/defects/crack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/defects/integrate_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/defects/misalignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/defects/rubbing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/disk_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross/fluid_flow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/fluid_flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113322 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/fluid_flow/cylindrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33197 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/fluid_flow/fluid_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16708 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/fluid_flow/fluid_flow_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/fluid_flow/fluid_flow_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/fluid_flow/fluid_flow_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/new_units.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/point_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158763 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142925 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/rotor_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78702 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/shaft_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross/stochastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19118 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/st_bearing_seal_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/st_disk_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/st_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/st_point_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82816 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/st_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/st_results_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31534 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/st_rotor_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/stochastic/st_shaft_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21813 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/ross/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross_rotordynamics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross_rotordynamics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross_rotordynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross_rotordynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross_rotordynamics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/ross_rotordynamics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 18:21:04.000000 ross-rotordynamics-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-11 18:20:53.000000 ross-rotordynamics-1.4.1/setup.py
```

### Comparing `ross-rotordynamics-1.4.0/LICENSE.md` & `ross-rotordynamics-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/README.md` & `ross-rotordynamics-1.4.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Rotordynamic Open Source Software (ROSS)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ross-rotordynamics/ross/1.4.0?filepath=%2Fdocs%2Ftutorials)
-![github actions](https://github.com/ross-rotordynamics/ross/workflows/Tests/badge.svg)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/petrobras/ross/1.4.0?filepath=%2Fdocs%2Ftutorials)
+![github actions](https://github.com/petrobras/ross/workflows/Tests/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/ross/badge/?version=latest)](https://ross.readthedocs.io/en/latest/?badge=latest)
-<a href="https://codecov.io/gh/ross-rotordynamics/ross">
-<img src="https://codecov.io/gh/ross-rotordynamics/ross/branch/master/graph/badge.svg">
+<a href="https://codecov.io/gh/petrobras/ross">
+<img src="https://codecov.io/gh/petrobras/ross/branch/main/graph/badge.svg">
 </a>
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.02120/status.svg)](https://doi.org/10.21105/joss.02120)
 
 ROSS is a Python library for rotordynamic analysis, which allows the construction of rotor models and their numerical
 simulation. Shaft elements are modeled with the Timoshenko beam theory, which considers shear and rotary inertia
 effects, and discretized by means of the Finite Element Method. Disks are assumed to be rigid bodies, thus their strain
 energy is not taken into account. Bearings and seals are included as linear stiffness and damping coefficients.
 
 After defining the elements for the model, you can plot the rotor geometry and run simulations such as static analysis,
 modal analysis, undamped critical speed, frequency response, unbalance response, time response, and more.
 
-You can try it out now by running the tutorial on [binder](https://mybinder.org/v2/gh/ross-rotordynamics/ross/1.1.0?filepath=%2Fdocs%2Ftutorials)
+You can try it out now by running the tutorial on [binder](https://mybinder.org/v2/gh/petrobras/ross/1.4.0?filepath=%2Fdocs%2Ftutorials)
 
 # Documentation 
 Access the documentation [here](https://ross.readthedocs.io/en/latest/index.html).
 The documentation provides the [installation procedure](https://ross.readthedocs.io/en/latest/getting_started/installation.html), 
 [a tutorial](https://ross.readthedocs.io/en/latest/tutorials/tutorial_part_1.html), 
 [examples](https://ross.readthedocs.io/en/latest/discussions/discussions.html) and the 
 [API reference](https://ross.readthedocs.io/en/latest/references/api.html).
 
 # Questions
-If you have any questions, you can use the [Discussions](https://github.com/ross-rotordynamics/ross/discussions) area in the repository.
+If you have any questions, you can use the [Discussions](https://github.com/petrobras/ross/discussions) area in the repository.
 
 # Contributing to ROSS
 ROSS is a community-driven project. If you want to contribute to the project, please
-check [CONTRIBUTING.rst](https://github.com/ross-rotordynamics/ross/blob/master/CONTRIBUTING.rst). 
+check [CONTRIBUTING.md](https://github.com/petrobras/ross/blob/main/CONTRIBUTING.md). 
 
 The code has been initially developed by Petrobras in cooperation with the Federal University of Rio de Janeiro (UFRJ)
 with contributions from the Federal University from Uberlândia (UFU).
 Currently, Petrobras has a cooperation agreement with UFRJ (LAVI) and UFU (LMEST) to develop and maintain the code.
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
 # Rotordynamic Open Source Software (ROSS) [![Binder](https://mybinder.org/
-badge_logo.svg)](https://mybinder.org/v2/gh/ross-rotordynamics/ross/
-1.4.0?filepath=%2Fdocs%2Ftutorials) ![github actions](https://github.com/ross-
-rotordynamics/ross/workflows/Tests/badge.svg) [![Documentation Status](https://
+badge_logo.svg)](https://mybinder.org/v2/gh/petrobras/ross/
+1.4.0?filepath=%2Fdocs%2Ftutorials) ![github actions](https://github.com/
+petrobras/ross/workflows/Tests/badge.svg) [![Documentation Status](https://
 readthedocs.org/projects/ross/badge/?version=latest)](https://
-ross.readthedocs.io/en/latest/?badge=latest) [https://codecov.io/gh/ross-
-rotordynamics/ross/branch/master/graph/badge.svg] [![Code style: black](https:/
-/img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
-black) [![DOI](https://joss.theoj.org/papers/10.21105/joss.02120/status.svg)]
-(https://doi.org/10.21105/joss.02120) ROSS is a Python library for rotordynamic
+ross.readthedocs.io/en/latest/?badge=latest) [https://codecov.io/gh/petrobras/
+ross/branch/main/graph/badge.svg] [![Code style: black](https://img.shields.io/
+badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![DOI]
+(https://joss.theoj.org/papers/10.21105/joss.02120/status.svg)](https://
+doi.org/10.21105/joss.02120) ROSS is a Python library for rotordynamic
 analysis, which allows the construction of rotor models and their numerical
 simulation. Shaft elements are modeled with the Timoshenko beam theory, which
 considers shear and rotary inertia effects, and discretized by means of the
 Finite Element Method. Disks are assumed to be rigid bodies, thus their strain
 energy is not taken into account. Bearings and seals are included as linear
 stiffness and damping coefficients. After defining the elements for the model,
 you can plot the rotor geometry and run simulations such as static analysis,
 modal analysis, undamped critical speed, frequency response, unbalance
 response, time response, and more. You can try it out now by running the
-tutorial on [binder](https://mybinder.org/v2/gh/ross-rotordynamics/ross/
-1.1.0?filepath=%2Fdocs%2Ftutorials) # Documentation Access the documentation
+tutorial on [binder](https://mybinder.org/v2/gh/petrobras/ross/
+1.4.0?filepath=%2Fdocs%2Ftutorials) # Documentation Access the documentation
 [here](https://ross.readthedocs.io/en/latest/index.html). The documentation
 provides the [installation procedure](https://ross.readthedocs.io/en/latest/
 getting_started/installation.html), [a tutorial](https://ross.readthedocs.io/
 en/latest/tutorials/tutorial_part_1.html), [examples](https://
 ross.readthedocs.io/en/latest/discussions/discussions.html) and the [API
 reference](https://ross.readthedocs.io/en/latest/references/api.html). #
 Questions If you have any questions, you can use the [Discussions](https://
-github.com/ross-rotordynamics/ross/discussions) area in the repository. #
-Contributing to ROSS ROSS is a community-driven project. If you want to
-contribute to the project, please check [CONTRIBUTING.rst](https://github.com/
-ross-rotordynamics/ross/blob/master/CONTRIBUTING.rst). The code has been
-initially developed by Petrobras in cooperation with the Federal University of
-Rio de Janeiro (UFRJ) with contributions from the Federal University from
-UberlÃ¢ndia (UFU). Currently, Petrobras has a cooperation agreement with UFRJ
-(LAVI) and UFU (LMEST) to develop and maintain the code.
+github.com/petrobras/ross/discussions) area in the repository. # Contributing
+to ROSS ROSS is a community-driven project. If you want to contribute to the
+project, please check [CONTRIBUTING.md](https://github.com/petrobras/ross/blob/
+main/CONTRIBUTING.md). The code has been initially developed by Petrobras in
+cooperation with the Federal University of Rio de Janeiro (UFRJ) with
+contributions from the Federal University from UberlÃ¢ndia (UFU). Currently,
+Petrobras has a cooperation agreement with UFRJ (LAVI) and UFU (LMEST) to
+develop and maintain the code.
```

### Comparing `ross-rotordynamics-1.4.0/ross/bearing_seal_element.py` & `ross-rotordynamics-1.4.1/ross/bearing_seal_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,41 +106,65 @@
 
     @check_units
     def __init__(
         self,
         n,
         kxx,
         cxx,
+        mxx=None,
         kyy=None,
         kxy=0,
         kyx=0,
         cyy=None,
         cxy=0,
         cyx=0,
+        myy=None,
+        mxy=0,
+        myx=0,
         frequency=None,
         tag=None,
         n_link=None,
         scale_factor=1,
         color="#355d7a",
         **kwargs,
     ):
         if frequency is not None:
             self.frequency = np.array(frequency, dtype=np.float64)
         else:
             self.frequency = frequency
-        args = ["kxx", "kyy", "kxy", "kyx", "cxx", "cyy", "cxy", "cyx"]
+        args = [
+            "kxx",
+            "kyy",
+            "kxy",
+            "kyx",
+            "cxx",
+            "cyy",
+            "cxy",
+            "cyx",
+            "mxx",
+            "myy",
+            "mxy",
+            "myx",
+        ]
 
         # all args to coefficients
         args_dict = locals()
 
         if kyy is None:
             args_dict["kyy"] = kxx
         if cyy is None:
             args_dict["cyy"] = cxx
 
+        if myy is None:
+            if mxx is None:
+                args_dict["mxx"] = 0
+                args_dict["myy"] = 0
+            else:
+                args_dict["myy"] = mxx
+
         # check coefficients len for consistency
         coefficients_len = []
 
         for arg in args:
             coefficient, interpolated = self._process_coefficient(args_dict[arg])
             setattr(self, arg, coefficient)
             setattr(self, f"{arg}_interpolated", interpolated)
@@ -312,14 +336,16 @@
         return (
             f"{self.__class__.__name__}"
             f"(n={self.n}, n_link={self.n_link},\n"
             f" kxx={self.kxx}, kxy={self.kxy},\n"
             f" kyx={self.kyx}, kyy={self.kyy},\n"
             f" cxx={self.cxx}, cxy={self.cxy},\n"
             f" cyx={self.cyx}, cyy={self.cyy},\n"
+            f" mxx={self.mxx}, mxy={self.mxy},\n"
+            f" myx={self.myx}, myy={self.myy},\n"
             f" frequency={self.frequency}, tag={self.tag!r})"
         )
 
     def __eq__(self, other):
         """Equality method for comparasions.
 
         Parameters
@@ -344,14 +370,18 @@
             "kyy",
             "kxy",
             "kyx",
             "cxx",
             "cyy",
             "cxy",
             "cyx",
+            "mxx",
+            "myy",
+            "mxy",
+            "myx",
             "frequency",
         ]
         if isinstance(other, self.__class__):
             init_args = []
             for arg in signature(self.__init__).parameters:
                 if arg not in ["kwargs"]:
                     init_args.append(arg)
@@ -395,14 +425,18 @@
             "kyy",
             "kxy",
             "kyx",
             "cxx",
             "cyy",
             "cxy",
             "cyx",
+            "mxx",
+            "myy",
+            "mxy",
+            "myx",
         ]
         brg_data = {}
         for arg in args:
             if arg not in ["kwargs"]:
                 brg_data[arg] = self.__dict__[arg]
 
         # change np.array to lists so that we can save in .toml as list(floats)
@@ -445,33 +479,44 @@
 
         >>> bearing = bearing_example()
         >>> bearing.dof_mapping()
         {'x_0': 0, 'y_0': 1}
         """
         return dict(x_0=0, y_0=1)
 
-    def M(self):
+    def M(self, frequency):
         """Mass matrix for an instance of a bearing element.
 
         This method returns the mass matrix for an instance of a bearing
         element.
 
         Returns
         -------
         M : np.ndarray
             Mass matrix (kg).
 
         Examples
         --------
         >>> bearing = bearing_example()
-        >>> bearing.M()
+        >>> bearing.M(0)
         array([[0., 0.],
                [0., 0.]])
         """
-        M = np.zeros_like(self.K(0))
+        mxx = self.mxx_interpolated(frequency)
+        myy = self.myy_interpolated(frequency)
+        mxy = self.mxy_interpolated(frequency)
+        myx = self.myx_interpolated(frequency)
+
+        M = np.array([[mxx, mxy], [myx, myy]])
+
+        if self.n_link is not None:
+            # fmt: off
+            M = np.vstack((np.hstack([M, -M]),
+                           np.hstack([-M, M])))
+            # fmt: on
 
         return M
 
     @check_units
     def K(self, frequency):
         """Stiffness matrix for an instance of a bearing element.
 
@@ -1039,20 +1084,24 @@
 
     @check_units
     def __init__(
         self,
         n,
         kxx,
         cxx,
+        mxx=None,
         kyy=None,
         kxy=0,
         kyx=0,
         cyy=None,
         cxy=0,
         cyx=0,
+        myy=None,
+        mxy=0,
+        myx=0,
         frequency=None,
         seal_leakage=None,
         tag=None,
         n_link=None,
         scale_factor=1.0,
         color="#77ACA2",
         **kwargs,
@@ -1066,14 +1115,18 @@
             kxy=kxy,
             kyx=kyx,
             kyy=kyy,
             cxx=cxx,
             cxy=cxy,
             cyx=cyx,
             cyy=cyy,
+            mxx=mxx,
+            mxy=mxy,
+            myx=myx,
+            myy=myy,
             tag=tag,
             n_link=n_link,
             scale_factor=seal_scale_factor,
             color=color,
         )
 
         self.seal_leakage = seal_leakage
@@ -1717,55 +1770,71 @@
 
     @check_units
     def __init__(
         self,
         n,
         kxx,
         cxx,
+        mxx=None,
         kyy=None,
         cyy=None,
+        myy=None,
         kxy=0.0,
         kyx=0.0,
         kzz=0.0,
         cxy=0.0,
         cyx=0.0,
         czz=0.0,
+        mxy=0.0,
+        myx=0.0,
+        mzz=0.0,
         frequency=None,
         tag=None,
         n_link=None,
         scale_factor=1,
         color="#355d7a",
     ):
         super().__init__(
             n=n,
             kxx=kxx,
             cxx=cxx,
+            mxx=mxx,
             kyy=kyy,
             kxy=kxy,
             kyx=kyx,
             cyy=cyy,
             cxy=cxy,
             cyx=cyx,
+            myy=myy,
+            mxy=mxy,
+            myx=myx,
             frequency=frequency,
             tag=tag,
             n_link=n_link,
             scale_factor=scale_factor,
             color=color,
         )
 
-        new_args = ["kzz", "czz"]
+        new_args = ["kzz", "czz", "mzz"]
 
         args_dict = locals()
         coefficients = {}
 
         if kzz is None:
             args_dict["kzz"] = kxx * 0.0
         if czz is None:
             args_dict["czz"] = cxx * 0.0
 
+        if mzz is None:
+            if mxx is None:
+                args_dict["mxx"] = 0
+                args_dict["mzz"] = 0
+            else:
+                args_dict["mzz"] = mxx * 0.0
+
         # check coefficients len for consistency
         coefficients_len = []
 
         for arg in new_args:
             coefficient, interpolated = self._process_coefficient(args_dict[arg])
             setattr(self, arg, coefficient)
             setattr(self, f"{arg}_interpolated", interpolated)
@@ -1809,14 +1878,17 @@
             f"{self.__class__.__name__}"
             f"(n={self.n}, n_link={self.n_link},\n"
             f" kxx={self.kxx}, kxy={self.kxy},\n"
             f" kyx={self.kyx}, kyy={self.kyy},\n"
             f" kzz={self.kzz}, cxx={self.cxx},\n"
             f" cxy={self.cxy}, cyx={self.cyx},\n"
             f" cyy={self.cyy}, czz={self.czz},\n"
+            f" mxx={self.mxx}, mxy={self.mxy},\n"
+            f" myx={self.myx}, myy={self.myy},\n"
+            f" mzz={self.mzz},\n"
             f" frequency={self.frequency}, tag={self.tag!r})"
         )
 
     def __eq__(self, other):
         """Equality method for comparasions.
 
         Parameters
@@ -1843,14 +1915,19 @@
             "kyx",
             "kzz",
             "cxx",
             "cyy",
             "cxy",
             "cyx",
             "czz",
+            "mxx",
+            "myy",
+            "mxy",
+            "myx",
+            "mzz",
             "frequency",
         ]
         if isinstance(other, self.__class__):
             init_args = []
             for arg in signature(self.__init__).parameters:
                 if arg not in ["kwargs"]:
                     init_args.append(arg)
@@ -1910,14 +1987,19 @@
             "kyx",
             "kzz",
             "cxx",
             "cyy",
             "cxy",
             "cyx",
             "czz",
+            "mxx",
+            "myy",
+            "mxy",
+            "myx",
+            "mzz",
             "frequency",
         ]
         for p in params:
             try:
                 brg_data[p] = [float(i) for i in brg_data[p]]
             except TypeError:
                 pass
@@ -1939,14 +2021,19 @@
             "kyx",
             "kzz",
             "cxx",
             "cyy",
             "cxy",
             "cyx",
             "czz",
+            "mxx",
+            "myy",
+            "mxy",
+            "myx",
+            "mzz",
             "frequency",
             "n",
             "tag",
             "n_link",
             "scale_factor",
         ]
         kwargs = {}
@@ -1984,14 +2071,44 @@
 
         >>> bearing = bearing_6dof_example()
         >>> bearing.dof_mapping()
         {'x_0': 0, 'y_0': 1, 'z_0': 2}
         """
         return dict(x_0=0, y_0=1, z_0=2)
 
+    def M(self, frequency):
+        """Mass matrix for an instance of a bearing element.
+
+        This method returns the mass matrix for an instance of a bearing
+        element.
+
+        Returns
+        -------
+        M : np.ndarray
+            Mass matrix (kg).
+
+        Examples
+        --------
+        >>> bearing = bearing_6dof_example()
+        >>> bearing.M(0)
+        array([[0., 0., 0.],
+               [0., 0., 0.],
+               [0., 0., 0.]])
+        """
+
+        mxx = self.mxx_interpolated(frequency)
+        myy = self.myy_interpolated(frequency)
+        mxy = self.mxy_interpolated(frequency)
+        myx = self.myx_interpolated(frequency)
+        mzz = self.mzz_interpolated(frequency)
+
+        M = np.array([[mxx, mxy, 0], [myx, myy, 0], [0, 0, mzz]])
+
+        return M
+
     def K(self, frequency):
         """Stiffness matrix for an instance of a bearing element.
 
         This method returns the stiffness matrix for an instance of a bearing element.
 
         Parameters
         ----------
```

### Comparing `ross-rotordynamics-1.4.0/ross/defects/abs_defect.py` & `ross-rotordynamics-1.4.1/ross/defects/abs_defect.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/defects/crack.py` & `ross-rotordynamics-1.4.1/ross/defects/crack.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         # TorqueV = sAT + sBT * np.exp(-lambdat * self.t)
         # AccelV = -lambdat * sB * np.exp(-lambdat * self.t)
 
         # Determining the modal matrix
         self.K = self.rotor.K(self.speed)
         self.C = self.rotor.C(self.speed)
         self.G = self.rotor.G()
-        self.M = self.rotor.M()
+        self.M = self.rotor.M(self.speed)
         self.Kst = self.rotor.Kst()
 
         _, ModMat = scipy.linalg.eigh(
             self.K,
             self.M,
             type=1,
             turbo=False,
```

### Comparing `ross-rotordynamics-1.4.0/ross/defects/integrate_solver.py` & `ross-rotordynamics-1.4.1/ross/defects/integrate_solver.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/defects/misalignment.py` & `ross-rotordynamics-1.4.1/ross/defects/misalignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         # TorqueV = sAT + sBT * np.exp(-lambdat * self.t)
         # AccelV = -lambdat * sB * np.exp(-lambdat * self.t)
 
         # Determining the modal matrix
         self.K = self.rotor.K(self.speed)
         self.C = self.rotor.C(self.speed)
         self.G = self.rotor.G()
-        self.M = self.rotor.M()
+        self.M = self.rotor.M(self.speed)
         self.Kst = self.rotor.Kst()
 
         _, ModMat = scipy.linalg.eigh(self.K, self.M, type=1, turbo=False)
         ModMat = ModMat[:, :12]
         self.ModMat = ModMat
 
         # Modal transformations
@@ -642,15 +642,15 @@
         # self.TorqueV = sAT + sBT * np.exp(-lambdat * t)
         # self.AccelV = -lambdat * sB * np.exp(-lambdat * t)
 
         # Determining the modal matrix
         self.K = self.rotor.K(self.speed)
         self.C = self.rotor.C(self.speed)
         self.G = self.rotor.G()
-        self.M = self.rotor.M()
+        self.M = self.rotor.M(self.speed)
         self.Kst = self.rotor.Kst()
 
         _, ModMat = scipy.linalg.eigh(self.K, self.M, type=1, turbo=False)
         ModMat = ModMat[:, :12]
         self.ModMat = ModMat
 
         # Modal transformations
```

### Comparing `ross-rotordynamics-1.4.0/ross/defects/rubbing.py` & `ross-rotordynamics-1.4.1/ross/defects/rubbing.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         # self.TorqueV = sAT + sBT * np.exp(-lambdat * t)
         # self.AccelV = -lambdat * sB * np.exp(-lambdat * t)
 
         # Determining the modal matrix
         self.K = self.rotor.K(self.speed)
         self.C = self.rotor.C(self.speed)
         self.G = self.rotor.G()
-        self.M = self.rotor.M()
+        self.M = self.rotor.M(self.speed)
         self.Kst = self.rotor.Kst()
 
         V1, ModMat = scipy.linalg.eigh(
             self.K,
             self.M,
             type=1,
             turbo=False,
```

### Comparing `ross-rotordynamics-1.4.0/ross/disk_element.py` & `ross-rotordynamics-1.4.1/ross/disk_element.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/element.py` & `ross-rotordynamics-1.4.1/ross/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         A matrix of floats.
 
         Examples
         --------
         >>> # Example using BearingElement
         >>> from ross.bearing_seal_element import bearing_example
         >>> bearing = bearing_example()
-        >>> bearing.M()
+        >>> bearing.M(0)
         array([[0., 0.],
                [0., 0.]])
         """
         pass
 
     @abstractmethod
     def C(self, frequency):
```

### Comparing `ross-rotordynamics-1.4.0/ross/fluid_flow/cylindrical.py` & `ross-rotordynamics-1.4.1/ross/fluid_flow/cylindrical.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow.py` & `ross-rotordynamics-1.4.1/ross/fluid_flow/fluid_flow.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_coefficients.py` & `ross-rotordynamics-1.4.1/ross/fluid_flow/fluid_flow_coefficients.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_geometry.py` & `ross-rotordynamics-1.4.1/ross/fluid_flow/fluid_flow_geometry.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_graphics.py` & `ross-rotordynamics-1.4.1/ross/fluid_flow/fluid_flow_graphics.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/materials.py` & `ross-rotordynamics-1.4.1/ross/materials.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/plotly_theme.py` & `ross-rotordynamics-1.4.1/ross/plotly_theme.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/point_mass.py` & `ross-rotordynamics-1.4.1/ross/point_mass.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/results.py` & `ross-rotordynamics-1.4.1/ross/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This module returns graphs for each type of analyses in rotor_assembly.py.
 """
 import copy
 import inspect
 from abc import ABC
 from collections.abc import Iterable
 from pathlib import Path
+from warnings import warn
 
 import numpy as np
 import pandas as pd
 import toml
 from plotly import graph_objects as go
 from plotly.subplots import make_subplots
 from scipy import linalg as la
@@ -384,15 +385,15 @@
 
         if self.normalize:
             modex = evec[0::4]
             modey = evec[1::4]
             xmax, ixmax = max(abs(modex)), np.argmax(abs(modex))
             ymax, iymax = max(abs(modey)), np.argmax(abs(modey))
 
-            if ymax > 0.4 * xmax:
+            if ymax > xmax:
                 evec /= modey[iymax]
             else:
                 evec /= modex[ixmax]
 
         self._evec = evec
         self.orbits = None
         self.whirl = None
@@ -1124,14 +1125,15 @@
 
         return fig
 
     def plot_mode_2d(
         self,
         mode=None,
         fig=None,
+        orientation="major",
         frequency_type="wd",
         title=None,
         length_units="m",
         frequency_units="rad/s",
         damping_parameter="log_dec",
         **kwargs,
     ):
@@ -1139,14 +1141,17 @@
 
         Parameters
         ----------
         mode : int
             The n'th vibration mode
         fig : Plotly graph_objects.Figure()
             The figure object with the plot.
+        orientation : str, optional
+            Orientation can be 'major', 'x' or 'y'.
+            Default is 'major' to display the major axis.
         frequency_type : str, optional
             "wd" calculates the damped natural frequencies.
             "wn" calculates the undamped natural frequencies.
             Defaults is "wd".
         title : str, optional
             A brief title to the mode shape plot, it will be displayed above other
             relevant data in the plot area. It does not modify the figure layout from
@@ -1182,15 +1187,15 @@
         frequency = {
             "wd": f"ω<sub>d</sub> = {Q_(self.wd[mode], 'rad/s').to(frequency_units).m:.2f}",
             "wn": f"ω<sub>n</sub> = {Q_(self.wn[mode], 'rad/s').to(frequency_units).m:.2f}",
             "speed": f"Speed = {Q_(self.speed, 'rad/s').to(frequency_units).m:.2f}",
         }
 
         shape = self.shapes[mode]
-        fig = shape.plot_2d(fig=fig)
+        fig = shape.plot_2d(fig=fig, orientation=orientation)
 
         if title is None:
             title = ""
 
         fig.update_xaxes(title_text=f"Rotor Length ({length_units})")
         fig.update_yaxes(title_text="Relative Displacement")
         fig.update_layout(
@@ -2079,24 +2084,15 @@
         amplitude_units="m",
     ):
         """Return the forced response (magnitude) in DataFrame format.
 
         Parameters
         ----------
         probe : list
-            List with tuples (node, orientation angle, tag).
-
-            node : int -> Indicate the node where the probe is located.
-
-            orientation : float -> Probe orientation angle about the shaft.
-            The 0 refers to +X direction.
-            The strings 'major' and 'minor' can also be used to reference the major
-            and minor axis.
-
-            tag : str, optional -> Probe tag to be add a DataFrame column title.
+            List with rs.Probe objects.
         probe_units : str, option
             Units for probe orientation.
             Default is "rad".
         frequency_units : str, optional
             Units for the frequency range.
             Default is "rad/s"
         amplitude_units : str, optional
@@ -2131,32 +2127,47 @@
 
         data = {}
         data["frequency"] = frequency_range
 
         for i, p in enumerate(probe):
             amplitude = []
             for speed_idx in range(len(self.speed_range)):
+                # first try to get the angle from the probe object
                 try:
-                    angle = Q_(p[1], probe_units).to("rad").m
-                except TypeError:
-                    angle = p[1]
+                    angle = p.angle
+                    node = p.node
+                # if it is a tuple, warn the user that the use of tuples is deprecated
+                except AttributeError:
+                    try:
+                        angle = Q_(p[1], probe_units).to("rad").m
+                        warn(
+                            "The use of tuples in the probe argument is deprecated. Use the Probe class instead.",
+                            DeprecationWarning,
+                        )
+                        node = p[0]
+                    except TypeError:
+                        angle = p[1]
+                        node = p[0]
 
                 ru_e, rv_e = response[:, speed_idx][
-                    self.rotor.number_dof * p[0] : self.rotor.number_dof * p[0] + 2
+                    self.rotor.number_dof * node : self.rotor.number_dof * node + 2
                 ]
                 orbit = Orbit(
-                    node=p[0], node_pos=self.rotor.nodes_pos[p[0]], ru_e=ru_e, rv_e=rv_e
+                    node=node, node_pos=self.rotor.nodes_pos[node], ru_e=ru_e, rv_e=rv_e
                 )
                 amp, phase = orbit.calculate_amplitude(angle=angle)
                 amplitude.append(amp)
 
             try:
-                probe_tag = p[2]
-            except IndexError:
-                probe_tag = f"Probe {i+1} - Node {p[0]}"
+                probe_tag = p.tag
+            except AttributeError:
+                try:
+                    probe_tag = p[2]
+                except IndexError:
+                    probe_tag = f"Probe {i+1} - Node {p[0]}"
 
             data[probe_tag] = Q_(amplitude, base_unit).to(amplitude_units).m
 
         df = pd.DataFrame(data)
 
         return df
 
@@ -2169,24 +2180,15 @@
         phase_units="rad",
     ):
         """Return the forced response (phase) in DataFrame format.
 
         Parameters
         ----------
         probe : list
-            List with tuples (node, orientation angle, tag).
-
-            node : int -> Indicate the node where the probe is located.
-
-            orientation : float -> Probe orientation angle about the shaft.
-            The 0 refers to +X direction.
-            The strings 'major' and 'minor' can also be used to reference the major
-            and minor axis.
-
-            tag : str, optional -> Probe tag to be add a DataFrame column title.
+            List with rs.Probe objects.
         probe_units : str, option
             Units for probe orientation.
             Default is "rad".
         frequency_units : str, optional
             Units for the x axis.
             Default is "rad/s"
         amplitude_units : str, optional
@@ -2224,32 +2226,47 @@
 
         data = {}
         data["frequency"] = frequency_range
 
         for i, p in enumerate(probe):
             phase_values = []
             for speed_idx in range(len(self.speed_range)):
+                # first try to get the angle from the probe object
                 try:
-                    angle = Q_(p[1], probe_units).to("rad").m
-                except TypeError:
-                    angle = p[1]
+                    angle = p.angle
+                    node = p.node
+                # if it is a tuple, warn the user that the use of tuples is deprecated
+                except AttributeError:
+                    try:
+                        angle = Q_(p[1], probe_units).to("rad").m
+                        warn(
+                            "The use of tuples in the probe argument is deprecated. Use the Probe class instead.",
+                            DeprecationWarning,
+                        )
+                        node = p[0]
+                    except TypeError:
+                        angle = p[1]
+                        node = p[0]
 
                 ru_e, rv_e = response[:, speed_idx][
-                    self.rotor.number_dof * p[0] : self.rotor.number_dof * p[0] + 2
+                    self.rotor.number_dof * node : self.rotor.number_dof * node + 2
                 ]
                 orbit = Orbit(
-                    node=p[0], node_pos=self.rotor.nodes_pos[p[0]], ru_e=ru_e, rv_e=rv_e
+                    node=node, node_pos=self.rotor.nodes_pos[node], ru_e=ru_e, rv_e=rv_e
                 )
                 amp, phase = orbit.calculate_amplitude(angle=angle)
                 phase_values.append(phase)
 
             try:
-                probe_tag = p[2]
-            except IndexError:
-                probe_tag = f"Probe {i+1} - Node {p[0]}"
+                probe_tag = p.tag
+            except AttributeError:
+                try:
+                    probe_tag = p[2]
+                except IndexError:
+                    probe_tag = f"Probe {i+1} - Node {p[0]}"
 
             data[probe_tag] = Q_(phase_values, "rad").to(phase_units).m
 
         df = pd.DataFrame(data)
 
         return df
 
@@ -2263,25 +2280,16 @@
         **kwargs,
     ):
         """Plot forced response (magnitude) using Plotly.
 
         Parameters
         ----------
         probe : list
-            List with tuples (node, orientation angle, tag).
-
-            node : int -> Indicate the node where the probe is located.
-
-            orientation : float -> Probe orientation angle about the shaft.
-            The 0 refers to +X direction.
-            The strings 'major' and 'minor' can also be used to reference the major
-            and minor axis.
-
-            tag : str, optional -> Probe tag to be add a DataFrame column title.
-        probe_units : str, option
+            List with rs.Probe objects.
+        probe_units : str, optional
             Units for probe orientation.
             Default is "rad".
         frequency_units : str, optional
             Units for the x axis.
             Default is "rad/s"
         amplitude_units : str, optional
             Units for the response magnitude.
@@ -2348,25 +2356,16 @@
         **kwargs,
     ):
         """Plot forced response (phase) using Plotly.
 
         Parameters
         ----------
         probe : list
-            List with tuples (node, orientation angle, tag).
-
-            node : int -> Indicate the node where the probe is located.
-
-            orientation : float -> Probe orientation angle about the shaft.
-            The 0 refers to +X direction.
-            The strings 'major' and 'minor' can also be used to reference the major
-            and minor axis.
-
-            tag : str, optional -> Probe tag to be add a DataFrame column title.
-        probe_units : str, option
+            List with rs.Probe objects.
+        probe_units : str, optional
             Units for probe orientation.
             Default is "rad".
         frequency_units : str, optional
             Units for the x axis.
             Default is "rad/s"
         amplitude_units : str, optional
             Units for the response magnitude.
@@ -2436,25 +2435,16 @@
         **kwargs,
     ):
         """Plot polar forced response using Plotly.
 
         Parameters
         ----------
         probe : list
-            List with tuples (node, orientation angle, tag).
-
-            node : int -> Indicate the node where the probe is located.
-
-            orientation : float -> Probe orientation angle about the shaft.
-            The 0 refers to +X direction.
-            The strings 'major' and 'minor' can also be used to reference the major
-            and minor axis.
-
-            tag : str, optional -> Probe tag to be add a DataFrame column title.
-        probe_units : str, option
+            List with rs.Probe objects.
+        probe_units : str, optional
             Units for probe orientation.
             Default is "rad".
         frequency_units : str, optional
             Units for the x axis.
             Default is "rad/s"
         amplitude_units : str, optional
             Units for the response magnitude.
@@ -2544,25 +2534,16 @@
             - Frequency vs Amplitude;
             - Frequency vs Phase Angle;
             - Polar plot Amplitude vs Phase Angle;
 
         Parameters
         ----------
         probe : list
-            List with tuples (node, orientation angle, tag).
-
-            node : int -> Indicate the node where the probe is located.
-
-            orientation : float -> Probe orientation angle about the shaft.
-            The 0 refers to +X direction.
-            The strings 'major' and 'minor' can also be used to reference the major
-            and minor axis.
-
-            tag : str, optional -> Probe tag to be add a DataFrame column title.
-        probe_units : str, option
+            List with rs.Probe objects.
+        probe_units : str, optional
             Units for probe orientation.
             Default is "rad".
         frequency_units : str, optional
             Frequency units.
             Default is "rad/s"
         amplitude_units : str, optional
             Units for the response magnitude.
@@ -4179,24 +4160,15 @@
 
         This method plots the time response given a tuple of probes with their nodes
         and orientations.
 
         Parameters
         ----------
         probe : list
-            List with tuples (node, orientation angle, tag).
-
-            node : int -> Indicate the node where the probe is located.
-
-            orientation : float -> Probe orientation angle about the shaft.
-            The 0 refers to +X direction.
-            The strings 'major' and 'minor' can also be used to reference the major
-            and minor axis.
-
-            tag : str, optional -> Probe tag to be add a DataFrame column title.
+            List with rs.Probe objects.
         probe_units : str, option
             Units for probe orientation.
             Default is "rad".
         displacement_units : str, optional
             Displacement units.
             Default is 'm'.
         time_units : str
@@ -4568,30 +4540,27 @@
         fig.update_layout(title=dict(text="Undamped Critical Speed Map"), **kwargs)
 
         return fig
 
     def plot_mode_2d(
         self,
         critical_mode,
-        evec=None,
         fig=None,
         frequency_type="wd",
         title=None,
         length_units="m",
         frequency_units="rad/s",
         **kwargs,
     ):
         """Plot (2D view) the mode shape.
 
         Parameters
         ----------
         critical_mode : int
             The n'th critical mode.
-        evec : array
-            Array containing the system eigenvectors
         fig : Plotly graph_objects.Figure()
             The figure object with the plot.
         frequency_type : str, optional
             "wd" calculates de map for the damped natural frequencies.
             "wn" calculates de map for the undamped natural frequencies.
             Defaults is "wd".
         title : str, optional
@@ -4620,45 +4589,41 @@
             modal_critical.whirl_direction() == "Forward"
         ]
         idx_forward = (np.abs(forward_frequencies - modal_critical.speed)).argmin()
         forward_frequency = forward_frequencies[idx_forward]
         idx = (np.abs(modal_critical.wd - forward_frequency)).argmin()
         fig = modal_critical.plot_mode_2d(
             idx,
-            evec=evec,
             fig=fig,
             frequency_type=frequency_type,
             title=title,
             length_units=length_units,
             frequency_units=frequency_units,
             **kwargs,
         )
 
         return fig
 
     def plot_mode_3d(
         self,
         critical_mode,
-        evec=None,
         fig=None,
         frequency_type="wd",
         title=None,
         length_units="m",
         frequency_units="rad/s",
         **kwargs,
     ):
         """Plot (3D view) the mode shapes.
 
         Parameters
         ----------
         critical_mode : int
             The n'th critical mode.
             Default is None
-        evec : array
-            Array containing the system eigenvectors
         fig : Plotly graph_objects.Figure()
             The figure object with the plot.
         frequency_type : str, optional
             "wd" calculates de map for the damped natural frequencies.
             "wn" calculates de map for the undamped natural frequencies.
             Defaults is "wd".
         title : str, optional
@@ -4687,23 +4652,24 @@
             modal_critical.whirl_direction() == "Forward"
         ]
         idx_forward = (np.abs(forward_frequencies - modal_critical.speed)).argmin()
         forward_frequency = forward_frequencies[idx_forward]
         idx = (np.abs(modal_critical.wd - forward_frequency)).argmin()
         fig = modal_critical.plot_mode_3d(
             idx,
-            evec=evec,
             fig=fig,
             frequency_type=frequency_type,
             title=title,
             length_units=length_units,
             frequency_units=frequency_units,
             **kwargs,
         )
 
+        return fig
+
 
 class Level1Results(Results):
     """Class used to store results and provide plots for Level 1 Stability Analysis.
 
     Parameters
     ----------
     stiffness_range : array
```

### Comparing `ross-rotordynamics-1.4.0/ross/rotor_assembly.py` & `ross-rotordynamics-1.4.1/ross/rotor_assembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -882,36 +882,44 @@
         self.__dict__ = aux_rotor.__dict__
         self.error_arr = error_arr
 
         results = ConvergenceResults(el_num[1:], eigv_arr[1:], error_arr[1:])
 
         return results
 
-    def M(self):
+    def M(self, frequency=None):
         """Mass matrix for an instance of a rotor.
 
         Returns
         -------
         M0 : np.ndarray
             Mass matrix for the rotor.
 
         Examples
         --------
         >>> rotor = rotor_example()
-        >>> rotor.M()[:4, :4]
+        >>> rotor.M(0)[:4, :4]
         array([[ 1.42050794,  0.        ,  0.        ,  0.04931719],
                [ 0.        ,  1.42050794, -0.04931719,  0.        ],
                [ 0.        , -0.04931719,  0.00231392,  0.        ],
                [ 0.04931719,  0.        ,  0.        ,  0.00231392]])
         """
         M0 = np.zeros((self.ndof, self.ndof))
 
+        # if frequency is None, we assume the rotor does not have any elements
+        # with frequency dependent mass matrices
+        if frequency is None:
+            frequency = 0
+
         for elm in self.elements:
             dofs = list(elm.dof_global_index.values())
-            M0[np.ix_(dofs, dofs)] += elm.M()
+            try:
+                M0[np.ix_(dofs, dofs)] += elm.M(frequency)
+            except TypeError:
+                M0[np.ix_(dofs, dofs)] += elm.M()
 
         return M0
 
     def K(self, frequency):
         """Stiffness matrix for an instance of a rotor.
 
         Parameters
@@ -1068,15 +1076,15 @@
 
         Z = np.zeros((self.ndof, self.ndof))
         I = np.eye(self.ndof)
 
         # fmt: off
         A = np.vstack(
             [np.hstack([Z, I]),
-             np.hstack([la.solve(-self.M(), self.K(frequency) + self.Kst()*speed), la.solve(-self.M(), (self.C(frequency) + self.G() * speed))])])
+             np.hstack([la.solve(-self.M(frequency), self.K(frequency) + self.Kst()*speed), la.solve(-self.M(frequency), (self.C(frequency) + self.G() * speed))])])
         # fmt: on
 
         return A
 
     def _check_frequency_array(self, frequency_range):
         """Verify if bearing elements coefficients are extrapolated.
 
@@ -1320,27 +1328,27 @@
         # x' = Ax + Bu
         B2 = I
         if frequency is None:
             frequency = speed
         A = self.A(speed=speed, frequency=frequency)
         # fmt: off
         B = np.vstack([Z,
-                       la.solve(self.M(), B2)])
+                       la.solve(self.M(frequency), B2)])
         # fmt: on
 
         # y = Cx + Du
         # Observation matrices
         Cd = I
         Cv = Z
         Ca = Z
 
         # fmt: off
-        C = np.hstack((Cd - Ca @ la.solve(self.M(), self.K(frequency)), Cv - Ca @ la.solve(self.M(), self.C(frequency))))
+        C = np.hstack((Cd - Ca @ la.solve(self.M(frequency), self.K(frequency)), Cv - Ca @ la.solve(self.M(frequency), self.C(frequency))))
         # fmt: on
-        D = Ca @ la.solve(self.M(), B2)
+        D = Ca @ la.solve(self.M(frequency), B2)
 
         sys = signal.lti(A, B, C, D)
 
         return sys
 
     def transfer_matrix(self, speed=None, frequency=None, modes=None):
         """Calculate the fer matrix for the frequency response function (FRF).
@@ -2630,15 +2638,15 @@
         >>> rotor = rotor_example()
         >>> rotor.save_mat(file, speed=0)
         """
         if frequency is None:
             frequency = speed
 
         dic = {
-            "M": self.M(),
+            "M": self.M(frequency),
             "K": self.K(frequency),
             "C": self.C(frequency),
             "G": self.G(),
             "nodes": self.nodes_pos,
         }
 
         sio.savemat(file, dic)
@@ -2813,17 +2821,17 @@
         aux_rotor = Rotor(self.shaft_elements, self.disk_elements, aux_brg)
         aux_rotor_1 = Rotor(self.shaft_elements, self.disk_elements, aux_brg_1)
 
         aux_K = aux_rotor.K(0)
 
         # gravity aceleration vector
         g = -9.8065
-        gravity = np.zeros(len(aux_rotor.M()))
+        gravity = np.zeros(len(aux_rotor.M(0)))
         gravity[1 :: self.number_dof] = g
-        weight = aux_rotor.M() @ gravity
+        weight = aux_rotor.M(0) @ gravity
 
         # calculates u, for [K]*(u) = (F)
         displacement = (la.solve(aux_K, weight)).flatten()
         displacement_y = displacement[1 :: self.number_dof]
 
         # calculate forces
         nodal_forces = aux_rotor_1.K(0) @ displacement
```

### Comparing `ross-rotordynamics-1.4.0/ross/shaft_element.py` & `ross-rotordynamics-1.4.1/ross/shaft_element.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/stochastic/st_bearing_seal_element.py` & `ross-rotordynamics-1.4.1/ross/stochastic/st_bearing_seal_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,20 +111,24 @@
 
     @check_units
     def __init__(
         self,
         n,
         kxx,
         cxx,
+        mxx=None,
         kyy=None,
         kxy=0,
         kyx=0,
         cyy=None,
         cxy=0,
         cyx=0,
+        myy=None,
+        mxy=0,
+        myx=0,
         frequency=None,
         tag=None,
         n_link=None,
         scale_factor=1,
         is_random=None,
     ):
         if "frequency" in is_random:
@@ -135,24 +139,37 @@
             if "kxx" in is_random and "kyy" not in is_random:
                 is_random.append("kyy")
         if cyy is None:
             cyy = cxx
             if "cxx" in is_random and "cyy" not in is_random:
                 is_random.append("cyy")
 
+        if myy is None:
+            if mxx is None:
+                myy = 0
+                mxx = 0
+            else:
+                myy = mxx
+            if "mxx" in is_random and "myy" not in is_random:
+                is_random.append("myy")
+
         attribute_dict = dict(
             n=n,
             kxx=kxx,
             cxx=cxx,
+            mxx=mxx,
             kyy=kyy,
             kxy=kxy,
             kyx=kyx,
             cyy=cyy,
             cxy=cxy,
             cyx=cyx,
+            myy=myy,
+            mxy=mxy,
+            myx=myx,
             frequency=frequency,
             tag=tag,
             n_link=n_link,
             scale_factor=scale_factor,
         )
         self.is_random = is_random
         self.attribute_dict = attribute_dict
@@ -333,14 +350,18 @@
             kxy="Kxy",
             kyx="Kyx",
             kyy="Kyy",
             cxx="Cxx",
             cxy="Cxy",
             cyx="Cyx",
             cyy="Cyy",
+            mxx="Mxx",
+            mxy="Mxy",
+            myx="Myx",
+            myy="Myy",
         )
         if var_list is None:
             var_list = self.is_random
         elif not all(var in self.is_random for var in var_list):
             raise ValueError(
                 "Random variable not in var_list. Select variables from {}".format(
                     self.is_random
```

### Comparing `ross-rotordynamics-1.4.0/ross/stochastic/st_disk_element.py` & `ross-rotordynamics-1.4.1/ross/stochastic/st_disk_element.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/stochastic/st_materials.py` & `ross-rotordynamics-1.4.1/ross/stochastic/st_materials.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/stochastic/st_point_mass.py` & `ross-rotordynamics-1.4.1/ross/stochastic/st_point_mass.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/stochastic/st_results.py` & `ross-rotordynamics-1.4.1/ross/stochastic/st_results.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/stochastic/st_results_elements.py` & `ross-rotordynamics-1.4.1/ross/stochastic/st_results_elements.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/stochastic/st_rotor_assembly.py` & `ross-rotordynamics-1.4.1/ross/stochastic/st_rotor_assembly.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/stochastic/st_shaft_element.py` & `ross-rotordynamics-1.4.1/ross/stochastic/st_shaft_element.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/units.py` & `ross-rotordynamics-1.4.1/ross/units.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.4.0/ross/utils.py` & `ross-rotordynamics-1.4.1/ross/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,15 @@
 
     Examples
     --------
     >>> import ross as rs
     >>> rotor = rs.rotor_example()
 
     Visualizing Mass Matrix:
-    >>> fig = rs.visualize_matrix(rotor, "M")
+    >>> fig = rs.visualize_matrix(rotor, "M", frequency=100)
 
     Visualizing Stiffness Matrix:
     >>> fig = rs.visualize_matrix(rotor, "K", frequency=100)
 
     Visualizing Gyroscopic Matrix:
     >>> fig = rs.visualize_matrix(rotor, "G")
     """
```

### Comparing `ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/SOURCES.txt` & `ross-rotordynamics-1.4.1/ross_rotordynamics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ross/bearing_seal_element.py
 ross/disk_element.py
 ross/element.py
 ross/materials.py
 ross/new_units.txt
 ross/plotly_theme.py
 ross/point_mass.py
+ross/probe.py
 ross/results.py
 ross/rotor_assembly.py
 ross/shaft_element.py
 ross/units.py
 ross/utils.py
 ross/defects/__init__.py
 ross/defects/abs_defect.py
```

### Comparing `ross-rotordynamics-1.4.0/setup.py` & `ross-rotordynamics-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
 
 
 # Package meta-data.
 NAME = "ross-rotordynamics"
 DESCRIPTION = "ROSS: Rotordynamic Open Source Software"
-URL = "https://github.com/ross-rotordynamics/ross"
-EMAIL = "raphaelts@gmail.com"
+EMAIL = "raphaelts@petrobras.com.br"
 AUTHOR = "ROSS developers"
 REQUIRES_PYTHON = ">=3.7.0"
 VERSION = version("ross/__init__.py")
 
 # What packages are required for this module to be executed?
 with open("requirements.txt") as f:
     REQUIRED = f.read().splitlines()
@@ -82,15 +81,20 @@
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
-    url=URL,
+    project_urls={
+        "Documentation": "https://ross.readthedocs.io/en/stable/",
+        "Bug Tracker": "https://github.com/petrobras/ross/issues",
+        "Discussions": "https://github.com/petrobras/ross/discussions",
+        "Source Code": "https://github.com/petrobras/ross",
+    },
     packages=find_packages(exclude=("tests",)),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
```

