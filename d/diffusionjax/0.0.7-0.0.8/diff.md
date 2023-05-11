# Comparing `tmp/diffusionjax-0.0.7.tar.gz` & `tmp/diffusionjax-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusionjax-0.0.7.tar", last modified: Sat Apr 22 09:36:12 2023, max compression
+gzip compressed data, was "diffusionjax-0.0.8.tar", last modified: Wed May 10 10:25:27 2023, max compression
```

## Comparing `diffusionjax-0.0.7.tar` & `diffusionjax-0.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.868917 diffusionjax-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/diffusionjax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/inverse_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/diffusionjax/test/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/diffusionjax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/examples/example1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/examples/example2.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    52645 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_empirical_score.png
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_heatmap_bounded_perturbation.png
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_heatmap_empirical_score.png
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_heatmap_inpainted.png
--rw-r--r--   0 runner    (1001) docker     (123)    28810 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_heatmap_trained_score.png
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_samples.png
--rw-r--r--   0 runner    (1001) docker     (123)    55853 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_trained_score.png
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.663787 diffusionjax-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.643787 diffusionjax-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.655787 diffusionjax-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-10 10:25:27.663787 diffusionjax-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.659787 diffusionjax-0.0.8/diffusionjax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 10:25:27.000000 diffusionjax-0.0.8/diffusionjax/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/inverse_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.659787 diffusionjax-0.0.8/diffusionjax/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/diffusionjax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.659787 diffusionjax-0.0.8/diffusionjax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-10 10:25:27.000000 diffusionjax-0.0.8/diffusionjax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-10 10:25:27.000000 diffusionjax-0.0.8/diffusionjax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:25:27.000000 diffusionjax-0.0.8/diffusionjax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 10:25:27.000000 diffusionjax-0.0.8/diffusionjax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 10:25:27.000000 diffusionjax-0.0.8/diffusionjax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.663787 diffusionjax-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    52645 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/readme_empirical_score.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/readme_heatmap_bounded_perturbation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/readme_heatmap_empirical_score.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/readme_heatmap_inpainted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/readme_heatmap_trained_score.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/readme_samples.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55867 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/readme_trained_score.png
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 10:25:27.663787 diffusionjax-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-10 10:25:05.000000 diffusionjax-0.0.8/setup.py
```

### Comparing `diffusionjax-0.0.7/.github/workflows/CI.yml` & `diffusionjax-0.0.8/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/.github/workflows/publish.yml` & `diffusionjax-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/.gitignore` & `diffusionjax-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/LICENSE.rst` & `diffusionjax-0.0.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/PKG-INFO` & `diffusionjax-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: diffusionjax
-Version: 0.0.7
-Summary: diffusionjax is a simple and accessible diffusion models package in JAX
-Home-page: https://github.com/bb515/diffusionjax
-Author: Jakiw Pidstrigach and Benjamin Boys
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 diffusionjax
 ============
 [![CI](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml/badge.svg)](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml)
 [![Coverage Status](https://coveralls.io/repos/github/bb515/diffusionjax/badge.svg?branch=master)](https://coveralls.io/github/bb515/diffusionjax?branch=master)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 diffusionjax is a simple, accessible introduction to diffusion models, also known as score-based generative models (SGMs). It is implemented in Python via the autodiff framework, [JAX](https://github.com/google/jax). In particular, diffusionjax uses the [Flax](https://github.com/google/flax) library for the neural network approximator of the score.
@@ -37,20 +27,19 @@
 
 ## Examples
 
 ### Introduction to diffusion models
 - Run the example by typing `python examples/example.py` on the command line from the root directory of the repository.
 ```python
 >>> num_epochs = 4000
->>> rng = random.PRNGKey(2023)
->>> rng, step_rng = random.split(rng, 2)
 >>> num_samples = 8
 >>> samples = sample_circle(num_samples)
 >>> N = samples.shape[1]
 >>> plot_samples(samples=samples, index=(0, 1), fname="samples", lims=((-3, 3), (-3, 3)))
+>>> rng = random.PRNGKey(2023)
 ```
 ![Prediction](readme_samples.png)
 ```python
 >>> # Get variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU) sde model
 >>> sde = VP()
 >>>
 >>> def log_hat_pt(x, t):
@@ -73,26 +62,29 @@
 >>> nabla_log_hat_pt = jit(vmap(grad(log_hat_pt), in_axes=(0, 0), out_axes=(0)))
 >>>
 >>> # Running the reverse SDE with the empirical drift
 >>> plot_score(score=nabla_log_hat_pt, t=0.01, area_min=-3, area_max=3, fname="empirical score")
 ```
 ![Prediction](readme_empirical_score.png)
 ```python
->>> sampler = get_sampler(EulerMaruyama(sde.reverse(nabla_log_hat_pt)))
->>> q_samples = sampler(rng, n_samples=5000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap empirical score")
+>>> sampler = get_sampler((5760, N), EulerMaruyama(sde.reverse(nabla_log_hat_pt)))
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(5760, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap empirical score")
 ```
 ![Prediction](readme_heatmap_empirical_score.png)
 ```python
 >>> # What happens when I perturb the score with a constant?
 >>> perturbed_score = lambda x, t: nabla_log_hat_pt(x, t) + 1
->>> rng, step_rng = random.split(rng)
->>> sampler = get_sampler(EulerMaruyama(sde.reverse(perturbed_score)))
->>> q_samples = sampler(rng, n_samples=5000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap bounded perturbation")
+>>> sampler = get_sampler((5760, N), EulerMaruyama(sde.reverse(perturbed_score)))
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(5760, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap bounded perturbation")
 ```
 ![Prediction](readme_heatmap_bounded_perturbation.png)
 ```python
 >>> # Neural network training via score matching
 >>> batch_size=16
 >>> score_model = MLP()
 >>> # Initialize parameters
@@ -117,27 +109,31 @@
 >>> # Get trained score
 >>> trained_score = get_score(sde, score_model, params, score_scaling=True)
 >>> plot_score(score=trained_score, t=0.01, area_min=-3, area_max=3, fname="trained score")
 ```
 ![Prediction](readme_trained_score.png)
 ```python
 >>> solver = EulerMaruyama(sde.reverse(trained_score))
->>> sampler = get_sampler(solver, stack_samples=False)
->>> q_samples = sampler(rng, n_samples=1000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap trained score")
+>>> sampler = get_sampler((720, N), solver, stack_samples=False)
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(720, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap trained score")
 ```
 ![Prediction](readme_heatmap_trained_score.png)
 ```python
 >>> inpainter = get_inpainter(solver, stack_samples=False)
 >>> data = jnp.array([-0.5, 0.0])
 >>> mask = jnp.array([1, 0])
 >>> data = jnp.tile(data, (64, 1))
 >>> mask = jnp.tile(mask, (64, 1))
->>> q_samples = inpainter(rng, data, mask)
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap inpainted")
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = inpainter(jnp.array(sample_rng), data, mask)
+>>> q_samples = q_samples.reshape(64, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap inpainted")
 ```
 ![Prediction](readme_heatmap_inpainted.png)
 
 ## Does haves
 - Training scores on (possibly, image) data and sampling from the generative model. Also inverse problems, such as inpainting.
 - Not many lines of code.
 - Easy to use, extendable. Get started with the example, provided.
```

### Comparing `diffusionjax-0.0.7/README.md` & `diffusionjax-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: diffusionjax
+Version: 0.0.8
+Summary: diffusionjax is a simple and accessible diffusion models package in JAX
+Home-page: https://github.com/bb515/diffusionjax
+Author: Jakiw Pidstrigach and Benjamin Boys
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 diffusionjax
 ============
 [![CI](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml/badge.svg)](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml)
 [![Coverage Status](https://coveralls.io/repos/github/bb515/diffusionjax/badge.svg?branch=master)](https://coveralls.io/github/bb515/diffusionjax?branch=master)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 diffusionjax is a simple, accessible introduction to diffusion models, also known as score-based generative models (SGMs). It is implemented in Python via the autodiff framework, [JAX](https://github.com/google/jax). In particular, diffusionjax uses the [Flax](https://github.com/google/flax) library for the neural network approximator of the score.
@@ -27,20 +37,19 @@
 
 ## Examples
 
 ### Introduction to diffusion models
 - Run the example by typing `python examples/example.py` on the command line from the root directory of the repository.
 ```python
 >>> num_epochs = 4000
->>> rng = random.PRNGKey(2023)
->>> rng, step_rng = random.split(rng, 2)
 >>> num_samples = 8
 >>> samples = sample_circle(num_samples)
 >>> N = samples.shape[1]
 >>> plot_samples(samples=samples, index=(0, 1), fname="samples", lims=((-3, 3), (-3, 3)))
+>>> rng = random.PRNGKey(2023)
 ```
 ![Prediction](readme_samples.png)
 ```python
 >>> # Get variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU) sde model
 >>> sde = VP()
 >>>
 >>> def log_hat_pt(x, t):
@@ -63,26 +72,29 @@
 >>> nabla_log_hat_pt = jit(vmap(grad(log_hat_pt), in_axes=(0, 0), out_axes=(0)))
 >>>
 >>> # Running the reverse SDE with the empirical drift
 >>> plot_score(score=nabla_log_hat_pt, t=0.01, area_min=-3, area_max=3, fname="empirical score")
 ```
 ![Prediction](readme_empirical_score.png)
 ```python
->>> sampler = get_sampler(EulerMaruyama(sde.reverse(nabla_log_hat_pt)))
->>> q_samples = sampler(rng, n_samples=5000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap empirical score")
+>>> sampler = get_sampler((5760, N), EulerMaruyama(sde.reverse(nabla_log_hat_pt)))
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(5760, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap empirical score")
 ```
 ![Prediction](readme_heatmap_empirical_score.png)
 ```python
 >>> # What happens when I perturb the score with a constant?
 >>> perturbed_score = lambda x, t: nabla_log_hat_pt(x, t) + 1
->>> rng, step_rng = random.split(rng)
->>> sampler = get_sampler(EulerMaruyama(sde.reverse(perturbed_score)))
->>> q_samples = sampler(rng, n_samples=5000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap bounded perturbation")
+>>> sampler = get_sampler((5760, N), EulerMaruyama(sde.reverse(perturbed_score)))
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(5760, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap bounded perturbation")
 ```
 ![Prediction](readme_heatmap_bounded_perturbation.png)
 ```python
 >>> # Neural network training via score matching
 >>> batch_size=16
 >>> score_model = MLP()
 >>> # Initialize parameters
@@ -107,27 +119,31 @@
 >>> # Get trained score
 >>> trained_score = get_score(sde, score_model, params, score_scaling=True)
 >>> plot_score(score=trained_score, t=0.01, area_min=-3, area_max=3, fname="trained score")
 ```
 ![Prediction](readme_trained_score.png)
 ```python
 >>> solver = EulerMaruyama(sde.reverse(trained_score))
->>> sampler = get_sampler(solver, stack_samples=False)
->>> q_samples = sampler(rng, n_samples=1000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap trained score")
+>>> sampler = get_sampler((720, N), solver, stack_samples=False)
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(720, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap trained score")
 ```
 ![Prediction](readme_heatmap_trained_score.png)
 ```python
 >>> inpainter = get_inpainter(solver, stack_samples=False)
 >>> data = jnp.array([-0.5, 0.0])
 >>> mask = jnp.array([1, 0])
 >>> data = jnp.tile(data, (64, 1))
 >>> mask = jnp.tile(mask, (64, 1))
->>> q_samples = inpainter(rng, data, mask)
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap inpainted")
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = inpainter(jnp.array(sample_rng), data, mask)
+>>> q_samples = q_samples.reshape(64, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap inpainted")
 ```
 ![Prediction](readme_heatmap_inpainted.png)
 
 ## Does haves
 - Training scores on (possibly, image) data and sampling from the generative model. Also inverse problems, such as inpainting.
 - Not many lines of code.
 - Easy to use, extendable. Get started with the example, provided.
```

### Comparing `diffusionjax-0.0.7/diffusionjax/inverse_problems.py` & `diffusionjax-0.0.8/diffusionjax/inverse_problems.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Inverse problems."""
+import jax
 import jax.numpy as jnp
 from jax.lax import scan
 import jax.random as random
 from diffusionjax.utils import batch_mul
 from jax.experimental.host_callback import id_print
 import numpy as np
 
@@ -15,15 +16,15 @@
     """Create an image inpainting function that uses sampler, that returns only the final sample.
 
     Args:
         inverse_scaler: The inverse data normalizer.
         denoise: Boolean variable that if `True` applies one-step denoising to final samples.
         stack_samples: Boolean variable that if `True` returns all samples on path(s).
     Returns:
-        A pmapped inpainting function.
+        A pmapped projection sampler function.
     """
     def update(rng, data, mask, x, vec_t, coeff):
         data_mean, std = solver.sde.marginal_prob(data, vec_t)
         z = random.normal(rng, x.shape)
         z_data = data_mean + batch_mul(std, z)
         x = merge_data_with_mask(x, z_data, mask, coeff)
 
@@ -48,29 +49,29 @@
         # Initial sample
         rng, step_rng = random.split(rng)
         shape = data.shape
         x = random.normal(step_rng, shape)
 
         def f(carry, t):
             rng, x, x_mean = carry
-            vec_t = jnp.ones((shape[0], 1)) * (1. - t)
+            vec_t = jnp.full(shape[0], t)
             rng, step_rng = random.split(rng)
             x, x_mean = update(step_rng, data, mask, x, vec_t, coeff)
             if not stack_samples:
                 return (rng, x, x_mean), ()
             else:
                 return (rng, x, x_mean), x
         if not stack_samples:
-            (_, x, _), _ = scan(f, (rng, x, x), ts)
+            (_, x, _), _ = scan(f, (rng, x, x), ts, reverse=True)
             return x
         else:
-            (_, _, _), xs = scan(f, (rng, x, x), ts)
+            (_, _, _), xs = scan(f, (rng, x, x), ts, reverse=True)
             return xs
 
-    return projection_sampler  # TODO: pmap axis_name="batch"
+    return jax.pmap(projection_sampler, in_axes=(0, None, None, None), axis_name='batch')
 
 
 def get_inpainter(solver, inverse_scaler=None,
                 denoise=True, stack_samples=False):
     """Create an image inpainting function that uses sampler, that returns only the final sample.
 
     Args:
@@ -105,21 +106,21 @@
         # Initial sample
         rng, step_rng = random.split(rng)
         shape = data.shape
         x = data * mask + random.normal(step_rng, shape) * (1. - mask)
 
         def f(carry, t):
             rng, x, x_mean = carry
-            vec_t = jnp.ones((shape[0], 1)) * (1. - t)
+            vec_t = jnp.full(shape[0], t)
             rng, step_rng = random.split(rng)
             x, x_mean = update(rng, data, mask, x, vec_t)
             if not stack_samples:
                 return (rng, x, x_mean), ()
             else:
                 return (rng, x, x_mean), x
         if not stack_samples:
-            (_, x, _), _ = scan(f, (rng, x, x), ts)
+            (_, x, _), _ = scan(f, (rng, x, x), ts, reverse=True)
             return x
         else:
-            (_, _, _), xs = scan(f, (rng, x, x), ts)
+            (_, _, _), xs = scan(f, (rng, x, x), ts, reverse=True)
             return xs
-    return inpainter  # TODO: pmap axis_name="batch"
+    return jax.pmap(inpainter, in_axes=(0, None, None), axis_name='batch')
```

### Comparing `diffusionjax-0.0.7/diffusionjax/losses.py` & `diffusionjax-0.0.8/diffusionjax/losses.py`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/diffusionjax/models.py` & `diffusionjax-0.0.8/diffusionjax/models.py`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/diffusionjax/plot.py` & `diffusionjax-0.0.8/diffusionjax/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 def plot_temperature_schedule(sde, solver):
     """Plots the temperature schedule of the SDE marginals.
 
     Args:
         sde: a valid SDE class.
     """
-    m2 = sde.mean_coeff(solver.ts)
+    m2 = sde.mean_coeff(solver.ts)**2
     v = sde.variance(solver.ts)
     plt.plot(solver.ts, m2, label="m2")
     plt.plot(solver.ts, v, label="v")
     plt.legend()
     plt.savefig("plot_temperature_schedule.png")
     plt.close()
```

### Comparing `diffusionjax-0.0.7/diffusionjax/samplers.py` & `diffusionjax-0.0.8/diffusionjax/samplers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """Samplers."""
+import jax
 import jax.numpy as jnp
 from jax.lax import scan
 import jax.random as random
 import functools
 
 
 def shared_update(rng, x, t, solver, probability_flow=None):
     """A wrapper that configures and returns the update function of the solvers.
 
     :probablity_flow: Placeholder for probability flow ODE (TODO).
     """
     return solver.update(rng, x, t)
 
 
-def get_sampler(outer_solver, inner_solver=None, denoise=True, stack_samples=False):
+def get_sampler(shape, outer_solver, inner_solver=None, denoise=True, stack_samples=False):
     """Get a sampler from (possibly interleaved) numerical solver(s).
 
     Args:
+        shape: Shape of array, x. (num_samples,) + obj_shape, where x_shape is the shape
+            of the object being sampled from, for example, an image may have
+            obj_shape==(H, W, C), and so shape==(N, H, W, C) where N is the number of samples.
         outer_solver: A valid numerical solver class that will act on an outer loop.
         inner_solver: '' that will act on an inner loop.
         denoise: Boolean variable that if `True` applies one-step denoising to final samples.
         stack_samples: Boolean variable that if `True` return all of the sample path or
             just returns the last sample.
     Returns:
         A sampler.
     """
 
-    def sampler(rng, num_samples, shape, x_0=None):
+    def sampler(rng, x_0=None):
         """
 
         Args:
             rng: A JAX random state.
-            num_samples: Number of samples to return.
-            shape: Shape of array, x.
             x_0: Initial condition. If `None`, then samples an initial condition from the
                 sde's initial condition prior. Note that this initial condition represents
                 `x_T \sim \text{Normal}(O, I)` in reverse-time diffusion.
         Returns:
             Samples.
         """
         outer_update = functools.partial(shared_update,
@@ -52,80 +54,80 @@
                 rng, x, x_mean, vec_t = carry
                 rng, step_rng = random.split(rng)
                 x, x_mean = inner_update(step_rng, x, vec_t)
                 return (rng, x, x_mean, vec_t), ()
 
             def outer_step(carry, t):
                 rng, x, x_mean = carry
-                vec_t = jnp.ones((num_samples, 1)) * (1 - t)
+                vec_t = jnp.full(shape[0], t)
                 rng, step_rng = random.split(rng)
                 x, x_mean = outer_update(step_rng, x, vec_t)
                 (rng, x, x_mean, vec_t), _ = scan(inner_step, (step_rng, x, x_mean, vec_t), inner_ts)
                 if not stack_samples:
                     return (rng, x, x_mean), ()
                 else:
                     if denoise:
                         return (rng, x, x_mean), x_mean
                     else:
                         return (rng, x, x_mean), x
         else:
             def outer_step(carry, t):
                 rng, x, x_mean = carry
-                vec_t = jnp.ones((num_samples, 1)) * (1 - t)
+                vec_t = jnp.full(shape[0], t)
                 rng, step_rng = random.split(rng)
                 x, x_mean = outer_update(step_rng, x, vec_t)
                 if not stack_samples:
                     return (rng, x, x_mean), ()
                 else:
                     if denoise:
                         return (rng, x, x_mean), x_mean
                     else:
                         return (rng, x, x_mean), x
 
         rng, step_rng = random.split(rng)
-        num_samples_shape = (num_samples,) + shape
         if x_0 is None:
-            x = outer_solver.sde.prior(step_rng, num_samples_shape)
+            x = outer_solver.sde.prior(step_rng, shape)
         else:
-            assert(x_0.shape==num_samples_shape)
+            assert(x_0.shape==shape)
             x = x_0
         if not stack_samples:
-            (_, x, x_mean), _ = scan(outer_step, (rng, x, x), outer_ts)
+            (_, x, x_mean), _ = scan(outer_step, (rng, x, x), outer_ts, reverse=True)
             if denoise:
                 return x_mean
             else:
                 return x
         else:
-            (_, _, _), xs = scan(outer_step, (rng, x, x), outer_ts)
+            (_, _, _), xs = scan(outer_step, (rng, x, x), outer_ts, reverse=True)
             return xs
-    return sampler
+    return jax.pmap(sampler, in_axes=(0), axis_name='batch')
 
 
-def get_augmented_sampler(outer_solver, inner_solver=None, stack_samples=False):
+def get_augmented_sampler(shape, outer_solver, inner_solver=None, stack_samples=False):
     """Get a sampler, with augmented state-space (position and velocity), from (possibly interleaved) numerical solver(s).
 
     Args:
+        shape: Shape of array, x. (num_samples,) + obj_shape, where x_shape is the shape
+            of the object being sampled from, for example, an image may have
+            obj_shape = (H, W, C), and so shape = (N, H, W, C) where N is the number of samples.
         outer_solver: A valid numerical solver class that will act on an outer loop.
         inner_solver: "" "" that will act on an inner loop.
         stack_samples: Boolean variable that if `True` return all of the sample path or
             just returns the last sample.
     Returns:
         A sampler.
     """
     outer_update = functools.partial(shared_update,
                                     solver=outer_solver)
     outer_ts = outer_solver.ts
 
-    def sampler(rng, num_samples, shape, x_0=None, xd_0=None):
+    def sampler(rng, x_0=None, xd_0=None):
         """
 
         Args:
             rng: A JAX random state.
-            num_samples: Number of samples to return.
-            shape: Shape of array, x.
             x_0: Initial condition position. If `None`, then samples an initial condition from the
                 sde's initial condition prior. Note that this initial condition represents
                 `x_T \sim \text{Normal}(O, I)` in reverse-time diffusion.
             x_d0: Initial condition velocity. If `None`, then samples an initial condition from the
                 sde's initial condition prior. Note that this initial condition represents
                 `x_T \sim \text{Normal}(O, I)` in reverse-time diffusion.
         Returns:
@@ -140,43 +142,42 @@
                 rng, x, xd, vec_t = carry
                 rng, step_rng = random.split(rng)
                 x, xd, xd_mean = inner_update(step_rng, x, xd, vec_t)
                 return (rng, x, xd, vec_t), ()
 
             def outer_step(carry, t):
                 rng, x, xd, xd_mean = carry
-                vec_t = jnp.ones((num_samples, 1)) * (1 - t)
+                vec_t = jnp.full(shape[0], t)
                 rng, step_rng = random.split(rng)
                 x, xd = outer_update(step_rng, x, xd, vec_t)
                 (rng, x, xd, xd_mean), _ = scan(
                     inner_step, (step_rng, x, xd, vec_t), inner_ts)
                 if not stack_samples:
                     return (rng, x, xd), ()
                 else:
                     return (rng, x, xd), x
         else:
             def outer_step(carry, t):
                 rng, x, xd, xd_mean = carry
-                vec_t = jnp.ones((num_samples, 1)) * (1 - t)
+                vec_t = jnp.full(shape[0], t)
                 rng, step_rng = random.split(rng)
                 x, xd = outer_update(step_rng, x, xd, vec_t)
                 if not stack_samples:
                     return (rng, x, xd), ()
                 else:
                     return (rng, x, xd), x
 
         rng, step_rng = random.split(rng)
-        num_samples_shape = (num_samples,) + shape
         if x_0 is None:
-            x, xd = outer_solver.sde.prior(step_rng, num_samples_shape)
+            x, xd = outer_solver.sde.prior(step_rng, shape)
         else:
-            assert(x_0.shape==num_samples_shape)
-            assert(xd_0.shape==num_samples_shape)
+            assert(x_0.shape==shape)
+            assert(xd_0.shape==shape)
             x = x_0
             xd = xd_0
         if not stack_samples:
             (_, x, xd, _), _ = scan(outer_step, (rng, x, xd, xd), outer_ts)
             return x, xd
         else:
             (_, _, _, _), xs = scan(outer_step, (rng, x, xd, xd), outer_ts)
             return xs
-    return sampler
+    return jax.pmap(sampler, in_axes=(0), axis_name='batch')
```

### Comparing `diffusionjax-0.0.7/diffusionjax/sde.py` & `diffusionjax-0.0.8/diffusionjax/sde.py`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/diffusionjax/solvers.py` & `diffusionjax-0.0.8/diffusionjax/solvers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Solver classes."""
+import jax
 import jax.numpy as jnp
 from jax.lax import scan
 import jax.random as random
 from diffusionjax.utils import batch_mul
 import abc
 
 
@@ -15,19 +16,21 @@
             num_steps: number of discretization time steps.
             dt: time step duration, float or `None`.
                 Optional, if provided then final time, t1 = dt * num_steps.
         """
         self.num_steps = num_steps
         if dt is None:
             self.dt = 1. / self.num_steps
-            self.ts = jnp.linspace(0, 1, num_steps + 1)[:-1].reshape(-1, 1)
+            # Defined in forward time, t \in [\epsilon, 1.0], 0 < \epsilon << 1
+            self.ts = jnp.linspace(0, 1, num_steps + 1)[1:].reshape(-1, 1)
         else:
             self.dt = dt
             t1 = dt * num_steps
-            self.ts = jnp.linspace(0, t1, num_steps + 1)[:-1].reshape(-1, 1)
+            # Defined in forward time, t \in [\epsilon, t1], 0 < \epsilon << t1
+            self.ts = jnp.linspace(0, t1, num_steps + 1)[1:].reshape(-1, 1)
 
     @abc.abstractmethod
     def update(self, rng, x, t):
         r"""Return the drift and diffusion coefficients of the SDE.
 
         Args:
             rng: A JAX random state.
@@ -69,18 +72,19 @@
         noise = random.normal(rng, x.shape)
         x_mean = x + f
         x = x_mean + batch_mul(G, noise)
         return x, x_mean
 
 
 class Annealed(Solver):
-    """Annealed numerical solver of an SDE. Functions are designed for a mini-batch of inputs."""
+    """Annealed Langevin numerical solver of an SDE.
+    Functions are designed for a mini-batch of inputs."""
 
     def __init__(self, sde, num_steps=2, snr=1e-2):
-        """Constructs an Euler Maruyama sampler.
+        """Constructs an Annealed Langevin Solver.
         Args:
             sde: A valid SDE class.
         """
         super().__init__(num_steps)
         self.sde = sde
         self.snr = snr
 
@@ -91,24 +95,21 @@
             x: A JAX array representing the current state.
             t: A JAX array representing the current step.
 
         Returns:
             x: A JAX array of the next state:
             x_mean: A JAX array. The next state without random noise. Useful for denoising.
         """
-        grad, diffusion = self.sde.sde(x, t)
+        grad = self.sde.score(x, t)
         grad_norm = jnp.linalg.norm(
             grad.reshape((grad.shape[0], -1)), axis=-1).mean()
-        # TODO: implement parallel mean across batches
-        # grad_norm = jax.lax.pmean(grad_norm, axis_name='batch')
+        grad_norm = jax.lax.pmean(grad_norm, axis_name='batch')
         noise = random.normal(rng, x.shape)
         noise_norm = jnp.linalg.norm(
             noise.reshape((noise.shape[0], -1)), axis=-1).mean()
-        # noise_norm = jax.lax.pmean(noise_norm, axis_name='batch')
-        # TODO: alpha need not be a mini-batch
+        noise_norm = jax.lax.pmean(noise_norm, axis_name='batch')
+        # Note: alpha need not be a mini-batch
         alpha = jnp.exp(2 * self.sde.log_mean_coeff(t))
         dt = (self.snr * noise_norm / grad_norm)**2 * 2 * alpha
-        f = batch_mul(grad, dt)
-        G = batch_mul(diffusion, jnp.sqrt(dt))
-        x_mean = x + f
-        x = x_mean + batch_mul(G, noise)
+        x_mean = x + batch_mul(grad, dt)
+        x = x_mean + batch_mul(2 * dt, noise)
         return x, x_mean
```

### Comparing `diffusionjax-0.0.7/diffusionjax/utils.py` & `diffusionjax-0.0.8/diffusionjax/utils.py`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/diffusionjax.egg-info/PKG-INFO` & `diffusionjax-0.0.8/diffusionjax.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusionjax
-Version: 0.0.7
+Version: 0.0.8
 Summary: diffusionjax is a simple and accessible diffusion models package in JAX
 Home-page: https://github.com/bb515/diffusionjax
 Author: Jakiw Pidstrigach and Benjamin Boys
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -37,20 +37,19 @@
 
 ## Examples
 
 ### Introduction to diffusion models
 - Run the example by typing `python examples/example.py` on the command line from the root directory of the repository.
 ```python
 >>> num_epochs = 4000
->>> rng = random.PRNGKey(2023)
->>> rng, step_rng = random.split(rng, 2)
 >>> num_samples = 8
 >>> samples = sample_circle(num_samples)
 >>> N = samples.shape[1]
 >>> plot_samples(samples=samples, index=(0, 1), fname="samples", lims=((-3, 3), (-3, 3)))
+>>> rng = random.PRNGKey(2023)
 ```
 ![Prediction](readme_samples.png)
 ```python
 >>> # Get variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU) sde model
 >>> sde = VP()
 >>>
 >>> def log_hat_pt(x, t):
@@ -73,26 +72,29 @@
 >>> nabla_log_hat_pt = jit(vmap(grad(log_hat_pt), in_axes=(0, 0), out_axes=(0)))
 >>>
 >>> # Running the reverse SDE with the empirical drift
 >>> plot_score(score=nabla_log_hat_pt, t=0.01, area_min=-3, area_max=3, fname="empirical score")
 ```
 ![Prediction](readme_empirical_score.png)
 ```python
->>> sampler = get_sampler(EulerMaruyama(sde.reverse(nabla_log_hat_pt)))
->>> q_samples = sampler(rng, n_samples=5000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap empirical score")
+>>> sampler = get_sampler((5760, N), EulerMaruyama(sde.reverse(nabla_log_hat_pt)))
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(5760, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap empirical score")
 ```
 ![Prediction](readme_heatmap_empirical_score.png)
 ```python
 >>> # What happens when I perturb the score with a constant?
 >>> perturbed_score = lambda x, t: nabla_log_hat_pt(x, t) + 1
->>> rng, step_rng = random.split(rng)
->>> sampler = get_sampler(EulerMaruyama(sde.reverse(perturbed_score)))
->>> q_samples = sampler(rng, n_samples=5000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap bounded perturbation")
+>>> sampler = get_sampler((5760, N), EulerMaruyama(sde.reverse(perturbed_score)))
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(5760, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap bounded perturbation")
 ```
 ![Prediction](readme_heatmap_bounded_perturbation.png)
 ```python
 >>> # Neural network training via score matching
 >>> batch_size=16
 >>> score_model = MLP()
 >>> # Initialize parameters
@@ -117,27 +119,31 @@
 >>> # Get trained score
 >>> trained_score = get_score(sde, score_model, params, score_scaling=True)
 >>> plot_score(score=trained_score, t=0.01, area_min=-3, area_max=3, fname="trained score")
 ```
 ![Prediction](readme_trained_score.png)
 ```python
 >>> solver = EulerMaruyama(sde.reverse(trained_score))
->>> sampler = get_sampler(solver, stack_samples=False)
->>> q_samples = sampler(rng, n_samples=1000, shape=(N,))
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap trained score")
+>>> sampler = get_sampler((720, N), solver, stack_samples=False)
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = sampler(jnp.array(sample_rng))
+>>> q_samples = q_samples.reshape(720, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap trained score")
 ```
 ![Prediction](readme_heatmap_trained_score.png)
 ```python
 >>> inpainter = get_inpainter(solver, stack_samples=False)
 >>> data = jnp.array([-0.5, 0.0])
 >>> mask = jnp.array([1, 0])
 >>> data = jnp.tile(data, (64, 1))
 >>> mask = jnp.tile(mask, (64, 1))
->>> q_samples = inpainter(rng, data, mask)
->>> plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap inpainted")
+>>> rng, *sample_rng = random.split(rng, 2)
+>>> q_samples = inpainter(jnp.array(sample_rng), data, mask)
+>>> q_samples = q_samples.reshape(64, N)
+>>> plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap inpainted")
 ```
 ![Prediction](readme_heatmap_inpainted.png)
 
 ## Does haves
 - Training scores on (possibly, image) data and sampling from the generative model. Also inverse problems, such as inpainting.
 - Not many lines of code.
 - Easy to use, extendable. Get started with the example, provided.
```

### Comparing `diffusionjax-0.0.7/diffusionjax.egg-info/SOURCES.txt` & `diffusionjax-0.0.8/diffusionjax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/examples/example.py` & `diffusionjax-0.0.8/examples/example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Diffusion models introduction.
 
 Based off the Jupyter notebook: https://jakiw.com/sgm_intro
 A tutorial on the theoretical and implementation aspects of score-based generative models, also called diffusion models.
 """
+import jax
 from jax import jit, vmap, grad
 import jax.random as random
 import jax.numpy as jnp
 from jax.scipy.special import logsumexp
 from flax import serialization
 import matplotlib.pyplot as plt
 from diffusionjax.plot import (
@@ -37,18 +38,33 @@
     alphas = jnp.linspace(0, 2 * jnp.pi * (1 - 1/num_samples), num_samples)
     xs = jnp.cos(alphas)
     ys = jnp.sin(alphas)
     samples = jnp.stack([xs, ys], axis=1)
     return samples
 
 
+def plot_beta_schedule(sde, solver):
+    """Plots the temperature schedule of the SDE marginals.
+
+    Args:
+        sde: a valid SDE class.
+    """
+    beta_t = sde.beta_min + solver.ts * (sde.beta_max - sde.beta_min)
+    diffusion = jnp.sqrt(beta_t)
+
+    plt.plot(solver.ts, beta_t, label="beta_t")
+    plt.plot(solver.ts, diffusion, label="diffusion_t")
+    plt.legend()
+    plt.savefig("plot_beta_schedule.png")
+    plt.close()
+
+
 def main():
     num_epochs = 4000
     rng = random.PRNGKey(2023)
-    rng, step_rng = random.split(rng, 2)
     num_samples = 8
     samples = sample_circle(num_samples)
     N = samples.shape[1]
     plot_samples(samples=samples, index=(0, 1), fname="samples", lims=((-3, 3), (-3, 3)))
 
     # Get sde model, variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU)
     sde = VP(beta_min=0.01, beta_max=3.0)
@@ -74,33 +90,38 @@
     # Get a jax grad function, which can be batched with vmap
     nabla_log_hat_pt = jit(vmap(grad(log_hat_pt), in_axes=(0, 0), out_axes=(0)))
 
     # Running the reverse SDE with the empirical drift
     plot_score(score=nabla_log_hat_pt, t=0.01, area_min=-3, area_max=3, fname="empirical score")
     reverse_sde = sde.reverse(nabla_log_hat_pt)
     solver = EulerMaruyama(reverse_sde)
-    sampler = get_sampler(solver, stack_samples=False)
-    q_samples = sampler(rng, num_samples=5000, shape=(N,))
-    plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap empirical score")
+    sampler = get_sampler((5760, N), solver, stack_samples=False)
+    rng, *sample_rng = random.split(rng, 2)
+    sample_rng = jnp.asarray(sample_rng)
+    q_samples = sampler(sample_rng)
+    q_samples = q_samples.reshape(5760, N)
+    plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap empirical score")
 
     # What happens when I perturb the score with a constant?
     perturbed_score = lambda x, t: nabla_log_hat_pt(x, t) + 1
-    rng, step_rng = random.split(rng)
     reverse_sde = sde.reverse(perturbed_score)
     solver = EulerMaruyama(reverse_sde)
-    sampler = get_sampler(solver)
-    q_samples = sampler(rng, num_samples=5000, shape=(N,))
-    plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap bounded perturbation")
+    sampler = get_sampler((5760, N), solver)
+    rng, *sample_rng = random.split(rng, 2)
+    sample_rng = jnp.asarray(sample_rng)
+    q_samples = sampler(sample_rng)
+    q_samples = q_samples.reshape(5760, N)
+    plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap bounded perturbation")
 
     # Neural network training via score matching
-    batch_size=16
+    batch_size=64
     score_model = MLP()
     score_scaling = True
     # Initialize parameters
-    params = score_model.init(step_rng, jnp.zeros((batch_size, N)), jnp.ones((batch_size,)))
+    params = score_model.init(rng, jnp.zeros((batch_size, N)), jnp.ones((batch_size,)))
     # Initialize optimizer
     opt_state = optimizer.init(params)
     if 0:  # Load pre-trained model parameters
         f = open('/tmp/output0', 'rb')
         output = f.read()
         params = serialization.from_bytes(params, output)
     else:
@@ -109,15 +130,15 @@
         loss = get_loss(
             sde, solver, score_model, score_scaling=score_scaling, likelihood_weighting=False,
             reduce_mean=True, pointwise_t=False)
         # Train with score matching
         score_model, params, opt_state, mean_losses = retrain_nn(
             update_step=update_step,
             num_epochs=num_epochs,
-            step_rng=step_rng,
+            step_rng=rng,
             samples=samples,
             score_model=score_model,
             params=params,
             opt_state=opt_state,
             loss=loss,
             batch_size=batch_size)
 
@@ -127,26 +148,32 @@
         f.write(output)
 
     # Get trained score
     trained_score = get_score(sde, score_model, params, score_scaling=score_scaling)
     plot_score(score=trained_score, t=0.01, area_min=-3, area_max=3, fname="trained score")
     reverse_sde = sde.reverse(trained_score)
     solver = EulerMaruyama(reverse_sde)
-    sampler = get_sampler(solver, stack_samples=False)
-    q_samples = sampler(rng, num_samples=1000, shape=(N,))
-    plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap trained score")
+    sampler = get_sampler((720, N), solver, stack_samples=False)
+    rng, *sample_rng = random.split(rng, 2)
+    sample_rng = jnp.asarray(sample_rng)
+    q_samples = sampler(sample_rng)
+    q_samples = q_samples.reshape(720, N)
+    plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap trained score")
 
     # Condition on one of the coordinates
     data = jnp.array([-0.5, 0.0])
     mask = jnp.array([1, 0])
     data = jnp.tile(data, (64, 1))
     mask = jnp.tile(mask, (64, 1))
     inpainter = get_inpainter(solver, stack_samples=False)
-    q_samples = inpainter(rng, data, mask)
-    plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap inpainted")
+    rng, *sample_rng = random.split(rng, 2)
+    sample_rng = jnp.asarray(sample_rng)
+    q_samples = inpainter(sample_rng, data, mask)
+    q_samples = q_samples.reshape(64, N)
+    plot_heatmap(samples=q_samples, area_min=-3, area_max=3, fname="heatmap inpainted")
 
     frames = 100
     fig, ax = plt.subplots(1, 1)
     plt.gca().set_aspect('equal', adjustable='box')
     def animate(i, ax):
         ax.clear()
         plot_score_ax(
```

### Comparing `diffusionjax-0.0.7/examples/example1.py` & `diffusionjax-0.0.8/examples/example1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """Diffusion models introduction.
 
 An example using 1 dimensional image data.
+
+Dependencies: This example requires mlkernels package,
+https://github.com/wesselb/mlkernels#installation
 """
 from jax import jit, vmap, grad
 import jax.random as random
 import jax.numpy as jnp
 from jax.scipy.special import logsumexp
 from flax import serialization
 import matplotlib.pyplot as plt
@@ -33,17 +36,17 @@
 
 def sample_image_rgb(rng, num_samples, image_size, kernel, num_channels=1):
     """Samples from a GMRF
     """
     x = np.linspace(-x_max, x_max, image_size)
     x = x.reshape(image_size, 1)
     C = B.dense(kernel(x)) + epsilon * B.eye(image_size)
-    x = random.multivariate_normal(rng, mean=jnp.zeros(x.shape[0]), cov=C, shape=(num_samples, num_channels))
-    x = x.transpose((0, 2, 1))
-    return x, C
+    u = random.multivariate_normal(rng, mean=jnp.zeros(x.shape[0]), cov=C, shape=(num_samples, num_channels))
+    u = u.transpose((0, 2, 1))
+    return u, C
 
 
 def plot_score_ax_sample(ax, sample, score, t, area_min=-1, area_max=1, fname="plot_score"):
     @partial(jit, static_argnums=[0,])
     def helper(score, sample, t, area_min, area_max):
         x = jnp.linspace(area_min, area_max, 16)
         x, y = jnp.meshgrid(x, x)
@@ -82,15 +85,15 @@
     sde = VE(sigma_min=0.01, sigma_max=3.0)
 
     def log_hat_pt_tmp(x, t):
         """
         Empirical distribution score.
 
         Args:
-            x: One location in $\mathbb{R}^2$
+            x: One location in $\mathbb{R}^{image_size}$
             t: time
         Returns:
             The empirical log density, as described in the Jupyter notebook
             .. math::
                 \hat{p}_{t}(x)
         """
         mean, std = sde.marginal_prob(samples[:, [0, 1], 0], t)
@@ -98,15 +101,15 @@
         return logsumexp(potentials, axis=0, b=1/num_samples)
 
     def log_hat_pt(x, t):
         """
         Empirical distribution score.
 
         Args:
-            x: One location in $\mathbb{R}^2$
+            x: One location in $\mathbb{R}^{image_size}$
             t: time
         Returns:
             The empirical log density, as described in the Jupyter notebook
             .. math::
                 \hat{p}_{t}(x)
         """
         mean, std = sde.marginal_prob(samples, t)
@@ -114,15 +117,15 @@
         # Needs to be reshaped, since x is an image
         potentials = jnp.sum(losses.reshape((losses.shape[0], -1)), axis=-1)
         return logsumexp(potentials, axis=0, b=1/num_samples)
 
     def nabla_log_pt(x, t):
         """
         Args:
-            x: One location in $\mathbb{R}^2$
+            x: One location in $\mathbb{R}^{image_size}$
             t: time
         Returns:
             The true log density.
             .. math::
                 p_{t}(x)
         """
         x_shape = x.shape
@@ -135,40 +138,42 @@
     if 0:  # This may take a while
         # Get a jax grad function, which can be batched with vmap
         nabla_log_hat_pt_tmp = jit(vmap(grad(log_hat_pt_tmp), in_axes=(0, 0), out_axes=(0)))
         nabla_log_hat_pt = jit(vmap(grad(log_hat_pt), in_axes=(0, 0), out_axes=(0)))
 
         # Running the reverse SDE with the empirical score
         plot_score(score=nabla_log_hat_pt_tmp, t=0.01, area_min=-3, area_max=3, fname="empirical score")
-        sampler = get_sampler(EulerMaruyama(sde.reverse(nabla_log_hat_pt)))
-        q_samples = sampler(rng, num_samples=64, shape=(image_size, num_channels))
+        sampler = get_sampler((64, image_size, num_channels), EulerMaruyama(sde.reverse(nabla_log_hat_pt)))
+        q_samples = sampler(rng)
         plot_samples_1D(q_samples, image_size=image_size, fname="samples empirical score")
         plot_heatmap(samples=q_samples[:, [0, 1], 0], area_min=-3, area_max=3, fname="heatmap empirical score")
 
         # What happens when I perturb the score with a constant?
         perturbed_score = lambda x, t: nabla_log_hat_pt(x, t) + 10.0 * jnp.ones(jnp.shape(x))
         rng, step_rng = random.split(rng)
-        sampler = get_sampler(EulerMaruyama(sde.reverse(perturbed_score)))
-        q_samples = sampler(rng, num_samples=64, shape=(image_size, num_channels))
+        sampler = get_sampler((64, image_size, num_channels), EulerMaruyama(sde.reverse(perturbed_score)))
+        q_samples = sampler(rng)
         plot_samples_1D(q_samples, image_size=image_size, fname="samples bounded perturbation")
         plot_heatmap(samples=q_samples[:, [0, 1], 0], area_min=-3, area_max=3, fname="heatmap bounded perturbation")
 
         nabla_log_pt = jit(vmap(nabla_log_pt, in_axes=(0, 0), out_axes=(0)))
 
         # Running the reverse SDE with the true score
-        sampler = get_sampler(EulerMaruyama(sde.reverse(nabla_log_pt)))
-        q_samples = sampler(rng, num_samples=64, shape=(image_size, num_channels))
+        sampler = get_sampler((64, image_size, num_channels), EulerMaruyama(sde.reverse(nabla_log_pt)))
+        q_samples = sampler(rng)
         plot_samples_1D(q_samples, image_size=image_size, fname="samples true score")
         plot_heatmap(samples=q_samples[:, [0, 1], 0], area_min=-3, area_max=3, fname="heatmap true score")
 
         # What happens when I perturb the score with a constant?
         perturbed_score = lambda x, t: nabla_log_pt(x, t) + 10.0 * jnp.ones(jnp.shape(x))
-        rng, step_rng = random.split(rng)
-        sampler = get_sampler(EulerMaruyama(sde.reverse(perturbed_score)))
-        q_samples = sampler(rng, num_samples=64, shape=(image_size, num_channels))
+        sampler = get_sampler((64, image_size, num_channels), EulerMaruyama(sde.reverse(perturbed_score)))
+        rng, *sample_rng = random.split(rng, 2)
+        sample_rng = jnp.asarray(sample_rng)
+        q_samples = sampler(sample_rng)
+        q_samples = q_samples.reshape(64, image_size, num_channels)
         plot_samples_1D(q_samples, image_size=image_size, fname="samples true bounded perturbation")
         plot_heatmap(samples=q_samples[:, [0, 1], 0], area_min=-3, area_max=3, fname="heatmap true bounded perturbation")
 
     # Neural network training via score matching
     batch_size = 64
     score_model = MLP()
 
@@ -205,17 +210,21 @@
         output = serialization.to_bytes(params)
         f = open('/tmp/output1', 'wb')
         f.write(output)
 
     # Get trained score
     trained_score = get_score(sde, score_model, params, score_scaling=True)
     solver = EulerMaruyama(sde.reverse(trained_score))
-    sampler = get_sampler(solver, denoise=True)
-    rng, step_rng = random.split(rng, 2)
-    q_samples = sampler(rng, num_samples=512, shape=(image_size, num_channels))
+    sampler = get_sampler((512, image_size, num_channels), solver, denoise=True)
+
+    rng, *sample_rng = random.split(rng, 2)
+    sample_rng = jnp.asarray(sample_rng)
+    q_samples = sampler(sample_rng)
+    q_samples = q_samples.reshape(512, image_size, num_channels)
+
     # C_emp = jnp.corrcoef(q_samples[:, :, 0].T)
     # delta = jnp.linalg.norm(C - C_emp) / image_size
 
     plot_samples_1D(q_samples[:64], image_size=image_size, fname="samples trained score")
     plot_heatmap(samples=q_samples[:, [0, 1], 0], area_min=-3, area_max=3, fname="heatmap trained score")
 
     if 0:
@@ -234,18 +243,24 @@
     mask = jnp.zeros((image_size, num_channels), dtype=int)
     mask = mask.at[[0, -1], 0].set([1, 1])
     data = jnp.tile(data, (5, 1, 1))
     mask = jnp.tile(mask, (5, 1, 1))
 
     # Get inpainter
     inpainter = get_inpainter(solver, stack_samples=False)
-    q_samples = inpainter(rng, data, mask)
+    rng, *sample_rng = random.split(rng, 2)
+    sample_rng = jnp.asarray(sample_rng)
+    q_samples = inpainter(sample_rng, data, mask)
+    q_samples = q_samples.reshape(5, image_size, num_channels)
     plot_samples_1D(q_samples, image_size=image_size, fname="samples inpainted")
 
     # Get projection sampler
     projection_sampler = get_projection_sampler(solver, stack_samples=False)
-    q_samples = projection_sampler(rng, data, mask, coeff=1e-2)
+    rng, *sample_rng = random.split(rng, 2)
+    sample_rng = jnp.asarray(sample_rng)
+    q_samples = projection_sampler(sample_rng, data, mask, 1e-2)
+    q_samples = q_samples.reshape(5, image_size, num_channels)
     plot_samples_1D(q_samples, image_size=image_size, fname="samples projected")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `diffusionjax-0.0.7/examples/example2.py` & `diffusionjax-0.0.8/examples/example2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """Diffusion models introduction.
 
 An example using 2 dimensional image data.
+
+Dependencies: This example requires mlkernels package,
+https://github.com/wesselb/mlkernels#installation
 """
+import jax
 from jax import jit, vmap, grad
 import jax.random as random
 import jax.numpy as jnp
 from jax.scipy.special import logsumexp
 from flax import serialization
 import matplotlib.pyplot as plt
 from diffusionjax.plot import plot_samples, plot_heatmap
 from diffusionjax.losses import get_loss
-from diffusionjax.solvers import EulerMaruyama, Annealed
+from diffusionjax.solvers import EulerMaruyama
+from diffusionjax.solvers import Annealed
 from diffusionjax.samplers import get_sampler
 from diffusionjax.models import CNN
 from diffusionjax.utils import (
     get_score,
     update_step,
     optimizer,
     retrain_nn)
@@ -48,17 +53,17 @@
     x = np.linspace(-x_max, x_max, image_size)
     y = np.linspace(-x_max, x_max, image_size)
     xx, yy = np.meshgrid(x, y)
     xx = xx.reshape(image_size**2, 1)
     yy = yy.reshape(image_size**2, 1)
     z = np.hstack((xx, yy))
     C = B.dense(kernel(z))  + epsilon * B.eye(image_size**2)
-    x = random.multivariate_normal(rng, mean=jnp.zeros(xx.shape[0]), cov=C, shape=(num_samples, num_channels))
-    x = x.transpose((0, 2, 1))
-    return x, C
+    u = random.multivariate_normal(rng, mean=jnp.zeros(xx.shape[0]), cov=C, shape=(num_samples, num_channels))
+    u = u.transpose((0, 2, 1))
+    return u, C
 
 
 def plot_samples_1D(samples, image_size, fname="samples 1D.png"):
     x = np.linspace(-x_max, x_max, image_size)
     plt.plot(x, samples[:, :, 0, 0].T)
     plt.savefig(fname)
     plt.close()
@@ -83,15 +88,15 @@
     sde = VP(beta_min=0.1, beta_max=10.0)
 
     def log_hat_pt(x, t):
         """
         Empirical distribution score.
 
         Args:
-            x: One location in $\mathbb{R}^2$
+            x: One location in $\mathbb{R}^{image_size}$
             t: time
         Returns:
             The empirical log density, as described in the Jupyter notebook
             .. math::
                 \hat{p}_{t}(x)
         """
         mean, std = sde.marginal_prob(samples, t)
@@ -99,43 +104,43 @@
         # Needs to be reshaped, since x is an image
         potentials = jnp.sum(losses.reshape((losses.shape[0], -1)), axis=-1)
         return logsumexp(potentials, axis=0, b=1/num_samples)
 
     def nabla_log_pt(x, t):
         """
         Args:
-            x: One location in $\mathbb{R}^2$
+            x: One location in $\mathbb{R}^{image_size}$
             t: time
         Returns:
             The true log density.
             .. math::
                 p_{t}(x)
         """
         x_shape = x.shape
         v_t = sde.variance(t)
         m_t = sde.mean_coeff(t)
         x = x.flatten()
-        score = - jnp.linalg.solve(m_t**2 * C + v_t * jnp.eye(x_shape[0] * x_shape[1]), x)
+        score = -jnp.linalg.solve(m_t**2 * C + v_t * jnp.eye(x_shape[0] * x_shape[1]), x)
         return score.reshape(x_shape)
 
     if 0:  # this may take a while
         # Get a jax grad function, which can be batched with vmap
         nabla_log_hat_pt = jit(vmap(grad(log_hat_pt), in_axes=(0, 0), out_axes=(0)))
-        nabla_log_pt = jit(vmap(nabla_log_pt, in_axes=(0, 0), out_axes=(0)))
+        # nabla_log_pt = jit(vmap(nabla_log_pt, in_axes=(0, 0), out_axes=(0)))
         # Running the reverse SDE with the empirical score
-        sampler = get_sampler(EulerMaruyama(sde.reverse(nabla_log_hat_pt), num_steps=num_steps))
-        q_samples = sampler(rng, n_samples=64, shape=(image_size, image_size, num_channels))
+        sampler = get_sampler((64, image_size, image_size, num_channels), EulerMaruyama(sde.reverse(nabla_log_hat_pt), num_steps=num_steps))
+        q_samples = sampler(rng)
         plot_samples(q_samples, image_size=image_size, num_channels=num_channels, fname="samples empirical score")
         plot_samples_1D(q_samples, image_size, "samples 1D empirical score")
         plot_heatmap(samples=q_samples[:, [0, 1], 0, 0], area_min=-3, area_max=3, fname="heatmap empirical score")
         # What happens when I perturb the score with a constant?
         perturbed_score = lambda x, t: nabla_log_hat_pt(x, t) + 10.0 * jnp.ones(jnp.shape(x))
         rng, step_rng = random.split(rng)
-        sampler = get_sampler(EulerMaruyama(sde.reverse(perturbed_score), num_steps=num_steps))
-        q_samples = sampler(rng, n_samples=64, shape=(image_size, image_size, num_channels))
+        sampler = get_sampler((64, image_size, image_size, num_channels), EulerMaruyama(sde.reverse(perturbed_score), num_steps=num_steps))
+        q_samples = sampler(rng)
         plot_samples(q_samples, image_size=image_size, num_channels=num_channels, fname="samples bounded perturbation")
         plot_heatmap(samples=q_samples[:, [0, 1], 0, 0], area_min=-3, area_max=3, fname="heatmap bounded perturbation")
 
     # Neural network training via score matching
     batch_size = 16
     score_model = CNN()
     # Initialize parameters
@@ -174,19 +179,22 @@
 
     # Get the outer loop of a numerical solver, also known as "predictor"
     outer_solver = EulerMaruyama(sde.reverse(trained_score), num_steps=num_steps)
 
     # Get the inner loop of a numerical solver, also known as "corrector"
     inner_solver = Annealed(sde.corrector(UDLangevin, trained_score), num_steps=2, snr=0.01)
 
-    sampler = get_sampler(outer_solver, inner_solver, denoise=True)
-    # sampler = get_sampler(outer_solver, denoise=True)
-
-    rng, step_rng = random.split(rng, 2)
-    q_samples = sampler(rng, num_samples=64, shape=(image_size, image_size, num_channels))
+    num_devices =  jax.local_device_count()
+    sampler = get_sampler((64//num_devices, image_size, image_size, num_channels), outer_solver, inner_solver, denoise=True)
+    # sampler = get_sampler((64//num_devices, image_size, image_size, num_channels), outer_solver, denoise=True)
+
+    rng, *sample_rng = random.split(rng, num_devices + 1)
+    sample_rng = jnp.asarray(sample_rng)
+    q_samples = sampler(sample_rng)
+    q_samples = q_samples.reshape(64, image_size, image_size, num_channels)
     plot_samples(q_samples, image_size=image_size, num_channels=num_channels, fname="samples trained score")
     plot_samples_1D(q_samples, image_size, fname="samples 1D trained score")
     plot_heatmap(samples=q_samples[:, [0, 1], 0, 0], area_min=-3, area_max=3, fname="heatmap trained score")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `diffusionjax-0.0.7/readme_empirical_score.png` & `diffusionjax-0.0.8/readme_empirical_score.png`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/readme_samples.png` & `diffusionjax-0.0.8/readme_samples.png`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.7/setup.py` & `diffusionjax-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,11 +36,9 @@
         'scipy',
         'matplotlib',
         'seaborn',
         'jaxlib>=0.4.1',
         'jax>=0.4.1',
         'optax',
         'flax',
-        'backends>=1.4.32',
-        'mlkernels>=0.3.6',
         ]
     )
```

