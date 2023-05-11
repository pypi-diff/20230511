# Comparing `tmp/pspy-1.6.tar.gz` & `tmp/pspy-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pspy-1.6.tar", last modified: Tue May  2 16:00:04 2023, max compression
+gzip compressed data, was "pspy-1.6.1.tar", last modified: Thu May 11 11:55:20 2023, max compression
```

## Comparing `pspy-1.6.tar` & `pspy-1.6.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.288178 pspy-1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-02 15:59:57.000000 pspy-1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:59:57.000000 pspy-1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-02 16:00:04.288178 pspy-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-02 15:59:57.000000 pspy-1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.288178 pspy-1.6/pspy/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-02 15:59:57.000000 pspy-1.6/pspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-02 16:00:04.288178 pspy-1.6/pspy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy/cov_fortran/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 15:59:57.000000 pspy-1.6/pspy/cov_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-05-02 15:59:57.000000 pspy-1.6/pspy/cov_fortran/cov_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-05-02 15:59:57.000000 pspy-1.6/pspy/flat_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy/mcm_fortran/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 15:59:57.000000 pspy-1.6/pspy/mcm_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-02 15:59:57.000000 pspy-1.6/pspy/mcm_fortran/mcm_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-05-02 15:59:57.000000 pspy-1.6/pspy/pspy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    35399 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    31739 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_map_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_mcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-02 15:59:57.000000 pspy-1.6/pspy/sph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   468866 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/data/generate_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/data/parameters_test_data.yml
--rw-r--r--   0 runner    (1001) docker     (123) 12059025 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/data/test_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/test_pspy_namaster.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/test_so_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/test_so_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/test_so_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.288178 pspy-1.6/pspy/wigner3j/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 15:59:57.000000 pspy-1.6/pspy/wigner3j/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   104274 2023-05-02 15:59:57.000000 pspy-1.6/pspy/wigner3j/wigner3j_sub.f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.288178 pspy-1.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-05-02 15:59:57.000000 pspy-1.6/scripts/test-pspy
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-02 16:00:04.288178 pspy-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-02 15:59:57.000000 pspy-1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-02 15:59:57.000000 pspy-1.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.488767 pspy-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-11 11:55:12.000000 pspy-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 11:55:12.000000 pspy-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-11 11:55:20.488767 pspy-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-11 11:55:12.000000 pspy-1.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.488767 pspy-1.6.1/pspy/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 11:55:20.488767 pspy-1.6.1/pspy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.472767 pspy-1.6.1/pspy/cov_fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/cov_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/cov_fortran/cov_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/flat_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.472767 pspy-1.6.1/pspy/mcm_fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/mcm_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/mcm_fortran/mcm_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/pspy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35346 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31529 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_map_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_mcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/sph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.472767 pspy-1.6.1/pspy/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.472767 pspy-1.6.1/pspy/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   468866 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/tests/data/generate_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/tests/data/parameters_test_data.yml
+-rw-r--r--   0 runner    (1001) docker     (123) 12059025 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/data/test_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/test_pspy_namaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/test_so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/test_so_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/test_so_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.488767 pspy-1.6.1/pspy/wigner3j/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/wigner3j/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104274 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/wigner3j/wigner3j_sub.f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.468767 pspy-1.6.1/pspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.488767 pspy-1.6.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-05-11 11:55:13.000000 pspy-1.6.1/scripts/test-pspy
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-11 11:55:20.488767 pspy-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-11 11:55:13.000000 pspy-1.6.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-11 11:55:13.000000 pspy-1.6.1/versioneer.py
```

### Comparing `pspy-1.6/LICENSE` & `pspy-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pspy-1.6/PKG-INFO` & `pspy-1.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.6
+Version: 1.6.1
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
@@ -83,16 +83,17 @@
         
         
         Authors
         ------------
         * `Thibaut Louis <https://thibautlouis.github.io>`_
         * Steve Choi
         * DW Han
