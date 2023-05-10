# Comparing `tmp/cupid_matching-1.1.0.tar.gz` & `tmp/cupid_matching-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupid_matching-1.1.0.tar", max compression
+gzip compressed data, was "cupid_matching-1.1.1.tar", max compression
```

## Comparing `cupid_matching-1.1.0.tar` & `cupid_matching-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    10260 2023-05-10 22:37:56.546277 cupid_matching-1.1.0/README.md
--rw-r--r--   0        0        0        1 2023-05-09 18:41:31.499628 cupid_matching-1.1.0/cupid_matching/__init__.py
--rw-r--r--   0        0        0     9402 2023-05-09 18:41:31.500025 cupid_matching-1.1.0/cupid_matching/choo_siow.py
--rw-r--r--   0        0        0     5651 2023-05-09 18:41:31.500175 cupid_matching-1.1.0/cupid_matching/choo_siow_gender_heteroskedastic.py
--rw-r--r--   0        0        0     6292 2023-05-09 18:41:31.500324 cupid_matching-1.1.0/cupid_matching/choo_siow_heteroskedastic.py
--rw-r--r--   0        0        0    14110 2023-05-09 18:41:31.500459 cupid_matching-1.1.0/cupid_matching/cupid_streamlit.py
--rw-r--r--   0        0        0    11660 2023-05-09 18:41:31.500592 cupid_matching-1.1.0/cupid_matching/entropy.py
--rw-r--r--   0        0        0     5224 2023-05-09 18:41:31.500731 cupid_matching-1.1.0/cupid_matching/example_choo_siow.py
--rw-r--r--   0        0        0     4124 2023-05-09 18:41:31.500860 cupid_matching-1.1.0/cupid_matching/example_nested_logit.py
--rw-r--r--   0        0        0    26215 2023-05-09 18:41:31.500997 cupid_matching-1.1.0/cupid_matching/ipfp_solvers.py
--rw-r--r--   0        0        0    12873 2023-05-09 18:41:31.501150 cupid_matching-1.1.0/cupid_matching/matching_utils.py
--rw-r--r--   0        0        0    11180 2023-05-09 18:41:31.501577 cupid_matching-1.1.0/cupid_matching/min_distance.py
--rw-r--r--   0        0        0     5587 2023-05-09 18:41:31.501715 cupid_matching-1.1.0/cupid_matching/min_distance_utils.py
--rw-r--r--   0        0        0    16046 2023-05-09 18:41:31.501854 cupid_matching-1.1.0/cupid_matching/model_classes.py
--rw-r--r--   0        0        0      369 2023-05-09 18:40:06.062931 cupid_matching-1.1.0/cupid_matching/mypy.ini
--rw-r--r--   0        0        0     9516 2023-05-09 18:41:31.501983 cupid_matching-1.1.0/cupid_matching/nested_logit.py
--rw-r--r--   0        0        0     7443 2023-05-09 18:41:31.502116 cupid_matching-1.1.0/cupid_matching/poisson_glm.py
--rw-r--r--   0        0        0     6302 2023-05-09 18:41:31.502254 cupid_matching-1.1.0/cupid_matching/poisson_glm_utils.py
--rw-r--r--   0        0        0     1929 2023-05-09 18:41:31.502386 cupid_matching-1.1.0/cupid_matching/utils.py
--rw-r--r--   0        0        0     2008 2023-05-10 20:49:34.810410 cupid_matching-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    11051 1970-01-01 00:00:00.000000 cupid_matching-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10308 2023-05-10 23:39:56.941039 cupid_matching-1.1.1/README.md
+-rw-r--r--   0        0        0        1 2023-05-09 18:41:31.499628 cupid_matching-1.1.1/cupid_matching/__init__.py
+-rw-r--r--   0        0        0     9402 2023-05-09 18:41:31.500025 cupid_matching-1.1.1/cupid_matching/choo_siow.py
+-rw-r--r--   0        0        0     5651 2023-05-09 18:41:31.500175 cupid_matching-1.1.1/cupid_matching/choo_siow_gender_heteroskedastic.py
+-rw-r--r--   0        0        0     6292 2023-05-09 18:41:31.500324 cupid_matching-1.1.1/cupid_matching/choo_siow_heteroskedastic.py
+-rw-r--r--   0        0        0    14110 2023-05-09 18:41:31.500459 cupid_matching-1.1.1/cupid_matching/cupid_streamlit.py
+-rw-r--r--   0        0        0    11660 2023-05-09 18:41:31.500592 cupid_matching-1.1.1/cupid_matching/entropy.py
+-rw-r--r--   0        0        0     5224 2023-05-09 18:41:31.500731 cupid_matching-1.1.1/cupid_matching/example_choo_siow.py
+-rw-r--r--   0        0        0     4124 2023-05-09 18:41:31.500860 cupid_matching-1.1.1/cupid_matching/example_nested_logit.py
+-rw-r--r--   0        0        0    26215 2023-05-09 18:41:31.500997 cupid_matching-1.1.1/cupid_matching/ipfp_solvers.py
+-rw-r--r--   0        0        0    12873 2023-05-09 18:41:31.501150 cupid_matching-1.1.1/cupid_matching/matching_utils.py
+-rw-r--r--   0        0        0    11180 2023-05-09 18:41:31.501577 cupid_matching-1.1.1/cupid_matching/min_distance.py
+-rw-r--r--   0        0        0     5587 2023-05-09 18:41:31.501715 cupid_matching-1.1.1/cupid_matching/min_distance_utils.py
+-rw-r--r--   0        0        0    16046 2023-05-09 18:41:31.501854 cupid_matching-1.1.1/cupid_matching/model_classes.py
+-rw-r--r--   0        0        0      369 2023-05-09 18:40:06.062931 cupid_matching-1.1.1/cupid_matching/mypy.ini
+-rw-r--r--   0        0        0     9516 2023-05-09 18:41:31.501983 cupid_matching-1.1.1/cupid_matching/nested_logit.py
+-rw-r--r--   0        0        0     7443 2023-05-09 18:41:31.502116 cupid_matching-1.1.1/cupid_matching/poisson_glm.py
+-rw-r--r--   0        0        0     6302 2023-05-09 18:41:31.502254 cupid_matching-1.1.1/cupid_matching/poisson_glm_utils.py
+-rw-r--r--   0        0        0     1929 2023-05-09 18:41:31.502386 cupid_matching-1.1.1/cupid_matching/utils.py
+-rw-r--r--   0        0        0     2008 2023-05-10 23:39:29.363291 cupid_matching-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11099 1970-01-01 00:00:00.000000 cupid_matching-1.1.1/PKG-INFO
```

### Comparing `cupid_matching-1.1.0/README.md` & `cupid_matching-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,48 +32,58 @@
 from cupid_matching.min_distance import estimate_semilinear_mde
 ```
 
 ## How it works
 
 The following only describes the general ideas. The full documentation is [here](https://bsalanie.github.io/cupid_matching).
 
-The `cupid_matching` package has code - to solve for the stable matching using our Iterative Projection Fitting Procedure (IPFP) in variants of the model of bipartite, one-to-one matching with perfectly transferable utility. It has IPFP solvers for variants of the [Choo and Siow 2006](https://www.jstor.org/stable/10.1086/498585?seq=1) model with or without singles, homoskedastic and heteroskedastic; and also for a class of nested logit models. - to estimate the parameters of separable models with semilinear surplus and entropy using a minimum distance estimator. - to estimate the parameters of semilinear Choo and Siow models using a Poisson GLM estimator. - for a [Streamlit](https://www.streamlit.io/) interactive app that demonstrates solving and estimating the Choo and Siow model using the `cupid_matching` package. You can try it [here](https://share.streamlit.io/bsalanie/cupid_matching_st/main/cupid_streamlit.py).
+The `cupid_matching` package has code 
+
+- to solve for the stable matching using our Iterative Projection Fitting Procedure (IPFP) in variants of the model of bipartite, one-to-one matching with perfectly transferable utility. It has IPFP solvers for variants of the [Choo and Siow 2006](https://www.jstor.org/stable/10.1086/498585?seq=1) model with or without singles, homoskedastic and heteroskedastic; and also for a class of nested logit models
+- to estimate the parameters of separable models with semilinear surplus and entropy using a minimum distance estimator
+- to estimate the parameters of semilinear Choo and Siow models using a Poisson GLM estimator
+- for a [Streamlit](https://www.streamlit.io/) interactive app that demonstrates solving and estimating the Choo and Siow model using the `cupid_matching` package. You can try it [here](https://share.streamlit.io/bsalanie/cupid_matching_st/main/cupid_streamlit.py).
 
 Incidentally, myy [ipfp_R](https://www.github.com/bsalanie/ipfp_R.git) Github repository contains R code to solve for equilibrium in (*only*) the basic version of the Choo and Siow model.
 
 The package builds on the pioneering work of [Choo and Siow *JPE* 2006](https://www.jstor.org/stable/10.1086/498585?seq=1) and on my work with Alfred Galichon, especially our [*REStud* 2022 paper](https://academic.oup.com/restud/article-abstract/89/5/2600/6478301) and [this working paper](https://econ.columbia.edu/working-paper/estimating-separable-matching-models/).
 
-At this stage, it only deals with bipartite models. As the heterosexual marriage market is a leading example, I will refer to the two sides as *men* and *women*. Each man $m$/each women \$w has an observed, discrete-valued type $x$/$y$, and some unobserved heterogeneity.
+At this stage, it only deals with bipartite models. As the heterosexual marriage market is a leading example, I will refer to the two sides as *men* and *women*. Each man $m$ (resp. each women $w$) has an observed, discrete-valued type $x$ (resp. $y$), along with unobserved heterogeneity.
 
 ### The primitives
 
-The primitives of this class of matching models are \* the *margins*: the numbers $n_x$ of men of type $x=1,\ldots,X$ and the numbers $m_y$ of women of type $y=1,\ldots,Y$ \* the joint surplus created by the match of a man $m$ of type $x$ and a woman $w$ of type $y$. We assume *separability*: this joint surplus takes the form 
+The primitives of this class of matching models are 
+
+- the *margins*: the numbers $n_x$ of men of type $x=1,\ldots,X$ and the numbers $m_y$ of women of type $y=1,\ldots,Y$
+- the *joint surplus* created by the match of a man $m$ of type $x$ and a woman $w$ of type $y$. We assume *separability*: this joint surplus takes the form 
 $$
 \Phi_{xy}+\varepsilon_{my} +\eta_{xw}.
 $$ 
 A single man has utility $\varepsilon_{m0}$ and a single woman has utility $\eta_{0w}$.
 
 The modeler chooses the distributions of the vectors $(\varepsilon_{m0},\varepsilon_{m1},\ldots, \varepsilon_{mY})$ and $(\eta_{0w},\eta_{1w},\ldots,\eta_{Xw})$.
 
 ### The solution: the stable matching
 
 We denote $\mu_{xy}$ the number of matches between men of type $x$ and women of type $y$, $\mu_{x0}$ the number of single men of type $x$, and $\mu_{0y}$ the number of single women of type $y$.
 
-The total numbers must add up to the margins: $$
+The total numbers must add up to the margins: 
+$$
 \sum_{y=1}^Y \mu_{xy}+\mu_{x0}=n_x \; \text{ and } \;
 \sum_{x=1}^X \mu_{xy}+\mu_{0y}=m_y.
-$$ The total number of individuals is $N_i=\sum_{x=1}^X n_x+ \sum_{y=1}^Y m_y$ and the total number of households is $N_h = N_i - \sum_{x=1}^X \sum_{y=1}^Y \mu_{xy}$.
+$$ 
+The total number of individuals is $N_i=\sum_{x=1}^X n_x+ \sum_{y=1}^Y m_y$ and the total number of households is $N_h = N_i - \sum_{x=1}^X \sum_{y=1}^Y \mu_{xy}$.
 
-Galichon-Salanié (\*REStud\* 2022) shows that in large markets, if the vectors $\varepsilon$ and $\eta$ have full support, the stable matching is the unique solution to the strictly convex program $$
+Galichon-Salanié (*REStud* 2022) shows that in large markets, if the vectors $\varepsilon$ and $\eta$ have full support, the stable matching is the unique solution to the strictly convex program $$
 \max_{\mu} \left(\sum_{x=1}^X \sum_{y=1}^Y \mu_{xy}\Phi_{xy} + \mathcal{E}(\mu; n, m)\right)
 $$ where $\mathcal{E}$, the *generalized entropy* function, depends on the assumed distributions of the $\varepsilon$ and $\eta$ random vectors.
 
 The files `choo_siow.py`, `choo_siow_gender_heteroskedastic`, `choo_siow_heteroskedastic`, and `nested_logit` provide `EntropyFunctions` objects that compute the generalized entropy and at least its first derivative for, respectively,
 
-1.  the original Choo and Siow 2006 model, in which the $\varepsilon$ and $\eta$ terms are iid draws from a type I extreme value distributio
+1.  the original Choo and Siow 2006 model, in which the $\varepsilon$ and $\eta$ terms are iid draws from a type I extreme value distribution
 2.  the same model, without singles (to be used when only couples are observed)
 3.  an extension of 1. that allows for a scale parameter $\tau$ for the distribution of $\eta$
 4.  an extension of 3. that has type-dependent scale parameters $\sigma_x$ and $\tau_y$ (with $\sigma_1=1$
 5.  a two-layer nested logit model in which singles (type 0) are in their own nest and the user chooses the structure of the other nests.
 
 Users of the package are welcome to code `EntropyFunctions` objects for different distributions of the unobserved heterogeneity terms.
 
@@ -99,29 +109,34 @@
 
 The vectors `error_x` and `error_y` are estimates of the precision of the solution (see the code in `ipfp_solvers.py`).
 
 ### Estimating the joint surplus
 
 Given observed matching patterns $\mu$; a class of generalized entropy functions $(\mathcal{E}^{\alpha})$; and a class of joint surplus functions $(\Phi^{\beta})$, one would like to estimate the parameter vectors $\alpha$ and $\beta$.
 
-The package provides two estimators, which are described extensively in [this paper](https://econ.columbia.edu/working-paper/estimating-separable-matching-models/). 
+The package provides two estimators, which are described extensively in [this paper](https://econ.columbia.edu/working-paper/estimating-separable-matching-models/):
+
 - the minimum distance estimator in `min_distance.py` 
 - the Poisson estimator in `poisson_glm.py`, which only applies to the Choo and Siow homoskedastic model.
 
 
 
 At this stage `cupid_matching` only allows for linear models of the joint surplus:
+
 $$
-\Phi^{\beta}_{xy} = \sum_{k=1}^K \phi_{xy}^k \beta_k,
+\Phi^{\beta}_{xy} = \sum_{k=1}^K \phi_{xy}^k \beta_k
 $$
-where the *basis functions* $(\phi^1,\ldots,\phi^K)$ are imposed by the analyst.
+
+
+where the *basis functions* $(\phi^1,\ldots,\phi^K)$ are imposed by the analyst. 
 
 The file `example_choosiow.py` has a demo of minimum distance and Poisson estimators on the Choo and Siow 2006 model. For other models, the minimum distance estimator works as follows, given 
 
-- an observed matching stored in a `Matching` object `mus`  - an `EntropyFunction` object `entropy_model` that allows for `p` parameters in $\alpha$
+- an observed matching stored in a `Matching` object `mus`
+- an `EntropyFunction` object `entropy_model` that allows for `p` parameters in $\alpha$
 - an $(X,Y,K)$ Numpy array of basis functions `phi_bases`:
   
 ```py
 mde_results = estimate_semilinear_mde(
     mus, phi_bases, entropy_model)
 mde_results.print_results(n_alpha=p)
 ```
@@ -138,16 +153,17 @@
 -   many of these models (including all variants of Choo and Siow) rely heavily on logarithms and exponentials. It is easy to generate examples where numeric instability sets in.
 -   as a consequence, the `numeric` versions of the minimum distance estimator (which use numerical derivatives) are not recommended.
 -   the bias-corrected minimum distance estimator (`corrected`) may have a larger mean-squared error and/or introduce numerical instabilities.
 -   the estimated variance of the estimators assumes that the observed matching was sampled at the household level, and that sampling weights are all equal.
 
 ## Release notes
 
-### version 1.1.0
+### version 1.1.1
 
+-  improved documentation
 -  the package now relies on my utilities package `bs_python_utils`.  The `VarianceMatching` class in `matching_utils,py` is new; this should be transparent for the user.
 
 ### version 1.0.8
 
 -   deleted spurious print statement.
 
 ### version 1.0.7
```

