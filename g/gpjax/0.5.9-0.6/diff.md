# Comparing `tmp/gpjax-0.5.9.tar.gz` & `tmp/gpjax-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpjax-0.5.9.tar", last modified: Thu Jan 19 23:56:32 2023, max compression
+gzip compressed data, was "gpjax-0.6.tar", max compression
```

## Comparing `gpjax-0.5.9.tar` & `gpjax-0.6.tar`

### file list

```diff
@@ -1,29 +1,58 @@
-drwxr-xr-x   0 tompinder   (501) staff       (20)        0 2023-01-19 23:56:32.180377 gpjax-0.5.9/
--rw-r--r--   0 tompinder   (501) staff       (20)     8916 2023-01-19 23:56:32.180460 gpjax-0.5.9/PKG-INFO
--rw-r--r--   0 tompinder   (501) staff       (20)     8452 2023-01-19 23:39:48.000000 gpjax-0.5.9/README.md
-drwxr-xr-x   0 tompinder   (501) staff       (20)        0 2023-01-19 23:56:32.181607 gpjax-0.5.9/gpjax/
--rw-r--r--   0 tompinder   (501) staff       (20)     2271 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/__init__.py
--rw-r--r--   0 tompinder   (501) staff       (20)      497 2023-01-19 23:56:32.181657 gpjax-0.5.9/gpjax/_version.py
--rw-r--r--   0 tompinder   (501) staff       (20)    14595 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/abstractions.py
--rw-r--r--   0 tompinder   (501) staff       (20)     1547 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/config.py
--rw-r--r--   0 tompinder   (501) staff       (20)     8544 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/gaussian_distribution.py
--rw-r--r--   0 tompinder   (501) staff       (20)    32479 2023-01-19 23:39:48.000000 gpjax-0.5.9/gpjax/gps.py
--rw-r--r--   0 tompinder   (501) staff       (20)    39117 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/kernels.py
--rw-r--r--   0 tompinder   (501) staff       (20)    10278 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/likelihoods.py
--rw-r--r--   0 tompinder   (501) staff       (20)     5773 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/mean_functions.py
--rw-r--r--   0 tompinder   (501) staff       (20)    10060 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/natural_gradients.py
--rw-r--r--   0 tompinder   (501) staff       (20)    13714 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/parameters.py
--rw-r--r--   0 tompinder   (501) staff       (20)     2076 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/quadrature.py
--rw-r--r--   0 tompinder   (501) staff       (20)     1090 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/types.py
--rw-r--r--   0 tompinder   (501) staff       (20)     1255 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/utils.py
--rw-r--r--   0 tompinder   (501) staff       (20)    33205 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/variational_families.py
--rw-r--r--   0 tompinder   (501) staff       (20)    12294 2023-01-19 23:13:55.000000 gpjax-0.5.9/gpjax/variational_inference.py
-drwxr-xr-x   0 tompinder   (501) staff       (20)        0 2023-01-19 23:56:32.180265 gpjax-0.5.9/gpjax.egg-info/
--rw-r--r--   0 tompinder   (501) staff       (20)     8916 2023-01-19 23:56:32.000000 gpjax-0.5.9/gpjax.egg-info/PKG-INFO
--rw-r--r--   0 tompinder   (501) staff       (20)      524 2023-01-19 23:56:32.000000 gpjax-0.5.9/gpjax.egg-info/SOURCES.txt
--rw-r--r--   0 tompinder   (501) staff       (20)        1 2023-01-19 23:56:32.000000 gpjax-0.5.9/gpjax.egg-info/dependency_links.txt
--rw-r--r--   0 tompinder   (501) staff       (20)      234 2023-01-19 23:56:32.000000 gpjax-0.5.9/gpjax.egg-info/requires.txt
--rw-r--r--   0 tompinder   (501) staff       (20)        6 2023-01-19 23:56:32.000000 gpjax-0.5.9/gpjax.egg-info/top_level.txt
--rw-r--r--   0 tompinder   (501) staff       (20)      688 2023-01-19 23:56:32.181315 gpjax-0.5.9/setup.cfg
--rw-r--r--   0 tompinder   (501) staff       (20)     1901 2023-01-19 23:47:19.000000 gpjax-0.5.9/setup.py
--rw-r--r--   0 tompinder   (501) staff       (20)    83780 2023-01-19 23:13:55.000000 gpjax-0.5.9/versioneer.py
+-rw-r--r--   0        0        0    11357 2023-05-11 20:54:48.036528 gpjax-0.6/LICENSE
+-rw-r--r--   0        0        0     7191 2023-05-11 21:33:47.089655 gpjax-0.6/README.md
+-rw-r--r--   0        0        0     2900 2023-05-11 21:33:47.126581 gpjax-0.6/gpjax/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-11 21:33:47.126847 gpjax-0.6/gpjax/base/__init__.py
+-rw-r--r--   0        0        0    12470 2023-05-11 21:33:47.126989 gpjax-0.6/gpjax/base/module.py
+-rw-r--r--   0        0        0     2254 2023-05-11 21:33:47.127060 gpjax-0.6/gpjax/base/param.py
+-rw-r--r--   0        0        0     3452 2023-05-11 21:33:47.127136 gpjax-0.6/gpjax/dataset.py
+-rw-r--r--   0        0        0     8119 2023-05-11 21:33:47.127221 gpjax-0.6/gpjax/fit.py
+-rw-r--r--   0        0        0     9121 2023-05-11 21:33:47.127395 gpjax-0.6/gpjax/gaussian_distribution.py
+-rw-r--r--   0        0        0    28181 2023-05-11 21:33:47.127606 gpjax-0.6/gpjax/gps.py
+-rw-r--r--   0        0        0     1815 2023-05-11 21:33:47.127892 gpjax-0.6/gpjax/kernels/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-11 21:33:47.128020 gpjax-0.6/gpjax/kernels/approximations/__init__.py
+-rw-r--r--   0        0        0     3183 2023-05-11 21:33:47.128137 gpjax-0.6/gpjax/kernels/approximations/rff.py
+-rw-r--r--   0        0        0     6680 2023-05-11 21:33:47.128282 gpjax-0.6/gpjax/kernels/base.py
+-rw-r--r--   0        0        0     1379 2023-05-11 21:33:47.128558 gpjax-0.6/gpjax/kernels/computations/__init__.py
+-rw-r--r--   0        0        0     2585 2023-05-11 21:33:47.128682 gpjax-0.6/gpjax/kernels/computations/base.py
+-rw-r--r--   0        0        0     2478 2023-05-11 21:33:47.128816 gpjax-0.6/gpjax/kernels/computations/basis_functions.py
+-rw-r--r--   0        0        0     2830 2023-05-11 21:33:47.128972 gpjax-0.6/gpjax/kernels/computations/constant_diagonal.py
+-rw-r--r--   0        0        0     1661 2023-05-11 21:33:47.129071 gpjax-0.6/gpjax/kernels/computations/dense.py
+-rw-r--r--   0        0        0     2383 2023-05-11 21:33:47.129171 gpjax-0.6/gpjax/kernels/computations/diagonal.py
+-rw-r--r--   0        0        0     2165 2023-05-11 21:33:47.129303 gpjax-0.6/gpjax/kernels/computations/eigen.py
+-rw-r--r--   0        0        0      790 2023-05-11 21:33:47.129595 gpjax-0.6/gpjax/kernels/non_euclidean/__init__.py
+-rw-r--r--   0        0        0     3511 2023-05-11 21:33:47.129716 gpjax-0.6/gpjax/kernels/non_euclidean/graph.py
+-rw-r--r--   0        0        0     1620 2023-05-11 21:33:47.129829 gpjax-0.6/gpjax/kernels/non_euclidean/utils.py
+-rw-r--r--   0        0        0      930 2023-05-11 21:33:47.130081 gpjax-0.6/gpjax/kernels/nonstationary/__init__.py
+-rw-r--r--   0        0        0     4078 2023-05-11 21:33:47.130162 gpjax-0.6/gpjax/kernels/nonstationary/arccosine.py
+-rw-r--r--   0        0        0     2016 2023-05-11 21:33:47.130277 gpjax-0.6/gpjax/kernels/nonstationary/linear.py
+-rw-r--r--   0        0        0     2384 2023-05-11 21:33:47.130397 gpjax-0.6/gpjax/kernels/nonstationary/polynomial.py
+-rw-r--r--   0        0        0     1323 2023-05-11 21:33:47.130534 gpjax-0.6/gpjax/kernels/stationary/__init__.py
+-rw-r--r--   0        0        0     2521 2023-05-11 21:33:47.130681 gpjax-0.6/gpjax/kernels/stationary/matern12.py
+-rw-r--r--   0        0        0     2723 2023-05-11 21:33:47.130817 gpjax-0.6/gpjax/kernels/stationary/matern32.py
+-rw-r--r--   0        0        0     2792 2023-05-11 21:33:47.130923 gpjax-0.6/gpjax/kernels/stationary/matern52.py
+-rw-r--r--   0        0        0     2420 2023-05-11 21:33:47.131037 gpjax-0.6/gpjax/kernels/stationary/periodic.py
+-rw-r--r--   0        0        0     2500 2023-05-11 21:33:47.131171 gpjax-0.6/gpjax/kernels/stationary/powered_exponential.py
+-rw-r--r--   0        0        0     2389 2023-05-11 21:33:47.131312 gpjax-0.6/gpjax/kernels/stationary/rational_quadratic.py
+-rw-r--r--   0        0        0     2440 2023-05-11 21:33:47.131400 gpjax-0.6/gpjax/kernels/stationary/rbf.py
+-rw-r--r--   0        0        0     2226 2023-05-11 21:33:47.131522 gpjax-0.6/gpjax/kernels/stationary/utils.py
+-rw-r--r--   0        0        0     2072 2023-05-11 21:33:47.131675 gpjax-0.6/gpjax/kernels/stationary/white.py
+-rw-r--r--   0        0        0     6643 2023-05-11 21:33:47.131830 gpjax-0.6/gpjax/likelihoods.py
+-rw-r--r--   0        0        0     1609 2023-05-11 21:33:47.132130 gpjax-0.6/gpjax/linops/__init__.py
+-rw-r--r--   0        0        0     6259 2023-05-11 21:33:47.132259 gpjax-0.6/gpjax/linops/constant_diagonal_linear_operator.py
+-rw-r--r--   0        0        0     6201 2023-05-11 21:33:47.132389 gpjax-0.6/gpjax/linops/dense_linear_operator.py
+-rw-r--r--   0        0        0     7179 2023-05-11 21:33:47.132536 gpjax-0.6/gpjax/linops/diagonal_linear_operator.py
+-rw-r--r--   0        0        0     3607 2023-05-11 21:33:47.132958 gpjax-0.6/gpjax/linops/identity_linear_operator.py
+-rw-r--r--   0        0        0     7131 2023-05-11 21:33:47.133134 gpjax-0.6/gpjax/linops/linear_operator.py
+-rw-r--r--   0        0        0     3187 2023-05-11 21:33:47.133506 gpjax-0.6/gpjax/linops/triangular_linear_operator.py
+-rw-r--r--   0        0        0     3443 2023-05-11 21:33:47.133703 gpjax-0.6/gpjax/linops/utils.py
+-rw-r--r--   0        0        0     5939 2023-05-11 21:33:47.133915 gpjax-0.6/gpjax/linops/zero_linear_operator.py
+-rw-r--r--   0        0        0     6081 2023-05-11 21:33:47.134064 gpjax-0.6/gpjax/mean_functions.py
+-rw-r--r--   0        0        0    15061 2023-05-11 21:33:47.134196 gpjax-0.6/gpjax/objectives.py
+-rw-r--r--   0        0        0     4407 2023-05-11 21:33:47.134282 gpjax-0.6/gpjax/progress_bar.py
+-rw-r--r--   0        0        0     2172 2023-05-11 21:33:47.134433 gpjax-0.6/gpjax/quadrature.py
+-rw-r--r--   0        0        0     5506 2023-05-11 21:33:47.134686 gpjax-0.6/gpjax/scan.py
+-rw-r--r--   0        0        0     1694 2023-05-11 21:33:47.134827 gpjax-0.6/gpjax/typing.py
+-rw-r--r--   0        0        0    26453 2023-05-11 21:33:47.135024 gpjax-0.6/gpjax/variational_families.py
+-rw-r--r--   0        0        0     4892 2023-05-11 21:44:55.712576 gpjax-0.6/pyproject.toml
+-rw-r--r--   0        0        0     8494 1970-01-01 00:00:00.000000 gpjax-0.6/setup.py
+-rw-r--r--   0        0        0     8372 1970-01-01 00:00:00.000000 gpjax-0.6/PKG-INFO
```

### Comparing `gpjax-0.5.9/PKG-INFO` & `gpjax-0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: gpjax
-Version: 0.5.9
-Summary: Didactic Gaussian processes in Jax.
-Author: Thomas Pinder
-Author-email: t.pinder2@lancaster.ac.uk
-License: LICENSE
-Project-URL: Documentation, https://gpjax.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/thomaspinder/GPJax
-Keywords: gaussian-processes jax machine-learning bayesian
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: cuda
-
 <!-- <h1 align='center'>GPJax</h1>
 <h2 align='center'>Gaussian processes in Jax.</h2> -->
 <p align="center">
 <img width="700" height="300" src="https://github.com/JaxGaussianProcesses/GPJax/raw/master/docs/_static/gpjax_logo.svg" alt="GPJax's logo">
 </p>
 
 [![codecov](https://codecov.io/gh/JaxGaussianProcesses/GPJax/branch/master/graph/badge.svg?token=DM1DRDASU2)](https://codecov.io/gh/JaxGaussianProcesses/GPJax)
@@ -28,47 +13,65 @@
 [![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
 
 [**Quickstart**](#simple-example)
 | [**Install guide**](#installation)
 | [**Documentation**](https://gpjax.readthedocs.io/en/latest/)
 | [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
 
-GPJax aims to provide a low-level interface to Gaussian process (GP) models in [Jax](https://github.com/google/jax), structured to give researchers maximum flexibility in extending the code to suit their own needs. The idea is that the code should be as close as possible to the maths we write on paper when working with GP models.
+GPJax aims to provide a low-level interface to Gaussian process (GP) models in
+[Jax](https://github.com/google/jax), structured to give researchers maximum
+flexibility in extending the code to suit their own needs. The idea is that the
+code should be as close as possible to the maths we write on paper when working
+with GP models.
 
 # Package support
 
-GPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today, the maintenance of GPJax is undertaken by [Thomas Pinder](https://github.com/thomaspinder) and [Daniel Dodd](https://github.com/Daniel-Dodd).
-
-We would be delighted to receive contributions from interested individuals and groups. To learn how you can get involved, please read our [guide for contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md). If you have any questions, we encourage you to [open an issue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For broader conversations, such as best GP fitting practices or questions about the mathematics of GPs, we invite you to [open a discussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).
-
-Feel free to join our [Slack Channel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw), where we can discuss the development of GPJax and broader support for Gaussian process modelling.
+GPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today,
+the maintenance of GPJax is undertaken by [Thomas
+Pinder](https://github.com/thomaspinder) and [Daniel
+Dodd](https://github.com/Daniel-Dodd).
+
+We would be delighted to receive contributions from interested individuals and
+groups. To learn how you can get involved, please read our [guide for
+contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md).
+If you have any questions, we encourage you to [open an
+issue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For
+broader conversations, such as best GP fitting practices or questions about the
+mathematics of GPs, we invite you to [open a
+discussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).
+
+Feel free to join our [Slack
+Channel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw),
+where we can discuss the development of GPJax and broader support for Gaussian
+process modelling.
 
 # Supported methods and interfaces
 
 ## Notebook examples
 
 > - [**Conjugate Inference**](https://gpjax.readthedocs.io/en/latest/examples/regression.html)
 > - [**Classification with MCMC**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
 > - [**Sparse Variational Inference**](https://gpjax.readthedocs.io/en/latest/examples/uncollapsed_vi.html)
 > - [**BlackJax Integration**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
 > - [**Laplace Approximation**](https://gpjax.readthedocs.io/en/latest/examples/classification.html#Laplace-approximation)
-> - [**TensorFlow Probability Integration**](https://gpjax.readthedocs.io/en/latest/examples/tfp_integration.html)
 > - [**Inference on Non-Euclidean Spaces**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
 > - [**Inference on Graphs**](https://gpjax.readthedocs.io/en/latest/examples/graph_kernels.html)
 > - [**Learning Gaussian Process Barycentres**](https://gpjax.readthedocs.io/en/latest/examples/barycentres.html)
 > - [**Deep Kernel Regression**](https://gpjax.readthedocs.io/en/latest/examples/haiku.html)
-> - [**Natural Gradients**](https://gpjax.readthedocs.io/en/latest/examples/natgrads.html)
 
 ## Guides for customisation
-> 
+>
 > - [**Custom kernels**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
 > - [**UCI regression**](https://gpjax.readthedocs.io/en/latest/examples/yacht.html)
 
 ## Conversion between `.ipynb` and `.py`
-Above examples are stored in [examples](examples) directory in the double percent (`py:percent`) format. Checkout [jupytext using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more info.
+Above examples are stored in [examples](examples) directory in the double
+percent (`py:percent`) format. Checkout [jupytext
+using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more
+info.
 
 * To convert `example.py` to `example.ipynb`, run:
 
 ```bash
 jupytext --to notebook example.py
 ```
 
@@ -83,89 +86,69 @@
 Let us import some dependencies and simulate a toy dataset $\mathcal{D}$.
 
 ```python
 import gpjax as gpx
 from jax import grad, jit
 import jax.numpy as jnp
 import jax.random as jr
-import jaxkern as jk
 import optax as ox
 
 key = jr.PRNGKey(123)
 
 f = lambda x: 10 * jnp.sin(x)
 
 n = 50
 x = jr.uniform(key=key, minval=-3.0, maxval=3.0, shape=(n,1)).sort()
 y = f(x) + jr.normal(key, shape=(n,1))
 D = gpx.Dataset(X=x, y=y)
-```
-
-The function of interest here, $f(\cdot)$, is sinusoidal, but our observations of it have been perturbed by Gaussian noise. We aim to utilise a Gaussian process to try and recover this latent function.
 
-## 1. Constructing the prior and posterior
+# Construct the prior
+meanf = gpx.mean_functions.Zero()
+kernel = gpx.kernels.RBF()
+prior = gpx.Prior(mean_function=meanf, kernel = kernel)
 
-We begin by defining a zero-mean Gaussian process prior with a radial basis function kernel and assume the likelihood to be Gaussian.
-
-```python
-prior = gpx.Prior(kernel = jk.RBF())
+# Define a likelihood
 likelihood = gpx.Gaussian(num_datapoints = n)
-```
-
-Similar to how we would write on paper, the posterior is constructed by the product of our prior with our likelihood.
 
-```python
+# Construct the posterior
 posterior = prior * likelihood
-```
 
-## 2. Learning hyperparameters
+# Define an optimiser
+optimiser = ox.adam(learning_rate=1e-2)
 
-Equipped with the posterior, we seek to learn the model's hyperparameters through gradient-optimisation of the marginal log-likelihood. We this below, adding Jax's [just-in-time (JIT)](https://jax.readthedocs.io/en/latest/jax-101/02-jitting.html) compilation to accelerate training. 
+# Define the marginal log-likelihood
+negative_mll = jit(gpx.objectives.ConjugateMLL(negative=True))
 
-```python
-mll = jit(posterior.marginal_log_likelihood(D, negative=True))
-```
+# Obtain Type 2 MLEs of the hyperparameters
+opt_posterior, history = gpx.fit(
+    model=posterior,
+    objective=negative_mll,
+    train_data=D,
+    optim=optimiser,
+    num_iters=500,
+    safe=True,
+    key=key,
+)
 
-For purposes of optimisation, we'll use optax's Adam.
-```
-opt = ox.adam(learning_rate=1e-3)
-```
-
-We define an initial parameter state through the `initialise` callable.
-
-```python
-parameter_state = gpx.initialise(posterior, key=key)
-```
-
-Finally, we run an optimisation loop using the Adam optimiser via the `fit` callable.
-
-```python
-inference_state = gpx.fit(mll, parameter_state, opt, num_iters=500)
-```
-
-## 3. Making predictions
-
-Using our learned hyperparameters, we can obtain the posterior distribution of the latent function at novel test points.
-
-```python
-learned_params, _ = inference_state.unpack()
+# Infer the predictive posterior distribution
 xtest = jnp.linspace(-3., 3., 100).reshape(-1, 1)
+latent_dist = opt_posterior(xtest, D)
+predictive_dist = opt_posterior.likelihood(latent_dist)
 
-latent_distribution = posterior(learned_params, D)(xtest)
-predictive_distribution = likelihood(learned_params, latent_distribution)
-
-predictive_mean = predictive_distribution.mean()
-predictive_cov = predictive_distribution.covariance()
+# Obtain the predictive mean and standard deviation
+pred_mean = predictive_dist.mean()
+pred_std = predictive_dist.stddev()
 ```
 
 # Installation
 
 ## Stable version
 
-The latest stable version of GPJax can be installed via [`pip`](https://pip.pypa.io/en/stable/):
+The latest stable version of GPJax can be installed via
+pip:
 
 ```bash
 pip install gpjax
 ```
 
 > **Note**
 >
@@ -175,35 +158,36 @@
 > ```
 
 
 
 ## Development version
 > **Warning**
 >
-> This version is possibly unstable and may contain bugs. 
+> This version is possibly unstable and may contain bugs.
 
-Clone a copy of the repository to your local machine and run the setup configuration in development mode.
+Clone a copy of the repository to your local machine and run the setup
+configuration in development mode.
 ```bash
 git clone https://github.com/JaxGaussianProcesses/GPJax.git
 cd GPJax
-python setup.py develop
+poetry install
 ```
 
 > **Note**
 >
 > We advise you create virtual environment before installing:
 > ```
 > conda create -n gpjax_experimental python=3.10.0
 > conda activate gpjax_experimental
 >  ```
 >
 > and recommend you check your installation passes the supplied unit tests:
 >
 > ```python
-> python -m pytest tests/
+> poetry run pytest
 > ```
 
 # Citing GPJax
 
 If you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).
 
 ```
```

### Comparing `gpjax-0.5.9/README.md` & `gpjax-0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,207 +1,46 @@
-<!-- <h1 align='center'>GPJax</h1>
-<h2 align='center'>Gaussian processes in Jax.</h2> -->
-<p align="center">
-<img width="700" height="300" src="https://github.com/JaxGaussianProcesses/GPJax/raw/master/docs/_static/gpjax_logo.svg" alt="GPJax's logo">
-</p>
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-[![codecov](https://codecov.io/gh/JaxGaussianProcesses/GPJax/branch/master/graph/badge.svg?token=DM1DRDASU2)](https://codecov.io/gh/JaxGaussianProcesses/GPJax)
-[![CodeFactor](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax/badge)](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax)
-[![Documentation Status](https://readthedocs.org/projects/gpjax/badge/?version=latest)](https://gpjax.readthedocs.io/en/latest/?badge=latest)
-[![PyPI version](https://badge.fury.io/py/GPJax.svg)](https://badge.fury.io/py/GPJax)
-[![DOI](https://joss.theoj.org/papers/10.21105/joss.04455/status.svg)](https://doi.org/10.21105/joss.04455)
-[![Downloads](https://pepy.tech/badge/gpjax)](https://pepy.tech/project/gpjax)
-[![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
-
-[**Quickstart**](#simple-example)
-| [**Install guide**](#installation)
-| [**Documentation**](https://gpjax.readthedocs.io/en/latest/)
-| [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
-
-GPJax aims to provide a low-level interface to Gaussian process (GP) models in [Jax](https://github.com/google/jax), structured to give researchers maximum flexibility in extending the code to suit their own needs. The idea is that the code should be as close as possible to the maths we write on paper when working with GP models.
-
-# Package support
-
-GPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today, the maintenance of GPJax is undertaken by [Thomas Pinder](https://github.com/thomaspinder) and [Daniel Dodd](https://github.com/Daniel-Dodd).
-
-We would be delighted to receive contributions from interested individuals and groups. To learn how you can get involved, please read our [guide for contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md). If you have any questions, we encourage you to [open an issue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For broader conversations, such as best GP fitting practices or questions about the mathematics of GPs, we invite you to [open a discussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).
-
-Feel free to join our [Slack Channel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw), where we can discuss the development of GPJax and broader support for Gaussian process modelling.
-
-# Supported methods and interfaces
-
-## Notebook examples
-
-> - [**Conjugate Inference**](https://gpjax.readthedocs.io/en/latest/examples/regression.html)
-> - [**Classification with MCMC**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
-> - [**Sparse Variational Inference**](https://gpjax.readthedocs.io/en/latest/examples/uncollapsed_vi.html)
-> - [**BlackJax Integration**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
-> - [**Laplace Approximation**](https://gpjax.readthedocs.io/en/latest/examples/classification.html#Laplace-approximation)
-> - [**TensorFlow Probability Integration**](https://gpjax.readthedocs.io/en/latest/examples/tfp_integration.html)
-> - [**Inference on Non-Euclidean Spaces**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
-> - [**Inference on Graphs**](https://gpjax.readthedocs.io/en/latest/examples/graph_kernels.html)
-> - [**Learning Gaussian Process Barycentres**](https://gpjax.readthedocs.io/en/latest/examples/barycentres.html)
-> - [**Deep Kernel Regression**](https://gpjax.readthedocs.io/en/latest/examples/haiku.html)
-> - [**Natural Gradients**](https://gpjax.readthedocs.io/en/latest/examples/natgrads.html)
-
-## Guides for customisation
-> 
-> - [**Custom kernels**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
-> - [**UCI regression**](https://gpjax.readthedocs.io/en/latest/examples/yacht.html)
-
-## Conversion between `.ipynb` and `.py`
-Above examples are stored in [examples](examples) directory in the double percent (`py:percent`) format. Checkout [jupytext using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more info.
-
-* To convert `example.py` to `example.ipynb`, run:
-
-```bash
-jupytext --to notebook example.py
-```
-
-* To convert `example.ipynb` to `example.py`, run:
-
-```bash
-jupytext --to py:percent example.ipynb
-```
-
-# Simple example
-
-Let us import some dependencies and simulate a toy dataset $\mathcal{D}$.
-
-```python
-import gpjax as gpx
-from jax import grad, jit
-import jax.numpy as jnp
-import jax.random as jr
-import jaxkern as jk
-import optax as ox
-
-key = jr.PRNGKey(123)
-
-f = lambda x: 10 * jnp.sin(x)
-
-n = 50
-x = jr.uniform(key=key, minval=-3.0, maxval=3.0, shape=(n,1)).sort()
-y = f(x) + jr.normal(key, shape=(n,1))
-D = gpx.Dataset(X=x, y=y)
-```
-
-The function of interest here, $f(\cdot)$, is sinusoidal, but our observations of it have been perturbed by Gaussian noise. We aim to utilise a Gaussian process to try and recover this latent function.
-
-## 1. Constructing the prior and posterior
-
-We begin by defining a zero-mean Gaussian process prior with a radial basis function kernel and assume the likelihood to be Gaussian.
-
-```python
-prior = gpx.Prior(kernel = jk.RBF())
-likelihood = gpx.Gaussian(num_datapoints = n)
-```
-
-Similar to how we would write on paper, the posterior is constructed by the product of our prior with our likelihood.
-
-```python
-posterior = prior * likelihood
-```
-
-## 2. Learning hyperparameters
-
-Equipped with the posterior, we seek to learn the model's hyperparameters through gradient-optimisation of the marginal log-likelihood. We this below, adding Jax's [just-in-time (JIT)](https://jax.readthedocs.io/en/latest/jax-101/02-jitting.html) compilation to accelerate training. 
-
-```python
-mll = jit(posterior.marginal_log_likelihood(D, negative=True))
-```
-
-For purposes of optimisation, we'll use optax's Adam.
-```
-opt = ox.adam(learning_rate=1e-3)
-```
-
-We define an initial parameter state through the `initialise` callable.
-
-```python
-parameter_state = gpx.initialise(posterior, key=key)
-```
-
-Finally, we run an optimisation loop using the Adam optimiser via the `fit` callable.
-
-```python
-inference_state = gpx.fit(mll, parameter_state, opt, num_iters=500)
-```
-
-## 3. Making predictions
-
-Using our learned hyperparameters, we can obtain the posterior distribution of the latent function at novel test points.
-
-```python
-learned_params, _ = inference_state.unpack()
-xtest = jnp.linspace(-3., 3., 100).reshape(-1, 1)
-
-latent_distribution = posterior(learned_params, D)(xtest)
-predictive_distribution = likelihood(learned_params, latent_distribution)
-
-predictive_mean = predictive_distribution.mean()
-predictive_cov = predictive_distribution.covariance()
-```
-
-# Installation
-
-## Stable version
-
-The latest stable version of GPJax can be installed via [`pip`](https://pip.pypa.io/en/stable/):
-
-```bash
-pip install gpjax
-```
-
-> **Note**
->
-> We recommend you check your installation version:
-> ```python
-> python -c 'import gpjax; print(gpjax.__version__)'
-> ```
-
-
-
-## Development version
-> **Warning**
->
-> This version is possibly unstable and may contain bugs. 
-
-Clone a copy of the repository to your local machine and run the setup configuration in development mode.
-```bash
-git clone https://github.com/JaxGaussianProcesses/GPJax.git
-cd GPJax
-python setup.py develop
-```
-
-> **Note**
->
-> We advise you create virtual environment before installing:
-> ```
-> conda create -n gpjax_experimental python=3.10.0
-> conda activate gpjax_experimental
->  ```
->
-> and recommend you check your installation passes the supplied unit tests:
->
-> ```python
-> python -m pytest tests/
-> ```
-
-# Citing GPJax
+packages = \
+['gpjax',
+ 'gpjax.base',
+ 'gpjax.kernels',
+ 'gpjax.kernels.approximations',
+ 'gpjax.kernels.computations',
+ 'gpjax.kernels.non_euclidean',
+ 'gpjax.kernels.nonstationary',
+ 'gpjax.kernels.stationary',
+ 'gpjax.linops']
+
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['beartype>=0.13.1,<0.14.0',
+ 'jax>=0.4.1',
+ 'jaxlib>=0.4.6,<0.5.0',
+ 'jaxtyping>=0.2.15,<0.3.0',
+ 'optax>=0.1.4,<0.2.0',
+ 'orbax-checkpoint>=0.2.0,<0.3.0',
+ 'simple-pytree>=0.1.7,<0.2.0',
+ 'tensorflow-probability>=0.19.0,<0.20.0',
+ 'tqdm>=4.65.0,<5.0.0']
+
+setup_kwargs = {
+    'name': 'gpjax',
+    'version': '0.6',
+    'description': 'Gaussian processes in JAX.',
+    'long_description': '<!-- <h1 align=\'center\'>GPJax</h1>\n<h2 align=\'center\'>Gaussian processes in Jax.</h2> -->\n<p align="center">\n<img width="700" height="300" src="https://github.com/JaxGaussianProcesses/GPJax/raw/master/docs/_static/gpjax_logo.svg" alt="GPJax\'s logo">\n</p>\n\n[![codecov](https://codecov.io/gh/JaxGaussianProcesses/GPJax/branch/master/graph/badge.svg?token=DM1DRDASU2)](https://codecov.io/gh/JaxGaussianProcesses/GPJax)\n[![CodeFactor](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax/badge)](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax)\n[![Documentation Status](https://readthedocs.org/projects/gpjax/badge/?version=latest)](https://gpjax.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/GPJax.svg)](https://badge.fury.io/py/GPJax)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.04455/status.svg)](https://doi.org/10.21105/joss.04455)\n[![Downloads](https://pepy.tech/badge/gpjax)](https://pepy.tech/project/gpjax)\n[![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)\n\n[**Quickstart**](#simple-example)\n| [**Install guide**](#installation)\n| [**Documentation**](https://gpjax.readthedocs.io/en/latest/)\n| [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)\n\nGPJax aims to provide a low-level interface to Gaussian process (GP) models in\n[Jax](https://github.com/google/jax), structured to give researchers maximum\nflexibility in extending the code to suit their own needs. The idea is that the\ncode should be as close as possible to the maths we write on paper when working\nwith GP models.\n\n# Package support\n\nGPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today,\nthe maintenance of GPJax is undertaken by [Thomas\nPinder](https://github.com/thomaspinder) and [Daniel\nDodd](https://github.com/Daniel-Dodd).\n\nWe would be delighted to receive contributions from interested individuals and\ngroups. To learn how you can get involved, please read our [guide for\ncontributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md).\nIf you have any questions, we encourage you to [open an\nissue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For\nbroader conversations, such as best GP fitting practices or questions about the\nmathematics of GPs, we invite you to [open a\ndiscussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).\n\nFeel free to join our [Slack\nChannel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw),\nwhere we can discuss the development of GPJax and broader support for Gaussian\nprocess modelling.\n\n# Supported methods and interfaces\n\n## Notebook examples\n\n> - [**Conjugate Inference**](https://gpjax.readthedocs.io/en/latest/examples/regression.html)\n> - [**Classification with MCMC**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)\n> - [**Sparse Variational Inference**](https://gpjax.readthedocs.io/en/latest/examples/uncollapsed_vi.html)\n> - [**BlackJax Integration**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)\n> - [**Laplace Approximation**](https://gpjax.readthedocs.io/en/latest/examples/classification.html#Laplace-approximation)\n> - [**Inference on Non-Euclidean Spaces**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)\n> - [**Inference on Graphs**](https://gpjax.readthedocs.io/en/latest/examples/graph_kernels.html)\n> - [**Learning Gaussian Process Barycentres**](https://gpjax.readthedocs.io/en/latest/examples/barycentres.html)\n> - [**Deep Kernel Regression**](https://gpjax.readthedocs.io/en/latest/examples/haiku.html)\n\n## Guides for customisation\n>\n> - [**Custom kernels**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)\n> - [**UCI regression**](https://gpjax.readthedocs.io/en/latest/examples/yacht.html)\n\n## Conversion between `.ipynb` and `.py`\nAbove examples are stored in [examples](examples) directory in the double\npercent (`py:percent`) format. Checkout [jupytext\nusing-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more\ninfo.\n\n* To convert `example.py` to `example.ipynb`, run:\n\n```bash\njupytext --to notebook example.py\n```\n\n* To convert `example.ipynb` to `example.py`, run:\n\n```bash\njupytext --to py:percent example.ipynb\n```\n\n# Simple example\n\nLet us import some dependencies and simulate a toy dataset $\\mathcal{D}$.\n\n```python\nimport gpjax as gpx\nfrom jax import grad, jit\nimport jax.numpy as jnp\nimport jax.random as jr\nimport optax as ox\n\nkey = jr.PRNGKey(123)\n\nf = lambda x: 10 * jnp.sin(x)\n\nn = 50\nx = jr.uniform(key=key, minval=-3.0, maxval=3.0, shape=(n,1)).sort()\ny = f(x) + jr.normal(key, shape=(n,1))\nD = gpx.Dataset(X=x, y=y)\n\n# Construct the prior\nmeanf = gpx.mean_functions.Zero()\nkernel = gpx.kernels.RBF()\nprior = gpx.Prior(mean_function=meanf, kernel = kernel)\n\n# Define a likelihood\nlikelihood = gpx.Gaussian(num_datapoints = n)\n\n# Construct the posterior\nposterior = prior * likelihood\n\n# Define an optimiser\noptimiser = ox.adam(learning_rate=1e-2)\n\n# Define the marginal log-likelihood\nnegative_mll = jit(gpx.objectives.ConjugateMLL(negative=True))\n\n# Obtain Type 2 MLEs of the hyperparameters\nopt_posterior, history = gpx.fit(\n    model=posterior,\n    objective=negative_mll,\n    train_data=D,\n    optim=optimiser,\n    num_iters=500,\n    safe=True,\n    key=key,\n)\n\n# Infer the predictive posterior distribution\nxtest = jnp.linspace(-3., 3., 100).reshape(-1, 1)\nlatent_dist = opt_posterior(xtest, D)\npredictive_dist = opt_posterior.likelihood(latent_dist)\n\n# Obtain the predictive mean and standard deviation\npred_mean = predictive_dist.mean()\npred_std = predictive_dist.stddev()\n```\n\n# Installation\n\n## Stable version\n\nThe latest stable version of GPJax can be installed via\npip:\n\n```bash\npip install gpjax\n```\n\n> **Note**\n>\n> We recommend you check your installation version:\n> ```python\n> python -c \'import gpjax; print(gpjax.__version__)\'\n> ```\n\n\n\n## Development version\n> **Warning**\n>\n> This version is possibly unstable and may contain bugs.\n\nClone a copy of the repository to your local machine and run the setup\nconfiguration in development mode.\n```bash\ngit clone https://github.com/JaxGaussianProcesses/GPJax.git\ncd GPJax\npoetry install\n```\n\n> **Note**\n>\n> We advise you create virtual environment before installing:\n> ```\n> conda create -n gpjax_experimental python=3.10.0\n> conda activate gpjax_experimental\n>  ```\n>\n> and recommend you check your installation passes the supplied unit tests:\n>\n> ```python\n> poetry run pytest\n> ```\n\n# Citing GPJax\n\nIf you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).\n\n```\n@article{Pinder2022,\n  doi = {10.21105/joss.04455},\n  url = {https://doi.org/10.21105/joss.04455},\n  year = {2022},\n  publisher = {The Open Journal},\n  volume = {7},\n  number = {75},\n  pages = {4455},\n  author = {Thomas Pinder and Daniel Dodd},\n  title = {GPJax: A Gaussian Process Framework in JAX},\n  journal = {Journal of Open Source Software}\n}\n```\n',
+    'author': 'Thomas Pinder',
+    'author_email': 'tompinder@live.co.uk',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/JaxGaussianProcesses/GPJax',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.8,<3.12',
+}
 
-If you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).
 
-```
-@article{Pinder2022,
-  doi = {10.21105/joss.04455},
-  url = {https://doi.org/10.21105/joss.04455},
-  year = {2022},
-  publisher = {The Open Journal},
-  volume = {7},
-  number = {75},
-  pages = {4455},
-  author = {Thomas Pinder and Daniel Dodd},
-  title = {GPJax: A Gaussian Process Framework in JAX},
-  journal = {Journal of Open Source Software}
-}
-```
+setup(**setup_kwargs)
```

### Comparing `gpjax-0.5.9/gpjax/__init__.py` & `gpjax-0.6/gpjax/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,72 +8,115 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-
-from .abstractions import fit, fit_batches, fit_natgrads
-from .gps import Prior, construct_posterior
-from .kernels import (
+from gpjax.base import (
+    Module,
+    param_field,
+)
+from gpjax.dataset import Dataset
+from gpjax.fit import fit
+from gpjax.gps import (
+    Prior,
+    construct_posterior,
+)
+from gpjax.kernels import (
     RBF,
+    RFF,
+    AbstractKernel,
+    BasisFunctionComputation,
+    ConstantDiagonalKernelComputation,
+    DenseKernelComputation,
+    DiagonalKernelComputation,
+    EigenKernelComputation,
     GraphKernel,
+    Linear,
     Matern12,
     Matern32,
     Matern52,
+    Periodic,
     Polynomial,
+    PoweredExponential,
     ProductKernel,
+    RationalQuadratic,
     SumKernel,
+    White,
+)
+from gpjax.likelihoods import (
+    Bernoulli,
+    Gaussian,
+    Poisson,
+)
+from gpjax.mean_functions import (
+    Constant,
+    Zero,
+)
+from gpjax.objectives import (
+    ELBO,
+    CollapsedELBO,
+    ConjugateMLL,
+    LogPosteriorDensity,
+    NonConjugateMLL,
 )
-from .likelihoods import Bernoulli, Gaussian
-from .mean_functions import Constant, Zero
-from .parameters import constrain, copy_dict_structure, initialise, unconstrain
-from .variational_families import (
+from gpjax.variational_families import (
     CollapsedVariationalGaussian,
     ExpectationVariationalGaussian,
     NaturalVariationalGaussian,
     VariationalGaussian,
     WhitenedVariationalGaussian,
 )
-from .types import Dataset
-from .variational_inference import CollapsedVI, StochasticVI
-from . import _version
 
-__version__ = _version.get_versions()["version"]
 __license__ = "MIT"
 __description__ = "Didactic Gaussian processes in JAX"
 __url__ = "https://github.com/thomaspinder/GPJax"
 __contributors__ = "https://github.com/thomaspinder/GPJax/graphs/contributors"
 
 
 __all__ = [
+    "Module",
+    "param_field",
+    "kernels",
     "fit",
-    "fit_batches",
-    "fit_natgrads",
     "Prior",
     "construct_posterior",
     "RBF",
     "GraphKernel",
     "Matern12",
     "Matern32",
     "Matern52",
     "Polynomial",
     "ProductKernel",
     "SumKernel",
     "Bernoulli",
     "Gaussian",
+    "Poisson",
     "Constant",
     "Zero",
-    "constrain",
-    "copy_dict_structure",
-    "initialise",
-    "unconstrain",
     "Dataset",
     "CollapsedVariationalGaussian",
     "ExpectationVariationalGaussian",
     "NaturalVariationalGaussian",
     "VariationalGaussian",
     "WhitenedVariationalGaussian",
     "CollapsedVI",
     "StochasticVI",
+    "ConjugateMLL",
+    "NonConjugateMLL",
+    "LogPosteriorDensity",
+    "CollapsedELBO",
+    "ELBO",
+    "AbstractKernel",
+    "Linear",
+    "DenseKernelComputation",
+    "DiagonalKernelComputation",
+    "ConstantDiagonalKernelComputation",
+    "EigenKernelComputation",
+    "PoweredExponential",
+    "Periodic",
+    "RationalQuadratic",
+    "White",
+    "BasisFunctionComputation",
+    "RFF",
 ]
```

### Comparing `gpjax-0.5.9/gpjax/gaussian_distribution.py` & `gpjax-0.6/gpjax/gaussian_distribution.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,85 +9,95 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-import jax.numpy as jnp
-from jaxlinop import LinearOperator, IdentityLinearOperator
 
-from jaxtyping import Array, Float
+from beartype.typing import (
+    Any,
+    Optional,
+    Tuple,
+)
 from jax import vmap
+import jax.numpy as jnp
+import jax.random as jr
+from jaxtyping import Float
+import tensorflow_probability.substrates.jax as tfp
 
-from typing import Tuple, Optional, Any
+from gpjax.linops import (
+    IdentityLinearOperator,
+    LinearOperator,
+)
+from gpjax.typing import (
+    Array,
+    KeyArray,
+    ScalarFloat,
+)
 
-import distrax as dx
-import jax.random as jr
-from jax.random import KeyArray
+tfd = tfp.distributions
 
 
 def _check_loc_scale(loc: Optional[Any], scale: Optional[Any]) -> None:
-    """Checks that the inputs are correct."""
-
+    r"""Checks that the inputs are correct."""
     if loc is None and scale is None:
         raise ValueError("At least one of `loc` or `scale` must be specified.")
 
     if loc is not None and loc.ndim < 1:
         raise ValueError("The parameter `loc` must have at least one dimension.")
 
     if scale is not None and scale.ndim < 2:
         raise ValueError(
-            f"The `scale` must have at least two dimensions, but "
+            "The `scale` must have at least two dimensions, but "
             f"`scale.shape = {scale.shape}`."
         )
 
     if scale is not None and not isinstance(scale, LinearOperator):
         raise ValueError(
             f"scale must be a LinearOperator or a JAX array, but got {type(scale)}"
         )
 
     if scale is not None and (scale.shape[-1] != scale.shape[-2]):
         raise ValueError(
-            f"The `scale` must be a square matrix, but "
-            f"`scale.shape = {scale.shape}`."
+            f"The `scale` must be a square matrix, but `scale.shape = {scale.shape}`."
         )
 
     if loc is not None:
         num_dims = loc.shape[-1]
         if scale is not None and (scale.shape[-1] != num_dims):
             raise ValueError(
                 f"Shapes are not compatible: `loc.shape = {loc.shape}` and "
                 f"`scale.shape = {scale.shape}`."
             )
 
 
-class GaussianDistribution(dx.Distribution):
-    """Multivariate Gaussian distribution with a linear operator scale matrix.
+class GaussianDistribution(tfd.Distribution):
+    r"""Multivariate Gaussian distribution with a linear operator scale matrix.
 
     Args:
-        loc (Optional[Float[Array, "N"]]): The mean of the distribution. Defaults to None.
+        loc (Optional[Float[Array, " N"]]): The mean of the distribution. Defaults to None.
         scale (Optional[LinearOperator]): The scale matrix of the distribution. Defaults to None.
 
-    Returns:
+    Returns
+    -------
         GaussianDistribution: A multivariate Gaussian distribution with a linear operator scale matrix.
     """
 
     # TODO: Consider `distrax.transformed.Transformed` object. Can we create a LinearOperator to `distrax.bijector` representation
     # and modify `distrax.MultivariateNormalFromBijector`?
 
     # TODO: Consider natural and expectation parameterisations in future work.
 
     def __init__(
         self,
-        loc: Optional[Float[Array, "N"]] = None,
+        loc: Optional[Float[Array, " N"]] = None,
         scale: Optional[LinearOperator] = None,
     ) -> None:
-        """Initialises the distribution."""
-
+        r"""Initialises the distribution."""
         _check_loc_scale(loc, scale)
 
         # Find dimensionality of the distribution.
         if loc is not None:
             num_dims = loc.shape[-1]
 
         elif scale is not None:
@@ -100,126 +110,139 @@
         # If not specified, set the scale to the identity matrix.
         if scale is None:
             scale = IdentityLinearOperator(num_dims)
 
         self.loc = loc
         self.scale = scale
 
-    def mean(self) -> Float[Array, "N"]:
-        """Calculates the mean."""
+    def mean(self) -> Float[Array, " N"]:
+        r"""Calculates the mean."""
         return self.loc
 
-    def median(self) -> Float[Array, "N"]:
-        """Calculates the median."""
+    def median(self) -> Float[Array, " N"]:
+        r"""Calculates the median."""
         return self.loc
 
-    def mode(self) -> Float[Array, "N"]:
-        """Calculates the mode."""
+    def mode(self) -> Float[Array, " N"]:
+        r"""Calculates the mode."""
         return self.loc
 
     def covariance(self) -> Float[Array, "N N"]:
-        """Calculates the covariance matrix."""
+        r"""Calculates the covariance matrix."""
         return self.scale.to_dense()
 
-    def variance(self) -> Float[Array, "N"]:
-        """Calculates the variance."""
+    def variance(self) -> Float[Array, " N"]:
+        r"""Calculates the variance."""
         return self.scale.diagonal()
 
-    def stddev(self) -> Float[Array, "N"]:
-        """Calculates the standard deviation."""
+    def stddev(self) -> Float[Array, " N"]:
+        r"""Calculates the standard deviation."""
         return jnp.sqrt(self.scale.diagonal())
 
     @property
     def event_shape(self) -> Tuple:
-        """Returns the event shape."""
+        r"""Returns the event shape."""
         return self.loc.shape[-1:]
 
-    def entropy(self) -> Float[Array, "1"]:
-        """Calculates the entropy of the distribution."""
+    def entropy(self) -> ScalarFloat:
+        r"""Calculates the entropy of the distribution."""
         return 0.5 * (
             self.event_shape[0] * (1.0 + jnp.log(2.0 * jnp.pi)) + self.scale.log_det()
         )
 
-    def log_prob(self, y: Float[Array, "N"]) -> Float[Array, "1"]:
-        """Calculates the log pdf of the multivariate Gaussian.
+    def log_prob(self, y: Float[Array, " N"]) -> ScalarFloat:
+        r"""Calculates the log pdf of the multivariate Gaussian.
 
         Args:
-            y (Float[Array, "N"]): The value to calculate the log probability of.
+            y (Float[Array, " N"]): The value to calculate the log probability of.
 
-        Returns:
-            Float[Array, "1"]: The log probability of the value.
+        Returns
+        -------
+            ScalarFloat: The log probability of the value.
         """
         mu = self.loc
         sigma = self.scale
         n = mu.shape[-1]
 
         # diff, y - µ
         diff = y - mu
 
         # compute the pdf, -1/2[ n log(2π) + log|Σ| + (y - µ)ᵀΣ⁻¹(y - µ) ]
         return -0.5 * (
             n * jnp.log(2.0 * jnp.pi) + sigma.log_det() + diff.T @ sigma.solve(diff)
         )
 
     def _sample_n(self, key: KeyArray, n: int) -> Float[Array, "n N"]:
-        """Samples from the distribution.
+        r"""Samples from the distribution.
 
         Args:
             key (KeyArray): The key to use for sampling.
 
-        Returns:
+        Returns
+        -------
             Float[Array, "n N"]: The samples.
         """
         # Obtain covariance root.
         sqrt = self.scale.to_root()
 
         # Gather n samples from standard normal distribution Z = [z₁, ..., zₙ]ᵀ.
         Z = jr.normal(key, shape=(n, *self.event_shape))
 
         # xᵢ ~ N(loc, cov) <=> xᵢ = loc + sqrt zᵢ, where zᵢ ~ N(0, I).
-        affine_transformation = lambda x: self.loc + sqrt @ x
+        def affine_transformation(x):
+            return self.loc + sqrt @ x
 
         return vmap(affine_transformation)(Z)
 
-    def kl_divergence(self, other: "GaussianDistribution") -> Float[Array, "1"]:
+    def sample(
+        self, seed: KeyArray, sample_shape: Tuple[int, ...]
+    ):  # pylint: disable=useless-super-delegation
+        r"""See `Distribution.sample`."""
+        return self._sample_n(
+            seed, sample_shape[0]
+        )  # TODO this looks weird, why ignore the second entry?
+
+    def kl_divergence(self, other: "GaussianDistribution") -> ScalarFloat:
         return _kl_divergence(self, other)
 
 
 def _check_and_return_dimension(
     q: GaussianDistribution, p: GaussianDistribution
 ) -> int:
-    """Checks that the dimensions of the distributions are compatible."""
+    r"""Checks that the dimensions of the distributions are compatible."""
     if q.event_shape != p.event_shape:
         raise ValueError(
-            f"Distribution event shapes are not compatible: `q.event_shape = {q.event_shape}` and "
-            f"`p.event_shape = {p.event_shape}`. Please check your mean and covariance shapes."
+            "Distribution event shapes are not compatible: `q.event_shape ="
+            f" {q.event_shape}` and `p.event_shape = {p.event_shape}`. Please check"
+            " your mean and covariance shapes."
         )
 
     return q.event_shape[-1]
 
 
-def _frobeinius_norm_squared(matrix: Float[Array, "N N"]) -> Float[Array, "1"]:
-    """Calculates the squared Frobenius norm of a matrix."""
+def _frobenius_norm_squared(matrix: Float[Array, "N N"]) -> ScalarFloat:
+    r"""Calculates the squared Frobenius norm of a matrix."""
     return jnp.sum(jnp.square(matrix))
 
 
-def _kl_divergence(
-    q: GaussianDistribution, p: GaussianDistribution
-) -> Float[Array, "1"]:
-    """Computes the KL divergence, KL[q||p], between two multivariate Gaussian distributions
-        q(x) = N(x; μq, Σq) and p(x) = N(x; μp, Σp).
+def _kl_divergence(q: GaussianDistribution, p: GaussianDistribution) -> ScalarFloat:
+    r"""KL-divergence between two Gaussians.
+
+    Computes the KL divergence, $`\operatorname{KL}[q\mid\mid p]`$, between two
+    multivariate Gaussian distributions $`q(x) = \mathcal{N}(x; \mu_q, \Sigma_q)`$
+    and $`p(x) = \mathcal{N}(x; \mu_p, \Sigma_p)`$.
 
     Args:
         q (GaussianDistribution): A multivariate Gaussian distribution.
-        p (GaussianDistribution): A multivariate Gaussia distribution.
+        p (GaussianDistribution): A multivariate Gaussian distribution.
 
-    Returns:
-        Float[Array, "1"]: The KL divergence between q and p.
+    Returns
+    -------
+        ScalarFloat: The KL divergence between q and p.
     """
-
     n_dim = _check_and_return_dimension(q, p)
 
     # Extract q mean and covariance.
     mu_q = q.loc
     sigma_q = q.scale
 
     # Extract p mean and covariance.
@@ -230,22 +253,22 @@
     sqrt_p = sigma_p.to_root()
     sqrt_q = sigma_q.to_root()
 
     # diff, μp - μq
     diff = mu_p - mu_q
 
     # trace term, tr[Σp⁻¹ Σq] = tr[(LpLpᵀ)⁻¹(LqLqᵀ)] = tr[(Lp⁻¹Lq)(Lp⁻¹Lq)ᵀ] = (fr[LqLp⁻¹])²
-    trace = _frobeinius_norm_squared(
+    trace = _frobenius_norm_squared(
         sqrt_p.solve(sqrt_q.to_dense())
     )  # TODO: Not most efficient, given the `to_dense()` call (e.g., consider diagonal p and q). Need to abstract solving linear operator against another linear operator.
 
     # Mahalanobis term, (μp - μq)ᵀ Σp⁻¹ (μp - μq) = tr [(μp - μq)ᵀ [LpLpᵀ]⁻¹ (μp - μq)] = (fr[Lp⁻¹(μp - μq)])²
-    mahalanobis = _frobeinius_norm_squared(
-        sqrt_p.solve(diff)
-    )  # TODO: Need to improve this. Perhaps add a Mahalanobis method to LinearOperators.
+    mahalanobis = jnp.sum(
+        jnp.square(sqrt_p.solve(diff))
+    )  # TODO: Need to improve this. Perhaps add a Mahalanobis method to ``LinearOperator``s.
 
     # KL[q(x)||p(x)] = [ [(μp - μq)ᵀ Σp⁻¹ (μp - μq)] - n - log|Σq| + log|Σp| + tr[Σp⁻¹ Σq] ] / 2
     return (mahalanobis - n_dim - sigma_q.log_det() + sigma_p.log_det() + trace) / 2.0
 
 
 __all__ = [
     "GaussianDistribution",
```

### Comparing `gpjax-0.5.9/gpjax/gps.py` & `gpjax-0.6/gpjax/gps.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,826 +10,707 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from abc import abstractmethod
-from typing import Any, Callable, Dict, Optional
+from dataclasses import dataclass
 
-import distrax as dx
+from beartype.typing import (
+    Any,
+    Callable,
+    Optional,
+)
 import jax.numpy as jnp
-from jaxtyping import Array, Float
-from jax.random import KeyArray
+from jax.random import (
+    PRNGKey,
+    normal,
+)
+from jaxtyping import (
+    Float,
+    Num,
+)
+
+from gpjax.base import (
+    Module,
+    param_field,
+    static_field,
+)
+from gpjax.dataset import Dataset
+from gpjax.gaussian_distribution import GaussianDistribution
+from gpjax.kernels import RFF
+from gpjax.kernels.base import AbstractKernel
+from gpjax.likelihoods import (
+    AbstractLikelihood,
+    Gaussian,
+)
+from gpjax.linops import identity
+from gpjax.mean_functions import AbstractMeanFunction
+from gpjax.typing import (
+    Array,
+    FunctionalSample,
+    KeyArray,
+)
+
+
+@dataclass
+class AbstractPrior(Module):
+    """Abstract Gaussian process prior."""
+
+    kernel: AbstractKernel
+    mean_function: AbstractMeanFunction
+    jitter: float = static_field(1e-6)
 
-from jaxlinop import identity
-from jaxkern.base import AbstractKernel
-from jaxutils import PyTree
+    def __call__(self, *args: Any, **kwargs: Any) -> GaussianDistribution:
+        r"""Evaluate the Gaussian process at the given points.
 
-from .config import get_global_config
-from .kernels import AbstractKernel
-from .likelihoods import AbstractLikelihood, Conjugate, NonConjugate
-from .mean_functions import AbstractMeanFunction, Zero
-from jaxutils import Dataset
-from .utils import concat_dictionaries
-from .gaussian_distribution import GaussianDistribution
-
-import deprecation
-
-
-class AbstractPrior(PyTree):
-    """Abstract Gaussian process prior.
-
-    All Gaussian processes priors should inherit from this class."""
-
-    def __call__(self, *args: Any, **kwargs: Any) -> dx.Distribution:
-        """Evaluate the Gaussian process at the given points. The output of this function
-        is a `Distrax distribution <https://github.com/deepmind/distrax>`_ from which the
+        The output of this function is a
+        [TensorFlow probability distribution](https://www.tensorflow.org/probability/api_docs/python/tfp/substrates/jax/distributions) from which the
         the latent function's mean and covariance can be evaluated and the distribution
         can be sampled.
 
-        Under the hood, ``__call__`` is calling the objects ``predict`` method. For this
-        reasons, classes inheriting the ``AbstractPrior`` class, should not overwrite the
-        ``__call__`` method and should instead define a ``predict`` method.
+        Under the hood, `__call__` is calling the objects `predict` method. For this
+        reasons, classes inheriting the `AbstractPrior` class, should not overwrite the
+        `__call__` method and should instead define a `predict` method.
 
         Args:
             *args (Any): The arguments to pass to the GP's `predict` method.
             **kwargs (Any): The keyword arguments to pass to the GP's `predict` method.
 
-        Returns:
-            dx.Distribution: A multivariate normal random variable representation of the Gaussian process.
+        Returns
+        -------
+            GaussianDistribution: A multivariate normal random variable representation
+                of the Gaussian process.
         """
         return self.predict(*args, **kwargs)
 
     @abstractmethod
-    def predict(self, *args: Any, **kwargs: Any) -> dx.Distribution:
-        """Compute the latent function's multivariate normal distribution for a
-        given set of parameters. For any class inheriting the ``AbstractPrior`` class,
+    def predict(self, *args: Any, **kwargs: Any) -> GaussianDistribution:
+        r"""Evaluate the predictive distribution.
+
+        Compute the latent function's multivariate normal distribution for a
+        given set of parameters. For any class inheriting the `AbstractPrior` class,
         this method must be implemented.
 
         Args:
             *args (Any): Arguments to the predict method.
             **kwargs (Any): Keyword arguments to the predict method.
 
-        Returns:
-            dx.Distribution: A multivariate normal random variable representation of the Gaussian process.
+        Returns
+        -------
+            GaussianDistribution: A multivariate normal random variable representation
+                of the Gaussian process.
         """
         raise NotImplementedError
 
-    @abstractmethod
-    def init_params(self, key: KeyArray) -> Dict:
-        """An initialisation method for the GP's parameters. This method should
-        be implemented for all classes that inherit the ``AbstractPrior`` class.
-        Whilst not always necessary, the method accepts a PRNG key to allow
-        for stochastic initialisation. The method should is most often invoked
-        through the ``initialise`` function given in GPJax.
-
-        Args:
-            key (KeyArray): The PRNG key.
-
-        Returns:
-            Dict: The initialised parameter set.
-        """
-        raise NotImplementedError
-
-    @deprecation.deprecated(
-        deprecated_in="0.5.7",
-        removed_in="0.6.0",
-        details="Use the ``init_params`` method for parameter initialisation.",
-    )
-    def _initialise_params(self, key: KeyArray) -> Dict:
-        """Deprecated method for initialising the GP's parameters. Succeded by ``init_params``."""
-        return self.init_params(key)
-
 
 #######################
 # GP Priors
 #######################
-
-
+@dataclass
 class Prior(AbstractPrior):
-    """A Gaussian process prior object. The GP is parameterised by a
-    `mean <https://gpjax.readthedocs.io/en/latest/api.html#module-gpjax.mean_functions>`_
-    and `kernel <https://gpjax.readthedocs.io/en/latest/api.html#module-gpjax.kernels>`_ function.
+    r"""A Gaussian process prior object.
 
-    A Gaussian process prior parameterised by a mean function :math:`m(\\cdot)` and a kernel
-    function :math:`k(\\cdot, \\cdot)` is given by
+    The GP is parameterised by a
+    [mean](https://gpjax.readthedocs.io/en/latest/api.html#module-gpjax.mean_functions)
+    and [kernel](https://gpjax.readthedocs.io/en/latest/api.html#module-gpjax.kernels)
+    function.
+
+    A Gaussian process prior parameterised by a mean function $`m(\cdot)`$ and a kernel
+    function $`k(\cdot, \cdot)`$ is given by
+    $`p(f(\cdot)) = \mathcal{GP}(m(\cdot), k(\cdot, \cdot))`$.
 
-    .. math::
-
-        p(f(\\cdot)) = \mathcal{GP}(m(\\cdot), k(\\cdot, \\cdot)).
-
-    To invoke a ``Prior`` distribution, only a kernel function is required. By
+    To invoke a `Prior` distribution, only a kernel function is required. By
     default, the mean function will be set to zero. In general, this assumption
     will be reasonable assuming the data being modelled has been centred.
 
     Example:
+    ```python
         >>> import gpjax as gpx
-        >>>
+
         >>> kernel = gpx.kernels.RBF()
-        >>> prior = gpx.Prior(kernel = kernel)
+        >>> meanf = gpx.mean_functions.Zero()
+        >>> prior = gpx.Prior(mean_function=meanf, kernel = kernel)
+    ```
     """
 
-    def __init__(
-        self,
-        kernel: AbstractKernel,
-        mean_function: Optional[AbstractMeanFunction] = Zero(),
-        name: Optional[str] = "GP prior",
-    ) -> None:
-        """Initialise the GP prior.
-
-        Args:
-            kernel (AbstractKernel): The kernel function used to parameterise the prior.
-            mean_function (Optional[MeanFunction]): The mean function used to parameterise the
-                prior. Defaults to zero.
-            name (Optional[str]): The name of the GP prior. Defaults to "GP prior".
-        """
-        self.kernel = kernel
-        self.mean_function = mean_function
-        self.name = name
-
     def __mul__(self, other: AbstractLikelihood):
-        """The product of a prior and likelihood is proportional to the
-        posterior distribution. By computing the product of a GP prior and a
-        likelihood object, a posterior GP object will be returned. Mathetically,
-        this can be described by:
-         .. math::
-
-             p(f(\\cdot) | y) \\propto p(y | f(\\cdot)) p(f(\\cdot)).
-
-         where :math:`p(y | f(\\cdot))` is the likelihood and :math:`p(f(\\cdot))`
-         is the prior.
-
-
-         Example:
-             >>> import gpjax as gpx
-             >>>
-             >>> kernel = gpx.kernels.RBF()
-             >>> prior = gpx.Prior(kernel = kernel)
-             >>> likelihood = gpx.likelihoods.Gaussian(num_datapoints=100)
-             >>>
-             >>> prior * likelihood
+        r"""Combine the prior with a likelihood to form a posterior distribution.
 
-         Args:
-             other (Likelihood): The likelihood distribution of the observed dataset.
+        The product of a prior and likelihood is proportional to the posterior
+        distribution. By computing the product of a GP prior and a likelihood
+        object, a posterior GP object will be returned. Mathematically, this can
+        be described by:
+        ```math
+        p(f(\cdot) \mid y) \propto p(y \mid f(\cdot))p(f(\cdot)),
+        ```
+        where $`p(y | f(\cdot))`$ is the likelihood and $`p(f(\cdot))`$ is the prior.
 
-         Returns:
-             Posterior: The relevant GP posterior for the given prior and
+        Example:
+        ```python
+            >>> import gpjax as gpx
+            >>>
+            >>> meanf = gpx.mean_functions.Zero()
+            >>> kernel = gpx.kernels.RBF()
+            >>> prior = gpx.Prior(mean_function=meanf, kernel = kernel)
+            >>> likelihood = gpx.likelihoods.Gaussian(num_datapoints=100)
+            >>>
+            >>> prior * likelihood
+        ```
+        Args:
+            other (Likelihood): The likelihood distribution of the observed dataset.
+
+        Returns
+        -------
+            Posterior: The relevant GP posterior for the given prior and
                 likelihood. Special cases are accounted for where the model
                 is conjugate.
         """
         return construct_posterior(prior=self, likelihood=other)
 
     def __rmul__(self, other: AbstractLikelihood):
-        """Reimplement the multiplication operator to allow for order-invariant
+        r"""Combine the prior with a likelihood to form a posterior distribution.
+
+        Reimplement the multiplication operator to allow for order-invariant
         product of a likelihood and a prior i.e., likelihood * prior.
 
         Args:
             other (Likelihood): The likelihood distribution of the observed
                 dataset.
 
-        Returns:
+        Returns
+        -------
             Posterior: The relevant GP posterior for the given prior and
                 likelihood. Special cases are accounted for where the model
                 is conjugate.
         """
         return self.__mul__(other)
 
-    def predict(
-        self, params: Dict
-    ) -> Callable[[Float[Array, "N D"]], GaussianDistribution]:
-        """Compute the predictive prior distribution for a given set of
+    def predict(self, test_inputs: Num[Array, "N D"]) -> GaussianDistribution:
+        r"""Compute the predictive prior distribution for a given set of
         parameters. The output of this function is a function that computes
-        a distrx distribution for a given set of inputs.
+        a TFP distribution for a given set of inputs.
 
         In the following example, we compute the predictive prior distribution
         and then evaluate it on the interval :math:`[0, 1]`:
 
         Example:
+        ```python
             >>> import gpjax as gpx
             >>> import jax.numpy as jnp
             >>>
             >>> kernel = gpx.kernels.RBF()
-            >>> prior = gpx.Prior(kernel = kernel)
+            >>> meanf = gpx.mean_functions.Zero()
+            >>> prior = gpx.Prior(mean_function=meanf, kernel = kernel)
             >>>
-            >>> parameter_state = gpx.initialise(prior)
-            >>> prior_predictive = prior.predict(parameter_state.params)
-            >>> prior_predictive(jnp.linspace(0, 1, 100))
+            >>> prior.predict(jnp.linspace(0, 1, 100))
+        ```
 
         Args:
-            params (Dict): The specific set of parameters for which the mean
-            function should be defined for.
+            test_inputs (Float[Array, "N D"]): The inputs at which to evaluate the
+                prior distribution.
 
-        Returns:
-            Callable[[Float[Array, "N D"]], GaussianDistribution]: A mean
-            function that accepts an input array for where the mean function
-            should be evaluated at. The mean function's value at these points is
-            then returned.
+        Returns
+        -------
+            GaussianDistribution: A multivariate normal random variable representation
+                of the Gaussian process.
         """
-        jitter = get_global_config()["jitter"]
-
-        # Unpack mean function and kernel
-        mean_function = self.mean_function
-        kernel = self.kernel
+        x = test_inputs
+        mx = self.mean_function(x)
+        Kxx = self.kernel.gram(x)
+        Kxx += identity(x.shape[0]) * self.jitter
 
-        def predict_fn(
-            test_inputs: Float[Array, "N D"]
-        ) -> GaussianDistribution:
+        return GaussianDistribution(jnp.atleast_1d(mx.squeeze()), Kxx)
 
-            # Unpack test inputs
-            t = test_inputs
-            n_test = test_inputs.shape[0]
-
-            μt = mean_function(params["mean_function"], t)
-            Ktt = kernel.gram(params["kernel"], t)
-            Ktt += identity(n_test) * jitter
+    def sample_approx(
+        self,
+        num_samples: int,
+        key: KeyArray,
+        num_features: Optional[int] = 100,
+    ) -> FunctionalSample:
+        r"""Approximate samples from the Gaussian process prior.
+
+        Build an approximate sample from the Gaussian process prior. This method
+        provides a function that returns the evaluations of a sample across any
+        given inputs.
+
+        In particular, we approximate the Gaussian processes' prior as the
+        finite feature approximation
+        $`\hat{f}(x) = \sum_{i=1}^m\phi_i(x)\theta_i`$ where $`\phi_i`$ are $`m`$ features
+        sampled from the Fourier feature decomposition of the model's kernel and
+        $`\theta_i`$ are samples from a unit Gaussian.
+
+        A key property of such functional samples is that the same sample draw is
+        evaluated for all queries. Consistency is a property that is prohibitively costly
+        to ensure when sampling exactly from the GP prior, as the cost of exact sampling
+        scales cubically with the size of the sample. In contrast, finite feature representations
+        can be evaluated with constant cost regardless of the required number of queries.
 
-            return GaussianDistribution(jnp.atleast_1d(μt.squeeze()), Ktt)
+        In the following example, we build 10 such samples and then evaluate them
+        over the interval $`[0, 1]`$:
 
-        return predict_fn
+        For a `prior` distribution, the following code snippet will
+        build and evaluate an approximate sample.
 
-    def init_params(self, key: KeyArray) -> Dict:
-        """Initialise the GP prior's parameter set.
+        Example:
+        ```python
+            >>> import gpjax as gpx
+            >>> import jax.numpy as jnp
+            >>> import jax.random as jr
+            >>> key = jr.PRNGKey(123)
+            >>>
+            >>> meanf = gpx.mean_functions.Zero()
+            >>> kernel = gpx.kernels.RBF()
+            >>> prior = gpx.Prior(mean_function=meanf, kernel = kernel)
+            >>>
+            >>> sample_fn = prior.sample_approx(10, key)
+            >>> sample_fn(jnp.linspace(0, 1, 100).reshape(-1, 1))
+        ```
 
         Args:
-            key (KeyArray): The PRNG key.
+            num_samples (int): The desired number of samples.
+            key (KeyArray): The random seed used for the sample(s).
+            num_features (int): The number of features used when approximating the
+                kernel.
 
-        Returns:
-            Dict: The initialised parameter set.
+        Returns
+        -------
+            FunctionalSample: A function representing an approximate sample from the
+                Gaussian process prior.
         """
-        return {
-            "kernel": self.kernel.init_params(key),
-            "mean_function": self.mean_function.init_params(key),
-        }
+
+        if (not isinstance(num_samples, int)) or num_samples <= 0:
+            raise ValueError("num_samples must be a positive integer")
+
+        # sample fourier features
+        fourier_feature_fn = _build_fourier_features_fn(self, num_features, key)
+
+        # sample fourier weights
+        feature_weights = normal(key, [num_samples, 2 * num_features])  # [B, L]
+
+        def sample_fn(test_inputs: Float[Array, "N D"]) -> Float[Array, "N B"]:
+            feature_evals = fourier_feature_fn(test_inputs)  # [N, L]
+            evaluated_sample = jnp.inner(feature_evals, feature_weights)  # [N, B]
+            return self.mean_function(test_inputs) + evaluated_sample
+
+        return sample_fn
 
 
 #######################
 # GP Posteriors
 #######################
-class AbstractPosterior(AbstractPrior):
-    """The base GP posterior object conditioned on an observed dataset. All
-    posterior objects should inherit from this class."""
-
-    def __init__(
-        self,
-        prior: AbstractPrior,
-        likelihood: AbstractLikelihood,
-        name: Optional[str] = "GP posterior",
-    ) -> None:
-        """Initialise the GP posterior object.
+@dataclass
+class AbstractPosterior(Module):
+    r"""Abstract Gaussian process posterior.
 
-        Args:
-            prior (Prior): The prior distribution of the GP.
-            likelihood (AbstractLikelihood): The likelihood distribution of the observed dataset.
-            name (Optional[str]): The name of the GP posterior. Defaults to "GP posterior".
-        """
-        self.prior = prior
-        self.likelihood = likelihood
-        self.name = name
+    The base GP posterior object conditioned on an observed dataset. All
+    posterior objects should inherit from this class.
+    """
 
-    @abstractmethod
-    def predict(self, *args: Any, **kwargs: Any) -> GaussianDistribution:
-        """Compute the predictive posterior distribution of the latent function
-        for a given set of parameters. For any class inheriting the
-        ``AbstractPosterior`` class, this method must be implemented.
+    prior: AbstractPrior
+    likelihood: AbstractLikelihood
+    jitter: float = static_field(1e-6)
+
+    def __call__(self, *args: Any, **kwargs: Any) -> GaussianDistribution:
+        r"""Evaluate the Gaussian process posterior at the given points.
+
+        The output of this function is a
+        [TFP distribution](https://www.tensorflow.org/probability/api_docs/python/tfp/substrates/jax/distributions)
+        from which the the latent function's mean and covariance can be
+        evaluated and the distribution can be sampled.
+
+        Under the hood, `__call__` is calling the objects `predict` method. For this
+        reasons, classes inheriting the `AbstractPrior` class, should not overwrite the
+        `__call__` method and should instead define a `predict` method.
 
         Args:
-            *args (Any): Arguments to the predict method. **kwargs (Any):
-            Keyword arguments to the predict method.
+            *args (Any): The arguments to pass to the GP's `predict` method.
+            **kwargs (Any): The keyword arguments to pass to the GP's `predict` method.
 
-        Returns:
-            GaussianDistribution: A multivariate normal random variable
-            representation of the Gaussian process.
+        Returns
+        -------
+            GaussianDistribution: A multivariate normal random variable representation
+                of the Gaussian process.
         """
-        raise NotImplementedError
+        return self.predict(*args, **kwargs)
 
-    def init_params(self, key: KeyArray) -> Dict:
-        """Initialise the parameter set of a GP posterior.
+    @abstractmethod
+    def predict(self, *args: Any, **kwargs: Any) -> GaussianDistribution:
+        r"""Compute the latent function's multivariate normal distribution for a
+        given set of parameters. For any class inheriting the `AbstractPrior` class,
+        this method must be implemented.
 
         Args:
-            key (KeyArray): The PRNG key.
+            *args (Any): Arguments to the predict method.
+            **kwargs (Any): Keyword arguments to the predict method.
 
-        Returns:
-            Dict: The initialised parameter set.
+        Returns
+        -------
+            GaussianDistribution: A multivariate normal random variable representation
+                of the Gaussian process.
         """
-        return concat_dictionaries(
-            self.prior.init_params(key),
-            {"likelihood": self.likelihood.init_params(key)},
-        )
+        raise NotImplementedError
 
 
+@dataclass
 class ConjugatePosterior(AbstractPosterior):
-    """A Gaussian process posterior distribution when the constituent likelihood
+    r"""A Conjuate Gaussian process posterior object.
+
+    A Gaussian process posterior distribution when the constituent likelihood
     function is a Gaussian distribution. In such cases, the latent function values
-    :math:`f` can be analytically integrated out of the posterior distribution.
+    $`f`$ can be analytically integrated out of the posterior distribution.
     As such, many computational operations can be simplified; something we make use
     of in this object.
 
-    For a Gaussian process prior :math:`p(\mathbf{f})` and a Gaussian likelihood
-    :math:`p(y | \\mathbf{f}) = \\mathcal{N}(y\\mid \mathbf{f}, \\sigma^2))` where
-    :math:`\mathbf{f} = f(\\mathbf{x})`, the predictive posterior distribution at
-    a set of inputs :math:`\\mathbf{x}` is given by
-
-    .. math::
-
-        p(\\mathbf{f}^{\\star}\mid \mathbf{y}) & = \\int p(\\mathbf{f}^{\\star} \\mathbf{f} \\mid \\mathbf{y})\\\\
-        & =\\mathcal{N}(\\mathbf{f}^{\\star} \\boldsymbol{\mu}_{\mid \mathbf{y}}, \\boldsymbol{\Sigma}_{\mid \mathbf{y}}
+    For a Gaussian process prior $`p(\mathbf{f})`$ and a Gaussian likelihood
+    $`p(y | \mathbf{f}) = \mathcal{N}(y\mid \mathbf{f}, \sigma^2))`$ where
+    $`\mathbf{f} = f(\mathbf{x})`$, the predictive posterior distribution at
+    a set of inputs $`\mathbf{x}`$ is given by
+    ```math
+    \begin{align}
+    p(\mathbf{f}^{\star}\mid \mathbf{y}) & = \int p(\mathbf{f}^{\star}, \mathbf{f} \mid \mathbf{y})\\
+        & =\mathcal{N}(\mathbf{f}^{\star} \boldsymbol{\mu}_{\mid \mathbf{y}}, \boldsymbol{\Sigma}_{\mid \mathbf{y}}
+    \end{align}
+    ```
     where
-
-    .. math::
-
-        \\boldsymbol{\mu}_{\mid \mathbf{y}} & = k(\\mathbf{x}^{\\star}, \\mathbf{x})\\left(k(\\mathbf{x}, \\mathbf{x}')+\\sigma^2\\mathbf{I}_n\\right)^{-1}\\mathbf{y}  \\\\
-        \\boldsymbol{\Sigma}_{\mid \mathbf{y}} & =k(\\mathbf{x}^{\\star}, \\mathbf{x}^{\\star\\prime}) -k(\\mathbf{x}^{\\star}, \\mathbf{x})\\left( k(\\mathbf{x}, \\mathbf{x}') + \\sigma^2\\mathbf{I}_n \\right)^{-1}k(\\mathbf{x}, \\mathbf{x}^{\\star}).
+    ```math
+    \begin{align}
+    \boldsymbol{\mu}_{\mid \mathbf{y}} & = k(\mathbf{x}^{\star}, \mathbf{x})\left(k(\mathbf{x}, \mathbf{x}')+\sigma^2\mathbf{I}_n\right)^{-1}\mathbf{y}  \\
+    \boldsymbol{\Sigma}_{\mid \mathbf{y}} & =k(\mathbf{x}^{\star}, \mathbf{x}^{\star\prime}) -k(\mathbf{x}^{\star}, \mathbf{x})\left( k(\mathbf{x}, \mathbf{x}') + \sigma^2\mathbf{I}_n \right)^{-1}k(\mathbf{x}, \mathbf{x}^{\star}).
+    \end{align}
+    ```
 
     Example:
-        >>> import gpjax as gpx
-        >>> import jax.numpy as jnp
-        >>>
-        >>> prior = gpx.Prior(kernel = gpx.kernels.RBF())
-        >>> likelihood = gpx.likelihoods.Gaussian()
-        >>>
-        >>> posterior = prior * likelihood
-    """
-
-    def __init__(
-        self,
-        prior: AbstractPrior,
-        likelihood: AbstractLikelihood,
-        name: Optional[str] = "GP posterior",
-    ) -> None:
-        """Initialise the conjugate GP posterior object.
+        ```python
+            >>> import gpjax as gpx
+            >>> import jax.numpy as jnp
 
-        Args:
-            prior (Prior): The prior distribution of the GP.
-            likelihood (AbstractLikelihood): The likelihood distribution of the observed dataset.
-            name (Optional[str]): The name of the GP posterior. Defaults to "GP posterior".
-        """
-        self.prior = prior
-        self.likelihood = likelihood
-        self.name = name
+            >>> prior = gpx.Prior(
+                    mean_function = gpx.mean_functions.Zero(),
+                    kernel = gpx.kernels.RBF()
+                )
+            >>> likelihood = gpx.likelihoods.Gaussian(num_datapoints=100)
+            >>>
+            >>> posterior = prior * likelihood
+        ```
+    """
 
     def predict(
         self,
-        params: Dict,
+        test_inputs: Num[Array, "N D"],
         train_data: Dataset,
-    ) -> Callable[[Float[Array, "N D"]], GaussianDistribution]:
-        """Conditional on a training data set, compute the GP's posterior
-        predictive distribution for a given set of parameters. The returned
-        function can be evaluated at a set of test inputs to compute the
-        corresponding predictive density.
+    ) -> GaussianDistribution:
+        r"""Query the predictive posterior distribution.
 
-        The predictive distribution of a conjugate GP is given by
-        .. math::
+        Conditional on a training data set, compute the GP's posterior
+        predictive distribution for a given set of parameters. The returned function
+        can be evaluated at a set of test inputs to compute the corresponding
+        predictive density.
 
-            p(\\mathbf{f}^{\\star}\mid \mathbf{y}) & = \\int p(\\mathbf{f}^{\\star} \\mathbf{f} \\mid \\mathbf{y})\\\\
-            & =\\mathcal{N}(\\mathbf{f}^{\\star} \\boldsymbol{\mu}_{\mid \mathbf{y}}, \\boldsymbol{\Sigma}_{\mid \mathbf{y}}
+        The predictive distribution of a conjugate GP is given by
+        $$
+            p(\mathbf{f}^{\star}\mid \mathbf{y}) & = \int p(\mathbf{f}^{\star} \mathbf{f} \mid \mathbf{y})\\
+            & =\mathcal{N}(\mathbf{f}^{\star} \boldsymbol{\mu}_{\mid \mathbf{y}}, \boldsymbol{\Sigma}_{\mid \mathbf{y}}
+        $$
         where
+        $$
+            \boldsymbol{\mu}_{\mid \mathbf{y}} & = k(\mathbf{x}^{\star}, \mathbf{x})\left(k(\mathbf{x}, \mathbf{x}')+\sigma^2\mathbf{I}_n\right)^{-1}\mathbf{y}  \\
+            \boldsymbol{\Sigma}_{\mid \mathbf{y}} & =k(\mathbf{x}^{\star}, \mathbf{x}^{\star\prime}) -k(\mathbf{x}^{\star}, \mathbf{x})\left( k(\mathbf{x}, \mathbf{x}') + \sigma^2\mathbf{I}_n \right)^{-1}k(\mathbf{x}, \mathbf{x}^{\star}).
+        $$
 
-        .. math::
-
-            \\boldsymbol{\mu}_{\mid \mathbf{y}} & = k(\\mathbf{x}^{\\star}, \\mathbf{x})\\left(k(\\mathbf{x}, \\mathbf{x}')+\\sigma^2\\mathbf{I}_n\\right)^{-1}\\mathbf{y}  \\\\
-            \\boldsymbol{\Sigma}_{\mid \mathbf{y}} & =k(\\mathbf{x}^{\\star}, \\mathbf{x}^{\\star\\prime}) -k(\\mathbf{x}^{\\star}, \\mathbf{x})\\left( k(\\mathbf{x}, \\mathbf{x}') + \\sigma^2\\mathbf{I}_n \\right)^{-1}k(\\mathbf{x}, \\mathbf{x}^{\\star}).
-
-        The conditioning set is a GPJax ``Dataset`` object, whilst predictions
+        The conditioning set is a GPJax `Dataset` object, whilst predictions
         are made on a regular Jax array.
 
-        £xample:
-            For a ``posterior`` distribution, the following code snippet will
+        Example:
+            For a `posterior` distribution, the following code snippet will
             evaluate the predictive distribution.
-
-            >>> import gpjax as gpx
-            >>>
-            >>> xtrain = jnp.linspace(0, 1).reshape(-1, 1)
-            >>> ytrain = jnp.sin(xtrain)
-            >>> xtest = jnp.linspace(0, 1).reshape(-1, 1)
-            >>>
-            >>> params = gpx.initialise(posterior)
-            >>> predictive_dist = posterior.predict(params, gpx.Dataset(X=xtrain, y=ytrain))
-            >>> predictive_dist(xtest)
-
-        Args:
-            params (Dict): A dictionary of parameters that should be used to
-                compute the posterior.
-            train_data (Dataset): A `gpx.Dataset` object that contains the
-                input and output data used for training dataset.
-
-        Returns:
-            Callable[[Float[Array, "N D"]], GaussianDistribution]: A
+            ```python
+                >>> import gpjax as gpx
+                >>> import jax.numpy as jnp
+                >>>
+                >>> xtrain = jnp.linspace(0, 1).reshape(-1, 1)
+                >>> ytrain = jnp.sin(xtrain)
+                >>> D = gpx.Dataset(X=xtrain, y=ytrain)
+                >>> xtest = jnp.linspace(0, 1).reshape(-1, 1)
+                >>>
+                >>> prior = gpx.Prior(mean_function = gpx.Zero(), kernel = gpx.RBF())
+                >>> posterior = prior * gpx.Gaussian(num_datapoints = D.n)
+                >>> predictive_dist = posterior(xtest, D)
+            ```
+
+        Args:
+            test_inputs (Num[Array, "N D"]): A Jax array of test inputs at which the
+                predictive distribution is evaluated.
+            train_data (Dataset): A `gpx.Dataset` object that contains the input and
+                output data used for training dataset.
+
+        Returns
+        -------
+            GaussianDistribution: A
                 function that accepts an input array and returns the predictive
-                distribution as a ``GaussianDistribution``.
+                    distribution as a `GaussianDistribution`.
         """
-        jitter = get_global_config()["jitter"]
-
         # Unpack training data
         x, y, n = train_data.X, train_data.y, train_data.n
 
-        # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        # Unpack test inputs
+        t, n_test = test_inputs, test_inputs.shape[0]
 
-        # Observation noise σ²
-        obs_noise = params["likelihood"]["obs_noise"]
-        μx = mean_function(params["mean_function"], x)
+        # Observation noise o²
+        obs_noise = self.likelihood.obs_noise
+        mx = self.prior.mean_function(x)
 
         # Precompute Gram matrix, Kxx, at training inputs, x
-        Kxx = kernel.gram(params["kernel"], x)
-        Kxx += identity(n) * jitter
+        Kxx = self.prior.kernel.gram(x) + (identity(n) * self.prior.jitter)
 
-        # Σ = Kxx + Iσ²
+        # Σ = Kxx + Io²
         Sigma = Kxx + identity(n) * obs_noise
 
-        def predict(test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
-            """Compute the predictive distribution at a set of test inputs.
-
-            Args:
-                test_inputs (Float[Array, "N D"]): A Jax array of test inputs.
+        mean_t = self.prior.mean_function(t)
+        Ktt = self.prior.kernel.gram(t)
+        Kxt = self.prior.kernel.cross_covariance(x, t)
 
-            Returns:
-                GaussianDistribution: A ``GaussianDistribution``
-                object that represents the predictive distribution.
-            """
+        # Σ⁻¹ Kxt
+        Sigma_inv_Kxt = Sigma.solve(Kxt)
 
-            # Unpack test inputs
-            t = test_inputs
-            n_test = test_inputs.shape[0]
+        # μt  +  Ktx (Kxx + Io²)⁻¹ (y  -  μx)
+        mean = mean_t + jnp.matmul(Sigma_inv_Kxt.T, y - mx)
 
-            μt = mean_function(params["mean_function"], t)
-            Ktt = kernel.gram(params["kernel"], t)
-            Kxt = kernel.cross_covariance(params["kernel"], x, t)
+        # Ktt  -  Ktx (Kxx + Io²)⁻¹ Kxt, TODO: Take advantage of covariance structure to compute Schur complement more efficiently.
+        covariance = Ktt - jnp.matmul(Kxt.T, Sigma_inv_Kxt)
+        covariance += identity(n_test) * self.prior.jitter
 
-            # Σ⁻¹ Kxt
-            Sigma_inv_Kxt = Sigma.solve(Kxt)
+        return GaussianDistribution(jnp.atleast_1d(mean.squeeze()), covariance)
 
-            # μt  +  Ktx (Kxx + Iσ²)⁻¹ (y  -  μx)
-            mean = μt + jnp.matmul(Sigma_inv_Kxt.T, y - μx)
-
-            # Ktt  -  Ktx (Kxx + Iσ²)⁻¹ Kxt, TODO: Take advantage of covariance structure to compute Schur complement more efficiently.
-            covariance = Ktt - jnp.matmul(Kxt.T, Sigma_inv_Kxt)
-            covariance += identity(n_test) * jitter
-
-            return GaussianDistribution(
-                jnp.atleast_1d(mean.squeeze()), covariance
-            )
-
-        return predict
-
-    def marginal_log_likelihood(
+    def sample_approx(
         self,
+        num_samples: int,
         train_data: Dataset,
-        negative: bool = False,
-    ) -> Callable[[Dict], Float[Array, "1"]]:
-        """Compute the marginal log-likelihood function of the Gaussian process.
-        The returned function can then be used for gradient based optimisation
-        of the model's parameters or for model comparison. The implementation
-        given here enables exact estimation of the Gaussian process' latent
-        function values.
-
-        For a training dataset :math:`\\{x_n, y_n\\}_{n=1}^N`, set of test
-        inputs :math:`\\mathbf{x}^{\\star}` the corresponding latent function
-        evaluations are given by :math:`\\mathbf{f} = f(\\mathbf{x})`
-        and :math:`\\mathbf{f}^{\\star} = f(\\mathbf{x}^{\\star})`, the marginal
-        log-likelihood is given by:
-
-        .. math::
-
-            \\log p(\\mathbf{y}) & = \\int p(\\mathbf{y}\\mid\\mathbf{f})p(\\mathbf{f}, \\mathbf{f}^{\\star}\\mathrm{d}\\mathbf{f}^{\\star}\\\\
-            &=0.5\\left(-\\mathbf{y}^{\\top}\\left(k(\\mathbf{x}, \\mathbf{x}') +\\sigma^2\\mathbf{I}_N  \\right)^{-1}\\mathbf{y}-\\log\\lvert k(\\mathbf{x}, \\mathbf{x}') + \\sigma^2\\mathbf{I}_N\\rvert - n\\log 2\\pi \\right).
-
-        Example:
-
-        For a given ``ConjugatePosterior`` object, the following code snippet shows
-        how the marginal log-likelihood can be evaluated.
-
-        >>> import gpjax as gpx
-        >>>
-        >>> xtrain = jnp.linspace(0, 1).reshape(-1, 1)
-        >>> ytrain = jnp.sin(xtrain)
-        >>> D = gpx.Dataset(X=xtrain, y=ytrain)
-        >>>
-        >>> params = gpx.initialise(posterior)
-        >>> mll = posterior.marginal_log_likelihood(train_data = D)
-        >>> mll(params)
-
-        Our goal is to maximise the marginal log-likelihood. Therefore, when
-        optimising the model's parameters with respect to the parameters, we
-        use the negative marginal log-likelihood. This can be realised through
-
-        >>> mll = posterior.marginal_log_likelihood(train_data = D, negative=True)
-
-        Further, prior distributions can be passed into the marginal log-likelihood
-
-        >>> mll = posterior.marginal_log_likelihood(train_data = D)
-
-        For optimal performance, the marginal log-likelihood should be ``jax.jit``
-        compiled.
-
-        >>> mll = jit(posterior.marginal_log_likelihood(train_data = D))
-
-        Args:
-            train_data (Dataset): The training dataset used to compute the
-                marginal log-likelihood.
-            negative (Optional[bool]): Whether or not the returned function
-                should be negative. For optimisation, the negative is useful
-                as minimisation of the negative marginal log-likelihood is
-                equivalent to maximisation of the marginal log-likelihood.
-                Defaults to False.
-
-        Returns:
-            Callable[[Dict], Float[Array, "1"]]: A functional representation
-                of the marginal log-likelihood that can be evaluated at a
-                given parameter set.
-        """
-        jitter = get_global_config()["jitter"]
-
-        # Unpack training data
-        x, y, n = train_data.X, train_data.y, train_data.n
-
-        # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
-
-        # The sign of the marginal log-likelihood depends on whether we are maximising or minimising
-        constant = jnp.array(-1.0) if negative else jnp.array(1.0)
-
-        def mll(
-            params: Dict,
-        ):
-            """Compute the marginal log-likelihood of the Gaussian process.
-
-            Args:
-                params (Dict): The model's parameters.
-
-            Returns:
-                Float[Array, "1"]: The marginal log-likelihood.
-            """
-
-            # Observation noise σ²
-            obs_noise = params["likelihood"]["obs_noise"]
-            μx = mean_function(params["mean_function"], x)
-
-            # TODO: This implementation does not take advantage of the covariance operator structure.
-            # Future work concerns implementation of a custom Gaussian distribution / measure object that accepts a covariance operator.
-
-            # Σ = (Kxx + Iσ²) = LLᵀ
-            Kxx = kernel.gram(params["kernel"], x)
-            Kxx += identity(n) * jitter
-            Sigma = Kxx + identity(n) * obs_noise
-
-            # p(y | x, θ), where θ are the model hyperparameters:
-            marginal_likelihood = GaussianDistribution(
-                jnp.atleast_1d(μx.squeeze()), Sigma
+        key: KeyArray,
+        num_features: Optional[int] = 100,
+    ) -> FunctionalSample:
+        r"""Draw approximate samples from the Gaussian process posterior.
+
+        Build an approximate sample from the Gaussian process posterior. This method
+        provides a function that returns the evaluations of a sample across any given
+        inputs.
+
+        Unlike when building approximate samples from a Gaussian process prior, decompositions
+        based on Fourier features alone rarely give accurate samples. Therefore, we must also
+        include an additional set of features (known as canonical features) to better model the
+        transition from Gaussian process prior to Gaussian process posterior. For more details
+        see [Wilson et. al. (2020)](https://arxiv.org/abs/2002.09309).
+
+        In particular, we approximate the Gaussian processes' posterior as the finite
+        feature approximation
+        $`\hat{f}(x) = \sum_{i=1}^m \phi_i(x)\theta_i + \sum{j=1}^N v_jk(.,x_j)`$
+        where $`\phi_i`$ are m features sampled from the Fourier feature decomposition of
+        the model's kernel and $`k(., x_j)`$ are N canonical features. The Fourier
+        weights $`\theta_i`$ are samples from a unit Gaussian. See
+        [Wilson et. al. (2020)](https://arxiv.org/abs/2002.09309) for expressions
+        for the canonical weights $`v_j`$.
+
+        A key property of such functional samples is that the same sample draw is
+        evaluated for all queries. Consistency is a property that is prohibitively costly
+        to ensure when sampling exactly from the GP prior, as the cost of exact sampling
+        scales cubically with the size of the sample. In contrast, finite feature representations
+        can be evaluated with constant cost regardless of the required number of queries.
+
+        Args:
+            num_samples (int): The desired number of samples.
+            key (KeyArray): The random seed used for the sample(s).
+            num_features (int): The number of features used when approximating the
+                kernel.
+
+        Returns
+        -------
+            FunctionalSample: A function representing an approximate sample from the Gaussian
+            process prior.
+        """
+        if (not isinstance(num_samples, int)) or num_samples <= 0:
+            raise ValueError("num_samples must be a positive integer")
+
+        # sample fourier features
+        fourier_feature_fn = _build_fourier_features_fn(self.prior, num_features, key)
+
+        # sample fourier weights
+        fourier_weights = normal(key, [num_samples, 2 * num_features])  # [B, L]
+
+        # sample weights v for canonical features
+        # v = Σ⁻¹ (y + ε - ɸ⍵) for  Σ = Kxx + Io² and ε ᯈ N(0, o²)
+        Kxx = self.prior.kernel.gram(train_data.X)  #  [N, N]
+        Sigma = Kxx + identity(train_data.n) * (
+            self.likelihood.obs_noise + self.jitter
+        )  #  [N, N]
+        eps = jnp.sqrt(self.likelihood.obs_noise) * normal(
+            key, [train_data.n, num_samples]
+        )  #  [N, B]
+        y = train_data.y - self.prior.mean_function(train_data.X)  # account for mean
+        Phi = fourier_feature_fn(train_data.X)
+        canonical_weights = Sigma.solve(
+            y + eps - jnp.inner(Phi, fourier_weights)
+        )  #  [N, B]
+
+        def sample_fn(test_inputs: Float[Array, "n D"]) -> Float[Array, "n B"]:
+            fourier_features = fourier_feature_fn(test_inputs)  # [n, L]
+            weight_space_contribution = jnp.inner(
+                fourier_features, fourier_weights
+            )  # [n, B]
+            canonical_features = self.prior.kernel.cross_covariance(
+                test_inputs, train_data.X
+            )  # [n, N]
+            function_space_contribution = jnp.matmul(
+                canonical_features, canonical_weights
             )
 
-            return constant * (
-                marginal_likelihood.log_prob(
-                    jnp.atleast_1d(y.squeeze())
-                ).squeeze()
+            return (
+                self.prior.mean_function(test_inputs)
+                + weight_space_contribution
+                + function_space_contribution
             )
 
-        return mll
+        return sample_fn
 
 
+@dataclass
 class NonConjugatePosterior(AbstractPosterior):
-    """
+    r"""A non-conjugate Gaussian process posterior object.
+
     A Gaussian process posterior object for models where the likelihood is
-    non-Gaussian. Unlike the ``ConjugatePosterior`` object, the
-    ``NonConjugatePosterior`` object does not provide an exact marginal
-    log-likelihood function. Instead, the ``NonConjugatePosterior`` object
+    non-Gaussian. Unlike the `ConjugatePosterior` object, the
+    `NonConjugatePosterior` object does not provide an exact marginal
+    log-likelihood function. Instead, the `NonConjugatePosterior` object
     represents the posterior distributions as a function of the model's
     hyperparameters and the latent function. Markov chain Monte Carlo,
     variational inference, or Laplace approximations can then be used to sample
     from, or optimise an approximation to, the posterior distribution.
     """
 
-    def __init__(
-        self,
-        prior: AbstractPrior,
-        likelihood: AbstractLikelihood,
-        name: Optional[str] = "GP posterior",
-    ) -> None:
-        """Initialise a non-conjugate Gaussian process posterior object.
-
-        Args:
-            prior (AbstractPrior): The Gaussian process prior distribution.
-            likelihood (AbstractLikelihood): The likelihood function that represents the data.
-            name (Optional[str]): The name of the posterior object. Defaults to "GP posterior".
-        """
-        self.prior = prior
-        self.likelihood = likelihood
-        self.name = name
-
-    def init_params(self, key: KeyArray) -> Dict:
-        """Initialise the parameter set of a non-conjugate GP posterior.
-
-        Args:
-            key (KeyArray): A PRNG key used to initialise the parameters.
-
-        Returns:
-            Dict: A dictionary containing the default parameter set.
-        """
-        parameters = concat_dictionaries(
-            self.prior.init_params(key),
-            {"likelihood": self.likelihood.init_params(key)},
-        )
-        parameters["latent"] = jnp.zeros(
-            shape=(self.likelihood.num_datapoints, 1)
-        )
-        return parameters
+    latent: Float[Array, "N 1"] = param_field(None)
+    key: KeyArray = static_field(PRNGKey(42))
+
+    def __post_init__(self):
+        if self.latent is None:
+            self.latent = normal(self.key, shape=(self.likelihood.num_datapoints, 1))
 
     def predict(
-        self,
-        params: Dict,
-        train_data: Dataset,
-    ) -> Callable[[Float[Array, "N D"]], dx.Distribution]:
-        """
+        self, test_inputs: Num[Array, "N D"], train_data: Dataset
+    ) -> GaussianDistribution:
+        r"""Query the predictive posterior distribution.
+
         Conditional on a set of training data, compute the GP's posterior
         predictive distribution for a given set of parameters. The returned
         function can be evaluated at a set of test inputs to compute the
         corresponding predictive density. Note, to gain predictions on the scale
         of the original data, the returned distribution will need to be
         transformed through the likelihood function's inverse link function.
 
         Args:
-            params (Dict): A dictionary of parameters that should be used to
-                compute the posterior.
             train_data (Dataset): A `gpx.Dataset` object that contains the input
                 and output data used for training dataset.
 
-        Returns:
-            Callable[[Array], dx.Distribution]: A function that accepts an
+        Returns
+        -------
+            GaussianDistribution: A function that accepts an
                 input array and returns the predictive distribution as
-                a ``dx.Distribution``.
+                a `dx.Distribution`.
         """
-        jitter = get_global_config()["jitter"]
-
         # Unpack training data
         x, n = train_data.X, train_data.n
 
         # Unpack mean function and kernel
         mean_function = self.prior.mean_function
         kernel = self.prior.kernel
 
         # Precompute lower triangular of Gram matrix, Lx, at training inputs, x
-        Kxx = kernel.gram(params["kernel"], x)
-        Kxx += identity(n) * jitter
+        Kxx = kernel.gram(x)
+        Kxx += identity(n) * self.prior.jitter
         Lx = Kxx.to_root()
 
-        def predict_fn(test_inputs: Float[Array, "N D"]) -> dx.Distribution:
-            """Predictive distribution of the latent function for a given set of test inputs.
-
-            Args:
-                test_inputs (Float[Array, "N D"]): A set of test inputs.
-
-            Returns:
-                dx.Distribution: The predictive distribution of the latent function.
-            """
+        # Unpack test inputs
+        t, n_test = test_inputs, test_inputs.shape[0]
 
-            # Unpack test inputs
-            t, n_test = test_inputs, test_inputs.shape[0]
+        # Compute terms of the posterior predictive distribution
+        Ktx = kernel.cross_covariance(t, x)
+        Ktt = kernel.gram(t) + identity(n_test) * self.prior.jitter
+        mean_t = mean_function(t)
 
-            # Compute terms of the posterior predictive distribution
-            Ktx = kernel.cross_covariance(params["kernel"], t, x)
-            Ktt = kernel.gram(params["kernel"], t) + identity(n_test) * jitter
-            μt = mean_function(params["mean_function"], t)
-
-            # Lx⁻¹ Kxt
-            Lx_inv_Kxt = Lx.solve(Ktx.T)
-
-            # Whitened function values, wx, correponding to the inputs, x
-            wx = params["latent"]
-
-            # μt + Ktx Lx⁻¹ wx
-            mean = μt + jnp.matmul(Lx_inv_Kxt.T, wx)
-
-            # Ktt - Ktx Kxx⁻¹ Kxt, TODO: Take advantage of covariance structure to compute Schur complement more efficiently.
-            covariance = Ktt - jnp.matmul(Lx_inv_Kxt.T, Lx_inv_Kxt)
-            covariance += identity(n_test) * jitter
-
-            return GaussianDistribution(
-                jnp.atleast_1d(mean.squeeze()), covariance
-            )
+        # Lx⁻¹ Kxt
+        Lx_inv_Kxt = Lx.solve(Ktx.T)
 
-        return predict_fn
-
-    def marginal_log_likelihood(
-        self,
-        train_data: Dataset,
-        negative: bool = False,
-    ) -> Callable[[Dict], Float[Array, "1"]]:
-        """
-        Compute the marginal log-likelihood function of the Gaussian process.
-        The returned function can then be used for gradient based optimisation
-        of the model's parameters or for model comparison. The implementation
-        given here is general and will work for any likelihood support by GPJax.
-
-        Unlike the marginal_log_likelihood function of the ConjugatePosterior
-        object, the marginal_log_likelihood function of the
-        NonConjugatePosterior object does not provide an exact marginal
-        log-likelihood function. Instead, the NonConjugatePosterior object
-        represents the posterior distributions as a function of the model's
-        hyperparameters and the latent function. Markov chain Monte Carlo,
-        variational inference, or Laplace approximations can then be used to
-        sample from, or optimise an approximation to, the posterior
-        distribution.
-
-        Args:
-            train_data (Dataset): The training dataset used to compute the
-                marginal log-likelihood.
-            negative (Optional[bool]): Whether or not the returned function
-                should be negative. For optimisation, the negative is useful as
-                minimisation of the negative marginal log-likelihood is equivalent
-                to maximisation of the marginal log-likelihood. Defaults to False.
-
-        Returns:
-            Callable[[Dict], Float[Array, "1"]]: A functional representation
-                of the marginal log-likelihood that can be evaluated at a given
-                parameter set.
-        """
-        jitter = get_global_config()["jitter"]
-
-        # Unpack dataset
-        x, y, n = train_data.X, train_data.y, train_data.n
-
-        # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        # Whitened function values, wx, corresponding to the inputs, x
+        wx = self.latent
 
-        # Link function of the likelihood
-        link_function = self.likelihood.link_function
+        # μt + Ktx Lx⁻¹ wx
+        mean = mean_t + jnp.matmul(Lx_inv_Kxt.T, wx)
 
-        # The sign of the marginal log-likelihood depends on whether we are maximising or minimising
-        constant = jnp.array(-1.0) if negative else jnp.array(1.0)
+        # Ktt - Ktx Kxx⁻¹ Kxt, TODO: Take advantage of covariance structure to compute Schur complement more efficiently.
+        covariance = Ktt - jnp.matmul(Lx_inv_Kxt.T, Lx_inv_Kxt)
+        covariance += identity(n_test) * self.prior.jitter
 
-        def mll(params: Dict):
-            """Compute the marginal log-likelihood of the model.
-
-            Args:
-                params (Dict): A dictionary of parameters that should be used
-                    to compute the marginal log-likelihood.
-
-            Returns:
-                Float[Array, "1"]: The marginal log-likelihood of the model.
-            """
-
-            # Compute lower triangular of the kernel Gram matrix
-            Kxx = kernel.gram(params["kernel"], x)
-            Kxx += identity(n) * jitter
-            Lx = Kxx.to_root()
-
-            # Compute the prior mean function
-            μx = mean_function(params["mean_function"], x)
-
-            # Whitened function values, wx, correponding to the inputs, x
-            wx = params["latent"]
-
-            # f(x) = μx  +  Lx wx
-            fx = μx + Lx @ wx
-
-            # p(y | f(x), θ), where θ are the model hyperparameters
-            likelihood = link_function(params, fx)
-
-            # Whitened latent function values prior, p(wx | θ) = N(0, I)
-            latent_prior = dx.Normal(loc=0.0, scale=1.0)
-
-            return constant * (
-                likelihood.log_prob(y).sum() + latent_prior.log_prob(wx).sum()
-            )
-
-        return mll
+        return GaussianDistribution(jnp.atleast_1d(mean.squeeze()), covariance)
 
 
+#######################
+# Utils
+#######################
 def construct_posterior(
     prior: Prior, likelihood: AbstractLikelihood
 ) -> AbstractPosterior:
-    """Utility function for constructing a posterior object from a prior and
+    r"""Utility function for constructing a posterior object from a prior and
     likelihood. The function will automatically select the correct posterior
     object based on the likelihood.
 
     Args:
         prior (Prior): The Prior distribution.
         likelihood (AbstractLikelihood): The likelihood that represents our
             beliefs around the distribution of the data.
 
-    Returns:
+    Returns
+    -------
         AbstractPosterior: A posterior distribution. If the likelihood is
-            Gaussian, then a ``ConjugatePosterior`` will be returned. Otherwise,
-            a ``NonConjugatePosterior`` will be returned.
+            Gaussian, then a `ConjugatePosterior` will be returned. Otherwise,
+            a `NonConjugatePosterior` will be returned.
     """
-    if isinstance(likelihood, Conjugate):
-        PosteriorGP = ConjugatePosterior
+    if isinstance(likelihood, Gaussian):
+        return ConjugatePosterior(prior=prior, likelihood=likelihood)
+
+    return NonConjugatePosterior(prior=prior, likelihood=likelihood)
 
-    elif isinstance(likelihood, NonConjugate):
-        PosteriorGP = NonConjugatePosterior
 
-    else:
-        raise NotImplementedError(
-            f"No posterior implemented for {likelihood.name} likelihood"
-        )
+def _build_fourier_features_fn(
+    prior: Prior, num_features: int, key: KeyArray
+) -> Callable[[Float[Array, "N D"]], Float[Array, "N L"]]:
+    """Return a function that evaluates features sampled from the Fourier feature
+    decomposition of the prior's kernel.
+
+    Args:
+        prior (Prior): The Prior distribution.
+        num_features (int): The number of feature functions to be sampled.
+        key (KeyArray): The random seed used.
+
+    Returns
+    -------
+        Callable: A callable function evaluation the sampled feature functions.
+    """
+    if (not isinstance(num_features, int)) or num_features <= 0:
+        raise ValueError("num_features must be a positive integer")
+
+    # Approximate kernel with feature decomposition
+    approximate_kernel = RFF(
+        base_kernel=prior.kernel, num_basis_fns=num_features, key=key
+    )
+
+    def eval_fourier_features(test_inputs: Float[Array, "N D"]) -> Float[Array, "N L"]:
+        Phi = approximate_kernel.compute_features(x=test_inputs)
+        Phi *= jnp.sqrt(prior.kernel.variance / num_features)
+        return Phi
 
-    return PosteriorGP(prior=prior, likelihood=likelihood)
+    return eval_fourier_features
 
 
 __all__ = [
     "AbstractPrior",
     "Prior",
     "AbstractPosterior",
     "ConjugatePosterior",
```

### Comparing `gpjax-0.5.9/gpjax/mean_functions.py` & `gpjax-0.6/gpjax/mean_functions.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,156 +9,194 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+
 import abc
-from typing import Dict, Optional
+import dataclasses
+from functools import partial
 
+from beartype.typing import (
+    Callable,
+    List,
+    Union,
+)
 import jax.numpy as jnp
-from jax.random import KeyArray
-from jaxtyping import Array, Float
-from jaxutils import PyTree
-
-import deprecation
-
-
-class AbstractMeanFunction(PyTree):
-    """Abstract mean function that is used to parameterise the Gaussian process."""
-
-    def __init__(
-        self, output_dim: Optional[int] = 1, name: Optional[str] = "Mean function"
-    ):
-        """Initialise the mean function.
-
-        Args:
-            output_dim (Optional[int]): The output dimension of the mean function. Defaults to 1.
-            name (Optional[str]): The name of the mean function. Defaults to "Mean function".
-        """
-        self.output_dim = output_dim
-        self.name = name
+from jaxtyping import (
+    Float,
+    Num,
+)
+
+from gpjax.base import (
+    Module,
+    param_field,
+    static_field,
+)
+from gpjax.typing import Array
+
+
+@dataclasses.dataclass
+class AbstractMeanFunction(Module):
+    r"""Mean function that is used to parameterise the Gaussian process."""
 
     @abc.abstractmethod
-    def __call__(self, params: Dict, x: Float[Array, "N D"]) -> Float[Array, "N Q"]:
-        """Evaluate the mean function at the given points. This method is required for all subclasses.
+    def __call__(self, x: Num[Array, "N D"]) -> Float[Array, "N 1"]:
+        r"""Evaluate the mean function at the given points. This method is required for all subclasses.
 
         Args:
-            params (Dict): The parameters of the mean function.
-            x (Float[Array, "N D"]): The input points at which to evaluate the mean function.
+            x (Float[Array, " D"]): The point at which to evaluate the mean function.
 
-        Returns:
-            Float[Array, "N Q"]: The mean function evaluated point-wise on the inputs.
+        Returns
+        -------
+            Float[Array, "1]: The evaluated mean function.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def init_params(self, key: KeyArray) -> Dict:
-        """Return the parameters of the mean function. This method is required for all subclasses.
+    def __add__(
+        self, other: Union["AbstractMeanFunction", Float[Array, "1"]]
+    ) -> "AbstractMeanFunction":
+        r"""Add two mean functions.
 
         Args:
-            key (KeyArray): The PRNG key to use for initialising the parameters.
+            other (AbstractMeanFunction): The other mean function to add.
 
-        Returns:
-            Dict: The parameters of the mean function.
+        Returns
+        -------
+            AbstractMeanFunction: The sum of the two mean functions.
         """
-        raise NotImplementedError
-
-    @deprecation.deprecated(
-        deprecated_in="0.5.7",
-        removed_in="0.6.0",
-        details="Use the ``init_params`` method for parameter initialisation.",
-    )
-    def _initialise_params(self, key: KeyArray) -> Dict:
-        """Deprecated method for initialising the GP's parameters. Succeded by ``init_params``."""
-        return self.init_params(key)
+        if isinstance(other, AbstractMeanFunction):
+            return SumMeanFunction([self, other])
 
+        return SumMeanFunction([self, Constant(other)])
 
-class Zero(AbstractMeanFunction):
-    """
-    A zero mean function. This function returns zero for all inputs.
-    """
-
-    def __init__(
-        self, output_dim: Optional[int] = 1, name: Optional[str] = "Mean function"
-    ):
-        """Initialise the zero-mean function.
+    def __radd__(
+        self,
+        other: Union[
+            "AbstractMeanFunction", Float[Array, "1"]
+        ],  # TODO should this be ScalarFloat? or Num?
+    ) -> "AbstractMeanFunction":
+        r"""Add two mean functions.
 
         Args:
-            output_dim (Optional[int]): The output dimension of the mean function. Defaults to 1.
-            name (Optional[str]): The name of the mean function. Defaults to "Mean function".
+            other (AbstractMeanFunction): The other mean function to add.
+
+        Returns
+        -------
+            AbstractMeanFunction: The sum of the two mean functions.
         """
-        super().__init__(output_dim, name)
+        return self.__add__(other)
 
-    def __call__(self, params: Dict, x: Float[Array, "N D"]) -> Float[Array, "N Q"]:
-        """Evaluate the mean function at the given points.
+    def __mul__(
+        self,
+        other: Union[
+            "AbstractMeanFunction", Float[Array, "1"]
+        ],  # TODO should this be ScalarFloat? or Num?
+    ) -> "AbstractMeanFunction":
+        r"""Multiply two mean functions.
 
         Args:
-            params (Dict): The parameters of the mean function.
-            x (Float[Array, "N D"]): The input points at which to evaluate the mean function.
+            other (AbstractMeanFunction): The other mean function to multiply.
 
-        Returns:
-            Float[Array, "N Q"]: A vector of zeros.
+        Returns
+        -------
+            AbstractMeanFunction: The product of the two mean functions.
         """
-        out_shape = (x.shape[0], self.output_dim)
-        return jnp.zeros(shape=out_shape)
+        if isinstance(other, AbstractMeanFunction):
+            return ProductMeanFunction([self, other])
+
+        return ProductMeanFunction([self, Constant(other)])
 
-    def init_params(self, key: KeyArray) -> Dict:
-        """The parameters of the mean function. For the zero-mean function, this is an empty dictionary.
+    def __rmul__(
+        self,
+        other: Union[
+            "AbstractMeanFunction", Float[Array, "1"]
+        ],  # TODO should this be ScalarFloat? or Num?
+    ) -> "AbstractMeanFunction":
+        r"""Multiply two mean functions.
 
         Args:
-            key (KeyArray): The PRNG key to use for initialising the parameters.
+            other (AbstractMeanFunction): The other mean function to multiply.
 
-        Returns:
-            Dict: The parameters of the mean function.
+        Returns
+        -------
+            AbstractMeanFunction: The product of the two mean functions.
         """
-        return {}
+        return self.__mul__(other)
 
 
+@dataclasses.dataclass
 class Constant(AbstractMeanFunction):
-    """
-    A zero mean function. This function returns a repeated scalar value for all inputs.
-    The scalar value itself can be treated as a model hyperparameter and learned during training.
+    r"""Constant mean function.
+
+    A constant mean function. This function returns a repeated scalar value for all
+    inputs.  The scalar value itself can be treated as a model hyperparameter and
+    learned during training but defaults to 1.0.
     """
 
-    def __init__(
-        self, output_dim: Optional[int] = 1, name: Optional[str] = "Mean function"
-    ):
-        """Initialise the constant-mean function.
+    constant: Float[Array, "1"] = param_field(jnp.array([0.0]))
+
+    def __call__(self, x: Num[Array, "N D"]) -> Float[Array, "N 1"]:
+        r"""Evaluate the mean function at the given points.
 
         Args:
-            output_dim (Optional[int]): The output dimension of the mean function. Defaults to 1.
-            name (Optional[str]): The name of the mean function. Defaults to "Mean function".
+            x (Float[Array, " D"]): The point at which to evaluate the mean function.
+
+        Returns
+        -------
+            Float[Array, "1"]: The evaluated mean function.
         """
-        super().__init__(output_dim, name)
+        return jnp.ones((x.shape[0], 1)) * self.constant
 
-    def __call__(self, params: Dict, x: Float[Array, "N D"]) -> Float[Array, "N Q"]:
-        """Evaluate the mean function at the given points.
 
-        Args:
-            params (Dict): The parameters of the mean function.
-            x (Float[Array, "N D"]): The input points at which to evaluate the mean function.
+@dataclasses.dataclass
+class CombinationMeanFunction(AbstractMeanFunction):
+    r"""A base class for products or sums of AbstractMeanFunctions."""
 
-        Returns:
-            Float[Array, "N Q"]: A vector of repeated constant values.
-        """
-        out_shape = (x.shape[0], self.output_dim)
-        return jnp.ones(shape=out_shape) * params["constant"]
+    means: List[AbstractMeanFunction]
+    operator: Callable = static_field()
+
+    def __init__(
+        self,
+        means: List[AbstractMeanFunction],
+        operator: Callable,
+        **kwargs,
+    ) -> None:
+        super().__init__(**kwargs)
+
+        # Add means to a list, flattening out instances of this class therein, as in GPFlow kernels.
+        items_list: List[AbstractMeanFunction] = []
+
+        for item in means:
+            if not isinstance(item, AbstractMeanFunction):
+                raise TypeError(
+                    "can only combine AbstractMeanFunction instances"
+                )  # pragma: no cover
+
+            if isinstance(item, self.__class__):
+                items_list.extend(item.means)
+            else:
+                items_list.append(item)
+
+        self.means = items_list
+        self.operator = operator
 
-    def init_params(self, key: KeyArray) -> Dict:
-        """The parameters of the mean function. For the constant-mean function, this is a dictionary with a single value.
+    def __call__(self, x: Num[Array, "N D"]) -> Float[Array, "N 1"]:
+        r"""Evaluate combination kernel on a pair of inputs.
 
         Args:
-            key (KeyArray): The PRNG key to use for initialising the parameters.
+            x (Float[Array, " D"]): The point at which to evaluate the mean function.
 
-        Returns:
-            Dict: The parameters of the mean function.
+        Returns
+        -------
+            Float[Array, " Q"]: The evaluated mean function.
         """
-        return {"constant": jnp.array([1.0])}
+        return self.operator(jnp.stack([m(x) for m in self.means]))
 
 
-__all__ = [
-    "AbstractMeanFunction",
-    "Zero",
-    "Constant",
-]
+SumMeanFunction = partial(CombinationMeanFunction, operator=partial(jnp.sum, axis=0))
+ProductMeanFunction = partial(
+    CombinationMeanFunction, operator=partial(jnp.sum, axis=0)
+)
+Zero = partial(Constant, constant=jnp.array([0.0]))
```

### Comparing `gpjax-0.5.9/gpjax/quadrature.py` & `gpjax-0.6/gpjax/quadrature.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,47 +9,53 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from typing import Callable, Optional
-
+from beartype.typing import (
+    Callable,
+    Optional,
+)
 import jax.numpy as jnp
+from jaxtyping import Float
 import numpy as np
-from jaxtyping import Array, Float
 
-"""The number of Gauss-Hermite points to use for quadrature"""
+from gpjax.typing import Array
+
+r"""The number of Gauss-Hermite points to use for quadrature"""
 DEFAULT_NUM_GAUSS_HERMITE_POINTS = 20
 
 
 def gauss_hermite_quadrature(
     fun: Callable,
     mean: Float[Array, "N D"],
     sd: Float[Array, "N D"],
     deg: Optional[int] = DEFAULT_NUM_GAUSS_HERMITE_POINTS,
     *args,
-    **kwargs
-) -> Float[Array, "N"]:
-    """
+    **kwargs,
+) -> Float[Array, " N"]:
+    r"""Compute Gauss-Hermite quadrature.
+
     Compute Gaussian-Hermite quadrature for a given function. The quadrature
     points are adjusted through the supplied mean and variance arrays.
 
     Args:
         fun (Callable): The function for which quadrature should be applied to.
         mean (Float[Array, "N D"]): The mean of the Gaussian distribution that
             is used to shift quadrature points.
         sd (Float[Array, "N D"]): The standard deviation of the Gaussian
             distribution that is used to scale quadrature points.
         deg (int, optional): The number of quadrature points that are to be used.
             Defaults to 20.
 
-    Returns:
-        Float[Array, "N"]: The evaluated integrals value.
+    Returns
+    -------
+        Float[Array, " N"]: The evaluated integrals value.
     """
     gh_points, gh_weights = np.polynomial.hermite.hermgauss(deg)
     X = mean + jnp.sqrt(2.0) * sd * gh_points
     W = gh_weights / jnp.sqrt(jnp.pi)
     return jnp.sum(fun(X, *args, **kwargs) * W, axis=1)
```

### Comparing `gpjax-0.5.9/gpjax/variational_families.py` & `gpjax-0.6/gpjax/variational_families.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,513 +10,437 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import abc
-from typing import Any, Callable, Dict, Optional
+from dataclasses import dataclass
 
-import distrax as dx
+from beartype.typing import Any
 import jax.numpy as jnp
 import jax.scipy as jsp
-from jax.random import KeyArray
-from jaxtyping import Array, Float
+from jaxtyping import Float
+import tensorflow_probability.substrates.jax.bijectors as tfb
 
-from jaxlinop import identity
-from jaxutils import PyTree, Dataset
-import jaxlinop as jlo
-
-from .config import get_global_config
-from .gps import Prior
-from .likelihoods import AbstractLikelihood, Gaussian
-from .utils import concat_dictionaries
-from .gaussian_distribution import GaussianDistribution
-
-import deprecation
-
-
-class AbstractVariationalFamily(PyTree):
-    """
+from gpjax.base import (
+    Module,
+    param_field,
+    static_field,
+)
+from gpjax.dataset import Dataset
+from gpjax.gaussian_distribution import GaussianDistribution
+from gpjax.gps import AbstractPosterior
+from gpjax.likelihoods import Gaussian
+from gpjax.linops import (
+    DenseLinearOperator,
+    LowerTriangularLinearOperator,
+    identity,
+)
+from gpjax.typing import (
+    Array,
+    ScalarFloat,
+)
+
+
+@dataclass
+class AbstractVariationalFamily(Module):
+    r"""
     Abstract base class used to represent families of distributions that can be
     used within variational inference.
     """
 
+    posterior: AbstractPosterior
+
     def __call__(self, *args: Any, **kwargs: Any) -> GaussianDistribution:
-        """For a given set of parameters, compute the latent function's prediction
+        r"""Evaluate the variational family's density.
+
+        For a given set of parameters, compute the latent function's prediction
         under the variational approximation.
 
         Args:
             *args (Any): Arguments of the variational family's `predict` method.
             **kwargs (Any): Keyword arguments of the variational family's `predict`
                 method.
 
-        Returns:
+        Returns
+        -------
             GaussianDistribution: The output of the variational family's `predict` method.
         """
         return self.predict(*args, **kwargs)
 
     @abc.abstractmethod
-    def init_params(self, key: KeyArray) -> Dict:
-        """
-        The parameters of the distribution. For example, the multivariate
-        Gaussian would return a mean vector and covariance matrix.
-
-        Args:
-            key (KeyArray): The PRNG key used to initialise the parameters.
-
-        Returns:
-            Dict: The parameters of the distribution.
-        """
-        raise NotImplementedError
-
-    @deprecation.deprecated(
-        deprecated_in="0.5.7",
-        removed_in="0.6.0",
-        details="Use the ``init_params`` method for parameter initialisation.",
-    )
-    def _initialise_params(self, key: KeyArray) -> Dict:
-        """Deprecated method for initialising the GP's parameters. Succeded by ``init_params``."""
-        return self.init_params(key)
-
-    @abc.abstractmethod
     def predict(self, *args: Any, **kwargs: Any) -> GaussianDistribution:
-        """Predict the GP's output given the input.
+        r"""Predict the GP's output given the input.
 
         Args:
             *args (Any): Arguments of the variational family's ``predict``
-            method.
+                method.
             **kwargs (Any): Keyword arguments of the variational family's
-            ``predict`` method.
+                ``predict`` method.
 
-        Returns:
+        Returns
+        -------
             GaussianDistribution: The output of the variational family's ``predict`` method.
         """
         raise NotImplementedError
 
 
+@dataclass
 class AbstractVariationalGaussian(AbstractVariationalFamily):
-    """The variational Gaussian family of probability distributions."""
+    r"""The variational Gaussian family of probability distributions."""
 
-    def __init__(
-        self,
-        prior: Prior,
-        inducing_inputs: Float[Array, "N D"],
-        name: Optional[str] = "Variational Gaussian",
-    ) -> None:
-        """
-        Args:
-            prior (Prior): The prior distribution.
-            inducing_inputs (Float[Array, "N D"]): The inducing inputs.
-            name (Optional[str]): The name of the variational family. Defaults to "Gaussian".
-        """
-        self.prior = prior
-        self.inducing_inputs = inducing_inputs
-        self.num_inducing = self.inducing_inputs.shape[0]
-        self.name = name
+    inducing_inputs: Float[Array, "N D"]
+    jitter: ScalarFloat = static_field(1e-6)
 
+    @property
+    def num_inducing(self) -> int:
+        """The number of inducing inputs."""
+        return self.inducing_inputs.shape[0]
 
+
+@dataclass
 class VariationalGaussian(AbstractVariationalGaussian):
-    """The variational Gaussian family of probability distributions.
+    r"""The variational Gaussian family of probability distributions.
 
-    The variational family is q(f(·)) = ∫ p(f(·)|u) q(u) du, where
-    :math:`u = f(z)` are the function values at the inducing inputs z
+    The variational family is $`q(f(\cdot)) = \int p(f(\cdot)\mid u) q(u) \mathrm{d}u`$, where
+    $`u = f(z)`$ are the function values at the inducing inputs $`z`$
     and the distribution over the inducing inputs is
-    :math:`q(u) = \\mathcal{N}(\\mu, S)`.  We parameterise this over
-    :math:`\\mu` and sqrt with S = sqrt sqrtᵀ.
+    $`q(u) = \mathcal{N}(\mu, S)`$.  We parameterise this over
+    $`\mu`$ and $`sqrt`$ with $`S = sqrt sqrt^{\top}`$.
     """
 
-    def init_params(self, key: KeyArray) -> Dict:
-        """
-        Return the variational mean vector, variational root covariance matrix,
-        and inducing input vector that parameterise the variational Gaussian
-        distribution.
+    variational_mean: Float[Array, "N 1"] = param_field(None)
+    variational_root_covariance: Float[Array, "N N"] = param_field(
+        None, bijector=tfb.FillTriangular()
+    )
 
-        Args:
-            key (KeyArray): The PRNG key used to initialise the parameters.
+    def __post_init__(self) -> None:
+        if self.variational_mean is None:
+            self.variational_mean = jnp.zeros((self.num_inducing, 1))
 
-        Returns:
-            Dict: The parameters of the distribution.
-        """
-        m = self.num_inducing
+        if self.variational_root_covariance is None:
+            self.variational_root_covariance = jnp.eye(self.num_inducing)
 
-        return concat_dictionaries(
-            self.prior.init_params(key),
-            {
-                "variational_family": {
-                    "inducing_inputs": self.inducing_inputs,
-                    "moments": {
-                        "variational_mean": jnp.zeros((m, 1)),
-                        "variational_root_covariance": jnp.eye(m),
-                    },
-                }
-            },
-        )
+    def prior_kl(self) -> ScalarFloat:
+        r"""Compute the prior KL divergence.
 
-    def prior_kl(self, params: Dict) -> Float[Array, "1"]:
-        """
         Compute the KL-divergence between our variational approximation and the
         Gaussian process prior.
 
-        For this variational family, we have KL[q(f(·))||p(·)] = KL[q(u)||p(u)]
-        = KL[ N(μ, S) || N(μz, Kzz) ], where u = f(z) and z are the inducing
-        inputs.
-
-        Args:
-            params (Dict): The parameters at which our variational distribution
-                and GP prior are to be evaluated.
-
-        Returns:
-             Float[Array, "1"]: The KL-divergence between our variational
+        For this variational family, we have
+        ```math
+        \begin{align}
+        \operatorname{KL}[q(f(\cdot))\mid\mid p(\cdot)] & = \operatorname{KL}[q(u)\mid\mid p(u)]\\
+        & = \operatorname{KL}[ \mathcal{N}(\mu, S) \mid\mid N(\mu z, \mathbf{K}_{zz}) ],
+        \end{align}
+        ```
+        where $`u = f(z)`$ and $`z`$ are the inducing inputs.
+
+        Returns
+        -------
+             ScalarFloat: The KL-divergence between our variational
                 approximation and the GP prior.
         """
-
-        jitter = get_global_config()["jitter"]
-
         # Unpack variational parameters
-        mu = params["variational_family"]["moments"]["variational_mean"]
-        sqrt = params["variational_family"]["moments"]["variational_root_covariance"]
-        z = params["variational_family"]["inducing_inputs"]
+        mu = self.variational_mean
+        sqrt = self.variational_root_covariance
+        z = self.inducing_inputs
         m = self.num_inducing
 
         # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        mean_function = self.posterior.prior.mean_function
+        kernel = self.posterior.prior.kernel
 
-        μz = mean_function(params["mean_function"], z)
-        Kzz = kernel.gram(params["kernel"], z)
-        Kzz += identity(m) * jitter
+        muz = mean_function(z)
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * self.jitter
 
-        sqrt = jlo.LowerTriangularLinearOperator.from_dense(sqrt)
-        S = jlo.DenseLinearOperator.from_root(sqrt)
+        sqrt = LowerTriangularLinearOperator.from_dense(sqrt)
+        S = DenseLinearOperator.from_root(sqrt)
 
         qu = GaussianDistribution(loc=jnp.atleast_1d(mu.squeeze()), scale=S)
-        pu = GaussianDistribution(loc=jnp.atleast_1d(μz.squeeze()), scale=Kzz)
+        pu = GaussianDistribution(loc=jnp.atleast_1d(muz.squeeze()), scale=Kzz)
 
         return qu.kl_divergence(pu)
 
-    def predict(
-        self, params: Dict
-    ) -> Callable[[Float[Array, "N D"]], GaussianDistribution]:
-        """
-        Compute the predictive distribution of the GP at the test inputs t.
-
-        This is the integral q(f(t)) = ∫ p(f(t)|u) q(u) du, which can be
-        computed in closed form as:
+    def predict(self, test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
+        r"""Compute the predictive distribution of the GP at the test inputs t.
 
-            N[f(t); μt + Ktz Kzz⁻¹ (μ - μz),  Ktt - Ktz Kzz⁻¹ Kzt + Ktz Kzz⁻¹ S Kzz⁻¹ Kzt ].
-
-        Args:
-            params (Dict): The set of parameters that are to be used to
-                parameterise our variational approximation and GP.
-
-        Returns:
-            Callable[[Float[Array, "N D"]], dx.MultivariateNormalTri]: A
-                function that accepts a set of test points and will return
-                the predictive distribution at those points.
+        This is the integral $`q(f(t)) = \int p(f(t)\mid u) q(u) \mathrm{d}u`$, which
+        can be computed in closed form as:
+        ```math
+            \mathcal{N}\left(f(t); \mu t + \mathbf{K}_{tz} \mathbf{K}_{zz}^{-1} (\mu - \mu z),  \mathbf{K}_{tt} - \mathbf{K}_{tz} \mathbf{K}_{zz}^{-1} \mathbf{K}_{zt} + \mathbf{K}_{tz} \mathbf{K}_{zz}^{-1} S \mathbf{K}_{zz}^{-1} \mathbf{K}_{zt}\right).
+        ```
+
+        Args:
+            test_inputs (Float[Array, "N D"]): The test inputs at which we wish to
+                make a prediction.
+
+        Returns
+        -------
+            GaussianDistribution: The predictive distribution of the low-rank GP at
+                the test inputs.
         """
-        jitter = get_global_config()["jitter"]
-
         # Unpack variational parameters
-        mu = params["variational_family"]["moments"]["variational_mean"]
-        sqrt = params["variational_family"]["moments"]["variational_root_covariance"]
-        z = params["variational_family"]["inducing_inputs"]
+        mu = self.variational_mean
+        sqrt = self.variational_root_covariance
+        z = self.inducing_inputs
         m = self.num_inducing
 
         # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        mean_function = self.posterior.prior.mean_function
+        kernel = self.posterior.prior.kernel
 
-        Kzz = kernel.gram(params["kernel"], z)
-        Kzz += identity(m) * jitter
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * self.jitter
         Lz = Kzz.to_root()
-        μz = mean_function(params["mean_function"], z)
-
-        def predict_fn(test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
-
-            # Unpack test inputs
-            t, n_test = test_inputs, test_inputs.shape[0]
+        muz = mean_function(z)
 
-            Ktt = kernel.gram(params["kernel"], t)
-            Kzt = kernel.cross_covariance(params["kernel"], z, t)
-            μt = mean_function(params["mean_function"], t)
+        # Unpack test inputs
+        t, n_test = test_inputs, test_inputs.shape[0]
 
-            # Lz⁻¹ Kzt
-            Lz_inv_Kzt = Lz.solve(Kzt)
+        Ktt = kernel.gram(t)
+        Kzt = kernel.cross_covariance(z, t)
+        mut = mean_function(t)
 
-            # Kzz⁻¹ Kzt
-            Kzz_inv_Kzt = Lz.T.solve(Lz_inv_Kzt)
+        # Lz⁻¹ Kzt
+        Lz_inv_Kzt = Lz.solve(Kzt)
 
-            # Ktz Kzz⁻¹ sqrt
-            Ktz_Kzz_inv_sqrt = jnp.matmul(Kzz_inv_Kzt.T, sqrt)
+        # Kzz⁻¹ Kzt
+        Kzz_inv_Kzt = Lz.T.solve(Lz_inv_Kzt)
 
-            # μt + Ktz Kzz⁻¹ (μ - μz)
-            mean = μt + jnp.matmul(Kzz_inv_Kzt.T, mu - μz)
+        # Ktz Kzz⁻¹ sqrt
+        Ktz_Kzz_inv_sqrt = jnp.matmul(Kzz_inv_Kzt.T, sqrt)
 
-            # Ktt - Ktz Kzz⁻¹ Kzt  +  Ktz Kzz⁻¹ S Kzz⁻¹ Kzt  [recall S = sqrt sqrtᵀ]
-            covariance = (
-                Ktt
-                - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
-                + jnp.matmul(Ktz_Kzz_inv_sqrt, Ktz_Kzz_inv_sqrt.T)
-            )
-            covariance += identity(n_test) * jitter
+        # μt + Ktz Kzz⁻¹ (μ - μz)
+        mean = mut + jnp.matmul(Kzz_inv_Kzt.T, mu - muz)
 
-            return GaussianDistribution(
-                loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
-            )
+        # Ktt - Ktz Kzz⁻¹ Kzt  +  Ktz Kzz⁻¹ S Kzz⁻¹ Kzt  [recall S = sqrt sqrtᵀ]
+        covariance = (
+            Ktt
+            - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
+            + jnp.matmul(Ktz_Kzz_inv_sqrt, Ktz_Kzz_inv_sqrt.T)
+        )
+        covariance += identity(n_test) * self.jitter
 
-        return predict_fn
+        return GaussianDistribution(
+            loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
+        )
 
 
+@dataclass
 class WhitenedVariationalGaussian(VariationalGaussian):
-    """
-    The whitened variational Gaussian family of probability distributions.
-
-    The variational family is q(f(·)) = ∫ p(f(·)|u) q(u) du, where u = f(z)
-    are the function values at the inducing inputs z and the distribution over
-    the inducing inputs is q(u) = N(Lz μ + mz, Lz S Lzᵀ). We parameterise this
-    over μ and sqrt with S = sqrt sqrtᵀ.
+    r"""The whitened variational Gaussian family of probability distributions.
 
+    The variational family is $`q(f(\cdot)) = \int p(f(\cdot)\mid u) q(u) \mathrm{d}u`$,
+    where $`u = f(z)`$
+    are the function values at the inducing inputs $`z`$ and the distribution over
+    the inducing inputs is $`q(u) = \mathcal{N}(Lz \mu + mz, Lz S Lz^{\top})`$. We parameterise this
+    over $`\mu`$ and $`sqrt`$ with $`S = sqrt sqrt^{\top}`$.
     """
 
-    def __init__(
-        self,
-        prior: Prior,
-        inducing_inputs: Float[Array, "N D"],
-        name: Optional[str] = "Whitened variational Gaussian",
-    ) -> None:
-        """Initialise the whitened variational Gaussian family.
-
-        Args:
-            prior (Prior): The GP prior.
-            inducing_inputs (Float[Array, "N D"]): The inducing inputs.
-            name (Optional[str]): The name of the variational family.
-        """
-
-        super().__init__(prior, inducing_inputs, name)
-
-    def prior_kl(self, params: Dict) -> Float[Array, "1"]:
-        """Compute the KL-divergence between our variational approximation and
+    def prior_kl(self) -> ScalarFloat:
+        r"""Compute the KL-divergence between our variational approximation and
         the Gaussian process prior.
 
-        For this variational family, we have KL[q(f(·))||p(·)] = KL[q(u)||p(u)] = KL[N(μ, S)||N(0, I)].
-
-        Args:
-            params (Dict): The parameters at which our variational distribution
-                and GP prior are to be evaluated.
-
-        Returns:
-            Float[Array, "1"]: The KL-divergence between our variational
+        For this variational family, we have
+        ```math
+        \begin{align}
+        \operatorname{KL}[q(f(\cdot))\mid\mid p(\cdot)] & = \operatorname{KL}[q(u)\mid\mid p(u)]\\
+            & = \operatorname{KL}[N(\mu  , S)\mid\mid N(0, I)].
+        \end{align}
+        ```
+
+        Returns
+        -------
+            ScalarFloat: The KL-divergence between our variational
                 approximation and the GP prior.
         """
-
         # Unpack variational parameters
-        mu = params["variational_family"]["moments"]["variational_mean"]
-        sqrt = params["variational_family"]["moments"]["variational_root_covariance"]
+        mu = self.variational_mean
+        sqrt = self.variational_root_covariance
 
-        sqrt = jlo.LowerTriangularLinearOperator.from_dense(sqrt)
-        S = jlo.DenseLinearOperator.from_root(sqrt)
+        sqrt = LowerTriangularLinearOperator.from_dense(sqrt)
+        S = DenseLinearOperator.from_root(sqrt)
 
         # Compute whitened KL divergence
         qu = GaussianDistribution(loc=jnp.atleast_1d(mu.squeeze()), scale=S)
         pu = GaussianDistribution(loc=jnp.zeros_like(jnp.atleast_1d(mu.squeeze())))
         return qu.kl_divergence(pu)
 
-    def predict(
-        self, params: Dict
-    ) -> Callable[[Float[Array, "N D"]], GaussianDistribution]:
-        """Compute the predictive distribution of the GP at the test inputs t.
-
-        This is the integral q(f(t)) = ∫ p(f(t)|u) q(u) du, which can be computed in closed form as
+    def predict(self, test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
+        r"""Compute the predictive distribution of the GP at the test inputs t.
 
-            N[f(t); μt  +  Ktz Lz⁻ᵀ μ,  Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Lz⁻ᵀ S Lz⁻¹ Kzt].
-
-        Args:
-            params (Dict): The set of parameters that are to be used to parameterise our variational approximation and GP.
-
-        Returns:
-            Callable[[Float[Array, "N D"]], dx.MultivariateNormalTri]: A function that accepts a set of test points and will return the predictive distribution at those points.
+        This is the integral q(f(t)) = \int p(f(t)\midu) q(u) du, which can be computed in
+        closed form as
+        ```math
+            \mathcal{N}\left(f(t); \mu t  +  \mathbf{K}_{tz} \mathbf{L}z^{\top} \mu  ,  \mathbf{K}_{tt}  -  \mathbf{K}_{tz} \mathbf{K}_{zz}^{-1} \mathbf{K}_{zt}  +  \mathbf{K}_{tz} \mathbf{L}z^{\top} S \mathbf{L}z^{-1} \mathbf{K}_{zt} \right).
+        ```
+
+        Args:
+            test_inputs (Float[Array, "N D"]): The test inputs at which we wish to
+                make a prediction.
+
+        Returns
+        -------
+            GaussianDistribution: The predictive distribution of the low-rank GP at
+                the test inputs.
         """
-        jitter = get_global_config()["jitter"]
-
         # Unpack variational parameters
-        mu = params["variational_family"]["moments"]["variational_mean"]
-        sqrt = params["variational_family"]["moments"]["variational_root_covariance"]
-        z = params["variational_family"]["inducing_inputs"]
+        mu = self.variational_mean
+        sqrt = self.variational_root_covariance
+        z = self.inducing_inputs
         m = self.num_inducing
 
         # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        mean_function = self.posterior.prior.mean_function
+        kernel = self.posterior.prior.kernel
 
-        Kzz = kernel.gram(params["kernel"], z)
-        Kzz += identity(m) * jitter
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * self.jitter
         Lz = Kzz.to_root()
 
-        def predict_fn(test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
-
-            # Unpack test inputs
-            t, n_test = test_inputs, test_inputs.shape[0]
-
-            Ktt = kernel.gram(params["kernel"], t)
-            Kzt = kernel.cross_covariance(params["kernel"], z, t)
-            μt = mean_function(params["mean_function"], t)
-
-            # Lz⁻¹ Kzt
-            Lz_inv_Kzt = Lz.solve(Kzt)
-
-            # Ktz Lz⁻ᵀ sqrt
-            Ktz_Lz_invT_sqrt = jnp.matmul(Lz_inv_Kzt.T, sqrt)
-
-            # μt  +  Ktz Lz⁻ᵀ μ
-            mean = μt + jnp.matmul(Lz_inv_Kzt.T, mu)
-
-            # Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Lz⁻ᵀ S Lz⁻¹ Kzt  [recall S = sqrt sqrtᵀ]
-            covariance = (
-                Ktt
-                - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
-                + jnp.matmul(Ktz_Lz_invT_sqrt, Ktz_Lz_invT_sqrt.T)
-            )
-            covariance += identity(n_test) * jitter
+        # Unpack test inputs
+        t, n_test = test_inputs, test_inputs.shape[0]
 
-            return GaussianDistribution(
-                loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
-            )
+        Ktt = kernel.gram(t)
+        Kzt = kernel.cross_covariance(z, t)
+        mut = mean_function(t)
+
+        # Lz⁻¹ Kzt
+        Lz_inv_Kzt = Lz.solve(Kzt)
+
+        # Ktz Lz⁻ᵀ sqrt
+        Ktz_Lz_invT_sqrt = jnp.matmul(Lz_inv_Kzt.T, sqrt)
+
+        # μt  +  Ktz Lz⁻ᵀ μ
+        mean = mut + jnp.matmul(Lz_inv_Kzt.T, mu)
+
+        # Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Lz⁻ᵀ S Lz⁻¹ Kzt  [recall S = sqrt sqrtᵀ]
+        covariance = (
+            Ktt
+            - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
+            + jnp.matmul(Ktz_Lz_invT_sqrt, Ktz_Lz_invT_sqrt.T)
+        )
+        covariance += identity(n_test) * self.jitter
 
-        return predict_fn
+        return GaussianDistribution(
+            loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
+        )
 
 
+@dataclass
 class NaturalVariationalGaussian(AbstractVariationalGaussian):
-    """The natural variational Gaussian family of probability distributions.
+    r"""The natural variational Gaussian family of probability distributions.
 
-    The variational family is q(f(·)) = ∫ p(f(·)|u) q(u) du, where u = f(z) are the function values at the inducing inputs z
-    and the distribution over the inducing inputs is q(u) = N(μ, S). Expressing the variational distribution, in the form of the
-    exponential family, q(u) = exp(θᵀ T(u) - a(θ)), gives rise to the natural paramerisation θ = (θ₁, θ₂) = (S⁻¹μ, -S⁻¹/2), to perform
-    model inference, where T(u) = [u, uuᵀ] are the sufficient statistics.
+    The variational family is $`q(f(\cdot)) = \int p(f(\cdot)\mid u) q(u) \mathrm{d}u`$,
+    where $`u = f(z)`$ are
+    the function values at the inducing inputs $`z`$ and the distribution over the
+    inducing inputs is $`q(u) = N(\mu, S)`$. Expressing the variational distribution, in
+    the form of the exponential family, $`q(u) = exp(\theta^{\top} T(u) - a(\theta))`$, gives rise to the
+    natural parameterisation $`\theta  = (\theta_{1}, \theta_{2}) = (S^{-1}\mu, -S^{-1}/2)`$, to perform model inference,
+    where $`T(u) = [u, uu^{\top}]`$ are the sufficient statistics.
     """
 
-    def __init__(
-        self,
-        prior: Prior,
-        inducing_inputs: Float[Array, "N D"],
-        name: Optional[str] = "Natural variational Gaussian",
-    ) -> None:
-        """Initialise the natural variational Gaussian family.
+    natural_vector: Float[Array, "M 1"] = None
+    natural_matrix: Float[Array, "M M"] = None
 
-        Args:
-            prior (Prior): The GP prior.
-            inducing_inputs (Float[Array, "N D"]): The inducing inputs.
-            name (Optional[str]): The name of the variational family.
+    def __post_init__(self):
+        if self.natural_vector is None:
+            self.natural_vector = jnp.zeros((self.num_inducing, 1))
+
+        if self.natural_matrix is None:
+            self.natural_matrix = -0.5 * jnp.eye(self.num_inducing)
+
+    def prior_kl(self) -> ScalarFloat:
+        r"""Compute the KL-divergence between our current variational approximation
+        and the Gaussian process prior.
+
+        For this variational family, we have
+        ```math
+        \begin{align}
+        \operatorname{KL}[q(f(\cdot))\mid\mid p(\cdot)] & = \operatorname{KL}[q(u)\mid\mid p(u)] \\
+            & = \operatorname{KL}[N(\mu, S)\mid\mid N(mz, \mathbf{K}_{zz})],
+        \end{align}
+        ```
+        with $\mu$ and $S$ computed from the natural parameterisation $\theta  = (S^{-1}\mu  , -S^{-1}/2)$.
+
+        Returns
+        -------
+            ScalarFloat: The KL-divergence between our variational approximation and
+                the GP prior.
         """
-
-        super().__init__(prior, inducing_inputs, name)
-
-    def init_params(self, key: KeyArray) -> Dict:
-        """Return the natural vector and matrix, inducing inputs, and hyperparameters that parameterise the natural Gaussian distribution."""
-
-        m = self.num_inducing
-
-        return concat_dictionaries(
-            self.prior.init_params(key),
-            {
-                "variational_family": {
-                    "inducing_inputs": self.inducing_inputs,
-                    "moments": {
-                        "natural_vector": jnp.zeros((m, 1)),
-                        "natural_matrix": -0.5 * jnp.eye(m),
-                    },
-                }
-            },
-        )
-
-    def prior_kl(self, params: Dict) -> Float[Array, "1"]:
-        """Compute the KL-divergence between our current variational approximation and the Gaussian process prior.
-
-        For this variational family, we have KL[q(f(·))||p(·)] = KL[q(u)||p(u)] = KL[N(μ, S)||N(mz, Kzz)],
-
-        with μ and S computed from the natural paramerisation θ = (S⁻¹μ, -S⁻¹/2).
-
-        Args:
-            params (Dict): The parameters at which our variational distribution and GP prior are to be evaluated.
-
-        Returns:
-            Float[Array, "1"]: The KL-divergence between our variational approximation and the GP prior.
-        """
-        jitter = get_global_config()["jitter"]
-
         # Unpack variational parameters
-        natural_vector = params["variational_family"]["moments"]["natural_vector"]
-        natural_matrix = params["variational_family"]["moments"]["natural_matrix"]
-        z = params["variational_family"]["inducing_inputs"]
+        natural_vector = self.natural_vector
+        natural_matrix = self.natural_matrix
+        z = self.inducing_inputs
         m = self.num_inducing
 
         # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        mean_function = self.posterior.prior.mean_function
+        kernel = self.posterior.prior.kernel
 
         # S⁻¹ = -2θ₂
         S_inv = -2 * natural_matrix
-        S_inv += jnp.eye(m) * jitter
+        S_inv += jnp.eye(m) * self.jitter
 
         # Compute L⁻¹, where LLᵀ = S, via a trick found in the NumPyro source code and https://nbviewer.org/gist/fehiepsi/5ef8e09e61604f10607380467eb82006#Precision-to-scale_tril:
         sqrt_inv = jnp.swapaxes(
             jnp.linalg.cholesky(S_inv[..., ::-1, ::-1])[..., ::-1, ::-1], -2, -1
         )
 
         # L = (L⁻¹)⁻¹I
         sqrt = jsp.linalg.solve_triangular(sqrt_inv, jnp.eye(m), lower=True)
-        sqrt = jlo.LowerTriangularLinearOperator.from_dense(sqrt)
+        sqrt = LowerTriangularLinearOperator.from_dense(sqrt)
 
         # S = LLᵀ:
-        S = jlo.DenseLinearOperator.from_root(sqrt)
+        S = DenseLinearOperator.from_root(sqrt)
 
         # μ = Sθ₁
         mu = S @ natural_vector
 
-        μz = mean_function(params["mean_function"], z)
-        Kzz = kernel.gram(params["kernel"], z)
-        Kzz += identity(m) * jitter
+        muz = mean_function(z)
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * self.jitter
 
         qu = GaussianDistribution(loc=jnp.atleast_1d(mu.squeeze()), scale=S)
-        pu = GaussianDistribution(loc=jnp.atleast_1d(μz.squeeze()), scale=Kzz)
+        pu = GaussianDistribution(loc=jnp.atleast_1d(muz.squeeze()), scale=Kzz)
 
         return qu.kl_divergence(pu)
 
-    def predict(
-        self, params: Dict
-    ) -> Callable[[Float[Array, "N D"]], GaussianDistribution]:
-        """Compute the predictive distribution of the GP at the test inputs t.
-
-        This is the integral q(f(t)) = ∫ p(f(t)|u) q(u) du, which can be computed in closed form as
-
-             N[f(t); μt + Ktz Kzz⁻¹ (μ - μz),  Ktt - Ktz Kzz⁻¹ Kzt + Ktz Kzz⁻¹ S Kzz⁻¹ Kzt ],
+    def predict(self, test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
+        r"""Compute the predictive distribution of the GP at the test inputs $t$.
 
-        with μ and S computed from the natural paramerisation θ = (S⁻¹μ, -S⁻¹/2).
-
-        Args:
-            params (Dict): The set of parameters that are to be used to parameterise our variational approximation and GP.
-
-        Returns:
-            Callable[[Float[Array, "N D"]], GaussianDistribution]: A function that accepts a set of test points and will return the predictive distribution at those points.
+        This is the integral $`q(f(t)) = \int p(f(t)\mid u) q(u) \mathrm{d}u`$, which
+        can be computed in closed form as
+        ```math
+             \mathcal{N}\left(f(t); \mu  t + \mathbf{K}_{tz} \mathbf{K}_{zz}^{-1} (\mu   - \mu  z),  \mathbf{K}_{tt} - \mathbf{K}_{tz} \mathbf{K}_{zz}^{-1} \mathbf{K}_{zt} + \mathbf{K}_{tz} \mathbf{K}_{zz}^{-1} S \mathbf{K}_{zz}^{-1} \mathbf{K}_{zt} \right),
+        ```
+        with $`\mu`$ and $`S`$ computed from the natural parameterisation
+        $`\theta = (S^{-1}\mu  , -S^{-1}/2)`$.
+
+        Returns
+        -------
+            GaussianDistribution: A function that accepts a set of test points and will
+                return the predictive distribution at those points.
         """
-        jitter = get_global_config()["jitter"]
-
         # Unpack variational parameters
-        natural_vector = params["variational_family"]["moments"]["natural_vector"]
-        natural_matrix = params["variational_family"]["moments"]["natural_matrix"]
-        z = params["variational_family"]["inducing_inputs"]
+        natural_vector = self.natural_vector
+        natural_matrix = self.natural_matrix
+        z = self.inducing_inputs
         m = self.num_inducing
 
         # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        mean_function = self.posterior.prior.mean_function
+        kernel = self.posterior.prior.kernel
 
         # S⁻¹ = -2θ₂
         S_inv = -2 * natural_matrix
-        S_inv += jnp.eye(m) * jitter
+        S_inv += jnp.eye(m) * self.jitter
 
         # Compute L⁻¹, where LLᵀ = S, via a trick found in the NumPyro source code and https://nbviewer.org/gist/fehiepsi/5ef8e09e61604f10607380467eb82006#Precision-to-scale_tril:
         sqrt_inv = jnp.swapaxes(
             jnp.linalg.cholesky(S_inv[..., ::-1, ::-1])[..., ::-1, ::-1], -2, -1
         )
 
         # L = (L⁻¹)⁻¹I
@@ -524,362 +448,295 @@
 
         # S = LLᵀ:
         S = jnp.matmul(sqrt, sqrt.T)
 
         # μ = Sθ₁
         mu = jnp.matmul(S, natural_vector)
 
-        Kzz = kernel.gram(params["kernel"], z)
-        Kzz += identity(m) * jitter
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * self.jitter
         Lz = Kzz.to_root()
-        μz = mean_function(params["mean_function"], z)
-
-        def predict_fn(test_inputs: Float[Array, "N D"]) -> dx.MultivariateNormalTri:
-
-            # Unpack test inputs
-            t, n_test = test_inputs, test_inputs.shape[0]
+        muz = mean_function(z)
 
-            Ktt = kernel.gram(params["kernel"], t)
-            Kzt = kernel.cross_covariance(params["kernel"], z, t)
-            μt = mean_function(params["mean_function"], t)
+        # Unpack test inputs
+        t, n_test = test_inputs, test_inputs.shape[0]
 
-            # Lz⁻¹ Kzt
-            Lz_inv_Kzt = Lz.solve(Kzt)
+        Ktt = kernel.gram(t)
+        Kzt = kernel.cross_covariance(z, t)
+        mut = mean_function(t)
 
-            # Kzz⁻¹ Kzt
-            Kzz_inv_Kzt = Lz.T.solve(Lz_inv_Kzt)
+        # Lz⁻¹ Kzt
+        Lz_inv_Kzt = Lz.solve(Kzt)
 
-            # Ktz Kzz⁻¹ L
-            Ktz_Kzz_inv_L = jnp.matmul(Kzz_inv_Kzt.T, sqrt)
+        # Kzz⁻¹ Kzt
+        Kzz_inv_Kzt = Lz.T.solve(Lz_inv_Kzt)
 
-            # μt  +  Ktz Kzz⁻¹ (μ  -  μz)
-            mean = μt + jnp.matmul(Kzz_inv_Kzt.T, mu - μz)
+        # Ktz Kzz⁻¹ L
+        Ktz_Kzz_inv_L = jnp.matmul(Kzz_inv_Kzt.T, sqrt)
 
-            # Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Kzz⁻¹ S Kzz⁻¹ Kzt  [recall S = LLᵀ]
-            covariance = (
-                Ktt
-                - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
-                + jnp.matmul(Ktz_Kzz_inv_L, Ktz_Kzz_inv_L.T)
-            )
-            covariance += identity(n_test) * jitter
+        # μt  +  Ktz Kzz⁻¹ (μ  -  μz)
+        mean = mut + jnp.matmul(Kzz_inv_Kzt.T, mu - muz)
 
-            return GaussianDistribution(
-                loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
-            )
+        # Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Kzz⁻¹ S Kzz⁻¹ Kzt  [recall S = LLᵀ]
+        covariance = (
+            Ktt
+            - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
+            + jnp.matmul(Ktz_Kzz_inv_L, Ktz_Kzz_inv_L.T)
+        )
+        covariance += identity(n_test) * self.jitter
 
-        return predict_fn
+        return GaussianDistribution(
+            loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
+        )
 
 
+@dataclass
 class ExpectationVariationalGaussian(AbstractVariationalGaussian):
-    """The natural variational Gaussian family of probability distributions.
+    r"""The natural variational Gaussian family of probability distributions.
 
-    The variational family is q(f(·)) = ∫ p(f(·)|u) q(u) du, where u = f(z) are the function values at the inducing inputs z
-    and the distribution over the inducing inputs is q(u) = N(μ, S). Expressing the variational distribution, in the form of the
-    exponential family, q(u) = exp(θᵀ T(u) - a(θ)), gives rise to the natural paramerisation θ = (θ₁, θ₂) = (S⁻¹μ, -S⁻¹/2) and
-    sufficient stastics T(u) = [u, uuᵀ]. The expectation parameters are given by η = ∫ T(u) q(u) du. This gives a parameterisation,
-    η = (η₁, η₁) = (μ, S + uuᵀ) to perform model inference over.
+    The variational family is $`q(f(\cdot)) = \int p(f(\cdot)\mid u) q(u) \mathrm{d}u`$, where $`u = f(z)`$ are the
+    function values at the inducing inputs $`z`$ and the distribution over the inducing
+    inputs is $`q(u) = \mathcal{N}(\mu, S)`$. Expressing the variational distribution, in the form of
+    the exponential family, $`q(u) = exp(\theta^{\top} T(u) - a(\theta))`$, gives rise to the natural
+    parameterisation $`\theta  = (\theta_{1}, \theta_{2}) = (S^{-1}\mu  , -S^{-1}/2)`$ and sufficient statistics
+    $`T(u) = [u, uu^{\top}]`$. The expectation parameters are given by $`\nu = \int T(u) q(u) \mathrm{d}u`$.
+    This gives a parameterisation, $`\nu = (\nu_{1}, \nu_{2}) = (\mu  , S + uu^{\top})`$ to perform model
+    inference over.
     """
 
-    def __init__(
-        self,
-        prior: Prior,
-        inducing_inputs: Float[Array, "N D"],
-        name: Optional[str] = "Expectation variational Gaussian",
-    ) -> None:
-        """Initialise the expectation variational Gaussian family.
-
-        Args:
-            prior (Prior): The GP prior.
-            inducing_inputs (Float[Array, "N D"]): The inducing inputs.
-            name (Optional[str]): The name of the variational family.
-        """
-
-        super().__init__(prior, inducing_inputs, name)
-
-    def init_params(self, key: KeyArray) -> Dict:
-        """Return the expectation vector and matrix, inducing inputs, and hyperparameters that parameterise the expectation Gaussian distribution."""
-
-        self.num_inducing = self.inducing_inputs.shape[0]
+    expectation_vector: Float[Array, "M 1"] = None
+    expectation_matrix: Float[Array, "M M"] = None
 
-        m = self.num_inducing
-
-        return concat_dictionaries(
-            self.prior.init_params(key),
-            {
-                "variational_family": {
-                    "inducing_inputs": self.inducing_inputs,
-                    "moments": {
-                        "expectation_vector": jnp.zeros((m, 1)),
-                        "expectation_matrix": jnp.eye(m),
-                    },
-                }
-            },
-        )
+    def __post_init__(self):
+        if self.expectation_vector is None:
+            self.expectation_vector = jnp.zeros((self.num_inducing, 1))
+        if self.expectation_matrix is None:
+            self.expectation_matrix = jnp.eye(self.num_inducing)
 
-    def prior_kl(self, params: Dict) -> Float[Array, "1"]:
-        """Compute the KL-divergence between our current variational approximation and the Gaussian process prior.
+    def prior_kl(self) -> ScalarFloat:
+        r"""Evaluate the prior KL-divergence.
 
-        For this variational family, we have KL[q(f(·))||p(·)] = KL[q(u)||p(u)] = KL[N(μ, S)||N(mz, Kzz)],
-
-        with μ and S computed from the expectation paramerisation η = (μ, S + uuᵀ).
+        Compute the KL-divergence between our current variational approximation and
+        the Gaussian process prior.
 
-        Args:
-            params (Dict): The parameters at which our variational distribution and GP prior are to be evaluated.
+        For this variational family, we have
+        ```math
+        \begin{align}
+        \operatorname{KL}(q(f(\cdot))\mid\mid p(\cdot)) & = \operatorname{KL}(q(u)\mid\mid p(u)) \\
+            & =\operatorname{KL}(\mathcal{N}(\mu, S)\mid\mid \mathcal{N}(m_z, K_{zz})),
+        \end{align}
+        ```
+        where $\mu$ and $S$ are the expectation parameters of the variational
+        distribution and $m_z$ and $K_{zz}$ are the mean and covariance of the prior
+        distribution.
 
-        Returns:
-            Float[Array, "1"]: The KL-divergence between our variational approximation and the GP prior.
+        Returns
+        -------
+            ScalarFloat: The KL-divergence between our variational approximation and
+                the GP prior.
         """
-        jitter = get_global_config()["jitter"]
-
         # Unpack variational parameters
-        expectation_vector = params["variational_family"]["moments"][
-            "expectation_vector"
-        ]
-        expectation_matrix = params["variational_family"]["moments"][
-            "expectation_matrix"
-        ]
-        z = params["variational_family"]["inducing_inputs"]
+        expectation_vector = self.expectation_vector
+        expectation_matrix = self.expectation_matrix
+        z = self.inducing_inputs
         m = self.num_inducing
 
         # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        mean_function = self.posterior.prior.mean_function
+        kernel = self.posterior.prior.kernel
 
         # μ = η₁
         mu = expectation_vector
 
         # S = η₂ - η₁ η₁ᵀ
         S = expectation_matrix - jnp.outer(mu, mu)
-        S = jlo.DenseLinearOperator(S)
-        S += identity(m) * jitter
+        S = DenseLinearOperator(S)
+        S += identity(m) * self.jitter
 
-        μz = mean_function(params["mean_function"], z)
-        Kzz = kernel.gram(params["kernel"], z)
-        Kzz += identity(m) * jitter
+        muz = mean_function(z)
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * self.jitter
 
         qu = GaussianDistribution(loc=jnp.atleast_1d(mu.squeeze()), scale=S)
-        pu = GaussianDistribution(loc=jnp.atleast_1d(μz.squeeze()), scale=Kzz)
+        pu = GaussianDistribution(loc=jnp.atleast_1d(muz.squeeze()), scale=Kzz)
 
         return qu.kl_divergence(pu)
 
-    def predict(
-        self, params: Dict
-    ) -> Callable[[Float[Array, "N D"]], GaussianDistribution]:
-        """Compute the predictive distribution of the GP at the test inputs t.
+    def predict(self, test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
+        r"""Evaluate the predictive distribution.
 
-        This is the integral q(f(t)) = ∫ p(f(t)|u) q(u) du, which can be computed in closed form as
+        Compute the predictive distribution of the GP at the test inputs $t$.
 
-             N[f(t); μt + Ktz Kzz⁻¹ (μ - μz),  Ktt - Ktz Kzz⁻¹ Kzt + Ktz Kzz⁻¹ S Kzz⁻¹ Kzt ],
-
-        with μ and S computed from the expectation paramerisation η = (μ, S + uuᵀ).
-
-        Args:
-            params (Dict): The set of parameters that are to be used to parameterise our variational approximation and GP.
-
-        Returns:
-            Callable[[Float[Array, "N D"]], GaussianDistribution]: A function that accepts a set of test points and will return the predictive distribution at those points.
+        This is the integral $q(f(t)) = \int p(f(t)\mid u)q(u)\mathrm{d}u$, which can
+        be computed in closed form as  which can be computed in closed form as
+        ```math
+        \mathcal{N}(f(t); \mu_t + \mathbf{K}_{tz}\mathbf{K}_{zz}^{-1}(\mu - \mu_z), \mathbf{K}_{tt} - \mathbf{K}_{tz}\mathbf{K}_{zz}^{-1}\mathbf{K}_{zt} + \mathbf{K}_{tz}\mathbf{K}_{zz}^{-1}\mathbf{S} \mathbf{K}_{zz}^{-1}\mathbf{K}_{zt})
+        ```
+
+        with $\mu$ and $S$ computed from the expectation parameterisation
+        $\eta = (\mu, S + uu^\top)$.
+
+        Returns
+        -------
+            GaussianDistribution: The predictive distribution of the GP at the
+                test inputs $t$.
         """
-        jitter = get_global_config()["jitter"]
-
         # Unpack variational parameters
-        expectation_vector = params["variational_family"]["moments"][
-            "expectation_vector"
-        ]
-        expectation_matrix = params["variational_family"]["moments"][
-            "expectation_matrix"
-        ]
-        z = params["variational_family"]["inducing_inputs"]
+        expectation_vector = self.expectation_vector
+        expectation_matrix = self.expectation_matrix
+        z = self.inducing_inputs
         m = self.num_inducing
 
         # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        mean_function = self.posterior.prior.mean_function
+        kernel = self.posterior.prior.kernel
 
         # μ = η₁
         mu = expectation_vector
 
         # S = η₂ - η₁ η₁ᵀ
         S = expectation_matrix - jnp.matmul(mu, mu.T)
-        S = jlo.DenseLinearOperator(S)
-        S += identity(m) * jitter
+        S = DenseLinearOperator(S)
+        S += identity(m) * self.jitter
 
         # S = sqrt sqrtᵀ
         sqrt = S.to_root().to_dense()
 
-        Kzz = kernel.gram(params["kernel"], z)
-        Kzz += identity(m) * jitter
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * self.jitter
         Lz = Kzz.to_root()
-        μz = mean_function(params["mean_function"], z)
-
-        def predict_fn(test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
-
-            # Unpack test inputs
-            t, n_test = test_inputs, test_inputs.shape[0]
-
-            Ktt = kernel.gram(params["kernel"], t)
-            Kzt = kernel.cross_covariance(params["kernel"], z, t)
-            μt = mean_function(params["mean_function"], t)
+        muz = mean_function(z)
 
-            # Lz⁻¹ Kzt
-            Lz_inv_Kzt = Lz.solve(Kzt)
+        # Unpack test inputs
+        t, n_test = test_inputs, test_inputs.shape[0]
 
-            # Kzz⁻¹ Kzt
-            Kzz_inv_Kzt = Lz.T.solve(Lz_inv_Kzt)
+        Ktt = kernel.gram(t)
+        Kzt = kernel.cross_covariance(z, t)
+        mut = mean_function(t)
 
-            # Ktz Kzz⁻¹ sqrt
-            Ktz_Kzz_inv_sqrt = jnp.matmul(Kzz_inv_Kzt.T, sqrt)
+        # Lz⁻¹ Kzt
+        Lz_inv_Kzt = Lz.solve(Kzt)
 
-            # μt  +  Ktz Kzz⁻¹ (μ  -  μz)
-            mean = μt + jnp.matmul(Kzz_inv_Kzt.T, mu - μz)
+        # Kzz⁻¹ Kzt
+        Kzz_inv_Kzt = Lz.T.solve(Lz_inv_Kzt)
 
-            # Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Kzz⁻¹ S Kzz⁻¹ Kzt  [recall S = sqrt sqrtᵀ]
-            covariance = (
-                Ktt
-                - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
-                + jnp.matmul(Ktz_Kzz_inv_sqrt, Ktz_Kzz_inv_sqrt.T)
-            )
-            covariance += identity(n_test) * jitter
+        # Ktz Kzz⁻¹ sqrt
+        Ktz_Kzz_inv_sqrt = jnp.matmul(Kzz_inv_Kzt.T, sqrt)
 
-            return GaussianDistribution(
-                loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
-            )
-
-        return predict_fn
+        # μt  +  Ktz Kzz⁻¹ (μ  -  μz)
+        mean = mut + jnp.matmul(Kzz_inv_Kzt.T, mu - muz)
 
+        # Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Kzz⁻¹ S Kzz⁻¹ Kzt  [recall S = sqrt sqrtᵀ]
+        covariance = (
+            Ktt
+            - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
+            + jnp.matmul(Ktz_Kzz_inv_sqrt, Ktz_Kzz_inv_sqrt.T)
+        )
+        covariance += identity(n_test) * self.jitter
 
-class CollapsedVariationalGaussian(AbstractVariationalFamily):
-    """Collapsed variational Gaussian family of probability distributions.
-    The key reference is Titsias, (2009) - Variational Learning of Inducing Variables in Sparse Gaussian Processes."""
+        return GaussianDistribution(
+            loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
+        )
 
-    def __init__(
-        self,
-        prior: Prior,
-        likelihood: AbstractLikelihood,
-        inducing_inputs: Float[Array, "M D"],
-        name: str = "Collapsed variational Gaussian",
-    ):
-        """Initialise the collapsed variational Gaussian family of probability distributions.
 
-        Args:
-            prior (Prior): The prior distribution that we are approximating.
-            likelihood (AbstractLikelihood): The likelihood function that we are using to model the data.
-            inducing_inputs (Float[Array, "M D"]): The inducing inputs that are to be used to parameterise the variational Gaussian distribution.
-            name (str, optional): The name of the variational family. Defaults to "Collapsed variational Gaussian".
-        """
+@dataclass
+class CollapsedVariationalGaussian(AbstractVariationalGaussian):
+    r"""Collapsed variational Gaussian.
+
+    Collapsed variational Gaussian family of probability distributions.
+    The key reference is Titsias, (2009) - Variational Learning of Inducing Variables
+    in Sparse Gaussian Processes.
+    """
 
-        if not isinstance(likelihood, Gaussian):
+    def __post_init__(self):
+        if not isinstance(self.posterior.likelihood, Gaussian):
             raise TypeError("Likelihood must be Gaussian.")
 
-        self.prior = prior
-        self.likelihood = likelihood
-        self.inducing_inputs = inducing_inputs
-        self.num_inducing = self.inducing_inputs.shape[0]
-        self.name = name
-
-    def init_params(self, key: KeyArray) -> Dict:
-        """Return the variational mean vector, variational root covariance matrix, and inducing input vector that parameterise the variational Gaussian distribution."""
-        return concat_dictionaries(
-            self.prior.init_params(key),
-            {
-                "variational_family": {"inducing_inputs": self.inducing_inputs},
-                "likelihood": {
-                    "obs_noise": self.likelihood.init_params(key)["obs_noise"]
-                },
-            },
-        )
-
     def predict(
-        self,
-        params: Dict,
-        train_data: Dataset,
-    ) -> Callable[[Float[Array, "N D"]], GaussianDistribution]:
-        """Compute the predictive distribution of the GP at the test inputs.
+        self, test_inputs: Float[Array, "N D"], train_data: Dataset
+    ) -> GaussianDistribution:
+        r"""Compute the predictive distribution of the GP at the test inputs.
 
         Args:
-            params (Dict): The set of parameters that are to be used to parameterise our variational approximation and GP.
+            test_inputs (Float[Array, "N D"]): The test inputs $t$ at which to make
+                predictions.
             train_data (Dataset): The training data that was used to fit the GP.
 
-        Returns:
-            Callable[[Float[Array, "N D"]], dx.MultivariateNormalTri]: A function that accepts a set of test points and will return the predictive distribution at those points.
+        Returns
+        -------
+            GaussianDistribution: The predictive distribution of the collapsed
+                variational Gaussian process at the test inputs $t$.
         """
-        jitter = get_global_config()["jitter"]
-
-        def predict_fn(test_inputs: Float[Array, "N D"]) -> GaussianDistribution:
+        # Unpack test inputs
+        t, n_test = test_inputs, test_inputs.shape[0]
 
-            # Unpack test inputs
-            t, n_test = test_inputs, test_inputs.shape[0]
+        # Unpack training data
+        x, y = train_data.X, train_data.y
 
-            # Unpack training data
-            x, y = train_data.X, train_data.y
-
-            # Unpack variational parameters
-            noise = params["likelihood"]["obs_noise"]
-            z = params["variational_family"]["inducing_inputs"]
-            m = self.num_inducing
-
-            # Unpack mean function and kernel
-            mean_function = self.prior.mean_function
-            kernel = self.prior.kernel
+        # Unpack variational parameters
+        noise = self.posterior.likelihood.obs_noise
+        z = self.inducing_inputs
+        m = self.num_inducing
 
-            Kzx = kernel.cross_covariance(params["kernel"], z, x)
-            Kzz = kernel.gram(params["kernel"], z)
-            Kzz += identity(m) * jitter
+        # Unpack mean function and kernel
+        mean_function = self.posterior.prior.mean_function
+        kernel = self.posterior.prior.kernel
 
-            # Lz Lzᵀ = Kzz
-            Lz = Kzz.to_root()
+        Kzx = kernel.cross_covariance(z, x)
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * self.jitter
 
-            # Lz⁻¹ Kzx
-            Lz_inv_Kzx = Lz.solve(Kzx)
+        # Lz Lzᵀ = Kzz
+        Lz = Kzz.to_root()
 
-            # A = Lz⁻¹ Kzt / σ
-            A = Lz_inv_Kzx / jnp.sqrt(noise)
+        # Lz⁻¹ Kzx
+        Lz_inv_Kzx = Lz.solve(Kzx)
 
-            # AAᵀ
-            AAT = jnp.matmul(A, A.T)
+        # A = Lz⁻¹ Kzt / o
+        A = Lz_inv_Kzx / jnp.sqrt(noise)
 
-            # LLᵀ = I + AAᵀ
-            L = jnp.linalg.cholesky(jnp.eye(m) + AAT)
+        # AAᵀ
+        AAT = jnp.matmul(A, A.T)
 
-            μx = mean_function(params["mean_function"], x)
-            diff = y - μx
+        # LLᵀ = I + AAᵀ
+        L = jnp.linalg.cholesky(jnp.eye(m) + AAT)
 
-            # Lz⁻¹ Kzx (y - μx)
-            Lz_inv_Kzx_diff = jsp.linalg.cho_solve(
-                (L, True), jnp.matmul(Lz_inv_Kzx, diff)
-            )
+        mux = mean_function(x)
+        diff = y - mux
 
-            # Kzz⁻¹ Kzx (y - μx)
-            Kzz_inv_Kzx_diff = Lz.T.solve(Lz_inv_Kzx_diff)
+        # Lz⁻¹ Kzx (y - μx)
+        Lz_inv_Kzx_diff = jsp.linalg.cho_solve((L, True), jnp.matmul(Lz_inv_Kzx, diff))
 
-            Ktt = kernel.gram(params["kernel"], t)
-            Kzt = kernel.cross_covariance(params["kernel"], z, t)
-            μt = mean_function(params["mean_function"], t)
+        # Kzz⁻¹ Kzx (y - μx)
+        Kzz_inv_Kzx_diff = Lz.T.solve(Lz_inv_Kzx_diff)
 
-            # Lz⁻¹ Kzt
-            Lz_inv_Kzt = Lz.solve(Kzt)
+        Ktt = kernel.gram(t)
+        Kzt = kernel.cross_covariance(z, t)
+        mut = mean_function(t)
 
-            # L⁻¹ Lz⁻¹ Kzt
-            L_inv_Lz_inv_Kzt = jsp.linalg.solve_triangular(L, Lz_inv_Kzt, lower=True)
+        # Lz⁻¹ Kzt
+        Lz_inv_Kzt = Lz.solve(Kzt)
 
-            # μt + 1/σ² Ktz Kzz⁻¹ Kzx (y - μx)
-            mean = μt + jnp.matmul(Kzt.T / noise, Kzz_inv_Kzx_diff)
+        # L⁻¹ Lz⁻¹ Kzt
+        L_inv_Lz_inv_Kzt = jsp.linalg.solve_triangular(L, Lz_inv_Kzt, lower=True)
 
-            # Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Lz⁻¹ (I + AAᵀ)⁻¹ Lz⁻¹ Kzt
-            covariance = (
-                Ktt
-                - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
-                + jnp.matmul(L_inv_Lz_inv_Kzt.T, L_inv_Lz_inv_Kzt)
-            )
-            covariance += identity(n_test) * jitter
+        # μt + 1/o² Ktz Kzz⁻¹ Kzx (y - μx)
+        mean = mut + jnp.matmul(Kzt.T / noise, Kzz_inv_Kzx_diff)
 
-            return GaussianDistribution(
-                loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
-            )
+        # Ktt  -  Ktz Kzz⁻¹ Kzt  +  Ktz Lz⁻¹ (I + AAᵀ)⁻¹ Lz⁻¹ Kzt
+        covariance = (
+            Ktt
+            - jnp.matmul(Lz_inv_Kzt.T, Lz_inv_Kzt)
+            + jnp.matmul(L_inv_Lz_inv_Kzt.T, L_inv_Lz_inv_Kzt)
+        )
+        covariance += identity(n_test) * self.jitter
 
-        return predict_fn
+        return GaussianDistribution(
+            loc=jnp.atleast_1d(mean.squeeze()), scale=covariance
+        )
 
 
 __all__ = [
     "AbstractVariationalFamily",
     "AbstractVariationalGaussian",
     "VariationalGaussian",
     "WhitenedVariationalGaussian",
```

### Comparing `gpjax-0.5.9/gpjax/variational_inference.py` & `gpjax-0.6/gpjax/objectives.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,286 +1,390 @@
-# Copyright 2022 The GPJax Contributors. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-import abc
-from typing import Callable, Dict
+from abc import abstractmethod
+from dataclasses import dataclass
 
+from jax import vmap
 import jax.numpy as jnp
 import jax.scipy as jsp
-from jax import vmap
-from jaxtyping import Array, Float
-
-from jaxlinop import identity
-from jax.random import KeyArray
-from jaxutils import PyTree
-
-from .config import get_global_config
-from .gps import AbstractPosterior
-from .likelihoods import Gaussian
-from .quadrature import gauss_hermite_quadrature
-from jaxutils import Dataset
-from .utils import concat_dictionaries
-from .variational_families import (
-    AbstractVariationalFamily,
-    CollapsedVariationalGaussian,
+import jax.tree_util as jtu
+from jaxtyping import Float
+import tensorflow_probability.substrates.jax as tfp
+
+from gpjax.base import (
+    Module,
+    static_field,
+)
+from gpjax.dataset import Dataset
+from gpjax.gaussian_distribution import GaussianDistribution
+from gpjax.linops import identity
+from gpjax.quadrature import gauss_hermite_quadrature
+from gpjax.typing import (
+    Array,
+    ScalarFloat,
 )
 
-import deprecation
-
+tfd = tfp.distributions
 
-class AbstractVariationalInference(PyTree):
-    """A base class for inference and training of variational families against an extact posterior"""
 
-    def __init__(
-        self,
-        posterior: AbstractPosterior,
-        variational_family: AbstractVariationalFamily,
-    ) -> None:
-        """Initialise the variational inference module.
+@dataclass
+class AbstractObjective(Module):
+    r"""Abstract base class for objectives."""
 
-        Args:
-            posterior (AbstractPosterior): The exact posterior distribution.
-            variational_family (AbstractVariationalFamily): The variational family to be trained.
-        """
-        self.posterior = posterior
-        self.prior = self.posterior.prior
-        self.likelihood = self.posterior.likelihood
-        self.variational_family = variational_family
-
-    def init_params(self, key: KeyArray) -> Dict:
-        """Construct the parameter set used within the variational scheme adopted."""
-        hyperparams = concat_dictionaries(
-            {"likelihood": self.posterior.likelihood.init_params(key)},
-            self.variational_family.init_params(key),
-        )
-        return hyperparams
+    negative: bool = static_field(False)
+    constant: float = static_field(init=False, repr=False)
 
-    @deprecation.deprecated(
-        deprecated_in="0.5.7",
-        removed_in="0.6.0",
-        details="Use the ``init_params`` method for parameter initialisation.",
-    )
-    def _initialise_params(self, key: KeyArray) -> Dict:
-        """Deprecated method for initialising the GP's parameters. Succeded by ``init_params``."""
-        return self.init_params(key)
+    def __post_init__(self) -> None:
+        self.constant = jnp.array(-1.0) if self.negative else jnp.array(1.0)
 
-    @abc.abstractmethod
-    def elbo(
-        self,
-        train_data: Dataset,
-    ) -> Callable[[Dict], Float[Array, "1"]]:
-        """Placeholder method for computing the evidence lower bound function (ELBO), given a training dataset and a set of transformations that map each parameter onto the entire real line.
+    def __hash__(self):
+        return hash(tuple(jtu.tree_leaves(self)))  # Probably put this on the Module!
 
-        Args:
-            train_data (Dataset): The training dataset for which the ELBO is to be computed.
+    def __call__(self, *args, **kwargs) -> ScalarFloat:
+        return self.step(*args, **kwargs)
 
-        Returns:
-            Callable[[Array], Array]: A function that computes the ELBO given a set of parameters.
-        """
+    @abstractmethod
+    def step(self, *args, **kwargs) -> ScalarFloat:
         raise NotImplementedError
 
 
-class StochasticVI(AbstractVariationalInference):
-    """Stochastic Variational inference training module. The key reference is Hensman et. al., (2013) - Gaussian processes for big data."""
-
-    def elbo(
-        self, train_data: Dataset, negative: bool = False
-    ) -> Callable[[Float[Array, "N D"]], Float[Array, "1"]]:
-        """Compute the evidence lower bound under this model. In short, this requires evaluating the expectation of the model's log-likelihood under the variational approximation. To this, we sum the KL divergence from the variational posterior to the prior. When batching occurs, the result is scaled by the batch size relative to the full dataset size.
+class ConjugateMLL(AbstractObjective):
+    def step(
+        self,
+        posterior: "gpjax.gps.ConjugatePosterior",  # noqa: F821
+        train_data: Dataset,  # noqa: F821
+    ) -> ScalarFloat:
+        r"""Evaluate the marginal log-likelihood of the Gaussian process.
+
+        Compute the marginal log-likelihood function of the Gaussian process.
+        The returned function can then be used for gradient based optimisation
+        of the model's parameters or for model comparison. The implementation
+        given here enables exact estimation of the Gaussian process' latent
+        function values.
+
+        For a training dataset $`\{x_n, y_n\}_{n=1}^N`$, set of test inputs
+        $`\mathbf{x}^{\star}`$ the corresponding latent function evaluations are given
+        by $`\mathbf{f}=f(\mathbf{x})`$ and $`\mathbf{f}^{\star}f(\mathbf{x}^{\star})`$,
+        the marginal log-likelihood is given by:
+        ```math
+        \begin{align}
+            \log p(\mathbf{y}) & = \int p(\mathbf{y}\mid\mathbf{f})p(\mathbf{f}, \mathbf{f}^{\star}\mathrm{d}\mathbf{f}^{\star}\\
+            &=0.5\left(-\mathbf{y}^{\top}\left(k(\mathbf{x}, \mathbf{x}') +\sigma^2\mathbf{I}_N  \right)^{-1}\mathbf{y}-\log\lvert k(\mathbf{x}, \mathbf{x}') + \sigma^2\mathbf{I}_N\rvert - n\log 2\pi \right).
+        \end{align}
+        ```
+
+        For a given ``ConjugatePosterior`` object, the following code snippet shows
+        how the marginal log-likelihood can be evaluated.
+
+        Example:
+        ```python
+            >>> import gpjax as gpx
+            >>>
+            >>> xtrain = jnp.linspace(0, 1).reshape(-1, 1)
+            >>> ytrain = jnp.sin(xtrain)
+            >>> D = gpx.Dataset(X=xtrain, y=ytrain)
+            >>>
+            >>> meanf = gpx.mean_functions.Constant()
+            >>> kernel = gpx.kernels.RBF()
+            >>> likelihood = gpx.likelihoods.Gaussian(num_datapoints=D.n)
+            >>> prior = gpx.Prior(mean_function = meanf, kernel=kernel)
+            >>> posterior = prior * likelihood
+            >>>
+            >>> mll = gpx.ConjugateMLL(negative=True)
+            >>> mll(posterior, train_data = D)
+        ```
+
+        Our goal is to maximise the marginal log-likelihood. Therefore, when optimising
+        the model's parameters with respect to the parameters, we use the negative
+        marginal log-likelihood. This can be realised through
+
+        ```python
+            mll = gpx.ConjugateMLL(negative=True)
+        ```
+
+        For optimal performance, the marginal log-likelihood should be ``jax.jit``
+        compiled.
+        ```python
+            mll = jit(gpx.ConjugateMLL(negative=True))
+        ```
 
         Args:
-            train_data (Dataset): The training data for which we should maximise the ELBO with respect to.
-            negative (bool, optional): Whether or not the resultant elbo function should be negative. For gradient descent where we minimise our objective function this argument should be true as minimisation of the negative corresponds to maximisation of the ELBO. Defaults to False.
-
-        Returns:
-            Callable[[Dict, Dataset], Array]: A callable function that accepts a current parameter estimate and batch of data for which gradients should be computed.
+            posterior (ConjugatePosterior): The posterior distribution for which
+                we want to compute the marginal log-likelihood.
+            train_data (Dataset): The training dataset used to compute the
+                marginal log-likelihood.
+
+        Returns
+        -------
+            ScalarFloat: The marginal log-likelihood of the Gaussian process for the
+                current parameter set.
         """
+        x, y, n = train_data.X, train_data.y, train_data.n
 
-        # Constant for whether or not to negate the elbo for optimisation purposes
-        constant = jnp.array(-1.0) if negative else jnp.array(1.0)
-
-        def elbo_fn(params: Dict, batch: Dataset) -> Float[Array, "1"]:
-            # KL[q(f(·)) || p(f(·))]
-            kl = self.variational_family.prior_kl(params)
-
-            # ∫[log(p(y|f(·))) q(f(·))] df(·)
-            var_exp = self.variational_expectation(params, batch)
-
-            # For batch size b, we compute  n/b * Σᵢ[ ∫log(p(y|f(xᵢ))) q(f(xᵢ)) df(xᵢ)] - KL[q(f(·)) || p(f(·))]
-            return constant * (jnp.sum(var_exp) * train_data.n / batch.n - kl)
-
-        return elbo_fn
-
-    def variational_expectation(
-        self, params: Dict, batch: Dataset
-    ) -> Float[Array, "N 1"]:
-        """Compute the expectation of our model's log-likelihood under our variational distribution. Batching can be done here to speed up computation.
+        # Observation noise o²
+        obs_noise = posterior.likelihood.obs_noise
+        mx = posterior.prior.mean_function(x)
+
+        # Σ = (Kxx + Io²) = LLᵀ
+        Kxx = posterior.prior.kernel.gram(x)
+        Kxx += identity(n) * posterior.prior.jitter
+        Sigma = Kxx + identity(n) * obs_noise
+
+        # p(y | x, θ), where θ are the model hyperparameters:
+        mll = GaussianDistribution(jnp.atleast_1d(mx.squeeze()), Sigma)
+
+        return self.constant * (mll.log_prob(jnp.atleast_1d(y.squeeze())).squeeze())
+
+
+class LogPosteriorDensity(AbstractObjective):
+    r"""The log-posterior density of a non-conjugate Gaussian process. This is
+    sometimes referred to as the marginal log-likelihood.
+    """
+
+    def step(
+        self, posterior: "gpjax.gps.NonConjugatePosterior", data: Dataset  # noqa: F821
+    ) -> ScalarFloat:
+        r"""Evaluate the log-posterior density of a Gaussian process.
+
+        Compute the marginal log-likelihood, or log-posterior density of the Gaussian
+        process. The returned function can then be used for gradient based optimisation
+        of the model's parameters or for model comparison. The implementation given
+        here is general and will work for any likelihood support by GPJax.
+
+        Unlike the marginal_log_likelihood function of the `ConjugatePosterior` object,
+        the marginal_log_likelihood function of the `NonConjugatePosterior` object does
+        not provide an exact marginal log-likelihood function. Instead, the
+        `NonConjugatePosterior` object represents the posterior distributions as a
+        function of the model's hyperparameters and the latent function. Markov chain
+        Monte Carlo, variational inference, or Laplace approximations can then be used
+        to sample from, or optimise an approximation to, the posterior distribution.
 
         Args:
-            params (Dict): The set of parameters that induce our variational approximation.
-            batch (Dataset): The data batch for which the expectation should be computed for.
-
-        Returns:
-            Array: The expectation of the model's log-likelihood under our variational distribution.
+            posterior (NonConjugatePosterior): The posterior distribution for which
+                we want to compute the marginal log-likelihood.
+            data (Dataset): The training dataset used to compute the
+                marginal log-likelihood.
+
+        Returns
+        -------
+            ScalarFloat: The log-posterior density of the Gaussian process for the
+                current parameter set.
         """
+        # Unpack the training data
+        x, y, n = data.X, data.y, data.n
+        Kxx = posterior.prior.kernel.gram(x)
+        Kxx += identity(n) * posterior.prior.jitter
+        Lx = Kxx.to_root()
 
-        # Unpack training batch
-        x, y = batch.X, batch.y
+        # Compute the prior mean function
+        mx = posterior.prior.mean_function(x)
 
-        # Variational distribution q(f(·)) = N(f(·); μ(·), Σ(·, ·))
-        q = self.variational_family(params)
+        # Whitened function values, wx, corresponding to the inputs, x
+        wx = posterior.latent
 
-        # Compute variational mean, μ(x), and variance, √diag(Σ(x, x)), at training inputs, x
-        def q_moments(x):
-            qx = q(x)
-            return qx.mean(), qx.variance()
+        # f(x) = mx  +  Lx wx
+        fx = mx + Lx @ wx
 
-        mean, variance = vmap(q_moments)(x[:, None])
+        # p(y | f(x), θ), where θ are the model hyperparameters
+        likelihood = posterior.likelihood.link_function(fx)
 
-        # log(p(y|f(x)))
-        link_function = self.likelihood.link_function
-        log_prob = vmap(lambda f, y: link_function(params["likelihood"], f).log_prob(y))
+        # Whitened latent function values prior, p(wx | θ) = N(0, I)
+        latent_prior = tfd.Normal(loc=0.0, scale=1.0)
 
-        # ≈ ∫[log(p(y|f(x))) q(f(x))] df(x)
-        expectation = gauss_hermite_quadrature(log_prob, mean, jnp.sqrt(variance), y=y)
+        return self.constant * (
+            likelihood.log_prob(y).sum() + latent_prior.log_prob(wx).sum()
+        )
 
-        return expectation
 
+NonConjugateMLL = LogPosteriorDensity
 
-class CollapsedVI(AbstractVariationalInference):
-    """Collapsed variational inference for a sparse Gaussian process regression model.
-    The key reference is Titsias, (2009) - Variational Learning of Inducing Variables in Sparse Gaussian Processes."""
 
-    def __init__(
+class ELBO(AbstractObjective):
+    def step(
         self,
-        posterior: AbstractPosterior,
-        variational_family: AbstractVariationalFamily,
-    ) -> None:
-        """Initialise the variational inference module.
+        variational_family: "gpjax.variational_families.AbstractVariationalFamily",  # noqa: F821
+        train_data: Dataset,
+    ) -> ScalarFloat:
+        r"""Compute the evidence lower bound of a variational approximation.
+
+        Compute the evidence lower bound under this model. In short, this requires
+        evaluating the expectation of the model's log-likelihood under the variational
+        approximation. To this, we sum the KL divergence from the variational posterior
+        to the prior. When batching occurs, the result is scaled by the batch size
+        relative to the full dataset size.
 
         Args:
-            posterior (AbstractPosterior): The exact posterior distribution.
-            variational_family (AbstractVariationalFamily): The variational family to be trained.
+            variational_family (AbstractVariationalFamily): The variational
+                approximation for whose parameters we should maximise the ELBO with
+                respect to.
+            train_data (Dataset): The training data for which we should maximise the
+                ELBO with respect to.
+
+        Returns
+        -------
+            ScalarFloat: The evidence lower bound of the variational approximation for
+                the current model parameter set.
         """
+        # KL[q(f(·)) || p(f(·))]
+        kl = variational_family.prior_kl()
 
-        if not isinstance(posterior.likelihood, Gaussian):
-            raise TypeError("Likelihood must be Gaussian.")
+        # ∫[log(p(y|f(·))) q(f(·))] df(·)
+        var_exp = variational_expectation(variational_family, train_data)
 
-        if not isinstance(variational_family, CollapsedVariationalGaussian):
-            raise TypeError("Variational family must be CollapsedVariationalGaussian.")
+        # For batch size b, we compute  n/b * Σᵢ[ ∫log(p(y|f(xᵢ))) q(f(xᵢ)) df(xᵢ)] - KL[q(f(·)) || p(f(·))]
+        return self.constant * (
+            jnp.sum(var_exp)
+            * variational_family.posterior.likelihood.num_datapoints
+            / train_data.n
+            - kl
+        )
 
-        super().__init__(posterior, variational_family)
 
-    def elbo(
-        self, train_data: Dataset, negative: bool = False
-    ) -> Callable[[Dict], Float[Array, "1"]]:
-        """Compute the evidence lower bound under this model. In short, this requires evaluating the expectation of the model's log-likelihood under the variational approximation. To this, we sum the KL divergence from the variational posterior to the prior. When batching occurs, the result is scaled by the batch size relative to the full dataset size.
+def variational_expectation(
+    variational_family: "gpjax.variational_families.AbstractVariationalFamily",  # noqa: F821
+    train_data: Dataset,
+) -> Float[Array, " N"]:
+    r"""Compute the variational expectation.
+
+    Compute the expectation of our model's log-likelihood under our variational
+    distribution. Batching can be done here to speed up computation.
+
+    Args:
+        variational_family (AbstractVariationalFamily): The variational family that we
+            are using to approximate the posterior.
+        train_data (Dataset): The batch for which the expectation should be computed
+            for.
+
+    Returns
+    -------
+        Array: The expectation of the model's log-likelihood under our variational
+            distribution.
+    """
+    # Unpack training batch
+    x, y = train_data.X, train_data.y
+
+    # Variational distribution q(f(·)) = N(f(·); μ(·), Σ(·, ·))
+    q = variational_family
+
+    # Compute variational mean, μ(x), and variance, √diag(Σ(x, x)), at the training
+    # inputs, x
+    def q_moments(x):
+        qx = q(x)
+        return qx.mean(), qx.variance()
+
+    mean, variance = vmap(q_moments)(x[:, None])
+
+    link_function = variational_family.posterior.likelihood.link_function
+    log_prob = vmap(lambda f, y: link_function(f).log_prob(y))
+
+    # ≈ ∫[log(p(y|f(x))) q(f(x))] df(x)
+    expectation = gauss_hermite_quadrature(log_prob, mean, jnp.sqrt(variance), y=y)
+
+    return expectation
+
+
+class CollapsedELBO(AbstractObjective):
+    r"""The collapsed evidence lower bound.
+
+    Collapsed variational inference for a sparse Gaussian process regression model.
+    The key reference is Titsias, (2009) - Variational Learning of Inducing Variables
+    in Sparse Gaussian Processes.
+    """
 
-        Args:
-            train_data (Dataset): The training data for which we should maximise the ELBO with respect to.
-            negative (bool, optional): Whether or not the resultant elbo function should be negative. For gradient descent where we minimise our objective function this argument should be true as minimisation of the negative corresponds to maximisation of the ELBO. Defaults to False.
+    def step(
+        self,
+        variational_family: "gpjax.variational_families.AbstractVariationalFamily",  # noqa: F821
+        train_data: Dataset,
+    ) -> ScalarFloat:
+        r"""Compute a single step of the collapsed evidence lower bound.
 
-        Returns:
-            Callable[[Dict, Dataset], Array]: A callable function that accepts a current parameter estimate for which gradients should be computed.
-        """
+        Compute the evidence lower bound under this model. In short, this requires
+        evaluating the expectation of the model's log-likelihood under the variational
+        approximation. To this, we sum the KL divergence from the variational posterior
+        to the prior. When batching occurs, the result is scaled by the batch size
+        relative to the full dataset size.
 
+        Args:
+            variational_family (AbstractVariationalFamily): The variational
+                approximation for whose parameters we should maximise the ELBO with
+                respect to.
+            train_data (Dataset): The training data for which we should maximise the
+                ELBO with respect to.
+
+        Returns
+        -------
+            ScalarFloat: The evidence lower bound of the variational approximation for
+                the current model parameter set.
+        """
         # Unpack training data
         x, y, n = train_data.X, train_data.y, train_data.n
 
         # Unpack mean function and kernel
-        mean_function = self.prior.mean_function
-        kernel = self.prior.kernel
+        mean_function = variational_family.posterior.prior.mean_function
+        kernel = variational_family.posterior.prior.kernel
+
+        m = variational_family.num_inducing
+
+        noise = variational_family.posterior.likelihood.obs_noise
+        z = variational_family.inducing_inputs
+        Kzz = kernel.gram(z)
+        Kzz += identity(m) * variational_family.jitter
+        Kzx = kernel.cross_covariance(z, x)
+        Kxx_diag = vmap(kernel, in_axes=(0, 0))(x, x)
+        μx = mean_function(x)
+
+        Lz = Kzz.to_root()
+
+        # Notation and derivation:
+        #
+        # Let Q = KxzKzz⁻¹Kzx, we must compute the log normal pdf:
+        #
+        #   log N(y; μx, o²I + Q) = -nπ - n/2 log|o²I + Q|
+        #   - 1/2 (y - μx)ᵀ (o²I + Q)⁻¹ (y - μx).
+        #
+        # The log determinant |o²I + Q| is computed via applying the matrix determinant
+        #   lemma
+        #
+        #   |o²I + Q| = log|o²I| + log|I + Lz⁻¹ Kzx (o²I)⁻¹ Kxz Lz⁻¹| = log(o²) +  log|B|,
+        #
+        #   with B = I + AAᵀ and A = Lz⁻¹ Kzx / o.
+        #
+        # Similarly we apply matrix inversion lemma to invert o²I + Q
+        #
+        #   (o²I + Q)⁻¹ = (Io²)⁻¹ - (Io²)⁻¹ Kxz Lz⁻ᵀ (I + Lz⁻¹ Kzx (Io²)⁻¹ Kxz Lz⁻ᵀ )⁻¹ Lz⁻¹ Kzx (Io²)⁻¹
+        #               = (Io²)⁻¹ - (Io²)⁻¹ oAᵀ (I + oA (Io²)⁻¹ oAᵀ)⁻¹ oA (Io²)⁻¹
+        #               = I/o² - Aᵀ B⁻¹ A/o²,
+        #
+        # giving the quadratic term as
+        #
+        #   (y - μx)ᵀ (o²I + Q)⁻¹ (y - μx) = [(y - μx)ᵀ(y - µx)  - (y - μx)ᵀ Aᵀ B⁻¹ A (y - μx)]/o²,
+        #
+        #   with A and B defined as above.
+
+        A = Lz.solve(Kzx) / jnp.sqrt(noise)
+
+        # AAᵀ
+        AAT = jnp.matmul(A, A.T)
+
+        # B = I + AAᵀ
+        B = jnp.eye(m) + AAT
+
+        # LLᵀ = I + AAᵀ
+        L = jnp.linalg.cholesky(B)
+
+        # log|B| = 2 trace(log|L|) = 2 Σᵢ log Lᵢᵢ  [since |B| = |LLᵀ| = |L|²  => log|B| = 2 log|L|, and |L| = Πᵢ Lᵢᵢ]
+        log_det_B = 2.0 * jnp.sum(jnp.log(jnp.diagonal(L)))
+
+        diff = y - μx
+
+        # L⁻¹ A (y - μx)
+        L_inv_A_diff = jsp.linalg.solve_triangular(L, jnp.matmul(A, diff), lower=True)
+
+        # (y - μx)ᵀ (Io² + Q)⁻¹ (y - μx)
+        quad = (jnp.sum(diff**2) - jnp.sum(L_inv_A_diff**2)) / noise
 
-        m = self.variational_family.num_inducing
-        jitter = get_global_config()["jitter"]
+        # 2 * log N(y; μx, Io² + Q)
+        two_log_prob = -n * jnp.log(2.0 * jnp.pi * noise) - log_det_B - quad
 
-        # Constant for whether or not to negate the elbo for optimisation purposes
-        constant = jnp.array(-1.0) if negative else jnp.array(1.0)
+        # 1/o² tr(Kxx - Q) [Trace law tr(AB) = tr(BA) => tr(KxzKzz⁻¹Kzx) = tr(KxzLz⁻ᵀLz⁻¹Kzx) = tr(Lz⁻¹Kzx KxzLz⁻ᵀ) = trace(o²AAᵀ)]
+        two_trace = jnp.sum(Kxx_diag) / noise - jnp.trace(AAT)
 
-        def elbo_fn(params: Dict) -> Float[Array, "1"]:
-            noise = params["likelihood"]["obs_noise"]
-            z = params["variational_family"]["inducing_inputs"]
-            Kzz = kernel.gram(params["kernel"], z)
-            Kzz += identity(m) * jitter
-            Kzx = kernel.cross_covariance(params["kernel"], z, x)
-            Kxx_diag = vmap(kernel, in_axes=(None, 0, 0))(params["kernel"], x, x)
-            μx = mean_function(params["mean_function"], x)
-
-            Lz = Kzz.to_root()
-
-            # Notation and derivation:
-            #
-            # Let Q = KxzKzz⁻¹Kzx, we must compute the log normal pdf:
-            #
-            #   log N(y; μx, σ²I + Q) = -nπ - n/2 log|σ²I + Q| - 1/2 (y - μx)ᵀ (σ²I + Q)⁻¹ (y - μx).
-            #
-            # The log determinant |σ²I + Q| is computed via applying the matrix determinant lemma
-            #
-            #   |σ²I + Q| = log|σ²I| + log|I + Lz⁻¹ Kzx (σ²I)⁻¹ Kxz Lz⁻¹| = log(σ²) +  log|B|,
-            #
-            #   with B = I + AAᵀ and A = Lz⁻¹ Kzx / σ.
-            #
-            # Similary we apply matrix inversion lemma to invert σ²I + Q
-            #
-            #   (σ²I + Q)⁻¹ = (Iσ²)⁻¹ - (Iσ²)⁻¹ Kxz Lz⁻ᵀ (I + Lz⁻¹ Kzx (Iσ²)⁻¹ Kxz Lz⁻ᵀ )⁻¹ Lz⁻¹ Kzx (Iσ²)⁻¹
-            #               = (Iσ²)⁻¹ - (Iσ²)⁻¹ σAᵀ (I + σA (Iσ²)⁻¹ σAᵀ)⁻¹ σA (Iσ²)⁻¹
-            #               = I/σ² - Aᵀ B⁻¹ A/σ²,
-            #
-            # giving the quadratic term as
-            #
-            #   (y - μx)ᵀ (σ²I + Q)⁻¹ (y - μx) = [(y - μx)ᵀ(y - µx)  - (y - μx)ᵀ Aᵀ B⁻¹ A (y - μx)]/σ²,
-            #
-            #   with A and B defined as above.
-
-            A = Lz.solve(Kzx) / jnp.sqrt(noise)
-
-            # AAᵀ
-            AAT = jnp.matmul(A, A.T)
-
-            # B = I + AAᵀ
-            B = jnp.eye(m) + AAT
-
-            # LLᵀ = I + AAᵀ
-            L = jnp.linalg.cholesky(B)
-
-            # log|B| = 2 trace(log|L|) = 2 Σᵢ log Lᵢᵢ  [since |B| = |LLᵀ| = |L|²  => log|B| = 2 log|L|, and |L| = Πᵢ Lᵢᵢ]
-            log_det_B = 2.0 * jnp.sum(jnp.log(jnp.diagonal(L)))
-
-            diff = y - μx
-
-            # L⁻¹ A (y - μx)
-            L_inv_A_diff = jsp.linalg.solve_triangular(
-                L, jnp.matmul(A, diff), lower=True
-            )
-
-            # (y - μx)ᵀ (Iσ² + Q)⁻¹ (y - μx)
-            quad = (jnp.sum(diff**2) - jnp.sum(L_inv_A_diff**2)) / noise
-
-            # 2 * log N(y; μx, Iσ² + Q)
-            two_log_prob = -n * jnp.log(2.0 * jnp.pi * noise) - log_det_B - quad
-
-            # 1/σ² tr(Kxx - Q) [Trace law tr(AB) = tr(BA) => tr(KxzKzz⁻¹Kzx) = tr(KxzLz⁻ᵀLz⁻¹Kzx) = tr(Lz⁻¹Kzx KxzLz⁻ᵀ) = trace(σ²AAᵀ)]
-            two_trace = jnp.sum(Kxx_diag) / noise - jnp.trace(AAT)
-
-            # log N(y; μx, Iσ² + KxzKzz⁻¹Kzx) - 1/2σ² tr(Kxx - KxzKzz⁻¹Kzx)
-            return constant * (two_log_prob - two_trace).squeeze() / 2.0
-
-        return elbo_fn
-
-
-__all__ = [
-    "AbstractVariationalInference",
-    "StochasticVI",
-    "CollapsedVI",
-]
+        # log N(y; μx, Io² + KxzKzz⁻¹Kzx) - 1/2o² tr(Kxx - KxzKzz⁻¹Kzx)
+        return self.constant * (two_log_prob - two_trace).squeeze() / 2.0
```

### Comparing `gpjax-0.5.9/gpjax.egg-info/PKG-INFO` & `gpjax-0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 Metadata-Version: 2.1
 Name: gpjax
-Version: 0.5.9
-Summary: Didactic Gaussian processes in Jax.
+Version: 0.6
+Summary: Gaussian processes in JAX.
+Home-page: https://github.com/JaxGaussianProcesses/GPJax
+License: Apache-2.0
+Keywords: gaussian-processes jax machine-learning bayesian
 Author: Thomas Pinder
-Author-email: t.pinder2@lancaster.ac.uk
-License: LICENSE
+Author-email: tompinder@live.co.uk
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beartype (>=0.13.1,<0.14.0)
+Requires-Dist: jax (>=0.4.1)
+Requires-Dist: jaxlib (>=0.4.6,<0.5.0)
+Requires-Dist: jaxtyping (>=0.2.15,<0.3.0)
+Requires-Dist: optax (>=0.1.4,<0.2.0)
+Requires-Dist: orbax-checkpoint (>=0.2.0,<0.3.0)
+Requires-Dist: simple-pytree (>=0.1.7,<0.2.0)
+Requires-Dist: tensorflow-probability (>=0.19.0,<0.20.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Documentation, https://gpjax.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/thomaspinder/GPJax
-Keywords: gaussian-processes jax machine-learning bayesian
-Requires-Python: >=3.7
+Project-URL: Repository, https://github.com/JaxGaussianProcesses/GPJax
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: cuda
 
 <!-- <h1 align='center'>GPJax</h1>
 <h2 align='center'>Gaussian processes in Jax.</h2> -->
 <p align="center">
 <img width="700" height="300" src="https://github.com/JaxGaussianProcesses/GPJax/raw/master/docs/_static/gpjax_logo.svg" alt="GPJax's logo">
 </p>
 
@@ -28,47 +42,65 @@
 [![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
 
 [**Quickstart**](#simple-example)
 | [**Install guide**](#installation)
 | [**Documentation**](https://gpjax.readthedocs.io/en/latest/)
 | [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
 
-GPJax aims to provide a low-level interface to Gaussian process (GP) models in [Jax](https://github.com/google/jax), structured to give researchers maximum flexibility in extending the code to suit their own needs. The idea is that the code should be as close as possible to the maths we write on paper when working with GP models.
+GPJax aims to provide a low-level interface to Gaussian process (GP) models in
+[Jax](https://github.com/google/jax), structured to give researchers maximum
+flexibility in extending the code to suit their own needs. The idea is that the
+code should be as close as possible to the maths we write on paper when working
+with GP models.
 
 # Package support
 
-GPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today, the maintenance of GPJax is undertaken by [Thomas Pinder](https://github.com/thomaspinder) and [Daniel Dodd](https://github.com/Daniel-Dodd).
-
-We would be delighted to receive contributions from interested individuals and groups. To learn how you can get involved, please read our [guide for contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md). If you have any questions, we encourage you to [open an issue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For broader conversations, such as best GP fitting practices or questions about the mathematics of GPs, we invite you to [open a discussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).
-
-Feel free to join our [Slack Channel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw), where we can discuss the development of GPJax and broader support for Gaussian process modelling.
+GPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today,
+the maintenance of GPJax is undertaken by [Thomas
+Pinder](https://github.com/thomaspinder) and [Daniel
+Dodd](https://github.com/Daniel-Dodd).
+
+We would be delighted to receive contributions from interested individuals and
+groups. To learn how you can get involved, please read our [guide for
+contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md).
+If you have any questions, we encourage you to [open an
+issue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For
+broader conversations, such as best GP fitting practices or questions about the
+mathematics of GPs, we invite you to [open a
+discussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).
+
+Feel free to join our [Slack
+Channel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw),
+where we can discuss the development of GPJax and broader support for Gaussian
+process modelling.
 
 # Supported methods and interfaces
 
 ## Notebook examples
 
 > - [**Conjugate Inference**](https://gpjax.readthedocs.io/en/latest/examples/regression.html)
 > - [**Classification with MCMC**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
 > - [**Sparse Variational Inference**](https://gpjax.readthedocs.io/en/latest/examples/uncollapsed_vi.html)
 > - [**BlackJax Integration**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
 > - [**Laplace Approximation**](https://gpjax.readthedocs.io/en/latest/examples/classification.html#Laplace-approximation)
-> - [**TensorFlow Probability Integration**](https://gpjax.readthedocs.io/en/latest/examples/tfp_integration.html)
 > - [**Inference on Non-Euclidean Spaces**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
 > - [**Inference on Graphs**](https://gpjax.readthedocs.io/en/latest/examples/graph_kernels.html)
 > - [**Learning Gaussian Process Barycentres**](https://gpjax.readthedocs.io/en/latest/examples/barycentres.html)
 > - [**Deep Kernel Regression**](https://gpjax.readthedocs.io/en/latest/examples/haiku.html)
-> - [**Natural Gradients**](https://gpjax.readthedocs.io/en/latest/examples/natgrads.html)
 
 ## Guides for customisation
-> 
+>
 > - [**Custom kernels**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
 > - [**UCI regression**](https://gpjax.readthedocs.io/en/latest/examples/yacht.html)
 
 ## Conversion between `.ipynb` and `.py`
-Above examples are stored in [examples](examples) directory in the double percent (`py:percent`) format. Checkout [jupytext using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more info.
+Above examples are stored in [examples](examples) directory in the double
+percent (`py:percent`) format. Checkout [jupytext
+using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more
+info.
 
 * To convert `example.py` to `example.ipynb`, run:
 
 ```bash
 jupytext --to notebook example.py
 ```
 
@@ -83,89 +115,69 @@
 Let us import some dependencies and simulate a toy dataset $\mathcal{D}$.
 
 ```python
 import gpjax as gpx
 from jax import grad, jit
 import jax.numpy as jnp
 import jax.random as jr
-import jaxkern as jk
 import optax as ox
 
 key = jr.PRNGKey(123)
 
 f = lambda x: 10 * jnp.sin(x)
 
 n = 50
 x = jr.uniform(key=key, minval=-3.0, maxval=3.0, shape=(n,1)).sort()
 y = f(x) + jr.normal(key, shape=(n,1))
 D = gpx.Dataset(X=x, y=y)
-```
-
-The function of interest here, $f(\cdot)$, is sinusoidal, but our observations of it have been perturbed by Gaussian noise. We aim to utilise a Gaussian process to try and recover this latent function.
-
-## 1. Constructing the prior and posterior
 
-We begin by defining a zero-mean Gaussian process prior with a radial basis function kernel and assume the likelihood to be Gaussian.
+# Construct the prior
+meanf = gpx.mean_functions.Zero()
+kernel = gpx.kernels.RBF()
+prior = gpx.Prior(mean_function=meanf, kernel = kernel)
 
-```python
-prior = gpx.Prior(kernel = jk.RBF())
+# Define a likelihood
 likelihood = gpx.Gaussian(num_datapoints = n)
-```
 
-Similar to how we would write on paper, the posterior is constructed by the product of our prior with our likelihood.
-
-```python
+# Construct the posterior
 posterior = prior * likelihood
-```
 
-## 2. Learning hyperparameters
+# Define an optimiser
+optimiser = ox.adam(learning_rate=1e-2)
 
-Equipped with the posterior, we seek to learn the model's hyperparameters through gradient-optimisation of the marginal log-likelihood. We this below, adding Jax's [just-in-time (JIT)](https://jax.readthedocs.io/en/latest/jax-101/02-jitting.html) compilation to accelerate training. 
+# Define the marginal log-likelihood
+negative_mll = jit(gpx.objectives.ConjugateMLL(negative=True))
 
-```python
-mll = jit(posterior.marginal_log_likelihood(D, negative=True))
-```
+# Obtain Type 2 MLEs of the hyperparameters
+opt_posterior, history = gpx.fit(
+    model=posterior,
+    objective=negative_mll,
+    train_data=D,
+    optim=optimiser,
+    num_iters=500,
+    safe=True,
+    key=key,
+)
 
-For purposes of optimisation, we'll use optax's Adam.
-```
-opt = ox.adam(learning_rate=1e-3)
-```
-
-We define an initial parameter state through the `initialise` callable.
-
-```python
-parameter_state = gpx.initialise(posterior, key=key)
-```
-
-Finally, we run an optimisation loop using the Adam optimiser via the `fit` callable.
-
-```python
-inference_state = gpx.fit(mll, parameter_state, opt, num_iters=500)
-```
-
-## 3. Making predictions
-
-Using our learned hyperparameters, we can obtain the posterior distribution of the latent function at novel test points.
-
-```python
-learned_params, _ = inference_state.unpack()
+# Infer the predictive posterior distribution
 xtest = jnp.linspace(-3., 3., 100).reshape(-1, 1)
+latent_dist = opt_posterior(xtest, D)
+predictive_dist = opt_posterior.likelihood(latent_dist)
 
-latent_distribution = posterior(learned_params, D)(xtest)
-predictive_distribution = likelihood(learned_params, latent_distribution)
-
-predictive_mean = predictive_distribution.mean()
-predictive_cov = predictive_distribution.covariance()
+# Obtain the predictive mean and standard deviation
+pred_mean = predictive_dist.mean()
+pred_std = predictive_dist.stddev()
 ```
 
 # Installation
 
 ## Stable version
 
-The latest stable version of GPJax can be installed via [`pip`](https://pip.pypa.io/en/stable/):
+The latest stable version of GPJax can be installed via
+pip:
 
 ```bash
 pip install gpjax
 ```
 
 > **Note**
 >
@@ -175,35 +187,36 @@
 > ```
 
 
 
 ## Development version
 > **Warning**
 >
-> This version is possibly unstable and may contain bugs. 
+> This version is possibly unstable and may contain bugs.
 
-Clone a copy of the repository to your local machine and run the setup configuration in development mode.
+Clone a copy of the repository to your local machine and run the setup
+configuration in development mode.
 ```bash
 git clone https://github.com/JaxGaussianProcesses/GPJax.git
 cd GPJax
-python setup.py develop
+poetry install
 ```
 
 > **Note**
 >
 > We advise you create virtual environment before installing:
 > ```
 > conda create -n gpjax_experimental python=3.10.0
 > conda activate gpjax_experimental
 >  ```
 >
 > and recommend you check your installation passes the supplied unit tests:
 >
 > ```python
-> python -m pytest tests/
+> poetry run pytest
 > ```
 
 # Citing GPJax
 
 If you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).
 
 ```
@@ -216,7 +229,8 @@
   number = {75},
   pages = {4455},
   author = {Thomas Pinder and Daniel Dodd},
   title = {GPJax: A Gaussian Process Framework in JAX},
   journal = {Journal of Open Source Software}
 }
 ```
+
```