-        * Xavier Garrido
+        * `Xavier Garrido <https://xgarrido.github.io>`_
         * Sigurd Naess
+        * `Adrien La Posta <https://adrien-laposta.github.io>`_
         
         The code is part of `PSpipe <https://github.com/simonsobs/PSpipe>`_ the Simons Observatory power spectrum pipeline.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pspy-1.6/README.rst` & `pspy-1.6.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -76,11 +76,12 @@
 
 
 Authors
 ------------
 * `Thibaut Louis <https://thibautlouis.github.io>`_
 * Steve Choi
 * DW Han
-* Xavier Garrido
+* `Xavier Garrido <https://xgarrido.github.io>`_
 * Sigurd Naess
+* `Adrien La Posta <https://adrien-laposta.github.io>`_
 
 The code is part of `PSpipe <https://github.com/simonsobs/PSpipe>`_ the Simons Observatory power spectrum pipeline.
```

### Comparing `pspy-1.6/pspy/cov_fortran/cov_fortran.f90` & `pspy-1.6.1/pspy/cov_fortran/cov_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/flat_tools.py` & `pspy-1.6.1/pspy/flat_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/mcm_fortran/mcm_fortran.f90` & `pspy-1.6.1/pspy/mcm_fortran/mcm_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/pspy_utils.py` & `pspy-1.6.1/pspy/pspy_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,42 +39,44 @@
         if start_at_zero:
             ps[f] = np.append(np.array([0, 0]), ps[f])
     if start_at_zero:
         l = np.append(np.array([0, 1]), l)
     return l, ps
 
 
-def ps_from_params(cosmo_params, output_type, lmax, start_at_zero=False):
+def ps_from_params(cosmo_params, output_type, lmax, start_at_zero=False, **accuracy_pars):
 
     """Given a set of cosmological parameters compute the corresponding lensed power spectrum
        You need to have camb installed to use this function
       ----------
       cosmo_params: dict
         dictionnary of cosmological parameters
         # e.g cosmo_params = {"cosmomc_theta":0.0104085, "logA": 3.044, "ombh2": 0.02237, "omch2": 0.1200, "ns": 0.9649, "Alens": 1.0, "tau": 0.0544}
       output_type :  string
         'Cl' or 'Dl'
       lmax: integer
         the maximum multipole to consider
       start_at_zero : boolean
         if True, ps start at l=0 and cl(l=0) and cl(l=1) are set to 0
         else, start at l=2
+      accuracy_pars : dict
+        optional accuracy parameters that CAMB understand (e.g. lens_potential_accuracy)
     """
     try:
         import camb
     except ModuleNotFoundError:
         raise ModuleNotFoundError("you need to install camb to use this function")
 
     if start_at_zero:
         lmin = 0
     else:
         lmin = 2
 
     camb_cosmo = {k: v for k, v in cosmo_params.items() if k not in ["logA", "As"]}
-    camb_cosmo.update({"As": 1e-10*np.exp(cosmo_params["logA"]), "lmax": lmax, "lens_potential_accuracy": 1})
+    camb_cosmo.update({"As": 1e-10*np.exp(cosmo_params["logA"]), "lmax": lmax, **accuracy_pars})
     pars = camb.set_params(**camb_cosmo)
     results = camb.get_results(pars)
     powers = results.get_cmb_power_spectra(pars, CMB_unit="muK", raw_cl=output_type == "Cl")
     l = np.arange(lmin, lmax)
     ps = {spec: powers["total"][l][:, count] for count, spec in enumerate(["TT", "EE", "BB", "TE" ])}
     ps["ET"] = ps["TE"].copy()
     for spec in ["TB", "BT", "EB", "BE" ]:
