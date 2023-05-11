# Comparing `tmp/lincs-0.2.2.tar.gz` & `tmp/lincs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.2.2.tar", last modified: Sun May  7 07:36:57 2023, max compression
+gzip compressed data, was "lincs-0.3.0.tar", last modified: Thu May 11 17:39:46 2023, max compression
```

## Comparing `lincs-0.2.2.tar` & `lincs-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 user       (501) user      (1000)        0 2023-05-07 07:36:57.263995 lincs-0.2.2/
--rw-r--r--   0 user       (501) user      (1000)       58 2023-05-04 08:59:02.000000 lincs-0.2.2/MANIFEST.in
--rw-r--r--   0 user       (501) user      (1000)    10602 2023-05-07 07:36:57.258234 lincs-0.2.2/PKG-INFO
--rw-r--r--   0 user       (501) user      (1000)     9715 2023-05-07 07:29:05.000000 lincs-0.2.2/README.md
-drwxr-xr-x   0 user       (501) user      (1000)        0 2023-05-07 07:36:57.102837 lincs-0.2.2/lincs/
--rw-r--r--   0 user       (501) user      (1000)      343 2023-05-05 13:09:35.000000 lincs-0.2.2/lincs/__init__.py
--rw-r--r--   0 user       (501) user      (1000)      136 2023-05-04 08:59:02.000000 lincs-0.2.2/lincs/__main__.py
--rw-r--r--   0 user       (501) user      (1000)    19010 2023-05-07 07:24:16.000000 lincs-0.2.2/lincs/command_line_interface.py
-drwxr-xr-x   0 user       (501) user      (1000)        0 2023-05-07 07:36:57.244083 lincs-0.2.2/lincs/liblincs/
--rw-r--r--   0 user       (501) user      (1000)    10693 2023-05-07 07:22:28.000000 lincs-0.2.2/lincs/liblincs/liblincs_module.cpp
--rw-r--r--   0 user       (501) user      (1000)    17260 2023-05-07 07:31:56.000000 lincs-0.2.2/lincs/liblincs/lincs.cpp
--rw-r--r--   0 user       (501) user      (1000)     5040 2023-05-07 07:22:20.000000 lincs-0.2.2/lincs/liblincs/lincs.hpp
--rw-r--r--   0 user       (501) user      (1000)      718 2023-05-05 13:51:37.000000 lincs-0.2.2/lincs/visualization.py
-drwxr-xr-x   0 user       (501) user      (1000)        0 2023-05-07 07:36:57.197053 lincs-0.2.2/lincs.egg-info/
--rw-r--r--   0 user       (501) user      (1000)    10602 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) user      (1000)      399 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) user      (1000)        1 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) user      (1000)       60 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) user      (1000)       27 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/requires.txt
--rw-r--r--   0 user       (501) user      (1000)       15 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/top_level.txt
--rw-r--r--   0 user       (501) user      (1000)       27 2023-05-05 13:01:57.000000 lincs-0.2.2/requirements.txt
--rw-r--r--   0 user       (501) user      (1000)       38 2023-05-07 07:36:57.266651 lincs-0.2.2/setup.cfg
--rw-r--r--   0 user       (501) user      (1000)     1720 2023-05-07 07:34:57.000000 lincs-0.2.2/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-11 17:39:46.074369 lincs-0.3.0/
+-rw-r--r--   0 user      (1002) user      (1002)      102 2023-05-11 16:35:31.000000 lincs-0.3.0/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)    16795 2023-05-11 17:39:46.074369 lincs-0.3.0/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)    16088 2023-05-11 17:35:39.000000 lincs-0.3.0/README.md
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-11 17:39:46.070369 lincs-0.3.0/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      762 2023-05-11 16:48:08.000000 lincs-0.3.0/lincs/__init__.py
+-rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.3.0/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    21943 2023-05-11 17:15:21.000000 lincs-0.3.0/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-11 17:39:46.074369 lincs-0.3.0/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1566 2023-05-09 14:37:35.000000 lincs-0.3.0/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     9942 2023-05-08 05:22:27.000000 lincs-0.3.0/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6492 2023-05-11 13:04:24.000000 lincs-0.3.0/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)    26434 2023-05-11 17:02:54.000000 lincs-0.3.0/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)    15089 2023-05-11 16:48:00.000000 lincs-0.3.0/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)    11471 2023-05-11 17:01:21.000000 lincs-0.3.0/lincs/liblincs/lincs.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2928 2023-05-11 13:04:24.000000 lincs-0.3.0/lincs/liblincs/median-and-max.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      741 2023-05-11 13:04:24.000000 lincs-0.3.0/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1391 2023-05-11 13:04:24.000000 lincs-0.3.0/lincs/liblincs/randomness-utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10384 2023-05-11 16:48:16.000000 lincs-0.3.0/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)      759 2023-05-11 17:16:10.000000 lincs-0.3.0/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-11 17:39:46.070369 lincs-0.3.0/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)    16795 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)      625 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/top_level.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:01:57.000000 lincs-0.3.0/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-11 17:39:46.074369 lincs-0.3.0/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     2439 2023-05-11 17:38:48.000000 lincs-0.3.0/setup.py
```

### Comparing `lincs-0.2.2/lincs/command_line_interface.py` & `lincs-0.3.0/lincs/command_line_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+import math
 import random
 import subprocess
 import sys
 
 import click
 
 import lincs