### Comparing `cupid_matching-1.1.0/cupid_matching/choo_siow.py` & `cupid_matching-1.1.1/cupid_matching/choo_siow.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/choo_siow_gender_heteroskedastic.py` & `cupid_matching-1.1.1/cupid_matching/choo_siow_gender_heteroskedastic.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/choo_siow_heteroskedastic.py` & `cupid_matching-1.1.1/cupid_matching/choo_siow_heteroskedastic.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/cupid_streamlit.py` & `cupid_matching-1.1.1/cupid_matching/cupid_streamlit.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/entropy.py` & `cupid_matching-1.1.1/cupid_matching/entropy.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/example_choo_siow.py` & `cupid_matching-1.1.1/cupid_matching/example_choo_siow.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/example_nested_logit.py` & `cupid_matching-1.1.1/cupid_matching/example_nested_logit.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/ipfp_solvers.py` & `cupid_matching-1.1.1/cupid_matching/ipfp_solvers.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/matching_utils.py` & `cupid_matching-1.1.1/cupid_matching/matching_utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/min_distance.py` & `cupid_matching-1.1.1/cupid_matching/min_distance.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/min_distance_utils.py` & `cupid_matching-1.1.1/cupid_matching/min_distance_utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/model_classes.py` & `cupid_matching-1.1.1/cupid_matching/model_classes.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/nested_logit.py` & `cupid_matching-1.1.1/cupid_matching/nested_logit.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/poisson_glm.py` & `cupid_matching-1.1.1/cupid_matching/poisson_glm.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/poisson_glm_utils.py` & `cupid_matching-1.1.1/cupid_matching/poisson_glm_utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/cupid_matching/utils.py` & `cupid_matching-1.1.1/cupid_matching/utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.1.0/pyproject.toml` & `cupid_matching-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cupid_matching"
-version = "1.1.0"
+version = "1.1.1"
 description = "Solves, simulates, and estimates separable matching TU models"
 authors = ["Bernard Salanie <bsalanie@columbia.edu>"]
 readme = "README.md"
 packages = [{include = "cupid_matching"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cupid_matching-1.1.0/PKG-INFO` & `cupid_matching-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupid-matching
-Version: 1.1.0
+Version: 1.1.1
 Summary: Solves, simulates, and estimates separable matching TU models
 Author: Bernard Salanie
 Author-email: bsalanie@columbia.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -54,48 +54,58 @@
 from cupid_matching.min_distance import estimate_semilinear_mde
 ```
 
 ## How it works
 
 The following only describes the general ideas. The full documentation is [here](https://bsalanie.github.io/cupid_matching).
 
-The `cupid_matching` package has code - to solve for the stable matching using our Iterative Projection Fitting Procedure (IPFP) in variants of the model of bipartite, one-to-one matching with perfectly transferable utility. It has IPFP solvers for variants of the [Choo and Siow 2006](https://www.jstor.org/stable/10.1086/498585?seq=1) model with or without singles, homoskedastic and heteroskedastic; and also for a class of nested logit models. - to estimate the parameters of separable models with semilinear surplus and entropy using a minimum distance estimator. - to estimate the parameters of semilinear Choo and Siow models using a Poisson GLM estimator. - for a [Streamlit](https://www.streamlit.io/) interactive app that demonstrates solving and estimating the Choo and Siow model using the `cupid_matching` package. You can try it [here](https://share.streamlit.io/bsalanie/cupid_matching_st/main/cupid_streamlit.py).
+The `cupid_matching` package has code 
+
+- to solve for the stable matching using our Iterative Projection Fitting Procedure (IPFP) in variants of the model of bipartite, one-to-one matching with perfectly transferable utility. It has IPFP solvers for variants of the [Choo and Siow 2006](https://www.jstor.org/stable/10.1086/498585?seq=1) model with or without singles, homoskedastic and heteroskedastic; and also for a class of nested logit models
+- to estimate the parameters of separable models with semilinear surplus and entropy using a minimum distance estimator
+- to estimate the parameters of semilinear Choo and Siow models using a Poisson GLM estimator
+- for a [Streamlit](https://www.streamlit.io/) interactive app that demonstrates solving and estimating the Choo and Siow model using the `cupid_matching` package. You can try it [here](https://share.streamlit.io/bsalanie/cupid_matching_st/main/cupid_streamlit.py).
 
 Incidentally, myy [ipfp_R](https://www.github.com/bsalanie/ipfp_R.git) Github repository contains R code to solve for equilibrium in (*only*) the basic version of the Choo and Siow model.
 
 The package builds on the pioneering work of [Choo and Siow *JPE* 2006](https://www.jstor.org/stable/10.1086/498585?seq=1) and on my work with Alfred Galichon, especially our [*REStud* 2022 paper](https://academic.oup.com/restud/article-abstract/89/5/2600/6478301) and [this working paper](https://econ.columbia.edu/working-paper/estimating-separable-matching-models/).
 
-At this stage, it only deals with bipartite models. As the heterosexual marriage market is a leading example, I will refer to the two sides as *men* and *women*. Each man $m$/each women \$w has an observed, discrete-valued type $x$/$y$, and some unobserved heterogeneity.
+At this stage, it only deals with bipartite models. As the heterosexual marriage market is a leading example, I will refer to the two sides as *men* and *women*. Each man $m$ (resp. each women $w$) has an observed, discrete-valued type $x$ (resp. $y$), along with unobserved heterogeneity.
 
 ### The primitives
 
-The primitives of this class of matching models are \* the *margins*: the numbers $n_x$ of men of type $x=1,\ldots,X$ and the numbers $m_y$ of women of type $y=1,\ldots,Y$ \* the joint surplus created by the match of a man $m$ of type $x$ and a woman $w$ of type $y$. We assume *separability*: this joint surplus takes the form 
+The primitives of this class of matching models are 
+
+- the *margins*: the numbers $n_x$ of men of type $x=1,\ldots,X$ and the numbers $m_y$ of women of type $y=1,\ldots,Y$
+- the *joint surplus* created by the match of a man $m$ of type $x$ and a woman $w$ of type $y$. We assume *separability*: this joint surplus takes the form 
 $$
 \Phi_{xy}+\varepsilon_{my} +\eta_{xw}.
 $$ 
 A single man has utility $\varepsilon_{m0}$ and a single woman has utility $\eta_{0w}$.
 
 The modeler chooses the distributions of the vectors $(\varepsilon_{m0},\varepsilon_{m1},\ldots, \varepsilon_{mY})$ and $(\eta_{0w},\eta_{1w},\ldots,\eta_{Xw})$.
 
 ### The solution: the stable matching
 
 We denote $\mu_{xy}$ the number of matches between men of type $x$ and women of type $y$, $\mu_{x0}$ the number of single men of type $x$, and $\mu_{0y}$ the number of single women of type $y$.
 
-The total numbers must add up to the margins: $$
+The total numbers must add up to the margins: 
+$$
 \sum_{y=1}^Y \mu_{xy}+\mu_{x0}=n_x \; \text{ and } \;
 \sum_{x=1}^X \mu_{xy}+\mu_{0y}=m_y.
-$$ The total number of individuals is $N_i=\sum_{x=1}^X n_x+ \sum_{y=1}^Y m_y$ and the total number of households is $N_h = N_i - \sum_{x=1}^X \sum_{y=1}^Y \mu_{xy}$.
+$$ 
+The total number of individuals is $N_i=\sum_{x=1}^X n_x+ \sum_{y=1}^Y m_y$ and the total number of households is $N_h = N_i - \sum_{x=1}^X \sum_{y=1}^Y \mu_{xy}$.
 
-Galichon-Salanié (\*REStud\* 2022) shows that in large markets, if the vectors $\varepsilon$ and $\eta$ have full support, the stable matching is the unique solution to the strictly convex program $$
+Galichon-Salanié (*REStud* 2022) shows that in large markets, if the vectors $\varepsilon$ and $\eta$ have full support, the stable matching is the unique solution to the strictly convex program $$
 \max_{\mu} \left(\sum_{x=1}^X \sum_{y=1}^Y \mu_{xy}\Phi_{xy} + \mathcal{E}(\mu; n, m)\right)
 $$ where $\mathcal{E}$, the *generalized entropy* function, depends on the assumed distributions of the $\varepsilon$ and $\eta$ random vectors.
 
 The files `choo_siow.py`, `choo_siow_gender_heteroskedastic`, `choo_siow_heteroskedastic`, and `nested_logit` provide `EntropyFunctions` objects that compute the generalized entropy and at least its first derivative for, respectively,
 
-1.  the original Choo and Siow 2006 model, in which the $\varepsilon$ and $\eta$ terms are iid draws from a type I extreme value distributio
+1.  the original Choo and Siow 2006 model, in which the $\varepsilon$ and $\eta$ terms are iid draws from a type I extreme value distribution
 2.  the same model, without singles (to be used when only couples are observed)
 3.  an extension of 1. that allows for a scale parameter $\tau$ for the distribution of $\eta$
 4.  an extension of 3. that has type-dependent scale parameters $\sigma_x$ and $\tau_y$ (with $\sigma_1=1$
 5.  a two-layer nested logit model in which singles (type 0) are in their own nest and the user chooses the structure of the other nests.
 
 Users of the package are welcome to code `EntropyFunctions` objects for different distributions of the unobserved heterogeneity terms.
 
@@ -121,29 +131,34 @@
 
 The vectors `error_x` and `error_y` are estimates of the precision of the solution (see the code in `ipfp_solvers.py`).
 
 ### Estimating the joint surplus
 
 Given observed matching patterns $\mu$; a class of generalized entropy functions $(\mathcal{E}^{\alpha})$; and a class of joint surplus functions $(\Phi^{\beta})$, one would like to estimate the parameter vectors $\alpha$ and $\beta$.
 
-The package provides two estimators, which are described extensively in [this paper](https://econ.columbia.edu/working-paper/estimating-separable-matching-models/). 
+The package provides two estimators, which are described extensively in [this paper](https://econ.columbia.edu/working-paper/estimating-separable-matching-models/):
+
 - the minimum distance estimator in `min_distance.py` 
 - the Poisson estimator in `poisson_glm.py`, which only applies to the Choo and Siow homoskedastic model.
 
 
 
 At this stage `cupid_matching` only allows for linear models of the joint surplus:
+
 $$
-\Phi^{\beta}_{xy} = \sum_{k=1}^K \phi_{xy}^k \beta_k,
+\Phi^{\beta}_{xy} = \sum_{k=1}^K \phi_{xy}^k \beta_k
 $$
-where the *basis functions* $(\phi^1,\ldots,\phi^K)$ are imposed by the analyst.
+
+
+where the *basis functions* $(\phi^1,\ldots,\phi^K)$ are imposed by the analyst. 
 
 The file `example_choosiow.py` has a demo of minimum distance and Poisson estimators on the Choo and Siow 2006 model. For other models, the minimum distance estimator works as follows, given 
 
-- an observed matching stored in a `Matching` object `mus`  - an `EntropyFunction` object `entropy_model` that allows for `p` parameters in $\alpha$
+- an observed matching stored in a `Matching` object `mus`
+- an `EntropyFunction` object `entropy_model` that allows for `p` parameters in $\alpha$
 - an $(X,Y,K)$ Numpy array of basis functions `phi_bases`:
   
 ```py
 mde_results = estimate_semilinear_mde(
     mus, phi_bases, entropy_model)
 mde_results.print_results(n_alpha=p)
 ```
@@ -160,16 +175,17 @@
 -   many of these models (including all variants of Choo and Siow) rely heavily on logarithms and exponentials. It is easy to generate examples where numeric instability sets in.
 -   as a consequence, the `numeric` versions of the minimum distance estimator (which use numerical derivatives) are not recommended.
 -   the bias-corrected minimum distance estimator (`corrected`) may have a larger mean-squared error and/or introduce numerical instabilities.
 -   the estimated variance of the estimators assumes that the observed matching was sampled at the household level, and that sampling weights are all equal.
 
 ## Release notes
 
-### version 1.1.0
+### version 1.1.1
 
+-  improved documentation
 -  the package now relies on my utilities package `bs_python_utils`.  The `VarianceMatching` class in `matching_utils,py` is new; this should be transparent for the user.
 
 ### version 1.0.8
 
 -   deleted spurious print statement.
 
 ### version 1.0.7
```