@@ -272,37 +274,37 @@
     delta_l_list: list of integers
         the different binsize we want to consider
     l_bound_list: list of integers
         the multipole at which the binsize ceases to apply
     write_binning_file: string
         if you want to write to disk, pass a string with the name of the file
     """
- 
+
     lmin_list = []
     lmax_list = []
     lmean_list = []
-    
+
     lmin = 2
     for count, ells in enumerate(l_bound_list):
         while True:
             lmax = lmin +  delta_l_list[count]
 
             if lmax > l_bound_list[count]:
                 break
 
             lmean = (lmax + lmin) / 2
 
             lmin_list += [lmin]
             lmax_list += [lmax]
             lmean_list += [lmean]
-            
+
             lmin = lmax + 1
     if binning_file is not None:
         np.savetxt(binning_file, np.transpose([lmin_list, lmax_list, lmean_list]))
-    
+
     return lmin_list, lmax_list, lmean_list
 
 def maximum_likelihood_combination(cov_mat, P_mat, data_vec, test_matrix=False):
     """
     This function solve for the maximum likelihood data_vec and covariance for a problem of the form
     chi2 = (data_vec - P ML_data_vec).T cov_mat ** -1 data_vec - P ML_data_vec)
 
@@ -313,31 +315,31 @@
         the covariance matrix of data_vec, of size N_ini x N_ini
     P_mat: 2d array
         the "pointing matrix" that project the final data vector of size N_f into the initial data vector space N_ini
         shape is (N_ini, N_f)
     data_vec: 1d array
         the initial data vector
     """
-    
+
     inv_cov_mat = np.linalg.inv(cov_mat)
 
     ML_cov_mat = np.linalg.inv(np.dot(np.dot(P_mat, inv_cov_mat), P_mat.T))
     ML_data_vec = np.dot(ML_cov_mat, np.dot(P_mat, np.dot(inv_cov_mat, data_vec)))
-    
+
     if test_matrix:
         is_symmetric(ML_cov_mat, tol=1e-7)
         is_pos_def(ML_cov_mat)
 
     return ML_cov_mat, ML_data_vec
 
 
 def is_symmetric(mat, tol=1e-8):
     """
     This function check if a matrix is symmetric
-    
+
     Parameters
     ----------
     mat: 2d array
         the matrix tested
     tol:
         the absolute tolerance on assymetry
     """
@@ -347,22 +349,58 @@
         print("the tested matrix is not symmetric")
     return
 
 
 def is_pos_def(mat):
     """
     This function check if a matrix is positive definite
-    
+
     Parameters
     ----------
     mat: 2d array
         the matrix tested
     """
     if np.all(np.linalg.eigvals(mat) > 0):
         print("the tested matrix is positive definite")
     else:
         print("the tested matrix is not positive definite")
         print(np.linalg.eigvals(mat))
     return
 
 
-    
+def calibrate_alms(alms, cal = 1.0, pol_eff = 1.0):
+    """
+    Apply a calibration amplitude
+    and a polarization efficiency
+    to a set of alms.
+
+    Parameters
+    ----------
+    alms: array
+    cal: float
+        calibration amplitude (default to 1)
+    pol_eff: float
+        polarization efficiency (default to 1)
+    """
+    alms[0] *= cal
+    alms[1] *= cal / pol_eff
+    alms[2] *= cal / pol_eff
+
+    return alms
+
+
+def rotate_pol_alms(alms, pol_rot_angle):
+    """
+    Apply a rotation on the alms due to
+    polangle miscalibration.
+
+    Parameters
+    ----------
+    alms: array
+    pol_rot_angle: float
+        must be in degree
+    """
+    cos_alpha = np.cos(np.deg2rad(2 * pol_rot_angle))
+    sin_alpha = np.sin(np.deg2rad(2 * pol_rot_angle))
+    alms[1], alms[2] = (alms[1] * cos_alpha + alms[2] * sin_alpha,
+                       -alms[1] * sin_alpha + alms[2] * cos_alpha)
+    return alms
```

### Comparing `pspy-1.6/pspy/so_config.py` & `pspy-1.6.1/pspy/so_config.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/so_consistency.py` & `pspy-1.6.1/pspy/so_consistency.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/so_cov.py` & `pspy-1.6.1/pspy/so_cov.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,29 +415,30 @@
     """
 
     cov = symmetrize(Clth_dict["TaTc"]) * symmetrize(Clth_dict["TbTd"]) * coupling_dict["TaTcTbTd"]
     cov += symmetrize(Clth_dict["TaTd"]) * symmetrize(Clth_dict["TbTc"]) * coupling_dict["TaTdTbTc"]
 
     if binned_mcm == True:
         analytic_cov = bin_mat(cov, binning_file, lmax)