@@ -81,16 +82,16 @@
     def walk(prefix, command):
         if command.hidden:
             return
 
         title = f"lincs {' '.join(prefix)}".rstrip()
         print(title)
         print("=" * len(title))
-        print(flush=True)
-        subprocess.run(["lincs"] + prefix + ["--help"], check=True)
+        print()
+        print(command.get_help(ctx=click.Context(info_name=" ".join(["lincs"] + prefix), command=command)))
         print()
 
         if isinstance(command, click.Group):
             for name, command in command.commands.items():
                 walk(prefix + [name], command)
 
     walk([], main)
@@ -104,15 +105,15 @@
         print("=" * len(f"lincs.{obj_name}"))
         print()
         if obj.__doc__:
             print(obj.__doc__)
             print()
         if isinstance(obj, type):
             for attr_name in sorted(dir(obj)):
-                if attr_name.startswith("_"):
+                if attr_name.startswith("_"):  # @todo Include __init__ and some other dunders
                     continue
                 if (
                     obj_name in {"CategoryCorrelation", "SufficientCoalitionsKind", "ValueType"}
                     and
                     attr_name in {"as_integer_ratio", "bit_count", "bit_length", "conjugate", "denominator", "from_bytes", "imag", "numerator", "to_bytes", "attr_name", "name", "names", "values"}
                 ):
                     continue
@@ -296,112 +297,103 @@
         alternatives_count,
         random_seed=random_seed,
         max_imbalance=max_imbalance,
     )
     alternatives.dump(output_classified_alternatives)
 
 
-@main.group()
+@main.group(
+    help="Make graphs from data.",
+)
 def visualize():
     pass
 
 
-@visualize.command()
+@visualize.command(
+    help="""
+        Visualize a classification model.
+
+        DOMAIN is a *classification domain* file.
+        MODEL is a *classification model* file for that domain describing the model to visualize.
+        The generated image is written to the OUTPUT file in PNG format.
+    """,
+)
 @click.argument(
     "domain",
     type=click.File(mode="r"),
 )
 @click.argument(
     "model",
     type=click.File(mode="r"),
 )
 @click.option(
     "--alternatives",
     type=click.File(mode="r"),
+    help="Add the alternatives from this *classified alternatives* file to the visualization.",
+)
+@click.option(
+    "--alternatives-count",
+    type=int,
+    help="Add only this number of alternatives.",
 )
 @click.argument(
     "output",
     type=click.File(mode="wb"),
 )
