# Comparing `tmp/mwrpy-0.1.6.tar.gz` & `tmp/mwrpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.1.6.tar", last modified: Wed May 10 12:19:06 2023, max compression
+gzip compressed data, was "mwrpy-0.1.7.tar", last modified: Thu May 11 08:07:08 2023, max compression
```

## Comparing `mwrpy-0.1.6.tar` & `mwrpy-0.1.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.218681 mwrpy-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 12:18:50.000000 mwrpy-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 12:18:50.000000 mwrpy-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-10 12:19:06.218681 mwrpy-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-10 12:18:50.000000 mwrpy-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/atmos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/level1/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/lev1_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/met_quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    48094 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/rpg_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/write_lev1_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/level2/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/get_ret_coeff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/lev2_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/lwp_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/write_lev2_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/plots/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51855 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/plots/generate_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/plots/plot_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/process_mwrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/rpg_mwr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/site_config/
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hatpro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/site_config/hyytiala/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.210681 mwrpy-0.1.6/mwrpy/site_config/juelich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.218681 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-10 12:19:05.000000 mwrpy-0.1.6/mwrpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-10 12:19:06.000000 mwrpy-0.1.6/mwrpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:19:05.000000 mwrpy-0.1.6/mwrpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 12:19:05.000000 mwrpy-0.1.6/mwrpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 12:19:05.000000 mwrpy-0.1.6/mwrpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:19:06.218681 mwrpy-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 12:18:50.000000 mwrpy-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 08:06:53.000000 mwrpy-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 08:06:53.000000 mwrpy-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-11 08:07:08.595337 mwrpy-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-11 08:06:53.000000 mwrpy-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.587336 mwrpy-0.1.7/mwrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/atmos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.591336 mwrpy-0.1.7/mwrpy/level1/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/lev1_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/met_quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48094 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/rpg_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24730 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/write_lev1_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.591336 mwrpy-0.1.7/mwrpy/level2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/get_ret_coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/lev2_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/lwp_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/write_lev2_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51855 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/plots/generate_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/plots/plot_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/process_mwrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/rpg_mwr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/site_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hatpro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/site_config/hyytiala/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.583336 mwrpy-0.1.7/mwrpy/site_config/juelich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.591336 mwrpy-0.1.7/mwrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:07:08.595337 mwrpy-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-11 08:06:53.000000 mwrpy-0.1.7/setup.py
```

### Comparing `mwrpy-0.1.6/LICENSE` & `mwrpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/PKG-INFO` & `mwrpy-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Home-page: https://github.com/actris-cloudnet/mwrpy
 Author: University of Cologne
 Author-email: actris-ccres-mwr@uni-koeln.de
 License: UNKNOWN
 Description: # MWRpy
```

### Comparing `mwrpy-0.1.6/README.md` & `mwrpy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/atmos.py` & `mwrpy-0.1.7/mwrpy/atmos.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/cli.py` & `mwrpy-0.1.7/mwrpy/cli.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.1.7/mwrpy/level1/lev1_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/level1/met_quality_control.py` & `mwrpy-0.1.7/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/level1/quality_control.py` & `mwrpy-0.1.7/mwrpy/level1/quality_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import ephem
 import netCDF4 as nc
 import numpy as np
 import pandas as pd
 from numpy import ma
 