-        analytic_cov = np.dot(np.dot(mbb_inv_ab, analytic_cov), mbb_inv_cd.T)
+        analytic_cov = mbb_inv_ab @ analytic_cov @ mbb_inv_cd.T
     else:
-        full_analytic_cov = np.dot(np.dot(mbb_inv_ab, cov), mbb_inv_cd.T)
+        full_analytic_cov = mbb_inv_ab @ cov @ mbb_inv_cd.T
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax)
         
     return analytic_cov
 
 def cov_spin0and2(Clth_dict,
                   coupling_dict,
                   binning_file,
                   lmax,
                   mbb_inv_ab,
                   mbb_inv_cd,
                   binned_mcm=True,
-                  cov_T_E_only=True):
+                  cov_T_E_only=True,
+                  dtype=np.float64):
                   
     """From the two point functions and the coupling kernel construct the T and E analytical covariance matrix of <(C_ab- Clth)(C_cd-Clth)>
 
     Parameters
     ----------
 
     Clth_dict: dictionnary
@@ -456,24 +457,23 @@
       specify if the mode coupling matrices are binned or not
     binned_mcm: boolean
       specify if the mode coupling matrices are binned or not
     cov_T_E_only: boolean
         if true don't do B
     """
 
-    bin_lo, bin_hi, bin_c, bin_size = pspy_utils.read_binning_file(binning_file, lmax)
     n_ell = Clth_dict["TaTb"].shape[0]
     
     if cov_T_E_only:
         speclist = ["TT", "TE", "ET", "EE"]
     else:
         speclist =  ["TT", "TE", "TB", "ET", "BT", "EE", "EB", "BE", "BB"]
     
     nspec = len(speclist)
-    full_analytic_cov = np.zeros((nspec * n_ell, nspec * n_ell))
+    full_analytic_cov = np.zeros((nspec * n_ell, nspec * n_ell), dtype=dtype)
 
     for i, (W, X) in enumerate(speclist):
         for j, (Y, Z) in enumerate(speclist):
             if i > j : continue
             id0 = W + "a" + Y + "c"
             id1 = X + "b" + Z + "d"
             id2 = W + "a" + Z + "d"
@@ -491,22 +491,22 @@
             M = Cl0Cl1 * coupling_dict[id0 + id1]
             M += Cl2Cl3 * coupling_dict[id2 + id3]
 
             full_analytic_cov[i * n_ell:(i + 1) * n_ell, j * n_ell:(j + 1) * n_ell] = M
     
     full_analytic_cov = np.triu(full_analytic_cov) + np.tril(full_analytic_cov.T, -1)
     
-    mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only)
-    mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only)
+    mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only, dtype=dtype)
+    mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only, dtype=dtype)
 
     if binned_mcm == True:
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
-        analytic_cov = np.dot(np.dot(mbb_inv_ab, analytic_cov), mbb_inv_cd.T)
+        analytic_cov = mbb_inv_ab @ analytic_cov @ mbb_inv_cd.T
     else:
-        full_analytic_cov = np.dot(np.dot(mbb_inv_ab, full_analytic_cov), mbb_inv_cd.T)
+        full_analytic_cov = mbb_inv_ab @ full_analytic_cov @ mbb_inv_cd.T
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
 
     return analytic_cov
 
 def generalized_cov_spin0and2(coupling_dict,
                               id_element,
                               ns,
@@ -514,15 +514,16 @@
                               nl_all,
                               lmax,
                               binning_file,
                               mbb_inv_ab,
                               mbb_inv_cd,
                               binned_mcm=True,
                               return_full_cov=False,
-                              cov_T_E_only=True):
+                              cov_T_E_only=True,
+                              dtype=np.float64):
 
     """
     This routine deserves some explanation
     We want to compute the covariance between two power spectra
     C1 = Wa * Xb, C2 =  Yc * Zd
     Here W, X, Y, Z can be either T or E and a,b,c,d will be an index
     corresponding to the survey and array we consider so for example a = s17&pa5_150 or a = dr6&pa4_090
@@ -559,23 +560,22 @@
     cov_T_E_only: boolean
         if true don't do B
     """
 
     na, nb, nc, nd = id_element
 
     n_ell = coupling_dict["TaTcTbTd"].shape[0]
-    bin_lo, bin_hi, bin_c, bin_size = pspy_utils.read_binning_file(binning_file, n_ell)
 
     if cov_T_E_only:
         speclist = ["TT", "TE", "ET", "EE"]
     else:
         speclist =  ["TT", "TE", "TB", "ET", "BT", "EE", "EB", "BE", "BB"]
     
     nspec = len(speclist)
-    full_analytic_cov = np.zeros((nspec * n_ell, nspec * n_ell))
+    full_analytic_cov = np.zeros((nspec * n_ell, nspec * n_ell), dtype=dtype)
 
     for i, (W, X) in enumerate(speclist):
         for j, (Y, Z) in enumerate(speclist):
     
             id0 = W + "a" + Y + "c"
             id1 = X + "b" + Z + "d"
             id2 = W + "a" + Z + "d"
@@ -588,22 +588,22 @@
                 id3 = id3.replace(field, "P")
 
         
             M = coupling_dict[id0 + id1] * chi(na, nc, nb, nd, ns, ps_all, nl_all, W + Y + X + Z)
             M += coupling_dict[id2 + id3] * chi(na, nd, nb, nc, ns, ps_all, nl_all, W + Z + X + Y)
             full_analytic_cov[i * n_ell: (i + 1) * n_ell, j * n_ell: (j + 1) * n_ell] = M
 
-    mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only)
-    mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only)
+    mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only, dtype=dtype)
+    mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only, dtype=dtype)
 
     if binned_mcm == True:
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
-        analytic_cov = np.dot(np.dot(mbb_inv_ab, analytic_cov), mbb_inv_cd.T)
+        analytic_cov = mbb_inv_ab @ analytic_cov @ mbb_inv_cd.T
     else:
-        full_analytic_cov = np.dot(np.dot(mbb_inv_ab, full_analytic_cov), mbb_inv_cd.T)
+        full_analytic_cov = mbb_inv_ab @ full_analytic_cov @ mbb_inv_cd.T
         if return_full_cov == True:
             return full_analytic_cov
 
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
 
     return analytic_cov
 
@@ -668,39 +668,39 @@
             M *=  np.outer(ps_all[na, nb, spec1], ps_all[nc, nd, spec2])
         
             analytic_cov_from_beam[i * nbins: (i + 1) * nbins, j * nbins: (j + 1) * nbins] = bin_mat(M, binning_file, lmax)
 
     return analytic_cov_from_beam
 
 
-def extract_mbb(mbb_inv, cov_T_E_only=True):
+def extract_mbb(mbb_inv, cov_T_E_only=True, dtype=np.float64):
     """The mode coupling marix is computed for T,E,B but for now we only construct analytical covariance matrix for T and E
     The B modes is complex with important E->B leakage, this routine extract the T and E part of the mode coupling matrix
 
     Parameters
     ----------
 
     mbb_inv: 2d array
       the inverse spin0 and 2 mode coupling matrix
     cov_T_E_only: boolean
         if true don't do B
     """
     nbins = mbb_inv["spin0xspin0"].shape[0]
     if cov_T_E_only:
-        mbb_inv_array = np.zeros((4*nbins, 4*nbins))
+        mbb_inv_array = np.zeros((4*nbins, 4*nbins), dtype=dtype)
         # TT
         mbb_inv_array[0*nbins:1*nbins, 0*nbins:1*nbins] = mbb_inv["spin0xspin0"]
         # TE
         mbb_inv_array[1*nbins:2*nbins, 1*nbins:2*nbins] = mbb_inv["spin0xspin2"]
         # ET
         mbb_inv_array[2*nbins:3*nbins, 2*nbins:3*nbins] = mbb_inv["spin2xspin0"]
         # EE
         mbb_inv_array[3*nbins:4*nbins, 3*nbins:4*nbins] = mbb_inv["spin2xspin2"][0:nbins, 0:nbins]
     else:
-        mbb_inv_array = np.zeros((9*nbins, 9*nbins))
+        mbb_inv_array = np.zeros((9*nbins, 9*nbins), dtype=dtype)
         # TT
         mbb_inv_array[0*nbins:1*nbins, 0*nbins:1*nbins] = mbb_inv["spin0xspin0"]
         # TE
         mbb_inv_array[1*nbins:2*nbins, 1*nbins:2*nbins] = mbb_inv["spin0xspin2"]
         # TB
         mbb_inv_array[2*nbins:3*nbins, 2*nbins:3*nbins] = mbb_inv["spin0xspin2"]
         # ET
```

### Comparing `pspy-1.6/pspy/so_dict.py` & `pspy-1.6.1/pspy/so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/so_map.py` & `pspy-1.6.1/pspy/so_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,28 @@
     """Class defining a ``so_map`` object."""
 
     def __init__(self):
         self.pixel = None
         self.nside = None
         self.ncomp = None
         self.data = None
-        self.geometry = None
         self.coordinate = None
 
     def copy(self):
         """Create a copy of the ``so_map`` object."""
 
         return deepcopy(self)
 
     def info(self):
         """Print information about the ``so_map`` object."""
 
         print("pixellisation:", self.pixel)
         print("number of components:", self.ncomp)
         print("number of pixels:", self.data.shape[:] if self.ncomp == 1 else self.data.shape[1:])
         print("nside:", self.nside)
-        print("geometry:", self.geometry)
         print("coordinates:", self.coordinate)
 
     def write_map(self, file_name):
         """Write the ``so_map`` to disk.
 
         Parameters
         ----------
@@ -91,15 +89,14 @@
         upgrade = self.copy()
         if self.pixel == "HEALPIX":
             nside_out = int(self.nside * factor)
             upgrade.data = hp.pixelfunc.ud_grade(self.data, nside_out=nside_out)
             upgrade.nside = nside_out
         if self.pixel == "CAR":
             upgrade.data = enmap.upgrade(self.data, factor)
-            upgrade.geometry = upgrade.data.geometry[1:]
         return upgrade
 
     def downgrade(self, factor):
         """Downgrade the ``so_map``.
 
         Parameters
         ----------
@@ -113,15 +110,14 @@
         downgrade = self.copy()
         if self.pixel == "HEALPIX":
             nside_out = int(self.nside / factor)
             downgrade.data = hp.pixelfunc.ud_grade(self.data, nside_out=nside_out)
             downgrade.nside = nside_out
         if self.pixel == "CAR":
             downgrade.data = enmap.downgrade(self.data, factor)