-def model(
+def classification_model(
     domain,
     model,
     alternatives,
+    alternatives_count,
     output,
 ):
     domain = lincs.load_domain(domain)
     model = lincs.load_model(domain, model)
     if alternatives is not None:
         alternatives = lincs.load_alternatives(domain, alternatives)
-    lincs.visualization.visualize_model(domain, model, alternatives, output)
+    lincs.visualization.visualize_model(domain, model, alternatives, alternatives_count, output)
 
 
 @main.group(
     help="Learn a model.",
-    hidden=True,
 )
 def learn():
     pass
 
 
 @learn.command(
     help="""
         Learn a classification model.
 
         DOMAIN is a *classification domain* file describing the domain to learn a model for.
         LEARNING_SET is a *classified alternatives* file for that domain.
         It's used as a source of truth to learn the model.
-
-        The learned *classification model* file is written to OUTPUT_MODEL, which defaults to - to write to the standard output.
     """,
 )
 @click.argument(
     "domain",
     type=click.File(mode="r"),
 )
 @click.argument(
     "learning-set",
     type=click.File(mode="r"),
 )
 @click.option(
-    "--target-accuracy",
-    help="The target accuracy to reach on the learning set.\n\n*",
-    type=click.FloatRange(min=0.0, max=1.0),
-    default=1.0,
-    show_default=True,
-)
-@click.option(
-    "--max-duration-seconds",
-    help="The maximum duration of the learning process in seconds.\n\n*",
-    type=click.FloatRange(min=0),
-    default=None,
-    show_default=True,
-)
-@click.argument(
-    "output-model",
+    "--output-model",
     type=click.File(mode="w"),
     default="-",
-)
-@click.option(
-    "--random-seed",
-    help="""
-        The random seed to use.
-
-        Some learning strategies are deterministic, pseudo-random processes.
-        This seed is used to initialize the pseudo-random number generator used by these strategies.
-
-        *
-    """,
-    type=click.IntRange(min=0),
+    help="Write the learned classification model to this file instead of standard output.",
 )
 @options_tree(
     "model-type",
     dict(
         help="The type of classification model to learn.",
         type=click.Choice(["mrsort"]),
+        default="mrsort",
+        show_default=True,
     ),
     {
         "ucncs": [],
         "mrsort": [
             (
                 "strategy",
                 dict(
@@ -409,14 +401,24 @@
                     type=click.Choice(["weights-profiles-breed"]),
                     default="weights-profiles-breed",
                     show_default=True,
                 ),
                 {
                     "weights-profiles-breed": [
                         (
+                            "target-accuracy",
+                            dict(
+                                help="The target accuracy to reach on the learning set.",
+                                type=click.FloatRange(min=0.0, max=1.0),
+                                default=1.0,
+                                show_default=True,
+                            ),
+                            {},
+                        ),
+                        (
                             "max-iterations",
                             dict(
                                 help="The maximum number of iterations to use to learn the MRSort model.",
                                 type=click.IntRange(min=1),
                                 default=None,
                                 show_default=True,
                             ),
@@ -472,18 +474,27 @@
                                 type=click.Choice(["accuracy-heuristic"]),
                                 default="accuracy-heuristic",
                                 show_default=True,
                             ),
                             {
                                 "accuracy-heuristic": [
                                     (
+                                        "random-seed",
+                                        dict(
+                                            help="The random seed to use for this heuristic.",
+                                            type=click.IntRange(min=0),
+                                            default=random.randrange(2**30),
+                                        ),
+                                        {},
+                                    ),
+                                    (
                                         "processor",
                                         dict(
                                             help="The processor to use to improve the profiles of the MRSort models.",
-                                            type=click.Choice(["cpu", "gpu"]),
+                                            type=click.Choice(["cpu"]),
                                             default="cpu",
                                             show_default=True,
                                         ),
                                         {},
                                     ),
                                 ],
                             },
@@ -516,30 +527,63 @@
             ),
         ],
     },
 )
 def classification_model(
     domain,
     learning_set,
-    target_accuracy,
-    max_duration_seconds,
     output_model,
     model_type,
     mrsort__strategy,
+    mrsort__weights_profiles_breed__target_accuracy,
     mrsort__weights_profiles_breed__max_iterations,
     mrsort__weights_profiles_breed__models_count,
     mrsort__weights_profiles_breed__initialization_strategy,
     mrsort__weights_profiles_breed__weights_strategy,
     mrsort__weights_profiles_breed__linear_program__solver,
     mrsort__weights_profiles_breed__profiles_strategy,
+    mrsort__weights_profiles_breed__accuracy_heuristic__random_seed,
     mrsort__weights_profiles_breed__accuracy_heuristic__processor,
     mrsort__weights_profiles_breed__breed_strategy,
     mrsort__weights_profiles_breed__reinitialize_least_accurate__portion,
 ):
-    pass
+    domain = lincs.load_domain(domain)
+    learning_set = lincs.load_alternatives(domain, learning_set)
+
+    if model_type == "mrsort":
+        if mrsort__strategy == "weights-profiles-breed":
+            models = lincs.make_models(domain, learning_set, mrsort__weights_profiles_breed__models_count, mrsort__weights_profiles_breed__accuracy_heuristic__random_seed)
+
+            assert mrsort__weights_profiles_breed__max_iterations is None
+            termination_strategy = lincs.TerminateAtAccuracy(math.ceil(mrsort__weights_profiles_breed__target_accuracy * len(learning_set.alternatives)))
+
+            if mrsort__weights_profiles_breed__initialization_strategy == "maximize-discrimination-per-criterion":
+                profiles_initialization_strategy = lincs.InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(models)
+
+            if mrsort__weights_profiles_breed__weights_strategy == "linear-program":
+                if mrsort__weights_profiles_breed__linear_program__solver == "glop":
+                    weights_optimization_strategy = lincs.OptimizeWeightsUsingGlop(models)
+
+            if mrsort__weights_profiles_breed__profiles_strategy == "accuracy-heuristic":
+                if mrsort__weights_profiles_breed__accuracy_heuristic__processor == "cpu":
+                    profiles_improvement_strategy = lincs.ImproveProfilesWithAccuracyHeuristic(models)
+
+            assert mrsort__weights_profiles_breed__breed_strategy == "reinitialize-least-accurate"
+            assert mrsort__weights_profiles_breed__reinitialize_least_accurate__portion == 0.5
+
+            learning = lincs.WeightsProfilesBreedMrSortLearning(
+                models,
+                profiles_initialization_strategy,
+                weights_optimization_strategy,
+                profiles_improvement_strategy,
+                termination_strategy,
+            )
+
+    model = learning.perform()
+    model.dump(output_model)
 
 
 @main.command(
     help="""
         Classify alternatives.
 
         DOMAIN is a *classification domain* file.
```

### Comparing `lincs-0.2.2/lincs/visualization.py` & `lincs-0.3.0/lincs/visualization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import matplotlib.pyplot as plt
 
 
-def visualize_model(domain, model, alternatives, out):
+def visualize_model(domain, model, alternatives, alternatives_count, out):
     fig, ax = plt.subplots(1, 1, figsize=(6, 4), layout="constrained")
 
     xs = [criterion.name for criterion in domain.criteria]
     for boundary_index, boundary in enumerate(model.boundaries):
         label = f"{domain.categories[boundary_index].name} and {domain.categories[boundary_index + 1].name}"
         ax.plot(xs, list(boundary.profile), "o-", label=label)
 
     if alternatives:
-        for alternative in alternatives.alternatives:
+        for alternative in alternatives.alternatives[:alternatives_count]:
             ax.plot(xs, list(alternative.profile), "o--", label=alternative.name)
 
     ax.legend()
     ax.set_ylim(0, 1)
 
     fig.savefig(out, format="png", dpi=100)
     plt.close(fig)
```

### Comparing `lincs-0.2.2/setup.py` & `lincs-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 import setuptools
 
 
-version = "0.2.2"
+version = "0.3.0"
 
 with open("README.md") as f:
     long_description = f.read()
 for image in ["model", "alternatives"]:
-    long_description = long_description.replace(f"{image}.png", f"https://github.com/jacquev6/lincs/raw/v{version}/{image}.png")
+    long_description = long_description.replace(f"]({image}.png)", f"](https://github.com/jacquev6/lincs/raw/v{version}/{image}.png)")
 
 with open("requirements.txt") as f:
     install_requires = f.readlines()
 
 
+# @todo Consider using scikit-build:
+# it should make it easier to compile CUDA code using nvcc and to run C++ unit tests during build.
+# Note that pybind11 comes with an example of building using scikit-build.
+# (see also https://www.benjack.io/hybrid-python/c-packages-revisited/)
 liblincs = setuptools.Extension(
     "liblincs",
     sources=[
         "lincs/liblincs/liblincs_module.cpp",
-        "lincs/liblincs/lincs.cpp",
+        "lincs/liblincs/classification.cpp",
+        "lincs/liblincs/generation.cpp",
+        "lincs/liblincs/io.cpp",
+        "lincs/liblincs/learning.cpp",
+        "lincs/liblincs/median-and-max.cpp",
+        "lincs/liblincs/randomness-utils.cpp",
     ],
     libraries=[
         "boost_python310",
+        "ortools",
         "python3.10",  # Make the Python module usable as a C++ shared library without -lpython3.10 (still linked, but implicitly)
         "yaml-cpp",
     ],
+    define_macros=[("DOCTEST_CONFIG_DISABLE", None)],
+    include_dirs=["/usr/local/cuda-12.1/targets/x86_64-linux/include"],
+    extra_compile_args=["-fopenmp"],
+    extra_link_args=["-fopenmp"],
 )
 
 setuptools.setup(
     name="lincs",
     version=version,
     description="MCDA algorithms",
     long_description=long_description,
```