-from mwrpy.utils import get_coeff_list, setbit
+from mwrpy.utils import get_coeff_list, setbit, time_to_datetime_index
 
 Fill_Value_Float = -999.0
 Fill_Value_Int = -99
 
 
 def apply_qc(site: str, data: dict, params: dict) -> None:
     """This function performs the quality control of level 1 data.
@@ -222,18 +222,18 @@
                         coeff["coefficient_mvr"][
                             coeff_ind + (len(data["frequency"]) - 1)
                         ].T
                         * np.array(data["tb"])[np.ix_(ele_ind, freq_ind)] ** 2,
                         axis=1,
                     )
                 )
-
+                ind = time_to_datetime_index(data["time"][:])
                 tb_df = pd.DataFrame(
                     {"Tb": (data["tb"][:, ifreq] - tb_ret[:, ifreq])},
-                    index=pd.to_datetime(data["time"][:], unit="s"),
+                    index=ind,
                 )
                 tb_mean = tb_df.resample(
                     "20min", origin="start", closed="left", label="left", offset="10min"
                 ).mean()
                 tb_mean = tb_mean.reindex(tb_df.index, method="nearest")
 
                 fact = [2.5, 3.5]  # factor for receiver retrieval uncertainty
```

### Comparing `mwrpy-0.1.6/mwrpy/level1/rpg_bin.py` & `mwrpy-0.1.7/mwrpy/level1/rpg_bin.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.1.7/mwrpy/level1/write_lev1_nc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from itertools import groupby
 from typing import TypeAlias
 
 import numpy as np
 import pandas as pd
 from numpy import ma
 
-from mwrpy import rpg_mwr
+from mwrpy import rpg_mwr, utils
 from mwrpy.level1.lev1_meta_nc import get_data_attributes
 from mwrpy.level1.met_quality_control import apply_met_qc
 from mwrpy.level1.quality_control import apply_qc
 from mwrpy.level1.rpg_bin import RpgBin
 from mwrpy.utils import (
     add_interpol1d,
     add_time_bounds,
@@ -339,37 +339,37 @@
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
     index = np.ones(len(ix)) * np.nan
     status = np.ones(len(ix), dtype=np.int32)
     freq_31 = np.where(np.round(lev1["frequency"][:], 1) == 31.4)[0]
     if len(freq_31) == 1:
-        time = lev1["time"][ix]
         tb = np.squeeze(lev1["tb"][ix, freq_31])
         tb[(lev1["pointing_flag"][ix] == 1) | (elevation_angle[ix] < 89.0)] = np.nan
-        tb_df = pd.DataFrame({"Tb": tb}, index=pd.to_datetime(time, unit="s"))
+        ind = utils.time_to_datetime_index(lev1["time"][ix])
+        tb_df = pd.DataFrame({"Tb": tb}, index=ind)
         tb_std = tb_df.rolling("2min", center=True, min_periods=10).std()
         tb_mx = tb_std.rolling("20min", center=True, min_periods=100).max()
 
         if "irt" in lev1:
             tb_thres = 0.1
             irt = lev1["irt"][ix, :]
             irt[irt == Fill_Value_Float] = np.nan
             irt = np.nanmean(irt, axis=1)
             irt[
                 (lev1["pointing_flag"][ix] == 1) | (elevation_angle[ix] < 89.0)
             ] = np.nan
-            irt_df = pd.DataFrame({"Irt": irt[:]}, index=pd.to_datetime(time, unit="s"))
+            irt_df = pd.DataFrame({"Irt": irt[:]}, index=ind)
             irt_mx = irt_df.rolling("20min", center=True, min_periods=100).max()
             index[(irt_mx["Irt"] > 263.15) & (tb_mx["Tb"] > tb_thres)] = 1
             status[:] = 0
 
         tb_thres = 0.2
         index[(tb_mx["Tb"] > tb_thres)] = 1
-        df = pd.DataFrame({"index": index}, index=pd.to_datetime(time, unit="s"))
+        df = pd.DataFrame({"index": index}, index=ind)
         df = df.fillna(method="bfill", limit=120)
         df = df.fillna(method="ffill", limit=120)
         index = np.array(df["index"])
         index[(tb_mx["Tb"] < tb_thres) & (index != 1.0)] = 0.0
         index[(elevation_angle[ix] < 89.0) & (index != 1.0)] = 2.0
 
     return np.nan_to_num(index, nan=2).astype(int), status
```

### Comparing `mwrpy-0.1.6/mwrpy/level2/get_ret_coeff.py` & `mwrpy-0.1.7/mwrpy/level2/get_ret_coeff.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.1.7/mwrpy/level2/lev2_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/level2/lwp_offset.py` & `mwrpy-0.1.7/mwrpy/level2/lwp_offset.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 # import os
 # from pathlib import Path
 # from time import gmtime
 
 import numpy as np
 import pandas as pd
 
+from mwrpy import utils
 from mwrpy.level1.write_lev1_nc import find_lwcl_free
 
 Fill_Value_Float = -999.0
 
 
 def correct_lwp_offset(
     lev1: dict, lwp_org: np.ndarray, index: np.ndarray
-) -> np.ndarray:
+) -> tuple[np.ndarray, np.ndarray]:
     """This function corrects Lwp offset using the
     2min standard deviation of the 31.4 GHz channel and IR temperature
 
     Args:
         lev1: Level 1 data.
         lwp_org: Lwp array.
         index: Index to use.