-            downgrade.geometry = downgrade.data.geometry[1:]
         return downgrade
 
     def synfast(self, clfile):
         """Fill a ``so_map`` with a cmb gaussian simulation.
 
         Parameters
         ----------
@@ -441,15 +437,14 @@
             try:
                 new_map.ncomp = len(fields_healpix)
             except:
                 new_map.ncomp = 1
             new_map.data = hp.fitsfunc.read_map(file, field=fields_healpix)
 
         new_map.nside = hp.pixelfunc.get_nside(new_map.data)
-        new_map.geometry = "healpix geometry"
         try:
             new_map.coordinate = header["SKYCOORD"]
         except:
             new_map.coordinate = None
 
     except:
         header = hdulist[0].header
@@ -464,15 +459,14 @@
             new_map.data = enmap.read_map(file, box=car_box)
         elif geometry is not None:
             new_map.data = enmap.read_map(file, geometry=geometry)
         else:
             new_map.data = enmap.read_map(file)
 
         new_map.nside = None
-        new_map.geometry = new_map.data.geometry[1:]
         new_map.coordinate = header["RADESYS"]
         if new_map.coordinate == "ICRS":
             new_map.coordinate = "equ"
 
     hdulist.close()
 
     if coordinate is not None:
@@ -504,15 +498,14 @@
     new_map.data = enmap.zeros(shape, wcs=wcs, dtype=None)
     new_map.data[0] = T
     new_map.data[1] = Q
     new_map.data[2] = U
     new_map.pixel = "CAR"
     new_map.nside = None
     new_map.ncomp = ncomp
-    new_map.geometry = T.geometry[1:]
     new_map.coordinate = "equ"
 
     return new_map
 
 def get_submap_car(map_car, box, mode="round"):
     """Cut a CAR submap (using pixell).
 
@@ -532,15 +525,14 @@
       "floor": both upper and lower bounds will be rounded down
       "ceil":  both upper and lower bounds will be rounded up
       "inclusive": lower bounds are rounded down, and upper bounds up
       "exclusive": lower bounds are rounded up, and upper bounds down"""
 
     submap = map_car.copy()
     submap.data = map_car.data.submap(box, mode=mode)
-    submap.geometry = map_car.data.submap(box, mode=mode).geometry[1:]
 
     return submap
 
 
 def get_box(ra0, ra1, dec0, dec1):
     """Create box in equatorial coordinates.
 
@@ -579,19 +571,17 @@
     """
 
     new_map = so_map()
     hdulist = emap.wcs.to_fits()
     header = hdulist[0].header
     new_map.pixel = header["CTYPE1"][-3:]
     shape, wcs = emap.geometry
-    new_map.geometry = shape[1:]
     new_map.ncomp = shape[0]
     new_map.data = emap.copy()
     new_map.nside = None
-    new_map.geometry = new_map.data.geometry[1:]
     new_map.coordinate = header["RADESYS"]
     if new_map.coordinate == "ICRS":
         new_map.coordinate = "equ"
 
     return new_map
 
 
@@ -682,15 +672,14 @@
         temp.data = np.zeros((3, 12 * nside ** 2))
     else:
         temp.data = np.zeros((12 * nside ** 2))
 
     temp.pixel = "HEALPIX"
     temp.ncomp = ncomp
     temp.nside = nside
-    temp.geometry = "healpix geometry"
     temp.coordinate = coordinate
     return temp
 
 
 def car_template(ncomp, ra0, ra1, dec0, dec1, res):
     """Create a ``so_map`` template with CAR pixellisation in equ coordinates.
 
@@ -707,23 +696,16 @@
     if ncomp == 3:
         pre = (3,)
     else:
         pre = ()
 
     box = get_box(ra0, ra1, dec0, dec1)
     res = res * np.pi / (180 * 60)
-    temp = so_map()
     shape, wcs = enmap.geometry(box, res=res, pre=pre)
