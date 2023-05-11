# Comparing `tmp/pyreduce-astro-0.5.8.tar.gz` & `tmp/pyreduce-astro-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreduce-astro-0.5.8.tar", last modified: Wed Oct 13 10:49:08 2021, max compression
+gzip compressed data, was "pyreduce-astro-0.5.9.tar", last modified: Thu Oct 28 12:15:28 2021, max compression
```

## Comparing `pyreduce-astro-0.5.8.tar` & `pyreduce-astro-0.5.9.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.397447 pyreduce-astro-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      448 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2021-10-13 10:49:08.397447 pyreduce-astro-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/codemeta.json
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.401447 pyreduce-astro-0.5.8/pyreduce/
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-10-13 10:49:08.401447 pyreduce-astro-0.5.8/pyreduce/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.381447 pyreduce-astro-0.5.8/pyreduce/clib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/clib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/clib/build_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)    50389 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/clib/slit_func_2d_xi_zeta_bd.c
--rw-r--r--   0 runner    (1001) docker     (121)      968 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/clib/slit_func_2d_xi_zeta_bd.h
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/clib/slit_func_bd.c
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/clib/slit_func_bd.h
--rw-r--r--   0 runner    (1001) docker     (121)     5581 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/clipnflip.py
--rw-r--r--   0 runner    (1001) docker     (121)    27002 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/combine_frames.py
--rw-r--r--   0 runner    (1001) docker     (121)     5842 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    11329 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/continuum_normalization.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11328 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/cwrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)    11186 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/echelle.py
--rw-r--r--   0 runner    (1001) docker     (121)     3930 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/estimate_background_scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)    44815 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/extraction_width.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.381447 pyreduce-astro-0.5.8/pyreduce/instruments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/common.json
--rw-r--r--   0 runner    (1001) docker     (121)    22317 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2189 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/crires_plus.json
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/crires_plus.py
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4215 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/harps.json
--rw-r--r--   0 runner    (1001) docker     (121)    10571 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/harps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3664 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/instrument_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     7540 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/instrument_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/jwst_miri.json
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/jwst_miri.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/jwst_niriss.json
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/jwst_niriss.py
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/lick_apf.json
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/lick_apf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/mcdonald.json
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/mcdonald.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/nirspec.json
--rw-r--r--   0 runner    (1001) docker     (121)     7965 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/nirspec.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1155 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/nte.json
--rwxr-xr-x   0 runner    (1001) docker     (121)     1487 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/nte.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/uves.json
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/uves.py
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/xshooter.json
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/instruments/xshooter.py
--rw-r--r--   0 runner    (1001) docker     (121)    20165 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/make_shear.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.389447 pyreduce-astro-0.5.8/pyreduce/masks/
--rw-r--r--   0 runner    (1001) docker     (121)   116600 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_crires_plus_det1.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)   149290 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_crires_plus_det2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)   149290 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_crires_plus_det3.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    11280 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_ctio_chiron.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     5871 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_elodie.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    61414 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_feros3.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    19740 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_flames_giraffe.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    24105 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_harps_blue.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    24835 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_harps_red.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    15587 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_hds_blue.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    11402 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_hds_red.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_het_hrs_2x5.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_jwst_miri_lrs_slitless.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_jwst_niriss_gr700xd.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    23847 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_lick_apf_.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    24057 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_nes.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     9466 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_nirspec_nirspec.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    97348 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_sarg.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    21718 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_sarg_2x2a.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    23078 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_sarg_2x2b.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    28440 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_subaru_hds_red.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    13763 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_blue.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     7590 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_blue_binned_2_2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    21652 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_middle.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     9930 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_middle_2x2_split.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    10409 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_middle_binned_2_2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    33317 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_red.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    14620 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_red_2x2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     9959 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_red_2x2_split.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    13277 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_red_binned_2_2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    28155 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/masks/mask_xshooter_nir.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/rectify.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    75320 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.389447 pyreduce-astro-0.5.8/pyreduce/settings/
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_CRIRES_PLUS.json
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_HARPS.json
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_JWST_MIRI.json
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_JWST_NIRISS.json
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_LICK_APF.json
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_MCDONALD.json
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_NIRSPEC.json
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_NTE.json
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_UVES.json
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_XSHOOTER.json
--rw-r--r--   0 runner    (1001) docker     (121)     4668 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_pyreduce.json
--rw-r--r--   0 runner    (1001) docker     (121)    33630 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/settings/settings_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.389447 pyreduce-astro-0.5.8/pyreduce/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4013 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/tools/combine.py
--rw-r--r--   0 runner    (1001) docker     (121)    19351 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/trace_orders.py
--rw-r--r--   0 runner    (1001) docker     (121)    37344 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.397447 pyreduce-astro-0.5.8/pyreduce/wavecal/
--rw-r--r--   0 runner    (1001) docker     (121)     9508 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/crires_plus_J1228_Open_det1.npz
--rw-r--r--   0 runner    (1001) docker     (121)     7976 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/crires_plus_J1228_Open_det2.npz
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/crires_plus_J1228_Open_det3.npz
--rw-r--r--   0 runner    (1001) docker     (121)   190128 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/harps_blue_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)   377987 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/harps_blue_pol_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    74679 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/harps_red_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)   147107 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/harps_red_pol_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/nirspec_K2.npz
--rw-r--r--   0 runner    (1001) docker     (121)    62739 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_blue_360nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)   130256 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_blue_390nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    96818 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_blue_437nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    66037 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_2x2_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    75994 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_565nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    28986 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_580nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    87881 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_600nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    56251 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_665nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    50889 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_860nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    26742 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_580nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    45163 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_600nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    27599 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_665nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    35978 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_760nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    10321 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_860nm_2D.npz
--rw-r--r--   0 runner    (1001) docker     (121)    21198 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavecal/xshooter_nir.npz
--rw-r--r--   0 runner    (1001) docker     (121)    67532 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/pyreduce/wavelength_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.397447 pyreduce-astro-0.5.8/pyreduce_astro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2021-10-13 10:49:08.000000 pyreduce-astro-0.5.8/pyreduce_astro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5008 2021-10-13 10:49:08.000000 pyreduce-astro-0.5.8/pyreduce_astro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-13 10:49:08.000000 pyreduce-astro-0.5.8/pyreduce_astro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-10-13 10:49:08.000000 pyreduce-astro-0.5.8/pyreduce_astro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-13 10:49:08.000000 pyreduce-astro-0.5.8/pyreduce_astro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-10-13 10:49:08.401447 pyreduce-astro-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 10:49:08.397447 pyreduce-astro-0.5.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_bias.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_clib_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     3227 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_clipnflip.py
--rw-r--r--   0 runner    (1001) docker     (121)     3813 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_continuum.py
--rw-r--r--   0 runner    (1001) docker     (121)     4915 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_cwrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4671 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_echelle.py
--rw-r--r--   0 runner    (1001) docker     (121)    11236 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_flat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_normflat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_reduce.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_science.py
--rw-r--r--   0 runner    (1001) docker     (121)     4736 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_shear.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/test/test_wavecal.py
--rw-r--r--   0 runner    (1001) docker     (121)    68777 2021-10-13 10:49:04.000000 pyreduce-astro-0.5.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.621141 pyreduce-astro-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3713 2021-10-28 12:15:28.621141 pyreduce-astro-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1688 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/codemeta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.621141 pyreduce-astro-0.5.9/pyreduce/
+-rw-r--r--   0 runner    (1001) docker     (121)     1436 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-10-28 12:15:28.621141 pyreduce-astro-0.5.9/pyreduce/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.597141 pyreduce-astro-0.5.9/pyreduce/clib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/clib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1979 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/clib/build_extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50389 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/clib/slit_func_2d_xi_zeta_bd.c
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/clib/slit_func_2d_xi_zeta_bd.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/clib/slit_func_bd.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/clib/slit_func_bd.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5581 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/clipnflip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27002 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/combine_frames.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5842 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11329 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/continuum_normalization.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11328 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/cwrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11186 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/echelle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3930 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/estimate_background_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44815 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2447 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/extraction_width.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.601141 pyreduce-astro-0.5.9/pyreduce/instruments/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/common.json
+-rw-r--r--   0 runner    (1001) docker     (121)    22317 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2189 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/crires_plus.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3530 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/crires_plus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5361 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4215 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/harps.json
+-rw-r--r--   0 runner    (1001) docker     (121)    10571 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/harps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3664 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/instrument_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7540 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/instrument_schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1142 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/jwst_miri.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/jwst_miri.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/jwst_niriss.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3385 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/jwst_niriss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1347 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/lick_apf.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/lick_apf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/mcdonald.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3905 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/mcdonald.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/nirspec.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7965 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/nirspec.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1155 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/nte.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1487 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/nte.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1742 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/uves.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/uves.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1771 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/xshooter.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/instruments/xshooter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20165 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/make_shear.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.609141 pyreduce-astro-0.5.9/pyreduce/masks/
+-rw-r--r--   0 runner    (1001) docker     (121)   116600 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_crires_plus_det1.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)   149290 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_crires_plus_det2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)   149290 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_crires_plus_det3.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    11280 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_ctio_chiron.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     5871 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_elodie.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    61414 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_feros3.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    19740 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_flames_giraffe.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    24105 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_harps_blue.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    24835 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_harps_red.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    15587 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_hds_blue.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    11402 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_hds_red.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_het_hrs_2x5.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_jwst_miri_lrs_slitless.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     4994 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_jwst_niriss_gr700xd.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    23847 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_lick_apf_.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    24057 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_nes.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     9466 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_nirspec_nirspec.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    97348 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_sarg.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    21718 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_sarg_2x2a.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    23078 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_sarg_2x2b.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    28440 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_subaru_hds_red.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    13763 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_blue.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     7590 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_blue_binned_2_2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    21652 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_middle.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     9930 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_middle_2x2_split.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    10409 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_middle_binned_2_2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    33317 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_red.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    14620 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_red_2x2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     9959 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_red_2x2_split.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    13277 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_red_binned_2_2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    28155 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/masks/mask_xshooter_nir.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/rectify.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    75320 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.609141 pyreduce-astro-0.5.9/pyreduce/settings/
+-rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_CRIRES_PLUS.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1445 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_HARPS.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_JWST_MIRI.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1236 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_JWST_NIRISS.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_LICK_APF.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_MCDONALD.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_NIRSPEC.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1428 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_NTE.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_UVES.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1774 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_XSHOOTER.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4668 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_pyreduce.json
+-rw-r--r--   0 runner    (1001) docker     (121)    33630 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/settings/settings_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.609141 pyreduce-astro-0.5.9/pyreduce/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4013 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/tools/combine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19351 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/trace_orders.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37344 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.617141 pyreduce-astro-0.5.9/pyreduce/wavecal/
+-rw-r--r--   0 runner    (1001) docker     (121)     9508 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/crires_plus_J1228_Open_det1.npz
+-rw-r--r--   0 runner    (1001) docker     (121)     7976 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/crires_plus_J1228_Open_det2.npz
+-rw-r--r--   0 runner    (1001) docker     (121)     5788 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/crires_plus_J1228_Open_det3.npz
+-rw-r--r--   0 runner    (1001) docker     (121)   190128 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/harps_blue_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)   377987 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/harps_blue_pol_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    74679 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/harps_red_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)   147107 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/harps_red_pol_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)     2588 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/nirspec_K2.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    62739 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_blue_360nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)   130256 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_blue_390nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    96818 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_blue_437nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    66037 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_2x2_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    75994 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_565nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    28986 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_580nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    87881 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_600nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    56251 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_665nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    50889 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_860nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    26742 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_580nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    45163 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_600nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    27599 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_665nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    35978 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_760nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    10321 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_860nm_2D.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    21198 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavecal/xshooter_nir.npz
+-rw-r--r--   0 runner    (1001) docker     (121)    67532 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/pyreduce/wavelength_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.617141 pyreduce-astro-0.5.9/pyreduce_astro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3713 2021-10-28 12:15:28.000000 pyreduce-astro-0.5.9/pyreduce_astro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5008 2021-10-28 12:15:28.000000 pyreduce-astro-0.5.9/pyreduce_astro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-28 12:15:28.000000 pyreduce-astro-0.5.9/pyreduce_astro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-10-28 12:15:28.000000 pyreduce-astro-0.5.9/pyreduce_astro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-28 12:15:28.000000 pyreduce-astro-0.5.9/pyreduce_astro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2021-10-28 12:15:28.621141 pyreduce-astro-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1818 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 12:15:28.621141 pyreduce-astro-0.5.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1787 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_bias.py
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_clib_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3227 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_clipnflip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3813 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1753 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4915 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_cwrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4671 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_echelle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11236 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_flat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3313 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_normflat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_science.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4736 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_shear.py
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/test/test_wavecal.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68777 2021-10-28 12:15:24.000000 pyreduce-astro-0.5.9/versioneer.py
```

### Comparing `pyreduce-astro-0.5.8/LICENSE` & `pyreduce-astro-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/PKG-INFO` & `pyreduce-astro-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreduce-astro
-Version: 0.5.8
+Version: 0.5.9
 Summary: A data reduction package for echelle spectrographs
 Home-page: https://github.com/AWehrhahn/PyReduce
 Author: Ansgar Wehrhahn
 Author-email: ansgar.wehrhahn@physics.uu.se
 License: UNKNOWN
 Description: ![Python application](https://github.com/AWehrhahn/PyReduce/workflows/Python%20application/badge.svg)
         [![Documentation Status](https://readthedocs.org/projects/pyreduce-astro/badge/?version=latest)](https://pyreduce-astro.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `pyreduce-astro-0.5.8/README.md` & `pyreduce-astro-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/codemeta.json` & `pyreduce-astro-0.5.9/codemeta.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/__init__.py` & `pyreduce-astro-0.5.9/pyreduce/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/__main__.py` & `pyreduce-astro-0.5.9/pyreduce/__main__.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/clib/build_extract.py` & `pyreduce-astro-0.5.9/pyreduce/clib/build_extract.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/clib/slit_func_2d_xi_zeta_bd.c` & `pyreduce-astro-0.5.9/pyreduce/clib/slit_func_2d_xi_zeta_bd.c`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/clib/slit_func_2d_xi_zeta_bd.h` & `pyreduce-astro-0.5.9/pyreduce/clib/slit_func_2d_xi_zeta_bd.h`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/clib/slit_func_bd.c` & `pyreduce-astro-0.5.9/pyreduce/clib/slit_func_bd.c`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/clib/slit_func_bd.h` & `pyreduce-astro-0.5.9/pyreduce/clib/slit_func_bd.h`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/clipnflip.py` & `pyreduce-astro-0.5.9/pyreduce/clipnflip.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/combine_frames.py` & `pyreduce-astro-0.5.9/pyreduce/combine_frames.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/configuration.py` & `pyreduce-astro-0.5.9/pyreduce/configuration.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/continuum_normalization.py` & `pyreduce-astro-0.5.9/pyreduce/continuum_normalization.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/cwrappers.py` & `pyreduce-astro-0.5.9/pyreduce/cwrappers.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/datasets.py` & `pyreduce-astro-0.5.9/pyreduce/datasets.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/echelle.py` & `pyreduce-astro-0.5.9/pyreduce/echelle.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/estimate_background_scatter.py` & `pyreduce-astro-0.5.9/pyreduce/estimate_background_scatter.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/extract.py` & `pyreduce-astro-0.5.9/pyreduce/extract.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/extraction_width.py` & `pyreduce-astro-0.5.9/pyreduce/extraction_width.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/common.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/common.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/common.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/common.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/crires_plus.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/crires_plus.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/crires_plus.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/crires_plus.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/filters.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,24 +31,32 @@
         self.data = []
         self.unique = unique
         self.ignorecase = ignorecase
 
         if self.ignorecase and not self.flags & re.IGNORECASE:
             self.flags += re.IGNORECASE
 
-    def collect(self, header):
+    def _collect_value(self, header):
         if self.keyword is None:
             value = ""
+        elif "{" in self.keyword:
+            kws = re.findall(r"{([^{}]+)}", self.keyword)
+            values = {kw: header.get(kw, "") for kw in kws}
+            value = self.keyword.format(**values)
         else:
             value = header.get(self.keyword)
         if value.__class__ == header.__class__:
             if len(value) > 0:
                 value = value[0]
             else:
                 value = ""
+        return value
+
+    def collect(self, header):
+        value = self._collect_value(header)
         self.data.append(value)
         return value
 
     def match(self, value):
         if self.keyword is None:
             result = np.full(len(self.data), False)
         else:
@@ -101,31 +109,40 @@
     def __init__(self, keyword="OBJECT", **kwargs):
         kwargs["dtype"] = "U20"
         kwargs["unique"] = False
         super().__init__(keyword, **kwargs)
 
 
 class NightFilter(Filter):
-    def __init__(self, keyword="DATE-OBS", timeformat="fits", **kwargs):
+    def __init__(
+        self,
+        keyword="DATE-OBS",
+        timeformat="fits",
+        timezone="utc",
+        timezone_local=None,
+        **kwargs,
+    ):
         super().__init__(keyword, dtype=datetime, **kwargs)
         self.timeformat = timeformat
+        self.timezone = timezone
+        self.timezone_local = timezone_local
 
     @staticmethod
     def observation_date_to_night(observation_date):
         """Convert an observation timestamp into the date of the observation night
         Nights start at 12am and end at 12 am the next day
         """
         if observation_date.to_datetime().hour < 12:
             observation_date -= 1 * u.day
         return observation_date.to_datetime().date()
 
     def collect(self, header):
-        value = header.get(self.keyword)
+        value = super()._collect_value(header)
         if value is not None:
-            value = Time(value, format=self.timeformat)
+            value = Time(value, format=self.timeformat, scale=self.timezone)
             value = NightFilter.observation_date_to_night(value)
         else:
             logger.warning(
                 "Could not determine the observation date of %s, skipping it", header
             )
         self.data.append(value)
         return value
```

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/harps.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/harps.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/harps.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/harps.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/instrument_info.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/instrument_info.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/instrument_schema.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/instrument_schema.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/jwst_miri.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/jwst_miri.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/jwst_miri.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/jwst_miri.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/jwst_niriss.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/jwst_niriss.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/jwst_niriss.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/jwst_niriss.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/lick_apf.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/lick_apf.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/lick_apf.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/lick_apf.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/mcdonald.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/mcdonald.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9893617021276596%*

 * *Differences: {"'category'": "'IMAGETYP'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__instrument__": "MCDONALD",
     "altitude": 2075,
     "amplifier": "AMPLIFIE",
-    "category": "",
+    "category": "IMAGETYP",
     "dark": 1,
     "dark_time": "DARKTIME",
     "date": "DATE-OBS",
     "dec": "DEC",
     "exposure_time": "EXPTIME",
     "extension": 0,
     "gain": "GAIN{amplifier}",
```

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/mcdonald.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/mcdonald.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 from .common import InstrumentWithModes, getter, observation_date_to_night
 from .filters import Filter
 
 logger = logging.getLogger(__name__)
 
 
 class MCDONALD(InstrumentWithModes):
+    def __init__(self):
+        super().__init__()
+        # The date is a combination of the two values
+        kw = f"{{{self.info['date']}}}T{{{self.info['universal_time']}}}"
+        self.filters["night"].keyword = kw
+
     def _convert_time_deg(self, v):
         v = [float(s) for s in v.split(":")]
         v = v[0] + v[1] / 60 + v[2] / 3600
         return v
 
     def add_header_info(self, header, mode, **kwargs):
         """read data from header and add it as REDUCE keyword back to the header"""
@@ -73,24 +79,27 @@
         header["e_backg"] = header["e_gain"] * (header["e_drk"] + header["e_sky"])
 
         header["e_imtype"] = get("observation_type")
         header["e_ctg"] = get("observation_type")
 
         obs_date = get("date")
         ut = get("universal_time")
+        if obs_date is not None and ut is not None:
+            obs_date = f"{obs_date}T{ut}"
+
         dark_time = get("dark_time")
         ra = get("ra")
         dec = get("dec")
 
         if ra is not None:
             ra = self._convert_time_deg(ra)
         if dec is not None:
             dec = self._convert_time_deg(dec)
-        if ut is not None and dark_time is not None:
-            tmid = self._convert_time_deg(ut) + dark_time / 2
+        if dark_time is not None:
+            tmid = dark_time / 2
         else:
             tmid = 0
         if obs_date is not None:
             jd = Time(obs_date).mjd + tmid + 0.5
         else:
             jd = 0
```

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/nirspec.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/nirspec.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/nirspec.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/nirspec.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/nte.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/nte.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/nte.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/nte.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/uves.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/uves.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/uves.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/uves.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/xshooter.json` & `pyreduce-astro-0.5.9/pyreduce/instruments/xshooter.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/instruments/xshooter.py` & `pyreduce-astro-0.5.9/pyreduce/instruments/xshooter.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/make_shear.py` & `pyreduce-astro-0.5.9/pyreduce/make_shear.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_crires_plus_det1.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_crires_plus_det1.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_crires_plus_det2.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_crires_plus_det2.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_crires_plus_det3.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_crires_plus_det3.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_ctio_chiron.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_ctio_chiron.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_elodie.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_elodie.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_feros3.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_feros3.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_flames_giraffe.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_flames_giraffe.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_harps_blue.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_harps_blue.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_harps_red.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_harps_red.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_hds_blue.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_hds_blue.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_hds_red.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_hds_red.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_het_hrs_2x5.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_het_hrs_2x5.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_jwst_miri_lrs_slitless.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_jwst_miri_lrs_slitless.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_jwst_niriss_gr700xd.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_jwst_niriss_gr700xd.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_lick_apf_.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_lick_apf_.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_nes.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_nes.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_nirspec_nirspec.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_nirspec_nirspec.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_sarg.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_sarg.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_sarg_2x2a.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_sarg_2x2a.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_sarg_2x2b.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_sarg_2x2b.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_subaru_hds_red.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_subaru_hds_red.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_blue.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_blue.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_blue_binned_2_2.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_blue_binned_2_2.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_middle.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_middle.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_middle_2x2_split.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_middle_2x2_split.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_middle_binned_2_2.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_middle_binned_2_2.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_red.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_red.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_red_2x2.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_red_2x2.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_red_2x2_split.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_red_2x2_split.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_uves_red_binned_2_2.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_uves_red_binned_2_2.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/masks/mask_xshooter_nir.fits.gz` & `pyreduce-astro-0.5.9/pyreduce/masks/mask_xshooter_nir.fits.gz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/rectify.py` & `pyreduce-astro-0.5.9/pyreduce/rectify.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/reduce.py` & `pyreduce-astro-0.5.9/pyreduce/reduce.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_CRIRES_PLUS.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_CRIRES_PLUS.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_HARPS.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_HARPS.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_JWST_MIRI.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_JWST_MIRI.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_JWST_NIRISS.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_JWST_NIRISS.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_LICK_APF.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_LICK_APF.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_MCDONALD.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_MCDONALD.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_NIRSPEC.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_NIRSPEC.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_NTE.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_NTE.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_UVES.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_UVES.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_XSHOOTER.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_XSHOOTER.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_pyreduce.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_pyreduce.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/settings/settings_schema.json` & `pyreduce-astro-0.5.9/pyreduce/settings/settings_schema.json`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/tools/combine.py` & `pyreduce-astro-0.5.9/pyreduce/tools/combine.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/trace_orders.py` & `pyreduce-astro-0.5.9/pyreduce/trace_orders.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/util.py` & `pyreduce-astro-0.5.9/pyreduce/util.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/crires_plus_J1228_Open_det1.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/crires_plus_J1228_Open_det1.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/crires_plus_J1228_Open_det2.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/crires_plus_J1228_Open_det2.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/crires_plus_J1228_Open_det3.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/crires_plus_J1228_Open_det3.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/harps_blue_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/harps_blue_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/harps_blue_pol_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/harps_blue_pol_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/harps_red_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/harps_red_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/harps_red_pol_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/harps_red_pol_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/nirspec_K2.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/nirspec_K2.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_blue_360nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_blue_360nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_blue_390nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_blue_390nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_blue_437nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_blue_437nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_2x2_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_2x2_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_565nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_565nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_580nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_580nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_600nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_600nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_665nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_665nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_middle_860nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_middle_860nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_580nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_580nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_600nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_600nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_665nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_665nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_760nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_760nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/uves_red_860nm_2D.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/uves_red_860nm_2D.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavecal/xshooter_nir.npz` & `pyreduce-astro-0.5.9/pyreduce/wavecal/xshooter_nir.npz`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce/wavelength_calibration.py` & `pyreduce-astro-0.5.9/pyreduce/wavelength_calibration.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/pyreduce_astro.egg-info/PKG-INFO` & `pyreduce-astro-0.5.9/pyreduce_astro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreduce-astro
-Version: 0.5.8
+Version: 0.5.9
 Summary: A data reduction package for echelle spectrographs
 Home-page: https://github.com/AWehrhahn/PyReduce
 Author: Ansgar Wehrhahn
 Author-email: ansgar.wehrhahn@physics.uu.se
 License: UNKNOWN
 Description: ![Python application](https://github.com/AWehrhahn/PyReduce/workflows/Python%20application/badge.svg)
         [![Documentation Status](https://readthedocs.org/projects/pyreduce-astro/badge/?version=latest)](https://pyreduce-astro.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `pyreduce-astro-0.5.8/pyreduce_astro.egg-info/SOURCES.txt` & `pyreduce-astro-0.5.9/pyreduce_astro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/setup.py` & `pyreduce-astro-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_bias.py` & `pyreduce-astro-0.5.9/test/test_bias.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_clipnflip.py` & `pyreduce-astro-0.5.9/test/test_clipnflip.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_combine.py` & `pyreduce-astro-0.5.9/test/test_combine.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_configuration.py` & `pyreduce-astro-0.5.9/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_continuum.py` & `pyreduce-astro-0.5.9/test/test_continuum.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_cwrappers.py` & `pyreduce-astro-0.5.9/test/test_cwrappers.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_echelle.py` & `pyreduce-astro-0.5.9/test/test_echelle.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_extract.py` & `pyreduce-astro-0.5.9/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_flat.py` & `pyreduce-astro-0.5.9/test/test_flat.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_instruments.py` & `pyreduce-astro-0.5.9/test/test_instruments.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_mask.py` & `pyreduce-astro-0.5.9/test/test_mask.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_normflat.py` & `pyreduce-astro-0.5.9/test/test_normflat.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_orders.py` & `pyreduce-astro-0.5.9/test/test_orders.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_reduce.py` & `pyreduce-astro-0.5.9/test/test_reduce.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_scatter.py` & `pyreduce-astro-0.5.9/test/test_scatter.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_science.py` & `pyreduce-astro-0.5.9/test/test_science.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_shear.py` & `pyreduce-astro-0.5.9/test/test_shear.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/test/test_wavecal.py` & `pyreduce-astro-0.5.9/test/test_wavecal.py`

 * *Files identical despite different names*

### Comparing `pyreduce-astro-0.5.8/versioneer.py` & `pyreduce-astro-0.5.9/versioneer.py`

 * *Files identical despite different names*