@@ -26,20 +27,17 @@
     if "elevation_angle" in lev1:
         elevation_angle = lev1["elevation_angle"][:]
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
     lwcl_i, _ = find_lwcl_free(lev1, index)
     lwp = np.copy(lwp_org)
-    lwp[(lwcl_i != 1) | (lwp > 0.04) | (elevation_angle[index] < 89.0)] = np.nan
-    time = lev1["time"][index]
-    if max(time) > 25:
-        lwp_df = pd.DataFrame({"Lwp": lwp}, index=pd.to_datetime(time, unit="s"))
-    else:
-        lwp_df = pd.DataFrame({"Lwp": lwp}, index=pd.to_datetime(time, unit="h"))
+    lwp[(lwcl_i != 0) | (lwp > 0.04) | (elevation_angle[index] < 89.0)] = np.nan
+    ind = utils.time_to_datetime_index(lev1["time"][index])
+    lwp_df = pd.DataFrame({"Lwp": lwp}, index=ind)
     lwp_std = lwp_df.rolling("2min", center=True, min_periods=10).std()
     lwp_max = lwp_std.rolling("20min", center=True, min_periods=100).max()
     lwp_df[lwp_max > 0.002] = np.nan
     lwp_offset = lwp_df.rolling("20min", center=True, min_periods=100).mean()
 
     # use previously determined offset (within 2h) and write current offset in csv file
     #
```

### Comparing `mwrpy-0.1.6/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.1.7/mwrpy/level2/write_lev2_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/plots/generate_plots.py` & `mwrpy-0.1.7/mwrpy/plots/generate_plots.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/plots/plot_meta.py` & `mwrpy-0.1.7/mwrpy/plots/plot_meta.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/plots/plot_utils.py` & `mwrpy-0.1.7/mwrpy/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/process_mwrpy.py` & `mwrpy-0.1.7/mwrpy/process_mwrpy.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/rpg_mwr.py` & `mwrpy-0.1.7/mwrpy/rpg_mwr.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/hatpro.yaml` & `mwrpy-0.1.7/mwrpy/site_config/hatpro.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/hyytiala/config.yaml` & `mwrpy-0.1.7/mwrpy/site_config/hyytiala/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc` & `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/mwrpy/utils.py` & `mwrpy-0.1.7/mwrpy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import time
 from datetime import date, datetime, timedelta, timezone
 from typing import Iterator, NamedTuple
 
 import netCDF4
 import numpy as np
+import pandas as pd
 import yaml
 from numpy import ma
 from scipy import signal
 from yaml.loader import SafeLoader
 
 SECONDS_PER_MINUTE = 60
 SECONDS_PER_HOUR = 3600
@@ -488,7 +489,12 @@
 
 def date_range(
     start_date: datetime.date, end_date: datetime.date
 ) -> Iterator[datetime.date]:
     """Returns range between two dates (datetimes)."""
     for n in range(int((end_date - start_date).days)):
         yield start_date + timedelta(n)
+
+
+def time_to_datetime_index(time_array: np.ndarray) -> pd.DatetimeIndex:
+    time_units = "s" if max(time_array) > 25 else "h"
+    return pd.to_datetime(time_array, unit=time_units)
```

### Comparing `mwrpy-0.1.6/mwrpy.egg-info/PKG-INFO` & `mwrpy-0.1.7/mwrpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Home-page: https://github.com/actris-cloudnet/mwrpy
 Author: University of Cologne
 Author-email: actris-ccres-mwr@uni-koeln.de
 License: UNKNOWN
 Description: # MWRpy
```

### Comparing `mwrpy-0.1.6/mwrpy.egg-info/SOURCES.txt` & `mwrpy-0.1.7/mwrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.6/setup.py` & `mwrpy-0.1.7/setup.py`

 * *Files identical despite different names*