-    temp.data = enmap.zeros(shape, wcs=wcs, dtype=None)
-    temp.pixel = "CAR"
-    temp.nside = None
-    temp.ncomp = ncomp
-    temp.geometry = temp.data.geometry[1:]
-    temp.coordinate = "equ"
-    return temp
+    return car_template_from_shape_wcs(ncomp, shape, wcs)
 
 
 def full_sky_car_template(ncomp, res):
     """Create a ``so_map`` full sky template with CAR pixellisation in equ coordinates.
 
     Parameters
     ----------
@@ -735,23 +717,42 @@
 
     if ncomp == 3:
         pre = (3,)
     else:
         pre = ()
 
     res = res * np.pi / (180 * 60)
-    temp = so_map()
     shape, wcs = enmap.fullsky_geometry(res=res, dims=pre)
-    temp.data = enmap.zeros(shape, wcs=wcs, dtype=None)
-    temp.pixel = "CAR"
-    temp.nside = None
-    temp.ncomp = ncomp
-    temp.geometry = temp.data.geometry[1:]
-    temp.coordinate = "equ"
-    return temp
+    return car_template_from_shape_wcs(ncomp, shape, wcs)
+
+def car_template_from_shape_wcs(ncomp_out, shape, wcs):
+    """
+    Create a template from shape and wcs args with
+    a number of components `ncomp_out`
+
+    Parameters
+    ----------
+    ncomp_out: int
+      number of components needed (e.g. 3 to create a
+      template for (I, Q, U))
+    shape: tuple
+    wcs: wcs object
+    """
+    shape_out = shape[-2:]
+    if ncomp_out > 1:
+        shape_out = (ncomp_out,) + shape_out
+
+    template = so_map()
+    template.data = enmap.zeros(shape_out, wcs=wcs, dtype=None)
+    template.pixel = "CAR"
+    template.nside = None
+    template.ncomp = ncomp_out
+    template.coordinate = "equ"
+
+    return template
 
 
 def white_noise(template, rms_uKarcmin_T, rms_uKarcmin_pol=None):
     """Generate a white noise realisation corresponding to the template pixellisation
 
     Parameters
     ----------
```

### Comparing `pspy-1.6/pspy/so_map_preprocessing.py` & `pspy-1.6.1/pspy/so_map_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/so_mcm.py` & `pspy-1.6.1/pspy/so_mcm.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/so_misc.py` & `pspy-1.6.1/pspy/so_misc.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/so_mpi.py` & `pspy-1.6.1/pspy/so_mpi.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/so_spectra.py` & `pspy-1.6.1/pspy/so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/so_window.py` & `pspy-1.6.1/pspy/so_window.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/sph_tools.py` & `pspy-1.6.1/pspy/sph_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat` & `pspy-1.6.1/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/tests/data/generate_test_data.py` & `pspy-1.6.1/pspy/tests/data/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/tests/data/test_data.pkl` & `pspy-1.6.1/pspy/tests/data/test_data.pkl`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/tests/test_pspy_namaster.py` & `pspy-1.6.1/pspy/tests/test_pspy_namaster.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/tests/test_so_dict.py` & `pspy-1.6.1/pspy/tests/test_so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/tests/test_so_map.py` & `pspy-1.6.1/pspy/tests/test_so_map.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/tests/test_so_spectra.py` & `pspy-1.6.1/pspy/tests/test_so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy/wigner3j/wigner3j_sub.f` & `pspy-1.6.1/pspy/wigner3j/wigner3j_sub.f`

 * *Files identical despite different names*

### Comparing `pspy-1.6/pspy.egg-info/PKG-INFO` & `pspy-1.6.1/pspy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.6
+Version: 1.6.1
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
@@ -83,16 +83,17 @@
         
         
         Authors
         ------------
         * `Thibaut Louis <https://thibautlouis.github.io>`_
         * Steve Choi
         * DW Han
-        * Xavier Garrido
+        * `Xavier Garrido <https://xgarrido.github.io>`_
         * Sigurd Naess
+        * `Adrien La Posta <https://adrien-laposta.github.io>`_
         
         The code is part of `PSpipe <https://github.com/simonsobs/PSpipe>`_ the Simons Observatory power spectrum pipeline.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pspy-1.6/pspy.egg-info/SOURCES.txt` & `pspy-1.6.1/pspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pspy-1.6/setup.py` & `pspy-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6/versioneer.py` & `pspy-1.6.1/versioneer.py`

 * *Files identical despite different names*

