# Comparing `tmp/grizli-1.8.5.tar.gz` & `tmp/grizli-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizli-1.8.5.tar", last modified: Mon Apr 24 11:43:19 2023, max compression
+gzip compressed data, was "grizli-1.8.7.tar", last modified: Wed May 10 16:44:43 2023, max compression
```

## Comparing `grizli-1.8.5.tar` & `grizli-1.8.7.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.824410 grizli-1.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.768410 grizli-1.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.772410 grizli-1.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-24 11:43:06.000000 grizli-1.8.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-24 11:43:06.000000 grizli-1.8.5/.github/workflows/python-package-ero.yml
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-24 11:43:06.000000 grizli-1.8.5/.github/workflows/python-package-with-jwst.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-24 11:43:06.000000 grizli-1.8.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-24 11:43:06.000000 grizli-1.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 11:43:06.000000 grizli-1.8.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-24 11:43:06.000000 grizli-1.8.5/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 11:43:06.000000 grizli-1.8.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 11:43:06.000000 grizli-1.8.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-24 11:43:06.000000 grizli-1.8.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-24 11:43:19.824410 grizli-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-24 11:43:06.000000 grizli-1.8.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.776410 grizli-1.8.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.776410 grizli-1.8.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/_static/grizli.ico
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/_static/grizli_favico.png
--rw-r--r--   0 runner    (1001) docker     (123)    35735 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/_static/grizli_favico_large.png
--rw-r--r--   0 runner    (1001) docker     (123)   193903 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/_static/grizli_logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/_static/grizli_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.768410 grizli-1.8.5/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.776410 grizli-1.8.5/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.780410 grizli-1.8.5/docs/grizli/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/grizli/basic.rst
--rw-r--r--   0 runner    (1001) docker     (123)   851247 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/grizli/ceers-sm.field.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    98779 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/grizli/image-release-v6.md
--rw-r--r--   0 runner    (1001) docker     (123)    65882 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/grizli/image-release-v6.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/grizli/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/grizli/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/grizli/prep.rst
--rw-r--r--   0 runner    (1001) docker     (123)    38260 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/grizli-for-dummies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 11:43:06.000000 grizli-1.8.5/docs/rtd-pip-requirements
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 11:43:06.000000 grizli-1.8.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.780410 grizli-1.8.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-24 11:43:06.000000 grizli-1.8.5/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-24 11:43:06.000000 grizli-1.8.5/examples/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-04-24 11:43:06.000000 grizli-1.8.5/examples/grizli_demo_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   100981 2023-04-24 11:43:06.000000 grizli-1.8.5/examples/grizli_demo_1.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   193903 2023-04-24 11:43:06.000000 grizli-1.8.5/examples/grizli_logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-04-24 11:43:06.000000 grizli-1.8.5/examples/grizli_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.784410 grizli-1.8.5/grizli/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.788410 grizli-1.8.5/grizli/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46017 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/aws/aws_drizzler.py
--rw-r--r--   0 runner    (1001) docker     (123)   131901 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/aws/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    44173 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/aws/field_tiles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9609 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/aws/fit_redshift_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)    32497 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/aws/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    56356 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/aws/tile_mosaic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    75375 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/aws/visit_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    40400 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.796410 grizli-1.8.5/grizli/data/
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/auto_script_defaults.yml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/db.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/gaia_dr2_vizier_columns.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/hst_encircled_energy.fits
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/jwst_bp_info.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nircam_wisp.yml
--rw-r--r--   0 runner    (1001) docker     (123)    47343 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_badpix_230120_NRCALONG.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    39840 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_badpix_230120_NRCBLONG.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    17258 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCA1.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCA2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16627 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCA3.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16943 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCA4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    35486 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCALONG.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCB1.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCB2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16962 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCB3.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCB4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    22659 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCBLONG.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/photom_correction.yml
--rw-r--r--   0 runner    (1001) docker     (123)    97707 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/sep_catalog_junk.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.800410 grizli-1.8.5/grizli/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    94256 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/FeII_VeronCetty2004.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/README
--rw-r--r--   0 runner    (1001) docker     (123)   221907 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/alf_SSP.dat
--rw-r--r--   0 runner    (1001) docker     (123)    48158 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/cvd12_t11_solar_Chabrier.dat
--rw-r--r--   0 runner    (1001) docker     (123)    51300 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/eazy_intermediate.dat
--rw-r--r--   0 runner    (1001) docker     (123)    44824 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/erb2010.dat
--rw-r--r--   0 runner    (1001) docker     (123)    31746 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/erb2010_continuum.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.808410 grizli-1.8.5/grizli/data/templates/fsps/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3.param
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3.param.fits
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_001.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156521 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_002.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156524 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_003.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156527 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_004.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156524 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_005.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156523 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_006.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156509 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_007.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156510 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_008.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156511 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_009.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156512 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_010.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156518 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_011.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156518 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_012.dat
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines.param
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_001.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156521 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_002.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156524 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_003.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156527 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_004.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156524 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_005.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156523 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_006.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156509 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_007.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156510 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_008.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156511 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_009.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156512 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_010.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156518 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_011.dat
--rw-r--r--   0 runner    (1001) docker     (123)   156518 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_012.dat
--rw-r--r--   0 runner    (1001) docker     (123)   143958 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/fsps_starburst_lines.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/post_starburst.dat
--rw-r--r--   0 runner    (1001) docker     (123)   557728 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/quasar_lines.txt
--rw-r--r--   0 runner    (1001) docker     (123)   382216 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/red_blue_continuum.txt
--rw-r--r--   0 runner    (1001) docker     (123)   381266 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/red_blue_continuum_noLya.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.816410 grizli-1.8.5/grizli/data/templates/stars/
--rw-r--r--   0 runner    (1001) docker     (123)   173069 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/L1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)   145419 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/L3.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/L6.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)   159659 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/M6.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   166768 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/M8.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    57965 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/T2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    55327 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/T6.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/T7.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)  3193920 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/bt-settl_t400-3500_z0.0.fits
--rw-r--r--   0 runner    (1001) docker     (123)    83291 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/carbon_star.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/templates/stars/stars_settl.param
--rw-r--r--   0 runner    (1001) docker     (123)   299891 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/visit_alignment.txt
--rw-r--r--   0 runner    (1001) docker     (123)    54096 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/wfc3ir_badpix_spars200_22.03.31.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/wfc3ir_dark_badpix_2019.01.12.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/data/wfc3ir_ee.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/ds9.py
--rw-r--r--   0 runner    (1001) docker     (123)    17575 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/fake_image.py
--rw-r--r--   0 runner    (1001) docker     (123)   185637 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.816410 grizli-1.8.5/grizli/galfit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/galfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15242 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/galfit/deconvolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/galfit/galfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/galfit/gfutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/galfit/psf.py
--rw-r--r--   0 runner    (1001) docker     (123)    39980 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/grismconf.py
--rw-r--r--   0 runner    (1001) docker     (123)    35836 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/jwst_level1.py
--rw-r--r--   0 runner    (1001) docker     (123)    77490 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/jwst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   203738 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)   203978 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/multifit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/nbutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.816410 grizli-1.8.5/grizli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   222662 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/pipeline/auto_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/pipeline/default_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    32369 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/pipeline/photoz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/pipeline/reprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/pipeline/run_MPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/pipeline/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)   248022 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/prep.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49392 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.820410 grizli-1.8.5/grizli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.820410 grizli-1.8.5/grizli/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/fit_args.npy
--rw-r--r--   0 runner    (1001) docker     (123)   812160 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/j033216m2743_00152.beams.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.824410 grizli-1.8.5/grizli/tests/data/jwst-headers/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/jwst-headers/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28024 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/jwst-headers/det_image_seq1_MIRIMAGE_F560Wexp1_cal.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    47863 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca1_rate.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    47877 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca2_rate.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca5_uncal_dispersed_GRISMR_crossing_F356W_rate.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    47827 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/jwst-headers/jw42424001001_01105_00002_nrca5_rate.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/jwst-headers/strip_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   509760 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/niriss_jw01324001001_test.beams.fits
--rw-r--r--   0 runner    (1001) docker     (123)  1120244 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/data/wfc3-parse-test.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/test_autoscript.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/test_cutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/test_grismconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/test_jwst.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   297616 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.824410 grizli-1.8.5/grizli/utils_c/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/utils_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   334421 2023-04-24 11:43:18.000000 grizli-1.8.5/grizli/utils_c/disperse.c
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/utils_c/disperse.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   659013 2023-04-24 11:43:18.000000 grizli-1.8.5/grizli/utils_c/interp.c
--rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-04-24 11:43:06.000000 grizli-1.8.5/grizli/utils_c/interp.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 11:43:19.000000 grizli-1.8.5/grizli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:43:19.788410 grizli-1.8.5/grizli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-24 11:43:19.000000 grizli-1.8.5/grizli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-24 11:43:19.000000 grizli-1.8.5/grizli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:43:19.000000 grizli-1.8.5/grizli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-24 11:43:19.000000 grizli-1.8.5/grizli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 11:43:19.000000 grizli-1.8.5/grizli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 11:43:06.000000 grizli-1.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-24 11:43:19.824410 grizli-1.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-24 11:43:06.000000 grizli-1.8.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-04-24 11:43:06.000000 grizli-1.8.5/test_pipeline_hst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.685714 grizli-1.8.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.637705 grizli-1.8.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.641706 grizli-1.8.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 16:44:28.000000 grizli-1.8.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-10 16:44:28.000000 grizli-1.8.7/.github/workflows/python-package-ero.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-10 16:44:28.000000 grizli-1.8.7/.github/workflows/python-package-with-jwst.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-10 16:44:28.000000 grizli-1.8.7/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-10 16:44:28.000000 grizli-1.8.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-10 16:44:28.000000 grizli-1.8.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-10 16:44:28.000000 grizli-1.8.7/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-10 16:44:28.000000 grizli-1.8.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-10 16:44:28.000000 grizli-1.8.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 16:44:28.000000 grizli-1.8.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-10 16:44:43.685714 grizli-1.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-10 16:44:28.000000 grizli-1.8.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.645707 grizli-1.8.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.645707 grizli-1.8.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/_static/grizli.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/_static/grizli_favico.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35735 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/_static/grizli_favico_large.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193903 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/_static/grizli_logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/_static/grizli_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.637705 grizli-1.8.7/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.645707 grizli-1.8.7/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.649707 grizli-1.8.7/docs/grizli/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/grizli/basic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   851247 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/grizli/ceers-sm.field.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    98779 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/grizli/image-release-v6.md
+-rw-r--r--   0 runner    (1001) docker     (123)    65882 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/grizli/image-release-v6.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/grizli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/grizli/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/grizli/prep.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38260 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/grizli-for-dummies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 16:44:28.000000 grizli-1.8.7/docs/rtd-pip-requirements
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 16:44:28.000000 grizli-1.8.7/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.649707 grizli-1.8.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-10 16:44:28.000000 grizli-1.8.7/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-10 16:44:28.000000 grizli-1.8.7/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-05-10 16:44:28.000000 grizli-1.8.7/examples/grizli_demo_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   100981 2023-05-10 16:44:28.000000 grizli-1.8.7/examples/grizli_demo_1.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   193903 2023-05-10 16:44:28.000000 grizli-1.8.7/examples/grizli_logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-05-10 16:44:28.000000 grizli-1.8.7/examples/grizli_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.653708 grizli-1.8.7/grizli/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.653708 grizli-1.8.7/grizli/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46017 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/aws/aws_drizzler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131901 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/aws/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45124 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/aws/field_tiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9609 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/aws/fit_redshift_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32497 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/aws/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56356 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/aws/tile_mosaic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    75867 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/aws/visit_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40400 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.657709 grizli-1.8.7/grizli/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/auto_script_defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/db.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/gaia_dr2_vizier_columns.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/hst_encircled_energy.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/jwst_bp_info.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nircam_wisp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    47343 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_badpix_230120_NRCALONG.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    39840 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_badpix_230120_NRCBLONG.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    17258 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCA1.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCA2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16627 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCA3.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16943 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCA4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    35486 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCALONG.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCB1.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCB2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16962 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCB3.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCB4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    22659 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCBLONG.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/photom_correction.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    97707 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/sep_catalog_junk.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.661710 grizli-1.8.7/grizli/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    94256 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/FeII_VeronCetty2004.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/README
+-rw-r--r--   0 runner    (1001) docker     (123)   221907 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/alf_SSP.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    48158 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/cvd12_t11_solar_Chabrier.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    51300 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/eazy_intermediate.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    44824 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/erb2010.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    31746 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/erb2010_continuum.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.669711 grizli-1.8.7/grizli/data/templates/fsps/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3.param
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3.param.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_001.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156521 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_002.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156524 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_003.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156527 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_004.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156524 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_005.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156523 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_006.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156509 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_007.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156510 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_008.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156511 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_009.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156512 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_010.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156518 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_011.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156518 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_012.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines.param
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_001.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156521 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_002.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156524 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_003.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156527 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_004.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156524 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_005.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156523 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_006.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156509 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_007.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156510 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_008.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156511 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_009.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156512 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_010.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156518 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_011.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   156518 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_012.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   143958 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/fsps_starburst_lines.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/post_starburst.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   557728 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/quasar_lines.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   382216 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/red_blue_continuum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   381266 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/red_blue_continuum_noLya.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.677713 grizli-1.8.7/grizli/data/templates/stars/
+-rw-r--r--   0 runner    (1001) docker     (123)   173069 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/L1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   145419 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/L3.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/L6.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   159659 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/M6.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   166768 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/M8.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    57965 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/T2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55327 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/T6.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/T7.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3193920 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/bt-settl_t400-3500_z0.0.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    83291 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/carbon_star.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/templates/stars/stars_settl.param
+-rw-r--r--   0 runner    (1001) docker     (123)   299891 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/visit_alignment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    54096 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/wfc3ir_badpix_spars200_22.03.31.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/wfc3ir_dark_badpix_2019.01.12.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/data/wfc3ir_ee.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/ds9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17575 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/fake_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   185637 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.677713 grizli-1.8.7/grizli/galfit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/galfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15242 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/galfit/deconvolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/galfit/galfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/galfit/gfutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/galfit/psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39980 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/grismconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35836 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/jwst_level1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77490 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/jwst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   203738 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   203978 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/multifit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/nbutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.677713 grizli-1.8.7/grizli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222662 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/pipeline/auto_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/pipeline/default_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32411 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/pipeline/photoz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/pipeline/reprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/pipeline/run_MPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/pipeline/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)   248024 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/prep.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49392 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.681713 grizli-1.8.7/grizli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.681713 grizli-1.8.7/grizli/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/fit_args.npy
+-rw-r--r--   0 runner    (1001) docker     (123)   812160 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/j033216m2743_00152.beams.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.685714 grizli-1.8.7/grizli/tests/data/jwst-headers/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/jwst-headers/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28024 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/jwst-headers/det_image_seq1_MIRIMAGE_F560Wexp1_cal.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    47863 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca1_rate.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    47877 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca2_rate.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca5_uncal_dispersed_GRISMR_crossing_F356W_rate.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    47827 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/jwst-headers/jw42424001001_01105_00002_nrca5_rate.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/jwst-headers/strip_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   509760 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/niriss_jw01324001001_test.beams.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  1120244 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/data/wfc3-parse-test.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/test_autoscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/test_cutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/test_grismconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/test_jwst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   298264 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.685714 grizli-1.8.7/grizli/utils_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/utils_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   334421 2023-05-10 16:44:42.000000 grizli-1.8.7/grizli/utils_c/disperse.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/utils_c/disperse.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   659013 2023-05-10 16:44:42.000000 grizli-1.8.7/grizli/utils_c/interp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-05-10 16:44:28.000000 grizli-1.8.7/grizli/utils_c/interp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 16:44:43.000000 grizli-1.8.7/grizli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:44:43.653708 grizli-1.8.7/grizli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-10 16:44:43.000000 grizli-1.8.7/grizli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-10 16:44:43.000000 grizli-1.8.7/grizli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:44:43.000000 grizli-1.8.7/grizli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-10 16:44:43.000000 grizli-1.8.7/grizli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 16:44:43.000000 grizli-1.8.7/grizli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-10 16:44:28.000000 grizli-1.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-10 16:44:43.689715 grizli-1.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-10 16:44:28.000000 grizli-1.8.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-05-10 16:44:28.000000 grizli-1.8.7/test_pipeline_hst.py
```

### Comparing `grizli-1.8.5/.github/workflows/publish-to-pypi.yml` & `grizli-1.8.7/.github/workflows/publish-to-pypi.yml`

 * *Files 14% similar despite different names*

```diff
@@ -10,30 +10,30 @@
   workflow_dispatch:
 
 env:
   CIBW_SKIP: pp*  # only build CPython wheels
   CIBW_ARCHS: auto64 # don't bother with 32bit wheels
 
 jobs:
-  build_wheels:
-    name: wheels on ${{ matrix.os }}
-    runs-on: ${{ matrix.os }}
-    strategy:
-      matrix:
-        os: [ubuntu-latest, macos-latest]
-    steps:
-      - name: Checkout code
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Build wheels
-        uses: pypa/cibuildwheel@v2.11.2
-      - uses: actions/upload-artifact@v3
-        with:
-          path: ./wheelhouse/*.whl
+  # build_wheels:
+  #   name: wheels on ${{ matrix.os }}
+  #   runs-on: ${{ matrix.os }}
+  #   strategy:
+  #     matrix:
+  #       os: [ubuntu-latest, macos-latest]
+  #   steps:
+  #     - name: Checkout code
+  #       uses: actions/checkout@v3
+  #       with:
+  #         fetch-depth: 0
+  #     - name: Build wheels
+  #       uses: pypa/cibuildwheel@v2.11.2
+  #     - uses: actions/upload-artifact@v3
+  #       with:
+  #         path: ./wheelhouse/*.whl
 
   build_sdist:
     name: source distribution
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v3
@@ -45,15 +45,16 @@
           python -m build --sdist
       - uses: actions/upload-artifact@v3
         with:
           path: dist/*.tar.gz
 
   upload_pypi:
     name: upload to PyPI
-    needs: [build_wheels, build_sdist]
+    #needs: [build_wheels, build_sdist]
+    needs: [build_sdist]
     runs-on: ubuntu-latest
     if: github.event_name == 'push' &&
         github.event.ref_type == 'tag' &&
         github.ref == 'refs/heads/${{ github.event.repository.default_branch }}'
     steps:
       - uses: actions/download-artifact@v3
         with:
```

### Comparing `grizli-1.8.5/.github/workflows/python-package-ero.yml` & `grizli-1.8.7/.github/workflows/python-package-ero.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/.github/workflows/python-package-with-jwst.yml` & `grizli-1.8.7/.github/workflows/python-package-with-jwst.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/.github/workflows/python-package.yml` & `grizli-1.8.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/.gitignore` & `grizli-1.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/.readthedocs.yml` & `grizli-1.8.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/.travis.yml` & `grizli-1.8.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/CHANGES.rst` & `grizli-1.8.7/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/CITATION.cff` & `grizli-1.8.7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/LICENSE.txt` & `grizli-1.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/PKG-INFO` & `grizli-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizli
-Version: 1.8.5
+Version: 1.8.7
 Summary: Grism redshift and line analysis software
 Home-page: https://github.com/gbrammer/grizli
 Author: G. Brammer
 Author-email: gbrammer@gmail.com
 License: MIT
 Project-URL: Documentation, https://grizli.readthedocs.io/
 Project-URL: Source, https://github.com/gbrammer/grizli
```

### Comparing `grizli-1.8.5/README.rst` & `grizli-1.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/Makefile` & `grizli-1.8.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/_static/grizli.ico` & `grizli-1.8.7/docs/_static/grizli.ico`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/_static/grizli_favico.png` & `grizli-1.8.7/docs/_static/grizli_favico.png`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/_static/grizli_favico_large.png` & `grizli-1.8.7/docs/_static/grizli_favico_large.png`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/_static/grizli_logo.pdf` & `grizli-1.8.7/docs/_static/grizli_logo.pdf`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/_static/grizli_logo.png` & `grizli-1.8.7/docs/_static/grizli_logo.png`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/conf.py` & `grizli-1.8.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/grizli/ceers-sm.field.jpg` & `grizli-1.8.7/docs/grizli/ceers-sm.field.jpg`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/grizli/image-release-v6.md` & `grizli-1.8.7/docs/grizli/image-release-v6.md`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/grizli/image-release-v6.rst` & `grizli-1.8.7/docs/grizli/image-release-v6.rst`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/grizli/index.rst` & `grizli-1.8.7/docs/grizli/index.rst`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/grizli/install.rst` & `grizli-1.8.7/docs/grizli/install.rst`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/grizli/prep.rst` & `grizli-1.8.7/docs/grizli/prep.rst`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/grizli-for-dummies.rst` & `grizli-1.8.7/docs/grizli-for-dummies.rst`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/index.rst` & `grizli-1.8.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/docs/make.bat` & `grizli-1.8.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/examples/demo.py` & `grizli-1.8.7/examples/demo.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/examples/grizli_demo_0.pdf` & `grizli-1.8.7/examples/grizli_demo_0.pdf`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/examples/grizli_demo_1.pdf` & `grizli-1.8.7/examples/grizli_demo_1.pdf`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/examples/grizli_logo.pdf` & `grizli-1.8.7/examples/grizli_logo.pdf`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/examples/grizli_logo.png` & `grizli-1.8.7/examples/grizli_logo.png`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/__init__.py` & `grizli-1.8.7/grizli/__init__.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/aws/aws_drizzler.py` & `grizli-1.8.7/grizli/aws/aws_drizzler.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/aws/db.py` & `grizli-1.8.7/grizli/aws/db.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/aws/field_tiles.py` & `grizli-1.8.7/grizli/aws/field_tiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,15 +411,15 @@
                     rgb_min=-0.018)
 
         plt.close('all')
     
     # All NIRCam
     if (len(glob.glob(f'{root}*.ncrgb.png')) == 0) & make_combinations:
         filters = ['f444w-clear','f277w-clear']
-        for f in ['f090w-clear','f115w-clear','f150w-clear']:
+        for f in ['f115w-clear','f090w-clear','f150w-clear']:
             if f in all_filters:
                 filters.append(f)
                 break
             
         split_tiles(root, ref_tile=ref_tile, 
                     filters=filters,
                     zoom_levels=zoom_levels,
@@ -659,15 +659,20 @@
         print(f'No images found, set status=4 in `combined_tiles` for {field} {tile}')
         
         return 4
     
     if make_catalog:
         import golfir.catalog
         
-        golfir.catalog.make_charge_detection(root, ext='ir')
+        golfir.catalog.make_charge_detection(root, ext='ir',
+                        filters=['f160w', 'f140w', 'f125w', 'f110w', 'f105w',
+                                 'f814w', 'f850lp',
+                                 'f277w-clear','f356w-clear','f444w-clear'],
+                                 use_hst_kernel=False,
+                                 subtract_background=True)
     
         phot = auto_script.multiband_catalog(field_root=root) #, **phot_kwargs)
     
         if len(phot) == 0:
             # Empty catalog
             db.execute(f"update combined_tiles set status=10 where tile = '{tile}' AND field = '{field}'")
         
@@ -752,15 +757,29 @@
         for c in ['xmin','xmax','ymin','ymax']:
             if c+'pix' in phot.colnames:
                 phot.rename_column(c+'pix', c)
     
         golfir.catalog.switch_segments(seg[0].data, phot, ids['id'][idx])
         pyfits.writeto(f'{root}-ir_seg.fits', data=seg[0].data, 
                        header=seg[0].header, overwrite=True)
-    
+        
+        # zip and copy
+        drz_files = glob.glob(f'{root}-ir_dr*fits')
+        drz_files += glob.glob(f'{root}*seg.fits')
+        drz_files.sort()
+        
+        for file in drz_files:
+            cmd = f'gzip --force {file}'
+            print(cmd)
+            os.system(cmd)
+        
+        os.system(f'aws s3 sync ./ s3://grizli-v2/ClusterTiles/{field}/' + 
+                  f' --exclude "*" --include "{root}*gz" --include "{root}_phot.fits"'
+                  ' --acl public-read')
+        
     if make_tile_images:
         ### Make subtiles
         ref_tiles = {'cos': (16,16), 
                      'uds': (11, 10),
                      'abell2744': (8, 8), 
                      'egs': (10,14),
                      'gds': (9,9), 
@@ -853,15 +872,15 @@
     if len(all_tiles) == 0:
         return None, None
     
     tile, field = all_tiles[np.random.randint(0, len(all_tiles))]
     return tile, field
 
 
-def run_one(own_directory=True, **kwargs):
+def run_one(own_directory=True, rgb_only=True, make_catalog=True, **kwargs):
     """
     Run a single random visit
     """
     import os
     import time
     from grizli.aws import db
 
@@ -885,15 +904,17 @@
             path = os.path.join(HOME, f'{field}-{tile}')
             if not os.path.exists(path):
                 os.makedirs(path)
                 
             os.chdir(path)
             
         #process_visit(tile, clean=clean, sync=sync)
-        process_tile(tile=tile, field=field, **kwargs)
+        process_tile(tile=tile, field=field, rgb_only=rgb_only, 
+                     make_catalog=make_catalog,
+                     **kwargs)
 
 
 def get_random_tile_filter():
     """
     Find a visit that needs processing
     """
     from grizli.aws import db
```

### Comparing `grizli-1.8.5/grizli/aws/fit_redshift_lambda.py` & `grizli-1.8.7/grizli/aws/fit_redshift_lambda.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/aws/lambda_handler.py` & `grizli-1.8.7/grizli/aws/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/aws/tile_mosaic.py` & `grizli-1.8.7/grizli/aws/tile_mosaic.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/aws/visit_processor.py` & `grizli-1.8.7/grizli/aws/visit_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -680,22 +680,23 @@
                       FROM assoc_table ORDER BY modtime DESC LIMIT {limit}""")
     
     time = astropy.time.Time(last['modtime'], format='mjd')
     last['iso'] = time.iso
     return last
 
 
-def launch_ec2_instances(nmax=50, count=None, templ='lt-0e8c2b8611c9029eb,Version=24'):
+def launch_ec2_instances(nmax=50, count=None, templ='lt-0e8c2b8611c9029eb,Version=33'):
     """
     Launch EC2 instances from a launch template that run through all 
     status=0 associations/tiles and then terminate
     
     Version 19 is the latest run_all_visits.sh
     Version 20 is the latest run_all_tiles.sh
     Version 24 is run_all_visits with a new python39 environment
+    Version 33 includes libglvnd-glx dependency for libGL
     """
 
     if count is None:
         assoc = db.SQL("""SELECT distinct(assoc_name)
                       FROM assoc_table
                       WHERE status = 0""")
     
@@ -1190,15 +1191,15 @@
     
     return fig, atab
     
 
 ALL_FILTERS = ['F410M', 'F467M', 'F547M', 'F550M', 'F621M', 'F689M', 'F763M', 'F845M', 'F200LP', 'F350LP', 'F435W', 'F438W', 'F439W', 'F450W', 'F475W', 'F475X', 'F555W', 'F569W', 'F600LP', 'F606W', 'F622W', 'F625W', 'F675W', 'F702W', 'F775W', 'F791W', 'F814W', 'F850LP', 'G800L', 'F098M', 'F127M', 'F139M', 'F153M', 'F105W', 'F110W', 'F125W', 'F140W', 'F160W', 'G102', 'G141']
 
 
-def process_visit(assoc, clean=True, sync=True, max_dt=4, combine_same_pa=False, visit_split_shift=1.2, blue_align_params=blue_align_params, ref_catalogs=['LS_DR9', 'PS1', 'DES', 'NSC', 'GAIA'], filters=None, prep_args={}, fetch_args={}, get_wcs_guess_from_table=True, master_radec='astrometry_db', align_guess=None, with_db=True, global_miri_skyflat=None, **kwargs):
+def process_visit(assoc, clean=True, sync=True, max_dt=4, combine_same_pa=False, visit_split_shift=1.2, blue_align_params=blue_align_params, ref_catalogs=['LS_DR9', 'PS1', 'DES', 'NSC', 'GAIA'], filters=None, prep_args={}, fetch_args={}, get_wcs_guess_from_table=True, master_radec='astrometry_db', align_guess=None, with_db=True, global_miri_skyflat=None, tab=None, **kwargs):
     """
     Run the `grizli.pipeline.auto_script.go` pipeline on an association defined
     in the `grizli` database.
     
     Parameters
     ----------
     assoc : str
@@ -1228,14 +1229,18 @@
     align_guess : [float, float]
         Shift guess (not used)
     
     with_db : bool
         Try to use the `grizli` archive.  Otherwise, get the assoc information
         from the web API
     
+    tab : `~astropy.table.Table`
+        Manually specify the datasets to process as an association.  Needs to be some 
+        result like ``SELECT * FROM assoc_table WHERE ...``.
+    
     `assoc_table.status`
     
      1 = start
      2 = finished
      9 = has failed files
     10 = no wcs.log files found, so probably nothing was done?
          This is most often the case when HST visits were ignored due to 
@@ -1249,22 +1254,26 @@
     import glob
     
     from grizli.pipeline import auto_script
     from grizli import utils, prep
 
     os.chdir(f'{ROOT_PATH}/')
     
-    if with_db:
-        tab = db.SQL(f"""SELECT * FROM assoc_table
-                     WHERE assoc_name='{assoc}'
-                     AND status != 99
-                     """)
+    if tab is None:
+        if with_db:
+            tab = db.SQL(f"""SELECT * FROM assoc_table
+                         WHERE assoc_name='{assoc}'
+                         AND status != 99
+                         """)
+        else:
+            _url = f'http://grizli-cutout.herokuapp.com/assoc_json?name={assoc}'
+            tab = utils.read_catalog(_url, format='pandas.json')
+            sync = False
+            get_wcs_guess_from_table = False
     else:
-        _url = f'http://grizli-cutout.herokuapp.com/assoc_json?name={assoc}'
-        tab = utils.read_catalog(_url, format='pandas.json')
         sync = False
         get_wcs_guess_from_table = False
         
     if len(tab) == 0:
         print(f"assoc_name='{assoc}' not found in assoc_table")
         return False
         
@@ -1431,15 +1440,18 @@
     
     os.environ['iref'] = f'{os.getcwd()}/{assoc}/iref/'
     os.environ['jref'] = f'{os.getcwd()}/{assoc}/jref/'
     
     is_jwst = False
     for f in ['f090w','f115w','f150w','f200w','f277w','f356w','f444w',
               'f182m','f140m','f210m','f410m','f430m','f460m','f300m',
-              'f250m','f480m']:
+              'f250m','f480m'
+              'f560w','f770w','f1000w','f1280w',
+              'f1500w','f1800w','f2100w',
+              ]:
         if f in assoc:
             is_jwst = True
             break
     
     if not is_jwst:        
         utils.fetch_default_calibs()
```

### Comparing `grizli-1.8.5/grizli/catalog.py` & `grizli-1.8.7/grizli/catalog.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/combine.py` & `grizli-1.8.7/grizli/combine.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/auto_script_defaults.yml` & `grizli-1.8.7/grizli/data/auto_script_defaults.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/gaia_dr2_vizier_columns.txt` & `grizli-1.8.7/grizli/data/gaia_dr2_vizier_columns.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/hst_encircled_energy.fits` & `grizli-1.8.7/grizli/data/hst_encircled_energy.fits`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/jwst_bp_info.yml` & `grizli-1.8.7/grizli/data/jwst_bp_info.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nircam_wisp.yml` & `grizli-1.8.7/grizli/data/nircam_wisp.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_badpix_230120_NRCALONG.fits.gz` & `grizli-1.8.7/grizli/data/nrc_badpix_230120_NRCALONG.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_badpix_230120_NRCBLONG.fits.gz` & `grizli-1.8.7/grizli/data/nrc_badpix_230120_NRCBLONG.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCA1.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCA1.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCA2.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCA2.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCA3.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCA3.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCA4.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCA4.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCALONG.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCALONG.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCB1.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCB1.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCB2.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCB2.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCB3.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCB3.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCB4.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCB4.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/nrc_lowpix_0916_NRCBLONG.fits.gz` & `grizli-1.8.7/grizli/data/nrc_lowpix_0916_NRCBLONG.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/photom_correction.yml` & `grizli-1.8.7/grizli/data/photom_correction.yml`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/sep_catalog_junk.pkl` & `grizli-1.8.7/grizli/data/sep_catalog_junk.pkl`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/FeII_VeronCetty2004.txt` & `grizli-1.8.7/grizli/data/templates/FeII_VeronCetty2004.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/README` & `grizli-1.8.7/grizli/data/templates/README`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/alf_SSP.dat` & `grizli-1.8.7/grizli/data/templates/alf_SSP.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/cvd12_t11_solar_Chabrier.dat` & `grizli-1.8.7/grizli/data/templates/cvd12_t11_solar_Chabrier.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/eazy_intermediate.dat` & `grizli-1.8.7/grizli/data/templates/eazy_intermediate.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/erb2010.dat` & `grizli-1.8.7/grizli/data/templates/erb2010.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/erb2010_continuum.dat` & `grizli-1.8.7/grizli/data/templates/erb2010_continuum.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3.param` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3.param`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3.param.fits` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3.param.fits`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_001.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_001.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_002.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_002.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_003.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_003.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_004.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_004.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_005.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_005.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_006.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_006.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_007.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_007.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_008.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_008.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_009.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_009.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_010.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_010.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_011.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_011.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_012.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_012.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines.param` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines.param`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_001.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_001.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_002.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_002.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_003.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_003.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_004.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_004.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_005.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_005.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_006.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_006.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_007.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_007.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_008.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_008.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_009.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_009.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_010.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_010.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_011.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_011.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_012.dat` & `grizli-1.8.7/grizli/data/templates/fsps/fsps_QSF_12_v3_nolines_012.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/fsps_starburst_lines.txt` & `grizli-1.8.7/grizli/data/templates/fsps_starburst_lines.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/post_starburst.dat` & `grizli-1.8.7/grizli/data/templates/post_starburst.dat`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/quasar_lines.txt` & `grizli-1.8.7/grizli/data/templates/quasar_lines.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/red_blue_continuum.txt` & `grizli-1.8.7/grizli/data/templates/red_blue_continuum.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/red_blue_continuum_noLya.txt` & `grizli-1.8.7/grizli/data/templates/red_blue_continuum_noLya.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/L1.0.txt` & `grizli-1.8.7/grizli/data/templates/stars/L1.0.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/L3.5.txt` & `grizli-1.8.7/grizli/data/templates/stars/L3.5.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/L6.0.txt` & `grizli-1.8.7/grizli/data/templates/stars/L6.0.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/M6.5.txt` & `grizli-1.8.7/grizli/data/templates/stars/M6.5.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/M8.0.txt` & `grizli-1.8.7/grizli/data/templates/stars/M8.0.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/T2.0.txt` & `grizli-1.8.7/grizli/data/templates/stars/T2.0.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/T6.0.txt` & `grizli-1.8.7/grizli/data/templates/stars/T6.0.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/T7.5.txt` & `grizli-1.8.7/grizli/data/templates/stars/T7.5.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/bt-settl_t400-3500_z0.0.fits` & `grizli-1.8.7/grizli/data/templates/stars/bt-settl_t400-3500_z0.0.fits`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/templates/stars/carbon_star.txt` & `grizli-1.8.7/grizli/data/templates/stars/carbon_star.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/visit_alignment.txt` & `grizli-1.8.7/grizli/data/visit_alignment.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/wfc3ir_badpix_spars200_22.03.31.fits.gz` & `grizli-1.8.7/grizli/data/wfc3ir_badpix_spars200_22.03.31.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/wfc3ir_dark_badpix_2019.01.12.fits.gz` & `grizli-1.8.7/grizli/data/wfc3ir_dark_badpix_2019.01.12.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/data/wfc3ir_ee.txt` & `grizli-1.8.7/grizli/data/wfc3ir_ee.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/ds9.py` & `grizli-1.8.7/grizli/ds9.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/fake_image.py` & `grizli-1.8.7/grizli/fake_image.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/fitting.py` & `grizli-1.8.7/grizli/fitting.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/galfit/deconvolve.py` & `grizli-1.8.7/grizli/galfit/deconvolve.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/galfit/galfit.py` & `grizli-1.8.7/grizli/galfit/galfit.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/galfit/gfutils.py` & `grizli-1.8.7/grizli/galfit/gfutils.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/galfit/psf.py` & `grizli-1.8.7/grizli/galfit/psf.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/grismconf.py` & `grizli-1.8.7/grizli/grismconf.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/jwst_level1.py` & `grizli-1.8.7/grizli/jwst_level1.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/jwst_utils.py` & `grizli-1.8.7/grizli/jwst_utils.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/model.py` & `grizli-1.8.7/grizli/model.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/multifit.py` & `grizli-1.8.7/grizli/multifit.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/nbutils.py` & `grizli-1.8.7/grizli/nbutils.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/pipeline/__init__.py` & `grizli-1.8.7/grizli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/pipeline/auto_script.py` & `grizli-1.8.7/grizli/pipeline/auto_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         prep.table_to_radec(gaia[gaia['valid']], f'{root}.gaia.radec')
         prep.table_to_regions(gaia[gaia['valid']], f'{root}.gaia.reg')
         
         if gaia['valid'].sum() > min_gaia_count:
             preprocess_args['master_radec'] = os.path.join(PATHS['home'],
                                                   f'{root}.gaia.radec')
             
-            preprocess_args['align_mag_limits'] = gaia_mag_limits
+            visit_prep_args['align_mag_limits'] = gaia_mag_limits
             
             msg = f"{root} : Use {root}.gaia.radec as master_radec"
             msg += f"\n{root} : Set align_mag_limits={gaia_mag_limits}"
             utils.log_comment(utils.LOGFILE, msg, show_date=False,
                               verbose=True)
         
     except:
```

### Comparing `grizli-1.8.5/grizli/pipeline/default_params.py` & `grizli-1.8.7/grizli/pipeline/default_params.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/pipeline/photoz.py` & `grizli-1.8.7/grizli/pipeline/photoz.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
         cat.write('{0}_phot{1}.fits'.format(root, suffix), overwrite=True)
 
     return cat
 
 FILTER_TRANS = {'f098m': 201, 'f105w': 202, 'f110w': 241, 'f125w': 203, 'f140w': 204, 'f160w': 205, 'f435w': 233, 'f475w': 234, 'f555w': 235, 'f606w': 236, 'f625w': 237, 'f775w': 238, 'f814w': 239, 'f850lp': 240, 'f702w': 15, 'f600lpu': 243, 'f225wu': 207, 'f275wu': 208, 'f336wu': 209, 'f350lpu': 339, 'f438wu': 211, 'f475wu': 212, 'f475xu': 242, 'f555wu': 213, 'f606wu': 214, 'f625wu': 215, 'f775wu': 216, 'f814wu': 217, 'f390wu': 210, 'ch1': 18, 'ch2': 19, 'f336w':209, 'f350lp':339, 'f115w': 309, 'f150w': 310, 'f200w': 311}
     
-def eazy_photoz(root, force=False, object_only=True, apply_background=True, aper_ix=1, apply_prior=False, beta_prior=True, get_external_photometry=False, external_limits=3, external_sys_err=0.3, external_timeout=300, sys_err=0.05, z_step=0.01, z_min=0.01, z_max=12, total_flux='flux_auto', auto_corr=True, compute_residuals=False, dummy_prior=False, extra_rf_filters=[], quiet=True, aperture_indices='all', zpfile='zphot.zeropoint', extra_params={}, filter_trans=FILTER_TRANS, extra_translate={}, force_apcorr=False, ebv=None, absmag_filters=[],  **kwargs):
+def eazy_photoz(root, force=False, object_only=True, apply_background=True, aper_ix=1, apply_prior=False, beta_prior=True, get_external_photometry=False, external_limits=3, external_sys_err=0.3, external_timeout=300, sys_err=0.05, z_step=0.01, z_min=0.01, z_max=12, total_flux='flux_auto', auto_corr=True, compute_residuals=False, dummy_prior=False, extra_rf_filters=[], quiet=True, aperture_indices='all', zpfile='zphot.zeropoint', extra_params={}, filter_trans=FILTER_TRANS, extra_translate={}, force_apcorr=False, ebv=None, absmag_filters=[], save_pickle=False, **kwargs):
 
     import os
     import eazy
     import numpy as np
 
     from grizli import utils
     import mastquery.utils
@@ -417,15 +417,16 @@
     
     self.standard_output(prior=apply_prior, beta_prior=beta_prior, 
                          extra_rf_filters=extra_rf_filters,
                          absmag_filters=absmag_filters)
 
     zout = utils.read_catalog('{0}.eazypy.zout.fits'.format(root))
 
-    np.save('{0}.eazypy.self.npy'.format(root), [self])
+    if save_pickle:
+        np.save('{0}.eazypy.self.npy'.format(root), [self])
 
     return self, cat, zout
 
 
 def show_from_ds9(ds9, self, zout, use_sky=True, **kwargs):
 
     import numpy as np
```

### Comparing `grizli-1.8.5/grizli/pipeline/reprocess.py` & `grizli-1.8.7/grizli/pipeline/reprocess.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/pipeline/run_MPI.py` & `grizli-1.8.7/grizli/pipeline/run_MPI.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/pipeline/summary.py` & `grizli-1.8.7/grizli/pipeline/summary.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/prep.py` & `grizli-1.8.7/grizli/prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,15 +737,15 @@
         if inliers.sum() > 2:
             m_i, in_i = ransac((input[input_ix[inliers], :], 
                                 output[output_ix[inliers], :]),
                                    transform, min_samples=3,
                                    residual_threshold=3, max_trials=100)
             if in_i.sum() > 2:
                 model = m_i
-                inliers[np.arange(len(inliers), dtype=np.int)[inliers][in_i]] = False
+                inliers[np.arange(len(inliers), dtype=np.int32)[inliers][in_i]] = False
 
         outliers = ~inliers
         mout = model(input[input_ix, :])
         dx = mout - output[output_ix]
 
     else:
         model = tf
```

### Comparing `grizli-1.8.5/grizli/stack.py` & `grizli-1.8.7/grizli/stack.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/fit_args.npy` & `grizli-1.8.7/grizli/tests/data/fit_args.npy`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/j033216m2743_00152.beams.fits` & `grizli-1.8.7/grizli/tests/data/j033216m2743_00152.beams.fits`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/jwst-headers/det_image_seq1_MIRIMAGE_F560Wexp1_cal.fits.gz` & `grizli-1.8.7/grizli/tests/data/jwst-headers/det_image_seq1_MIRIMAGE_F560Wexp1_cal.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca1_rate.fits.gz` & `grizli-1.8.7/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca1_rate.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca2_rate.fits.gz` & `grizli-1.8.7/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca2_rate.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca5_uncal_dispersed_GRISMR_crossing_F356W_rate.fits.gz` & `grizli-1.8.7/grizli/tests/data/jwst-headers/jw42424001001_01101_00001_nrca5_uncal_dispersed_GRISMR_crossing_F356W_rate.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/jwst-headers/jw42424001001_01105_00002_nrca5_rate.fits.gz` & `grizli-1.8.7/grizli/tests/data/jwst-headers/jw42424001001_01105_00002_nrca5_rate.fits.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/jwst-headers/strip_data.py` & `grizli-1.8.7/grizli/tests/data/jwst-headers/strip_data.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/niriss_jw01324001001_test.beams.fits` & `grizli-1.8.7/grizli/tests/data/niriss_jw01324001001_test.beams.fits`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/data/wfc3-parse-test.tar.gz` & `grizli-1.8.7/grizli/tests/data/wfc3-parse-test.tar.gz`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/test_autoscript.py` & `grizli-1.8.7/grizli/tests/test_autoscript.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/test_cutils.py` & `grizli-1.8.7/grizli/tests/test_cutils.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/test_fits.py` & `grizli-1.8.7/grizli/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/test_grismconf.py` & `grizli-1.8.7/grizli/tests/test_grismconf.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/test_jwst.py` & `grizli-1.8.7/grizli/tests/test_jwst.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/tests/test_utils.py` & `grizli-1.8.7/grizli/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/utils.py` & `grizli-1.8.7/grizli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18036,566 +18036,607 @@
 00046730: 2020 2073 656c 662e 696e 6469 6365 7320     self.indices 
 00046740: 3d20 5f5b 315d 0a20 2020 2020 2020 2073  = _[1].        s
 00046750: 656c 662e 636f 756e 7473 203d 205f 5b32  elf.counts = _[2
 00046760: 5d0a 2020 2020 2020 2020 6966 2076 6572  ].        if ver
 00046770: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
 00046780: 2020 7365 6c66 2e69 6e66 6f28 736f 7274    self.info(sort
 00046790: 5f63 6f75 6e74 733d 7665 7262 6f73 6529  _counts=verbose)
-000467a0: 0a20 2020 200a 2020 2020 4070 726f 7065  .    .    @prope
-000467b0: 7274 790a 2020 2020 6465 6620 4e28 7365  rty.    def N(se
-000467c0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000467d0: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
-000467e0: 6f66 2075 6e69 7175 6520 6060 7661 6c75  of unique ``valu
-000467f0: 6573 6060 0a20 2020 2020 2020 2022 2222  es``.        """
-00046800: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00046810: 6c65 6e28 7365 6c66 2e76 616c 7565 7329  len(self.values)
-00046820: 0a0a 0a20 2020 2064 6566 2069 6e66 6f28  ...    def info(
-00046830: 7365 6c66 2c20 736f 7274 5f63 6f75 6e74  self, sort_count
-00046840: 733d 2d31 293a 0a20 2020 2020 2020 2022  s=-1):.        "
-00046850: 2222 0a20 2020 2020 2020 2050 7269 6e74  "".        Print
-00046860: 2061 2073 756d 6d61 7279 0a20 2020 2020   a summary.     
-00046870: 2020 2022 2222 0a20 2020 2020 2020 2070     """.        p
-00046880: 7269 6e74 2866 277b 224e 223a 3e34 7d20  rint(f'{"N":>4} 
-00046890: 207b 2276 616c 7565 223a 3130 7d27 290a   {"value":10}').
-000468a0: 2020 2020 2020 2020 7072 696e 7428 273d          print('=
-000468b0: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d27  ===  =========='
-000468c0: 290a 2020 2020 2020 2020 6966 2073 6f72  ).        if sor
-000468d0: 745f 636f 756e 7473 3a0a 2020 2020 2020  t_counts:.      
-000468e0: 2020 2020 2020 736f 203d 206e 702e 6172        so = np.ar
-000468f0: 6773 6f72 7428 7365 6c66 2e63 6f75 6e74  gsort(self.count
-00046900: 7329 5b3a 3a69 6e74 2873 6f72 745f 636f  s)[::int(sort_co
-00046910: 756e 7473 295d 0a20 2020 2020 2020 2065  unts)].        e
-00046920: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00046930: 2073 6f20 3d20 6e70 2e61 7261 6e67 6528   so = np.arange(
-00046940: 7365 6c66 2e4e 290a 2020 2020 2020 2020  self.N).        
-00046950: 2020 2020 0a20 2020 2020 2020 2066 6f72      .        for
-00046960: 2069 2069 6e20 736f 3a0a 2020 2020 2020   i in so:.      
-00046970: 2020 2020 2020 762c 2063 203d 2073 656c        v, c = sel
-00046980: 662e 7661 6c75 6573 5b69 5d2c 2073 656c  f.values[i], sel
-00046990: 662e 636f 756e 7473 5b69 5d0a 2020 2020  f.counts[i].    
-000469a0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-000469b0: 7b63 3a3e 347d 2020 7b76 3a31 307d 2729  {c:>4}  {v:10}')
-000469c0: 0a0a 0a20 2020 2064 6566 2063 6f75 6e74  ...    def count
-000469d0: 2873 656c 662c 206b 6579 293a 0a20 2020  (self, key):.   
-000469e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000469f0: 2047 6574 206f 6363 7572 7265 6e63 6573   Get occurrences
-00046a00: 2063 6f75 6e74 206f 6620 6120 7061 7274   count of a part
-00046a10: 6963 756c 6172 2060 6076 616c 7565 6060  icular ``value``
-00046a20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00046a30: 2020 2020 2069 6620 6b65 7920 696e 2073       if key in s
-00046a40: 656c 662e 7661 6c75 6573 3a0a 2020 2020  elf.values:.    
-00046a50: 2020 2020 2020 2020 6978 203d 2073 656c          ix = sel
-00046a60: 662e 7661 6c75 6573 2e69 6e64 6578 286b  f.values.index(k
-00046a70: 6579 290a 2020 2020 2020 2020 2020 2020  ey).            
-00046a80: 7265 7475 726e 2073 656c 662e 636f 756e  return self.coun
-00046a90: 7473 5b69 785d 0a20 2020 2020 2020 2065  ts[ix].        e
-00046aa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00046ab0: 2072 6574 7572 6e20 300a 0a0a 2020 2020   return 0...    
-00046ac0: 6465 6620 5f5f 6974 6572 5f5f 2873 656c  def __iter__(sel
-00046ad0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00046ae0: 2020 2020 2020 2020 4974 6572 6162 6c65          Iterable
-00046af0: 206f 7665 7220 6076 616c 7565 7360 2061   over `values` a
-00046b00: 7474 7269 6275 7465 0a20 2020 2020 2020  ttribute.       
-00046b10: 200a 2020 2020 2020 2020 5265 7475 726e   .        Return
-00046b20: 7320 6120 7475 706c 6520 6f66 2074 6865  s a tuple of the
-00046b30: 2076 616c 7565 2061 6e64 2074 6865 2062   value and the b
-00046b40: 6f6f 6c65 616e 2073 656c 6563 7469 6f6e  oolean selection
-00046b50: 2061 7272 6179 2066 6f72 2074 6861 7420   array for that 
-00046b60: 0a20 2020 2020 2020 2076 616c 7565 2e0a  .        value..
-00046b70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00046b80: 2020 2020 6920 3d20 300a 2020 2020 2020      i = 0.      
-00046b90: 2020 7768 696c 6520 6920 3c20 7365 6c66    while i < self
-00046ba0: 2e4e 3a0a 2020 2020 2020 2020 2020 2020  .N:.            
-00046bb0: 7669 203d 2073 656c 662e 7661 6c75 6573  vi = self.values
-00046bc0: 5b69 5d0a 2020 2020 2020 2020 2020 2020  [i].            
-00046bd0: 7969 656c 6420 2876 692c 2073 656c 665b  yield (vi, self[
-00046be0: 7669 5d29 0a20 2020 2020 2020 2020 2020  vi]).           
-00046bf0: 2069 202b 3d20 310a 0a0a 2020 2020 6465   i += 1...    de
-00046c00: 6620 5f5f 6765 7469 7465 6d5f 5f28 7365  f __getitem__(se
-00046c10: 6c66 2c20 6b65 7929 3a0a 2020 2020 2020  lf, key):.      
-00046c20: 2020 6966 206b 6579 2069 6e20 7365 6c66    if key in self
-00046c30: 2e76 616c 7565 733a 0a20 2020 2020 2020  .values:.       
-00046c40: 2020 2020 2069 7820 3d20 7365 6c66 2e76       ix = self.v
-00046c50: 616c 7565 732e 696e 6465 7828 6b65 7929  alues.index(key)
-00046c60: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-00046c70: 7420 3d20 7365 6c66 2e69 6e64 6963 6573  t = self.indices
-00046c80: 203d 3d20 6978 0a20 2020 2020 2020 2020   == ix.         
-00046c90: 2020 2072 6574 7572 6e20 7465 7374 0a20     return test. 
-00046ca0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00046cb0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00046cc0: 7365 6c66 2e7a 6572 6f73 0a0a 0a20 2020  self.zeros...   
-00046cd0: 2023 2064 6566 205f 5f69 7465 725f 5f28   # def __iter__(
-00046ce0: 7365 6c66 293a 0a20 2020 2023 2020 2020  self):.    #    
-00046cf0: 2066 6f72 2069 6478 2069 6e20 6974 6572   for idx in iter
-00046d00: 746f 6f6c 732e 636f 756e 7428 293a 0a20  tools.count():. 
-00046d10: 2020 2023 2020 2020 2020 2020 2074 7279     #         try
-00046d20: 3a0a 2020 2020 2320 2020 2020 2020 2020  :.    #         
-00046d30: 2020 2020 7969 656c 6420 7365 6c66 2e76      yield self.v
-00046d40: 616c 7565 735b 6964 785d 0a20 2020 2023  alues[idx].    #
-00046d50: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00046d60: 496e 6465 7845 7272 6f72 3a0a 2020 2020  IndexError:.    
-00046d70: 2320 2020 2020 2020 2020 2020 2020 6272  #             br
-00046d80: 6561 6b0a 0a20 2020 2064 6566 205f 5f6c  eak..    def __l
-00046d90: 656e 5f5f 2873 656c 6629 3a0a 2020 2020  en__(self):.    
-00046da0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00046db0: 4e0a 0a0a 636c 6173 7320 4875 6262 6c65  N...class Hubble
-00046dc0: 5859 5a28 6f62 6a65 6374 293a 0a20 2020  XYZ(object):.   
-00046dd0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00046de0: 6c66 2c20 7370 745f 6669 6c65 3d27 272c  lf, spt_file='',
-00046df0: 2070 6172 616d 5f64 6963 743d 7b7d 293a   param_dict={}):
-00046e00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00046e10: 2020 2020 2048 656c 7065 7220 746f 2063       Helper to c
-00046e20: 6f6d 7075 7465 2048 5354 2067 656f 6365  ompute HST geoce
-00046e30: 6e74 7269 6320 636f 6f72 6469 6e61 7465  ntric coordinate
-00046e40: 7320 6672 6f6d 206f 7262 6974 616c 2070  s from orbital p
-00046e50: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00046e60: 2020 0a20 2020 2020 2020 2028 7465 7374    .        (test
-00046e70: 696e 6729 0a20 2020 2020 2020 200a 2020  ing).        .  
-00046e80: 2020 2020 2020 4261 7365 6420 6f6e 2068        Based on h
-00046e90: 7474 703a 2f2f 6172 7469 636c 6573 2e61  ttp://articles.a
-00046ea0: 6473 6162 732e 6861 7276 6172 642e 6564  dsabs.harvard.ed
-00046eb0: 752f 2f66 756c 6c2f 3139 3935 4153 5043  u//full/1995ASPC
-00046ec0: 2e2e 2e37 372e 2e34 3634 412f 0a20 2020  ...77..464A/.   
-00046ed0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00046ee0: 2069 6620 7370 745f 6669 6c65 3a0a 2020   if spt_file:.  
-00046ef0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00046f00: 6172 616d 5f64 6963 7420 3d20 7365 6c66  aram_dict = self
-00046f10: 2e70 6172 7365 5f66 726f 6d5f 7370 7428  .parse_from_spt(
-00046f20: 7370 745f 6669 6c65 290a 2020 2020 2020  spt_file).      
-00046f30: 2020 0a20 2020 2020 2020 2065 6c69 6620    .        elif 
-00046f40: 7061 7261 6d5f 6469 6374 3a0a 2020 2020  param_dict:.    
-00046f50: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
-00046f60: 616d 5f64 6963 7420 3d20 7061 7261 6d5f  am_dict = param_
-00046f70: 6469 6374 0a20 2020 2020 2020 200a 2020  dict.        .  
-00046f80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00046f90: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
-00046fa0: 616d 5f64 6963 7420 3d20 7b7d 0a20 2020  am_dict = {}.   
-00046fb0: 2020 2020 200a 2020 2020 2020 2020 7365       .        se
-00046fc0: 6c66 2e63 6f6d 7075 7465 6420 3d20 7b7d  lf.computed = {}
-00046fd0: 0a0a 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00046fe0: 200a 2020 2020 6465 6620 5f74 3139 3835   .    def _t1985
-00046ff0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00047000: 2222 220a 2020 2020 2020 2020 5265 6665  """.        Refe
-00047010: 7265 6e63 6520 7469 6d65 0a20 2020 2020  rence time.     
-00047020: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00047030: 6d70 6f72 7420 6173 7472 6f70 792e 7469  mport astropy.ti
-00047040: 6d65 0a20 2020 2020 2020 2074 3020 3d20  me.        t0 = 
-00047050: 6173 7472 6f70 792e 7469 6d65 2e54 696d  astropy.time.Tim
-00047060: 6528 2731 3938 352d 3031 2d30 3154 3030  e('1985-01-01T00
-00047070: 3a30 303a 3030 5a27 290a 2020 2020 2020  :00:00Z').      
-00047080: 2020 7265 7475 726e 2074 300a 0a0a 2020    return t0...  
-00047090: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
-000470a0: 656c 662c 2074 5f69 6e2c 202a 2a6b 7761  elf, t_in, **kwa
-000470b0: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
-000470c0: 220a 2020 2020 2020 2020 436f 6e76 6572  ".        Conver
-000470d0: 7420 696e 7075 7420 7469 6d65 2060 6074  t input time ``t
-000470e0: 5f69 6e60 6020 746f 2073 6563 6f6e 6473  _in`` to seconds
-000470f0: 2073 696e 6365 2031 2f31 2f38 3520 616e   since 1/1/85 an
-00047100: 6420 6060 6576 616c 7561 7465 6060 2e0a  d ``evaluate``..
-00047110: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00047120: 2020 2020 696d 706f 7274 2061 7374 726f      import astro
-00047130: 7079 2e74 696d 650a 2020 2020 2020 2020  py.time.        
-00047140: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-00047150: 6528 745f 696e 2c20 6173 7472 6f70 792e  e(t_in, astropy.
-00047160: 7469 6d65 2e54 696d 6529 3a0a 2020 2020  time.Time):.    
-00047170: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00047180: 6c75 6545 7272 6f72 2827 745f 696e 206d  lueError('t_in m
-00047190: 7573 7420 6265 2061 7374 726f 7079 2e74  ust be astropy.t
-000471a0: 696d 652e 5469 6d65 206f 626a 6563 7427  ime.Time object'
-000471b0: 290a 0a20 2020 2020 2020 2064 7420 3d20  )..        dt = 
-000471c0: 745f 696e 202d 2073 656c 662e 5f74 3139  t_in - self._t19
-000471d0: 3835 0a20 2020 2020 2020 2078 797a 203d  85.        xyz =
-000471e0: 2073 656c 662e 6576 616c 7561 7465 2864   self.evaluate(d
-000471f0: 742e 7365 632c 202a 2a6b 7761 7267 7329  t.sec, **kwargs)
-00047200: 0a20 2020 2020 2020 2069 6620 2761 735f  .        if 'as_
-00047210: 7461 626c 6527 2069 6e20 6b77 6172 6773  table' in kwargs
-00047220: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00047230: 206b 7761 7267 735b 2761 735f 7461 626c   kwargs['as_tabl
-00047240: 6527 5d3a 0a20 2020 2020 2020 2020 2020  e']:.           
-00047250: 2020 2020 2078 797a 5b27 7469 6d65 275d       xyz['time']
-00047260: 203d 2074 5f69 6e0a 2020 2020 2020 2020   = t_in.        
-00047270: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00047280: 2072 6574 7572 6e20 7879 7a0a 0a0a 2020   return xyz...  
-00047290: 2020 6465 6620 5f5f 6765 7469 7465 6d5f    def __getitem_
-000472a0: 5f28 7365 6c66 2c20 6b65 7929 3a0a 2020  _(self, key):.  
-000472b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000472c0: 662e 7061 7261 6d5f 6469 6374 5b6b 6579  f.param_dict[key
-000472d0: 5d0a 0a0a 2020 2020 6465 6620 6576 616c  ]...    def eval
-000472e0: 7561 7465 2873 656c 662c 2064 742c 2075  uate(self, dt, u
-000472f0: 6e69 743d 4e6f 6e65 2c20 6173 5f74 6162  nit=None, as_tab
-00047300: 6c65 3d46 616c 7365 293a 0a20 2020 2020  le=False):.     
-00047310: 2020 2022 2222 0a20 2020 2020 2020 2045     """.        E
-00047320: 7661 6c75 6174 6520 6571 7561 7469 6f6e  valuate equation
-00047330: 7320 746f 2067 6574 2070 6f73 6974 696f  s to get positio
-00047340: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
-00047350: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00047360: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00047370: 2020 2020 782c 2079 2c20 7a2c 2072 3a20      x, y, z, r: 
-00047380: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
-00047390: 2020 436f 6f72 6469 6e61 7465 732c 2069    Coordinates, i
-000473a0: 6e20 6b6d 206f 7220 6060 756e 6974 6060  n km or ``unit``
-000473b0: 2e0a 2020 2020 2020 2020 2020 2020 0a20  ..            . 
-000473c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000473d0: 2020 200a 2020 2020 2020 2020 6966 206e     .        if n
-000473e0: 6f74 2073 656c 662e 7061 7261 6d5f 6469  ot self.param_di
-000473f0: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
+000467a0: 0a20 2020 200a 2020 2020 0a20 2020 2040  .    .    .    @
+000467b0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000467c0: 204e 2873 656c 6629 3a0a 2020 2020 2020   N(self):.      
+000467d0: 2020 2222 220a 2020 2020 2020 2020 4e75    """.        Nu
+000467e0: 6d62 6572 206f 6620 756e 6971 7565 2060  mber of unique `
+000467f0: 6076 616c 7565 7360 600a 2020 2020 2020  `values``.      
+00046800: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00046810: 7475 726e 206c 656e 2873 656c 662e 7661  turn len(self.va
+00046820: 6c75 6573 290a 0a0a 2020 2020 6465 6620  lues)...    def 
+00046830: 696e 666f 2873 656c 662c 2073 6f72 745f  info(self, sort_
+00046840: 636f 756e 7473 3d2d 3129 3a0a 2020 2020  counts=-1):.    
+00046850: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00046860: 5072 696e 7420 6120 7375 6d6d 6172 790a  Print a summary.
+00046870: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00046880: 2020 2020 7072 696e 7428 6627 7b22 4e22      print(f'{"N"
+00046890: 3a3e 347d 2020 7b22 7661 6c75 6522 3a31  :>4}  {"value":1
+000468a0: 307d 2729 0a20 2020 2020 2020 2070 7269  0}').        pri
+000468b0: 6e74 2827 3d3d 3d3d 2020 3d3d 3d3d 3d3d  nt('====  ======
+000468c0: 3d3d 3d3d 2729 0a20 2020 2020 2020 2069  ====').        i
+000468d0: 6620 736f 7274 5f63 6f75 6e74 733a 0a20  f sort_counts:. 
+000468e0: 2020 2020 2020 2020 2020 2073 6f20 3d20             so = 
+000468f0: 6e70 2e61 7267 736f 7274 2873 656c 662e  np.argsort(self.
+00046900: 636f 756e 7473 295b 3a3a 696e 7428 736f  counts)[::int(so
+00046910: 7274 5f63 6f75 6e74 7329 5d0a 2020 2020  rt_counts)].    
+00046920: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00046930: 2020 2020 2020 736f 203d 206e 702e 6172        so = np.ar
+00046940: 616e 6765 2873 656c 662e 4e29 0a20 2020  ange(self.N).   
+00046950: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00046960: 2020 666f 7220 6920 696e 2073 6f3a 0a20    for i in so:. 
+00046970: 2020 2020 2020 2020 2020 2076 2c20 6320             v, c 
+00046980: 3d20 7365 6c66 2e76 616c 7565 735b 695d  = self.values[i]
+00046990: 2c20 7365 6c66 2e63 6f75 6e74 735b 695d  , self.counts[i]
+000469a0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000469b0: 6e74 2866 277b 633a 3e34 7d20 207b 763a  nt(f'{c:>4}  {v:
+000469c0: 3130 7d27 290a 0a0a 2020 2020 6465 6620  10}')...    def 
+000469d0: 636f 756e 7428 7365 6c66 2c20 6b65 7929  count(self, key)
+000469e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000469f0: 2020 2020 2020 4765 7420 6f63 6375 7272        Get occurr
+00046a00: 656e 6365 7320 636f 756e 7420 6f66 2061  ences count of a
+00046a10: 2070 6172 7469 6375 6c61 7220 6060 7661   particular ``va
+00046a20: 6c75 6560 600a 2020 2020 2020 2020 2222  lue``.        ""
+00046a30: 220a 2020 2020 2020 2020 6966 206b 6579  ".        if key
+00046a40: 2069 6e20 7365 6c66 2e76 616c 7565 733a   in self.values:
+00046a50: 0a20 2020 2020 2020 2020 2020 2069 7820  .            ix 
+00046a60: 3d20 7365 6c66 2e76 616c 7565 732e 696e  = self.values.in
+00046a70: 6465 7828 6b65 7929 0a20 2020 2020 2020  dex(key).       
+00046a80: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00046a90: 2e63 6f75 6e74 735b 6978 5d0a 2020 2020  .counts[ix].    
+00046aa0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00046ab0: 2020 2020 2020 7265 7475 726e 2030 0a20        return 0. 
+00046ac0: 2020 200a 2020 2020 0a20 2020 2040 7072     .    .    @pr
+00046ad0: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
+00046ae0: 6973 745f 696e 6469 6365 7328 7365 6c66  ist_indices(self
+00046af0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00046b00: 2020 2020 2020 2042 7569 6c64 206c 6973         Build lis
+00046b10: 7420 6f66 206c 6973 7473 206f 6620 696e  t of lists of in
+00046b20: 6469 6365 7320 7468 6174 2065 6163 6820  dices that each 
+00046b30: 756e 6971 7565 2076 616c 7565 0a20 2020  unique value.   
+00046b40: 2020 2020 2022 2222 0a20 2020 200a 2020       """.    .  
+00046b50: 2020 2020 2020 696e 6473 203d 205b 5b5d        inds = [[]
+00046b60: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00046b70: 7365 6c66 2e4e 295d 2020 2020 0a20 2020  self.N)]    .   
+00046b80: 2020 2020 2073 6f20 3d20 6e70 2e61 7267       so = np.arg
+00046b90: 736f 7274 2873 656c 662e 696e 6469 6365  sort(self.indice
+00046ba0: 7329 0a20 2020 200a 2020 2020 2020 2020  s).    .        
+00046bb0: 666f 7220 692c 2069 6920 696e 207a 6970  for i, ii in zip
+00046bc0: 2873 6f2c 2073 656c 662e 696e 6469 6365  (so, self.indice
+00046bd0: 735b 736f 5d29 3a0a 2020 2020 2020 2020  s[so]):.        
+00046be0: 2020 2020 696e 6473 5b69 695d 2e61 7070      inds[ii].app
+00046bf0: 656e 6428 6929 0a20 2020 2020 2020 200a  end(i).        .
+00046c00: 2020 2020 2020 2020 2320 536f 7274 2074          # Sort t
+00046c10: 6865 2073 7562 6c69 7374 730a 2020 2020  he sublists.    
+00046c20: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00046c30: 6765 2873 656c 662e 4e29 3a0a 2020 2020  ge(self.N):.    
+00046c40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00046c50: 636f 756e 7473 5b69 5d20 3e20 313a 0a20  counts[i] > 1:. 
+00046c60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00046c70: 6e64 735b 695d 2e73 6f72 7428 290a 2020  nds[i].sort().  
+00046c80: 2020 0a20 2020 2020 2020 2072 6574 7572    .        retur
+00046c90: 6e20 696e 6473 0a20 2020 200a 2020 2020  n inds.    .    
+00046ca0: 0a20 2020 2064 6566 2075 6e69 7175 655f  .    def unique_
+00046cb0: 696e 6465 7828 7365 6c66 2c20 696e 6465  index(self, inde
+00046cc0: 783d 3029 3a0a 2020 2020 2020 2020 2222  x=0):.        ""
+00046cd0: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00046ce0: 2061 7272 6179 206f 6620 696e 6469 6365   array of indice
+00046cf0: 7320 6f66 2074 6865 2070 6172 656e 7420  s of the parent 
+00046d00: 6172 7261 7920 7468 6174 206d 616b 6573  array that makes
+00046d10: 2061 2075 6e69 7175 6520 6f75 7470 7574   a unique output
+00046d20: 2061 7272 6179 0a20 2020 2020 2020 200a   array.        .
+00046d30: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00046d40: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00046d50: 2020 2020 2020 2020 7569 7820 3a20 6c69          uix : li
+00046d60: 7374 0a20 2020 2020 2020 2020 2020 204c  st.            L
+00046d70: 6973 7420 6f66 2075 6e69 7175 6520 696e  ist of unique in
+00046d80: 6469 6365 730a 2020 2020 2020 2020 2222  dices.        ""
+00046d90: 220a 2020 2020 2020 2020 7569 7820 3d20  ".        uix = 
+00046da0: 5b69 6e64 5b69 6e64 6578 5d20 666f 7220  [ind[index] for 
+00046db0: 696e 6420 696e 2073 656c 662e 6c69 7374  ind in self.list
+00046dc0: 5f69 6e64 6963 6573 5d0a 2020 2020 2020  _indices].      
+00046dd0: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+00046de0: 2020 2020 2020 2072 6574 7572 6e20 7569         return ui
+00046df0: 780a 2020 2020 0a20 2020 200a 2020 2020  x.    .    .    
+00046e00: 6465 6620 5f5f 6974 6572 5f5f 2873 656c  def __iter__(sel
+00046e10: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00046e20: 2020 2020 2020 2020 4974 6572 6162 6c65          Iterable
+00046e30: 206f 7665 7220 6076 616c 7565 7360 2061   over `values` a
+00046e40: 7474 7269 6275 7465 0a20 2020 2020 2020  ttribute.       
+00046e50: 200a 2020 2020 2020 2020 5265 7475 726e   .        Return
+00046e60: 7320 6120 7475 706c 6520 6f66 2074 6865  s a tuple of the
+00046e70: 2076 616c 7565 2061 6e64 2074 6865 2062   value and the b
+00046e80: 6f6f 6c65 616e 2073 656c 6563 7469 6f6e  oolean selection
+00046e90: 2061 7272 6179 2066 6f72 2074 6861 7420   array for that 
+00046ea0: 0a20 2020 2020 2020 2076 616c 7565 2e0a  .        value..
+00046eb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00046ec0: 2020 2020 6920 3d20 300a 2020 2020 2020      i = 0.      
+00046ed0: 2020 7768 696c 6520 6920 3c20 7365 6c66    while i < self
+00046ee0: 2e4e 3a0a 2020 2020 2020 2020 2020 2020  .N:.            
+00046ef0: 7669 203d 2073 656c 662e 7661 6c75 6573  vi = self.values
+00046f00: 5b69 5d0a 2020 2020 2020 2020 2020 2020  [i].            
+00046f10: 7969 656c 6420 2876 692c 2073 656c 665b  yield (vi, self[
+00046f20: 7669 5d29 0a20 2020 2020 2020 2020 2020  vi]).           
+00046f30: 2069 202b 3d20 310a 0a0a 2020 2020 6465   i += 1...    de
+00046f40: 6620 5f5f 6765 7469 7465 6d5f 5f28 7365  f __getitem__(se
+00046f50: 6c66 2c20 6b65 7929 3a0a 2020 2020 2020  lf, key):.      
+00046f60: 2020 6966 206b 6579 2069 6e20 7365 6c66    if key in self
+00046f70: 2e76 616c 7565 733a 0a20 2020 2020 2020  .values:.       
+00046f80: 2020 2020 2069 7820 3d20 7365 6c66 2e76       ix = self.v
+00046f90: 616c 7565 732e 696e 6465 7828 6b65 7929  alues.index(key)
+00046fa0: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
+00046fb0: 7420 3d20 7365 6c66 2e69 6e64 6963 6573  t = self.indices
+00046fc0: 203d 3d20 6978 0a20 2020 2020 2020 2020   == ix.         
+00046fd0: 2020 2072 6574 7572 6e20 7465 7374 0a20     return test. 
+00046fe0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00046ff0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00047000: 7365 6c66 2e7a 6572 6f73 0a0a 0a20 2020  self.zeros...   
+00047010: 2064 6566 205f 5f6c 656e 5f5f 2873 656c   def __len__(sel
+00047020: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00047030: 726e 2073 656c 662e 4e0a 0a0a 636c 6173  rn self.N...clas
+00047040: 7320 4875 6262 6c65 5859 5a28 6f62 6a65  s HubbleXYZ(obje
+00047050: 6374 293a 0a20 2020 2064 6566 205f 5f69  ct):.    def __i
+00047060: 6e69 745f 5f28 7365 6c66 2c20 7370 745f  nit__(self, spt_
+00047070: 6669 6c65 3d27 272c 2070 6172 616d 5f64  file='', param_d
+00047080: 6963 743d 7b7d 293a 0a20 2020 2020 2020  ict={}):.       
+00047090: 2022 2222 0a20 2020 2020 2020 2048 656c   """.        Hel
+000470a0: 7065 7220 746f 2063 6f6d 7075 7465 2048  per to compute H
+000470b0: 5354 2067 656f 6365 6e74 7269 6320 636f  ST geocentric co
+000470c0: 6f72 6469 6e61 7465 7320 6672 6f6d 206f  ordinates from o
+000470d0: 7262 6974 616c 2070 6172 616d 6574 6572  rbital parameter
+000470e0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
+000470f0: 2020 2028 7465 7374 696e 6729 0a20 2020     (testing).   
+00047100: 2020 2020 200a 2020 2020 2020 2020 4261       .        Ba
+00047110: 7365 6420 6f6e 2068 7474 703a 2f2f 6172  sed on http://ar
+00047120: 7469 636c 6573 2e61 6473 6162 732e 6861  ticles.adsabs.ha
+00047130: 7276 6172 642e 6564 752f 2f66 756c 6c2f  rvard.edu//full/
+00047140: 3139 3935 4153 5043 2e2e 2e37 372e 2e34  1995ASPC...77..4
+00047150: 3634 412f 0a20 2020 2020 2020 2022 2222  64A/.        """
+00047160: 0a20 2020 2020 2020 2069 6620 7370 745f  .        if spt_
+00047170: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00047180: 2020 7365 6c66 2e70 6172 616d 5f64 6963    self.param_dic
+00047190: 7420 3d20 7365 6c66 2e70 6172 7365 5f66  t = self.parse_f
+000471a0: 726f 6d5f 7370 7428 7370 745f 6669 6c65  rom_spt(spt_file
+000471b0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000471c0: 2020 2065 6c69 6620 7061 7261 6d5f 6469     elif param_di
+000471d0: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
+000471e0: 7365 6c66 2e70 6172 616d 5f64 6963 7420  self.param_dict 
+000471f0: 3d20 7061 7261 6d5f 6469 6374 0a20 2020  = param_dict.   
+00047200: 2020 2020 200a 2020 2020 2020 2020 656c       .        el
+00047210: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00047220: 7365 6c66 2e70 6172 616d 5f64 6963 7420  self.param_dict 
+00047230: 3d20 7b7d 0a20 2020 2020 2020 200a 2020  = {}.        .  
+00047240: 2020 2020 2020 7365 6c66 2e63 6f6d 7075        self.compu
+00047250: 7465 6420 3d20 7b7d 0a0a 0a20 2020 2040  ted = {}...    @
+00047260: 7072 6f70 6572 7479 200a 2020 2020 6465  property .    de
+00047270: 6620 5f74 3139 3835 2873 656c 6629 3a0a  f _t1985(self):.
+00047280: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00047290: 2020 2020 5265 6665 7265 6e63 6520 7469      Reference ti
+000472a0: 6d65 0a20 2020 2020 2020 2022 2222 0a20  me.        """. 
+000472b0: 2020 2020 2020 2069 6d70 6f72 7420 6173         import as
+000472c0: 7472 6f70 792e 7469 6d65 0a20 2020 2020  tropy.time.     
+000472d0: 2020 2074 3020 3d20 6173 7472 6f70 792e     t0 = astropy.
+000472e0: 7469 6d65 2e54 696d 6528 2731 3938 352d  time.Time('1985-
+000472f0: 3031 2d30 3154 3030 3a30 303a 3030 5a27  01-01T00:00:00Z'
+00047300: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00047310: 2074 300a 0a0a 2020 2020 6465 6620 5f5f   t0...    def __
+00047320: 6361 6c6c 5f5f 2873 656c 662c 2074 5f69  call__(self, t_i
+00047330: 6e2c 202a 2a6b 7761 7267 7329 3a0a 2020  n, **kwargs):.  
+00047340: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00047350: 2020 436f 6e76 6572 7420 696e 7075 7420    Convert input 
+00047360: 7469 6d65 2060 6074 5f69 6e60 6020 746f  time ``t_in`` to
+00047370: 2073 6563 6f6e 6473 2073 696e 6365 2031   seconds since 1
+00047380: 2f31 2f38 3520 616e 6420 6060 6576 616c  /1/85 and ``eval
+00047390: 7561 7465 6060 2e0a 2020 2020 2020 2020  uate``..        
+000473a0: 2222 220a 2020 2020 2020 2020 696d 706f  """.        impo
+000473b0: 7274 2061 7374 726f 7079 2e74 696d 650a  rt astropy.time.
+000473c0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+000473d0: 7369 6e73 7461 6e63 6528 745f 696e 2c20  sinstance(t_in, 
+000473e0: 6173 7472 6f70 792e 7469 6d65 2e54 696d  astropy.time.Tim
+000473f0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
 00047400: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00047410: 2827 4f72 6269 7461 6c20 7061 7261 6d65  ('Orbital parame
-00047420: 7465 7273 206e 6f74 2064 6566 696e 6564  ters not defined
-00047430: 2069 6e20 270a 2020 2020 2020 2020 2020   in '.          
-00047440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00047450: 2020 2027 7365 6c66 2e70 6172 616d 5f64     'self.param_d
-00047460: 6963 7427 290a 2020 2020 2020 2020 2020  ict').          
-00047470: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00047480: 2020 2070 203d 2073 656c 662e 7061 7261     p = self.para
-00047490: 6d5f 6469 6374 0a20 2020 2020 2020 200a  m_dict.        .
-000474a0: 2020 2020 2020 2020 7420 3d20 6e70 2e61          t = np.a
-000474b0: 746c 6561 7374 5f31 6428 6474 290a 2020  tleast_1d(dt).  
-000474c0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000474d0: 2045 712e 2031 0a20 2020 2020 2020 2062   Eq. 1.        b
-000474e0: 7261 636b 6574 203d 2070 5b27 4d2e 275d  racket = p['M.']
-000474f0: 2a28 742d 705b 2774 6175 275d 2920 2b20  *(t-p['tau']) + 
-00047500: 302e 352a 705b 274d 2e2e 275d 2a28 742d  0.5*p['M..']*(t-
-00047510: 705b 2774 6175 275d 292a 2a32 0a20 2020  p['tau'])**2.   
-00047520: 2020 2020 204d 203d 2070 5b27 4d30 275d       M = p['M0']
-00047530: 202b 2032 2a6e 702e 7069 2a62 7261 636b   + 2*np.pi*brack
-00047540: 6574 0a20 2020 2020 2020 200a 2020 2020  et.        .    
-00047550: 2020 2020 2320 4571 2e20 320a 2020 2020      # Eq. 2.    
-00047560: 2020 2020 7369 6e4d 203d 206e 702e 7369      sinM = np.si
-00047570: 6e28 4d29 0a20 2020 2020 2020 2063 6f73  n(M).        cos
-00047580: 4d20 3d20 6e70 2e63 6f73 284d 290a 2020  M = np.cos(M).  
-00047590: 2020 2020 2020 6520 3d20 705b 2765 275d        e = p['e']
-000475a0: 0a20 2020 2020 2020 206e 7520 3d20 4d20  .        nu = M 
-000475b0: 2b20 7369 6e4d 2a28 322a 6520 2b20 332a  + sinM*(2*e + 3*
-000475c0: 652a 2a33 2a63 6f73 4d2a 2a32 202d 2034  e**3*cosM**2 - 4
-000475d0: 2e2f 332a 652a 2a33 2a73 696e 4d2a 2a32  ./3*e**3*sinM**2
-000475e0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-000475f0: 2020 2020 2020 2020 202b 2035 2e2f 322a           + 5./2*
-00047600: 652a 2a32 2a63 6f73 4d29 0a20 2020 2020  e**2*cosM).     
-00047610: 2020 200a 2020 2020 2020 2020 2320 4571     .        # Eq
-00047620: 2e20 330a 2020 2020 2020 2020 7220 3d20  . 3.        r = 
-00047630: 705b 2761 2831 2d65 2a2a 3229 275d 2f28  p['a(1-e**2)']/(
-00047640: 312b 652a 6e70 2e63 6f73 286e 7529 290a  1+e*np.cos(nu)).
-00047650: 2020 2020 2020 2020 2320 546f 206b 6d0a          # To km.
-00047660: 2020 2020 2020 2020 7220 2f3d 2031 3030          r /= 100
-00047670: 302e 0a20 2020 2020 2020 200a 2020 2020  0..        .    
-00047680: 2020 2020 2320 4571 2e20 340a 2020 2020      # Eq. 4.    
-00047690: 2020 2020 4f6d 203d 2032 2a6e 702e 7069      Om = 2*np.pi
-000476a0: 2a28 705b 274f 6d30 275d 202b 2070 5b27  *(p['Om0'] + p['
-000476b0: 4f6d 2e27 5d2a 2874 2d70 5b27 7461 7527  Om.']*(t-p['tau'
-000476c0: 5d29 290a 2020 2020 2020 2020 0a20 2020  ])).        .   
-000476d0: 2020 2020 2023 2045 712e 2035 0a20 2020       # Eq. 5.   
-000476e0: 2020 2020 2077 203d 2032 2a6e 702e 7069       w = 2*np.pi
-000476f0: 2a28 705b 2777 3027 5d20 2b20 705b 2777  *(p['w0'] + p['w
-00047700: 2e27 5d2a 2874 2d70 5b27 7461 7527 5d29  .']*(t-p['tau'])
-00047710: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00047720: 2020 2073 656c 662e 6361 6c63 5f64 6963     self.calc_dic
-00047730: 7420 3d20 7b27 4d27 3a4d 2c20 276e 7527  t = {'M':M, 'nu'
-00047740: 3a6e 752c 200a 2020 2020 2020 2020 2020  :nu, .          
-00047750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00047760: 2761 273a 705b 2761 275d 2c20 0a20 2020  'a':p['a'], .   
-00047770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00047780: 2020 2020 2020 2027 6927 3a6e 702e 6172         'i':np.ar
-00047790: 6373 696e 2870 5b27 7369 6e69 275d 292c  csin(p['sini']),
-000477a0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-000477b0: 2020 2020 2020 2020 2020 2020 274f 6d27              'Om'
-000477c0: 3a4f 6d2c 0a20 2020 2020 2020 2020 2020  :Om,.           
-000477d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000477e0: 7727 3a77 7d0a 2020 2020 2020 2020 0a20  w':w}.        . 
-000477f0: 2020 2020 2020 2023 2045 712e 2036 0a20         # Eq. 6. 
-00047800: 2020 2020 2020 2063 6f73 4f6d 203d 206e         cosOm = n
-00047810: 702e 636f 7328 4f6d 290a 2020 2020 2020  p.cos(Om).      
-00047820: 2020 7369 6e4f 6d20 3d20 6e70 2e73 696e    sinOm = np.sin
-00047830: 284f 6d29 0a20 2020 2020 2020 2063 6f73  (Om).        cos
-00047840: 7776 203d 206e 702e 636f 7328 772b 6e75  wv = np.cos(w+nu
-00047850: 290a 2020 2020 2020 2020 7369 6e77 7620  ).        sinwv 
-00047860: 3d20 6e70 2e73 696e 2877 2b6e 7529 0a20  = np.sin(w+nu). 
-00047870: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00047880: 6966 2075 6e69 7420 6973 206e 6f74 204e  if unit is not N
-00047890: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000478a0: 2072 203d 2028 722a 752e 6b6d 292e 746f   r = (r*u.km).to
-000478b0: 2875 6e69 7429 0a20 2020 2020 2020 2020  (unit).         
-000478c0: 2020 200a 2020 2020 2020 2020 7820 3d20     .        x = 
-000478d0: 722a 2863 6f73 4f6d 2a63 6f73 7776 202d  r*(cosOm*coswv -
-000478e0: 2070 5b27 636f 7369 275d 2a73 696e 4f6d   p['cosi']*sinOm
-000478f0: 2a73 696e 7776 290a 2020 2020 2020 2020  *sinwv).        
-00047900: 7920 3d20 722a 2873 696e 4f6d 2a63 6f73  y = r*(sinOm*cos
-00047910: 7776 202b 2070 5b27 636f 7369 275d 2a63  wv + p['cosi']*c
-00047920: 6f73 4f6d 2a73 696e 7776 290a 2020 2020  osOm*sinwv).    
-00047930: 2020 2020 7a20 3d20 722a 705b 2773 696e      z = r*p['sin
-00047940: 6927 5d2a 7369 6e77 760a 2020 2020 2020  i']*sinwv.      
-00047950: 2020 0a20 2020 2020 2020 2069 6620 6173    .        if as
-00047960: 5f74 6162 6c65 3a0a 2020 2020 2020 2020  _table:.        
-00047970: 2020 2020 7461 6220 3d20 4754 6162 6c65      tab = GTable
-00047980: 2829 0a20 2020 2020 2020 2020 2020 2074  ().            t
-00047990: 6162 5b27 6474 275d 203d 2074 0a20 2020  ab['dt'] = t.   
-000479a0: 2020 2020 2020 2020 2074 6162 5b27 7827           tab['x'
-000479b0: 5d20 3d20 780a 2020 2020 2020 2020 2020  ] = x.          
-000479c0: 2020 7461 625b 2779 275d 203d 2079 0a20    tab['y'] = y. 
-000479d0: 2020 2020 2020 2020 2020 2074 6162 5b27             tab['
-000479e0: 7a27 5d20 3d20 7a0a 2020 2020 2020 2020  z'] = z.        
-000479f0: 2020 2020 7461 625b 2772 275d 203d 2072      tab['r'] = r
-00047a00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00047a10: 7572 6e20 7461 620a 2020 2020 2020 2020  urn tab.        
-00047a20: 656c 7365 3a20 0a20 2020 2020 2020 2020  else: .         
-00047a30: 2020 2072 6574 7572 6e20 782c 2079 2c20     return x, y, 
-00047a40: 7a2c 2072 0a0a 0a20 2020 2064 6566 2066  z, r...    def f
-00047a50: 726f 6d5f 666c 7428 7365 6c66 2c20 666c  rom_flt(self, fl
-00047a60: 745f 6669 6c65 2c20 2a2a 6b77 6172 6773  t_file, **kwargs
-00047a70: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00047a80: 2020 2020 2020 2043 6f6d 7075 7465 2070         Compute p
-00047a90: 6f73 6974 696f 6e73 2061 7420 6578 7073  ositions at exps
-00047aa0: 7461 7274 2c20 6578 706d 6964 2c20 6578  tart, expmid, ex
-00047ab0: 7065 6e64 0a20 2020 2020 2020 2022 2222  pend.        """
-00047ac0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00047ad0: 6173 7472 6f70 792e 7469 6d65 0a20 2020  astropy.time.   
-00047ae0: 2020 2020 200a 2020 2020 2020 2020 666c       .        fl
-00047af0: 7420 3d20 7079 6669 7473 2e6f 7065 6e28  t = pyfits.open(
-00047b00: 666c 745f 6669 6c65 290a 2020 2020 2020  flt_file).      
-00047b10: 2020 6578 7073 7461 7274 203d 2066 6c74    expstart = flt
-00047b20: 5b30 5d2e 6865 6164 6572 5b27 4558 5053  [0].header['EXPS
-00047b30: 5441 5254 275d 0a20 2020 2020 2020 2065  TART'].        e
-00047b40: 7870 656e 6420 3d20 666c 745b 305d 2e68  xpend = flt[0].h
-00047b50: 6561 6465 725b 2745 5850 454e 4427 5d0a  eader['EXPEND'].
-00047b60: 2020 2020 2020 2020 6578 706d 6964 203d          expmid =
-00047b70: 2028 6578 7073 7461 7274 2b65 7870 656e   (expstart+expen
-00047b80: 6429 2f32 2e0a 2020 2020 2020 2020 0a20  d)/2..        . 
-00047b90: 2020 2020 2020 2074 5f69 6e20 3d20 6173         t_in = as
-00047ba0: 7472 6f70 792e 7469 6d65 2e54 696d 6528  tropy.time.Time(
-00047bb0: 5b65 7870 7374 6172 742c 2065 7870 6d69  [expstart, expmi
-00047bc0: 642c 2065 7870 656e 645d 2c20 666f 726d  d, expend], form
-00047bd0: 6174 3d27 6d6a 6427 290a 2020 2020 2020  at='mjd').      
-00047be0: 2020 666c 742e 636c 6f73 6528 290a 2020    flt.close().  
-00047bf0: 2020 2020 2020 0a20 2020 2020 2020 2072        .        r
-00047c00: 6574 7572 6e20 7365 6c66 2874 5f69 6e2c  eturn self(t_in,
-00047c10: 202a 2a6b 7761 7267 7329 0a0a 0a20 2020   **kwargs)...   
-00047c20: 2064 6566 2064 656c 7461 7428 7365 6c66   def deltat(self
-00047c30: 2c20 6474 293a 0a20 2020 2020 2020 2022  , dt):.        "
-00047c40: 2222 0a20 2020 2020 2020 2043 6f6e 7665  "".        Conve
-00047c50: 7274 2061 2074 696d 6520 6060 7460 6020  rt a time ``t`` 
-00047c60: 696e 2073 6563 6f6e 6473 2066 726f 6d20  in seconds from 
-00047c70: 312f 312f 3835 2074 6f20 616e 2049 534f  1/1/85 to an ISO
-00047c80: 2074 696d 650a 2020 2020 2020 2020 2222   time.        ""
-00047c90: 2220 2020 200a 2020 2020 2020 2020 6966  "    .        if
-00047ca0: 206e 6f74 2068 6173 6174 7472 2864 742c   not hasattr(dt,
-00047cb0: 2027 756e 6974 2729 3a0a 2020 2020 2020   'unit'):.      
-00047cc0: 2020 2020 2020 6474 7365 6320 3d20 6474        dtsec = dt
-00047cd0: 2a75 2e73 6563 6f6e 640a 2020 2020 2020  *u.second.      
-00047ce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00047cf0: 2020 2020 6474 7365 6320 3d20 6474 0a20      dtsec = dt. 
-00047d00: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00047d10: 2020 2020 7420 3d20 7365 6c66 2e5f 7431      t = self._t1
-00047d20: 3938 3520 2b20 6474 7365 630a 2020 2020  985 + dtsec.    
-00047d30: 2020 2020 7265 7475 726e 2074 0a0a 0a20      return t... 
-00047d40: 2020 2064 6566 2070 6172 7365 5f66 726f     def parse_fro
-00047d50: 6d5f 7370 7428 7365 6c66 2c20 7370 745f  m_spt(self, spt_
-00047d60: 6669 6c65 293a 0a20 2020 2020 2020 2022  file):.        "
-00047d70: 2222 0a20 2020 2020 2020 2047 6574 206f  "".        Get o
-00047d80: 7262 6974 616c 2065 6c65 6d65 6e74 7320  rbital elements 
-00047d90: 6672 6f6d 2053 5054 2068 6561 6465 720a  from SPT header.
-00047da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00047db0: 2020 2020 696d 706f 7274 2061 7374 726f      import astro
-00047dc0: 7079 2e69 6f2e 6669 7473 2061 7320 7079  py.io.fits as py
-00047dd0: 6669 7473 0a20 2020 2020 2020 2069 6d70  fits.        imp
-00047de0: 6f72 7420 6173 7472 6f70 792e 7469 6d65  ort astropy.time
-00047df0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00047e00: 2020 7769 7468 2070 7966 6974 732e 6f70    with pyfits.op
-00047e10: 656e 2873 7074 5f66 696c 6529 2061 7320  en(spt_file) as 
-00047e20: 5f69 6d3a 0a20 2020 2020 2020 2020 2020  _im:.           
-00047e30: 2073 7074 203d 205f 696d 5b30 5d2e 6865   spt = _im[0].he
-00047e40: 6164 6572 2e63 6f70 7928 290a 2020 2020  ader.copy().    
-00047e50: 2020 2020 0a20 2020 2020 2020 2070 6172      .        par
-00047e60: 616d 5f64 6963 7420 3d20 7b7d 0a20 2020  am_dict = {}.   
-00047e70: 2020 2020 2070 6172 616d 5f64 6963 745b       param_dict[
-00047e80: 2774 6175 275d 203d 2073 7074 5b27 4550  'tau'] = spt['EP
-00047e90: 4348 5449 4d45 275d 0a20 2020 2020 2020  CHTIME'].       
-00047ea0: 2070 6172 616d 5f64 6963 745b 274d 3027   param_dict['M0'
-00047eb0: 5d20 3d20 7370 745b 274d 4541 4e41 4e4f  ] = spt['MEANANO
-00047ec0: 4d27 5d0a 2020 2020 2020 2020 7061 7261  M'].        para
-00047ed0: 6d5f 6469 6374 5b27 4d2e 275d 203d 2073  m_dict['M.'] = s
-00047ee0: 7074 5b27 4644 4d45 414e 414e 275d 0a20  pt['FDMEANAN']. 
-00047ef0: 2020 2020 2020 2070 6172 616d 5f64 6963         param_dic
-00047f00: 745b 274d 2e2e 275d 203d 2073 7074 5b27  t['M..'] = spt['
-00047f10: 5344 4d45 414e 414e 275d 0a20 2020 2020  SDMEANAN'].     
-00047f20: 2020 2070 6172 616d 5f64 6963 745b 2765     param_dict['e
-00047f30: 275d 203d 2073 7074 5b27 4543 4345 4e54  '] = spt['ECCENT
-00047f40: 5259 275d 0a20 2020 2020 2020 2070 6172  RY'].        par
-00047f50: 616d 5f64 6963 745b 2761 2831 2d65 2a2a  am_dict['a(1-e**
-00047f60: 3229 275d 203d 2073 7074 5b27 5345 4d49  2)'] = spt['SEMI
-00047f70: 4c52 4543 275d 0a20 2020 2020 2020 2070  LREC'].        p
-00047f80: 6172 616d 5f64 6963 745b 2761 275d 203d  aram_dict['a'] =
-00047f90: 2070 6172 616d 5f64 6963 745b 2761 2831   param_dict['a(1
-00047fa0: 2d65 2a2a 3229 275d 202f 2028 312d 7061  -e**2)'] / (1-pa
-00047fb0: 7261 6d5f 6469 6374 5b27 6527 5d2a 2a32  ram_dict['e']**2
-00047fc0: 290a 2020 2020 2020 2020 7061 7261 6d5f  ).        param_
-00047fd0: 6469 6374 5b27 4f6d 3027 5d20 3d20 7370  dict['Om0'] = sp
-00047fe0: 745b 2752 4153 4341 5343 4e27 5d0a 2020  t['RASCASCN'].  
-00047ff0: 2020 2020 2020 7061 7261 6d5f 6469 6374        param_dict
-00048000: 5b27 4f6d 2e27 5d20 3d20 7370 745b 2752  ['Om.'] = spt['R
-00048010: 4341 5343 4e52 5627 5d0a 2020 2020 2020  CASCNRV'].      
-00048020: 2020 7061 7261 6d5f 6469 6374 5b27 7730    param_dict['w0
-00048030: 275d 203d 2073 7074 5b27 4152 4750 4552  '] = spt['ARGPER
-00048040: 4947 275d 0a20 2020 2020 2020 2070 6172  IG'].        par
-00048050: 616d 5f64 6963 745b 2777 2e27 5d20 3d20  am_dict['w.'] = 
-00048060: 7370 745b 2752 4341 5247 5045 5227 5d0a  spt['RCARGPER'].
-00048070: 2020 2020 2020 2020 7061 7261 6d5f 6469          param_di
-00048080: 6374 5b27 636f 7369 275d 203d 2073 7074  ct['cosi'] = spt
-00048090: 5b27 434f 5349 4e43 4c49 275d 0a20 2020  ['COSINCLI'].   
-000480a0: 2020 2020 2070 6172 616d 5f64 6963 745b       param_dict[
-000480b0: 2773 696e 6927 5d20 3d20 7370 745b 2753  'sini'] = spt['S
-000480c0: 494e 4549 4e43 4c27 5d0a 2020 2020 2020  INEINCL'].      
-000480d0: 2020 7061 7261 6d5f 6469 6374 5b27 5663    param_dict['Vc
-000480e0: 275d 203d 2073 7074 5b27 4349 5256 454c  '] = spt['CIRVEL
-000480f0: 4f43 275d 0a20 2020 2020 2020 2070 6172  OC'].        par
-00048100: 616d 5f64 6963 745b 2774 696d 6566 6665  am_dict['timeffe
-00048110: 6327 5d20 3d20 7370 745b 2754 494d 4546  c'] = spt['TIMEF
-00048120: 4645 4327 5d0a 2020 2020 2020 2020 7061  FEC'].        pa
-00048130: 7261 6d5f 6469 6374 5b27 546f 7262 275d  ram_dict['Torb']
-00048140: 203d 2073 7074 5b27 4853 5448 4f52 4227   = spt['HSTHORB'
-00048150: 5d2a 320a 2020 2020 2020 2020 7061 7261  ]*2.        para
-00048160: 6d5f 6469 6374 5b27 7473 7461 7274 275d  m_dict['tstart']
-00048170: 203d 2073 7074 5b27 4f42 5353 5452 5454   = spt['OBSSTRTT
-00048180: 275d 0a20 2020 2020 2020 200a 2020 2020  '].        .    
-00048190: 2020 2020 7061 7261 6d5f 6469 6374 5b27      param_dict['
-000481a0: 7461 755f 7469 6d65 275d 203d 2073 656c  tau_time'] = sel
-000481b0: 662e 6465 6c74 6174 2870 6172 616d 5f64  f.deltat(param_d
-000481c0: 6963 745b 2774 6175 275d 290a 2020 2020  ict['tau']).    
-000481d0: 2020 2020 7061 7261 6d5f 6469 6374 5b27      param_dict['
-000481e0: 7473 7461 7274 5f74 696d 6527 5d20 3d20  tstart_time'] = 
-000481f0: 7365 6c66 2e64 656c 7461 7428 7061 7261  self.deltat(para
-00048200: 6d5f 6469 6374 5b27 7473 7461 7274 275d  m_dict['tstart']
-00048210: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00048220: 2020 0a20 2020 2020 2020 2072 6574 7572    .        retur
-00048230: 6e20 7061 7261 6d5f 6469 6374 0a20 2020  n param_dict.   
-00048240: 200a 2020 2020 4073 7461 7469 636d 6574   .    @staticmet
-00048250: 686f 640a 2020 2020 6465 6620 7879 7a5f  hod.    def xyz_
-00048260: 746f 5f6c 6f6e 6c61 7428 7365 6c66 2c20  to_lonlat(self, 
-00048270: 782c 2079 2c20 7a2c 2072 6164 6961 6e73  x, y, z, radians
-00048280: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
-00048290: 2022 2222 0a20 2020 2020 2020 2043 6f6d   """.        Com
-000482a0: 7075 7465 2073 7562 6c6f 6e2c 2073 7562  pute sublon, sub
-000482b0: 6c61 742c 2061 6c74 2066 726f 6d20 7879  lat, alt from xy
-000482c0: 7a20 636f 6f72 6473 2077 6974 6820 7079  z coords with py
-000482d0: 7072 6f6a 0a20 2020 2020 2020 200a 2020  proj.        .  
-000482e0: 2020 2020 2020 7879 7a20 6d75 7374 2062        xyz must b
-000482f0: 6520 696e 206d 6574 6572 730a 2020 2020  e in meters.    
-00048300: 2020 2020 0a20 2020 2020 2020 2022 2222      .        """
-00048310: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00048320: 7079 7072 6f6a 0a20 2020 2020 2020 2065  pyproj.        e
-00048330: 6365 6620 3d20 7079 7072 6f6a 2e50 726f  cef = pyproj.Pro
-00048340: 6a28 7072 6f6a 3d27 6765 6f63 656e 7427  j(proj='geocent'
-00048350: 2c20 656c 6c70 733d 2757 4753 3834 272c  , ellps='WGS84',
-00048360: 2064 6174 756d 3d27 5747 5338 3427 290a   datum='WGS84').
-00048370: 2020 2020 2020 2020 6c6c 6120 3d20 7079          lla = py
-00048380: 7072 6f6a 2e50 726f 6a28 7072 6f6a 3d27  proj.Proj(proj='
-00048390: 6c61 746c 6f6e 6727 2c20 656c 6c70 733d  latlong', ellps=
-000483a0: 2757 4753 3834 272c 2064 6174 756d 3d27  'WGS84', datum='
-000483b0: 5747 5338 3427 290a 2020 2020 2020 2020  WGS84').        
-000483c0: 6c6f 6e2c 206c 6174 2c20 616c 7420 3d20  lon, lat, alt = 
-000483d0: 7079 7072 6f6a 2e74 7261 6e73 666f 726d  pyproj.transform
-000483e0: 2865 6365 662c 206c 6c61 2c20 782c 2079  (ecef, lla, x, y
-000483f0: 2c20 7a2c 2072 6164 6961 6e73 3d72 6164  , z, radians=rad
-00048400: 6961 6e73 290a 2020 2020 2020 2020 7265  ians).        re
-00048410: 7475 726e 206c 6f6e 2c20 6c61 742c 2061  turn lon, lat, a
-00048420: 6c74 0a0a 0a64 6566 2070 6174 6368 5f70  lt...def patch_p
-00048430: 686f 7475 7469 6c73 2829 3a0a 2020 2020  hotutils():.    
-00048440: 2222 220a 2020 2020 5061 7463 6820 746f  """.    Patch to
-00048450: 2066 6978 2069 6e63 6f6e 7369 7374 656e   fix inconsisten
-00048460: 6379 2077 6974 6820 6472 697a 7a6c 6570  cy with drizzlep
-00048470: 6163 3d33 2e32 2e31 2061 6e64 2070 686f  ac=3.2.1 and pho
-00048480: 7475 7469 6c73 3e31 2e30 2c20 7768 6572  tutils>1.0, wher
-00048490: 6520 0a20 2020 2054 6865 206c 6174 7465  e .    The latte
-000484a0: 7220 6973 206e 6565 6465 6420 666f 7220  r is needed for 
-000484b0: 6a77 7374 3d31 2e33 2e32 0a20 2020 2022  jwst=1.3.2.    "
-000484c0: 2222 0a20 2020 2069 6d70 6f72 7420 6f73  "".    import os
-000484d0: 0a0a 2020 2020 7472 793a 0a20 2020 2020  ..    try:.     
-000484e0: 2020 2069 6d70 6f72 7420 6472 697a 7a6c     import drizzl
-000484f0: 6570 6163 0a20 2020 2065 7863 6570 7420  epac.    except 
-00048500: 4174 7472 6962 7574 6545 7272 6f72 3a0a  AttributeError:.
-00048510: 2020 2020 0a20 2020 2020 2020 2069 6d70      .        imp
-00048520: 6f72 7420 7068 6f74 7574 696c 730a 2020  ort photutils.  
-00048530: 2020 2020 2020 7369 7465 5f70 6163 6b61        site_packa
-00048540: 6765 7320 3d20 6f73 2e70 6174 682e 6469  ges = os.path.di
-00048550: 726e 616d 6528 7068 6f74 7574 696c 732e  rname(photutils.
-00048560: 5f5f 6669 6c65 5f5f 290a 2020 2020 2020  __file__).      
-00048570: 2020 2320 6d61 6e75 616c 2061 7070 6c79    # manual apply
-00048580: 2070 6174 6368 0a20 2020 2020 2020 2074   patch.        t
-00048590: 6865 5f66 696c 6520 3d20 6627 7b73 6974  he_file = f'{sit
-000485a0: 655f 7061 636b 6167 6573 7d2f 2e2e 2f64  e_packages}/../d
-000485b0: 7269 7a7a 6c65 7061 632f 6861 7075 7469  rizzlepac/haputi
-000485c0: 6c73 2f61 6c69 676e 5f75 7469 6c73 2e70  ls/align_utils.p
-000485d0: 7927 0a20 2020 2020 2020 2077 6974 6820  y'.        with 
-000485e0: 6f70 656e 2874 6865 5f66 696c 652c 2772  open(the_file,'r
-000485f0: 2729 2061 7320 6670 3a0a 2020 2020 2020  ') as fp:.      
-00048600: 2020 2020 2020 6c69 6e65 7320 3d20 6670        lines = fp
-00048610: 2e72 6561 646c 696e 6573 2829 0a20 2020  .readlines().   
-00048620: 200a 2020 2020 2020 2020 7072 696e 7428   .        print(
-00048630: 7369 7465 5f70 6163 6b61 6765 732c 206c  site_packages, l
-00048640: 656e 286c 696e 6573 2929 0a20 2020 2020  en(lines)).     
-00048650: 2020 2066 6f72 2069 2c20 6c69 6e65 2069     for i, line i
-00048660: 6e20 656e 756d 6572 6174 6528 6c69 6e65  n enumerate(line
-00048670: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00048680: 6966 206c 696e 652e 7374 6172 7473 7769  if line.startswi
-00048690: 7468 2827 4e6f 4465 7465 6374 696f 6e73  th('NoDetections
-000486a0: 5761 726e 696e 6727 293a 0a20 2020 2020  Warning'):.     
-000486b0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-000486c0: 0a20 2020 200a 2020 2020 2020 2020 6966  .    .        if
-000486d0: 2027 6861 7361 7474 7228 7068 6f74 7574   'hasattr(photut
-000486e0: 696c 732e 6669 6e64 7374 6172 7327 2069  ils.findstars' i
-000486f0: 6e20 6c69 6e65 735b 692b 315d 3a0a 2020  n lines[i+1]:.  
-00048700: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00048710: 6627 4920 666f 756e 6420 7468 6520 7072  f'I found the pr
-00048720: 6f62 6c65 6d20 6f6e 206c 696e 6573 207b  oblem on lines {
-00048730: 697d 2d7b 692b 327d 3a20 2729 0a20 2020  i}-{i+2}: ').   
-00048740: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00048750: 2020 2020 2020 206d 7367 203d 2022 2222         msg = """
-00048760: 0a4c 696e 6573 207b 307d 2d7b 317d 2069  .Lines {0}-{1} i
-00048770: 6e20 7b32 7d20 696d 706f 7274 696e 6720  n {2} importing 
-00048780: 7068 6f74 7574 696c 7320 7765 7265 206e  photutils were n
-00048790: 6f74 2061 7320 6578 7065 6374 6564 2e20  ot as expected. 
-000487a0: 2049 2066 6f75 6e64 200a 0a7b 337d 0a0a   I found ..{3}..
-000487b0: 6275 7420 6578 7065 6374 6564 200a 0a20  but expected .. 
-000487c0: 2020 4e6f 4465 7465 6374 696f 6e73 5761    NoDetectionsWa
-000487d0: 726e 696e 6720 3d20 7068 6f74 7574 696c  rning = photutil
-000487e0: 732e 6669 6e64 7374 6172 732e 4e6f 4465  s.findstars.NoDe
-000487f0: 7465 6374 696f 6e73 5761 726e 696e 6720  tectionsWarning 
-00048800: 6966 205c 5c0a 2020 2020 2020 2020 2020  if \\.          
-00048810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00048820: 2068 6173 6174 7472 2870 686f 7475 7469   hasattr(photuti
-00048830: 6c73 2e66 696e 6473 7461 7273 2c20 274e  ls.findstars, 'N
-00048840: 6f44 6574 6563 7469 6f6e 7357 6172 6e69  oDetectionsWarni
-00048850: 6e67 2729 2065 6c73 6520 5c5c 0a20 2020  ng') else \\.   
-00048860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00048870: 2020 2020 2020 2020 7068 6f74 7574 696c          photutil
-00048880: 732e 7574 696c 732e 4e6f 4465 7465 6374  s.utils.NoDetect
-00048890: 696f 6e73 5761 726e 696e 670a 0a0a 2020  ionsWarning...  
-000488a0: 2020 2222 222e 666f 726d 6174 2869 2c20    """.format(i, 
-000488b0: 692b 322c 2074 6865 5f66 696c 652c 206c  i+2, the_file, l
-000488c0: 696e 6573 5b69 3a69 2b33 5d29 0a20 2020  ines[i:i+3]).   
-000488d0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-000488e0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000488f0: 6f72 286d 7367 290a 2020 2020 2020 2020  or(msg).        
-00048900: 0a20 2020 2020 2020 2062 6164 203d 205b  .        bad = [
-00048910: 2720 2020 272b 6c69 6e65 732e 706f 7028  '   '+lines.pop(
-00048920: 692b 322d 6a29 2066 6f72 206a 2069 6e20  i+2-j) for j in 
-00048930: 7261 6e67 6528 3329 5d0a 2020 2020 2020  range(3)].      
-00048940: 2020 7072 696e 7428 2727 2e6a 6f69 6e28    print(''.join(
-00048950: 6261 645b 3a3a 2d31 5d29 290a 0a20 2020  bad[::-1]))..   
-00048960: 2020 2020 2023 2049 6e73 6572 7420 7468       # Insert th
-00048970: 6520 6669 780a 2020 2020 2020 2020 6c69  e fix.        li
-00048980: 6e65 735b 695d 203d 2027 6672 6f6d 2070  nes[i] = 'from p
-00048990: 686f 7475 7469 6c73 2e75 7469 6c73 2e65  hotutils.utils.e
-000489a0: 7863 6570 7469 6f6e 7320 696d 706f 7274  xceptions import
-000489b0: 204e 6f44 6574 6563 7469 6f6e 7357 6172   NoDetectionsWar
-000489c0: 6e69 6e67 5c6e 5c6e 270a 2020 2020 2020  ning\n\n'.      
-000489d0: 2020 2320 5265 7772 6974 6520 7468 6520    # Rewrite the 
-000489e0: 6669 650a 2020 2020 2020 2020 7769 7468  fie.        with
-000489f0: 206f 7065 6e28 6627 7b73 6974 655f 7061   open(f'{site_pa
-00048a00: 636b 6167 6573 7d2f 2e2e 2f64 7269 7a7a  ckages}/../drizz
-00048a10: 6c65 7061 632f 6861 7075 7469 6c73 2f61  lepac/haputils/a
-00048a20: 6c69 676e 5f75 7469 6c73 2e70 7927 2c27  lign_utils.py','
-00048a30: 7727 2920 6173 2066 703a 0a20 2020 2020  w') as fp:.     
-00048a40: 2020 2020 2020 2066 702e 7772 6974 656c         fp.writel
-00048a50: 696e 6573 286c 696e 6573 290a 2020 2020  ines(lines).    
-00048a60: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-00048a70: 2750 6174 6368 2061 7070 6c69 6564 2074  'Patch applied t
-00048a80: 6f20 7b74 6865 5f66 696c 657d 2127 290a  o {the_file}!').
+00047410: 2827 745f 696e 206d 7573 7420 6265 2061  ('t_in must be a
+00047420: 7374 726f 7079 2e74 696d 652e 5469 6d65  stropy.time.Time
+00047430: 206f 626a 6563 7427 290a 0a20 2020 2020   object')..     
+00047440: 2020 2064 7420 3d20 745f 696e 202d 2073     dt = t_in - s
+00047450: 656c 662e 5f74 3139 3835 0a20 2020 2020  elf._t1985.     
+00047460: 2020 2078 797a 203d 2073 656c 662e 6576     xyz = self.ev
+00047470: 616c 7561 7465 2864 742e 7365 632c 202a  aluate(dt.sec, *
+00047480: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
+00047490: 2069 6620 2761 735f 7461 626c 6527 2069   if 'as_table' i
+000474a0: 6e20 6b77 6172 6773 3a0a 2020 2020 2020  n kwargs:.      
+000474b0: 2020 2020 2020 6966 206b 7761 7267 735b        if kwargs[
+000474c0: 2761 735f 7461 626c 6527 5d3a 0a20 2020  'as_table']:.   
+000474d0: 2020 2020 2020 2020 2020 2020 2078 797a               xyz
+000474e0: 5b27 7469 6d65 275d 203d 2074 5f69 6e0a  ['time'] = t_in.
+000474f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00047500: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00047510: 7879 7a0a 0a0a 2020 2020 6465 6620 5f5f  xyz...    def __
+00047520: 6765 7469 7465 6d5f 5f28 7365 6c66 2c20  getitem__(self, 
+00047530: 6b65 7929 3a0a 2020 2020 2020 2020 7265  key):.        re
+00047540: 7475 726e 2073 656c 662e 7061 7261 6d5f  turn self.param_
+00047550: 6469 6374 5b6b 6579 5d0a 0a0a 2020 2020  dict[key]...    
+00047560: 6465 6620 6576 616c 7561 7465 2873 656c  def evaluate(sel
+00047570: 662c 2064 742c 2075 6e69 743d 4e6f 6e65  f, dt, unit=None
+00047580: 2c20 6173 5f74 6162 6c65 3d46 616c 7365  , as_table=False
+00047590: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000475a0: 2020 2020 2020 2045 7661 6c75 6174 6520         Evaluate 
+000475b0: 6571 7561 7469 6f6e 7320 746f 2067 6574  equations to get
+000475c0: 2070 6f73 6974 696f 6e73 0a20 2020 2020   positions.     
+000475d0: 2020 200a 2020 2020 2020 2020 5265 7475     .        Retu
+000475e0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+000475f0: 2d2d 2d0a 2020 2020 2020 2020 782c 2079  ---.        x, y
+00047600: 2c20 7a2c 2072 3a20 666c 6f61 740a 2020  , z, r: float.  
+00047610: 2020 2020 2020 2020 2020 436f 6f72 6469            Coordi
+00047620: 6e61 7465 732c 2069 6e20 6b6d 206f 7220  nates, in km or 
+00047630: 6060 756e 6974 6060 2e0a 2020 2020 2020  ``unit``..      
+00047640: 2020 2020 2020 0a20 2020 2020 2020 2022        .        "
+00047650: 2222 0a20 2020 2020 2020 200a 2020 2020  "".        .    
+00047660: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00047670: 7061 7261 6d5f 6469 6374 3a0a 2020 2020  param_dict:.    
+00047680: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00047690: 6c75 6545 7272 6f72 2827 4f72 6269 7461  lueError('Orbita
+000476a0: 6c20 7061 7261 6d65 7465 7273 206e 6f74  l parameters not
+000476b0: 2064 6566 696e 6564 2069 6e20 270a 2020   defined in '.  
+000476c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000476d0: 2020 2020 2020 2020 2020 2027 7365 6c66             'self
+000476e0: 2e70 6172 616d 5f64 6963 7427 290a 2020  .param_dict').  
+000476f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00047700: 2020 0a20 2020 2020 2020 2070 203d 2073    .        p = s
+00047710: 656c 662e 7061 7261 6d5f 6469 6374 0a20  elf.param_dict. 
+00047720: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00047730: 7420 3d20 6e70 2e61 746c 6561 7374 5f31  t = np.atleast_1
+00047740: 6428 6474 290a 2020 2020 2020 2020 0a20  d(dt).        . 
+00047750: 2020 2020 2020 2023 2045 712e 2031 0a20         # Eq. 1. 
+00047760: 2020 2020 2020 2062 7261 636b 6574 203d         bracket =
+00047770: 2070 5b27 4d2e 275d 2a28 742d 705b 2774   p['M.']*(t-p['t
+00047780: 6175 275d 2920 2b20 302e 352a 705b 274d  au']) + 0.5*p['M
+00047790: 2e2e 275d 2a28 742d 705b 2774 6175 275d  ..']*(t-p['tau']
+000477a0: 292a 2a32 0a20 2020 2020 2020 204d 203d  )**2.        M =
+000477b0: 2070 5b27 4d30 275d 202b 2032 2a6e 702e   p['M0'] + 2*np.
+000477c0: 7069 2a62 7261 636b 6574 0a20 2020 2020  pi*bracket.     
+000477d0: 2020 200a 2020 2020 2020 2020 2320 4571     .        # Eq
+000477e0: 2e20 320a 2020 2020 2020 2020 7369 6e4d  . 2.        sinM
+000477f0: 203d 206e 702e 7369 6e28 4d29 0a20 2020   = np.sin(M).   
+00047800: 2020 2020 2063 6f73 4d20 3d20 6e70 2e63       cosM = np.c
+00047810: 6f73 284d 290a 2020 2020 2020 2020 6520  os(M).        e 
+00047820: 3d20 705b 2765 275d 0a20 2020 2020 2020  = p['e'].       
+00047830: 206e 7520 3d20 4d20 2b20 7369 6e4d 2a28   nu = M + sinM*(
+00047840: 322a 6520 2b20 332a 652a 2a33 2a63 6f73  2*e + 3*e**3*cos
+00047850: 4d2a 2a32 202d 2034 2e2f 332a 652a 2a33  M**2 - 4./3*e**3
+00047860: 2a73 696e 4d2a 2a32 200a 2020 2020 2020  *sinM**2 .      
+00047870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00047880: 202b 2035 2e2f 322a 652a 2a32 2a63 6f73   + 5./2*e**2*cos
+00047890: 4d29 0a20 2020 2020 2020 200a 2020 2020  M).        .    
+000478a0: 2020 2020 2320 4571 2e20 330a 2020 2020      # Eq. 3.    
+000478b0: 2020 2020 7220 3d20 705b 2761 2831 2d65      r = p['a(1-e
+000478c0: 2a2a 3229 275d 2f28 312b 652a 6e70 2e63  **2)']/(1+e*np.c
+000478d0: 6f73 286e 7529 290a 2020 2020 2020 2020  os(nu)).        
+000478e0: 2320 546f 206b 6d0a 2020 2020 2020 2020  # To km.        
+000478f0: 7220 2f3d 2031 3030 302e 0a20 2020 2020  r /= 1000..     
+00047900: 2020 200a 2020 2020 2020 2020 2320 4571     .        # Eq
+00047910: 2e20 340a 2020 2020 2020 2020 4f6d 203d  . 4.        Om =
+00047920: 2032 2a6e 702e 7069 2a28 705b 274f 6d30   2*np.pi*(p['Om0
+00047930: 275d 202b 2070 5b27 4f6d 2e27 5d2a 2874  '] + p['Om.']*(t
+00047940: 2d70 5b27 7461 7527 5d29 290a 2020 2020  -p['tau'])).    
+00047950: 2020 2020 0a20 2020 2020 2020 2023 2045      .        # E
+00047960: 712e 2035 0a20 2020 2020 2020 2077 203d  q. 5.        w =
+00047970: 2032 2a6e 702e 7069 2a28 705b 2777 3027   2*np.pi*(p['w0'
+00047980: 5d20 2b20 705b 2777 2e27 5d2a 2874 2d70  ] + p['w.']*(t-p
+00047990: 5b27 7461 7527 5d29 290a 2020 2020 2020  ['tau'])).      
+000479a0: 2020 0a20 2020 2020 2020 2073 656c 662e    .        self.
+000479b0: 6361 6c63 5f64 6963 7420 3d20 7b27 4d27  calc_dict = {'M'
+000479c0: 3a4d 2c20 276e 7527 3a6e 752c 200a 2020  :M, 'nu':nu, .  
+000479d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000479e0: 2020 2020 2020 2020 2761 273a 705b 2761          'a':p['a
+000479f0: 275d 2c20 0a20 2020 2020 2020 2020 2020  '], .           
+00047a00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00047a10: 6927 3a6e 702e 6172 6373 696e 2870 5b27  i':np.arcsin(p['
+00047a20: 7369 6e69 275d 292c 200a 2020 2020 2020  sini']), .      
+00047a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00047a40: 2020 2020 274f 6d27 3a4f 6d2c 0a20 2020      'Om':Om,.   
+00047a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00047a60: 2020 2020 2020 2027 7727 3a77 7d0a 2020         'w':w}.  
+00047a70: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00047a80: 2045 712e 2036 0a20 2020 2020 2020 2063   Eq. 6.        c
+00047a90: 6f73 4f6d 203d 206e 702e 636f 7328 4f6d  osOm = np.cos(Om
+00047aa0: 290a 2020 2020 2020 2020 7369 6e4f 6d20  ).        sinOm 
+00047ab0: 3d20 6e70 2e73 696e 284f 6d29 0a20 2020  = np.sin(Om).   
+00047ac0: 2020 2020 2063 6f73 7776 203d 206e 702e       coswv = np.
+00047ad0: 636f 7328 772b 6e75 290a 2020 2020 2020  cos(w+nu).      
+00047ae0: 2020 7369 6e77 7620 3d20 6e70 2e73 696e    sinwv = np.sin
+00047af0: 2877 2b6e 7529 0a20 2020 2020 2020 200a  (w+nu).        .
+00047b00: 2020 2020 2020 2020 6966 2075 6e69 7420          if unit 
+00047b10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00047b20: 2020 2020 2020 2020 2072 203d 2028 722a           r = (r*
+00047b30: 752e 6b6d 292e 746f 2875 6e69 7429 0a20  u.km).to(unit). 
+00047b40: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00047b50: 2020 2020 7820 3d20 722a 2863 6f73 4f6d      x = r*(cosOm
+00047b60: 2a63 6f73 7776 202d 2070 5b27 636f 7369  *coswv - p['cosi
+00047b70: 275d 2a73 696e 4f6d 2a73 696e 7776 290a  ']*sinOm*sinwv).
+00047b80: 2020 2020 2020 2020 7920 3d20 722a 2873          y = r*(s
+00047b90: 696e 4f6d 2a63 6f73 7776 202b 2070 5b27  inOm*coswv + p['
+00047ba0: 636f 7369 275d 2a63 6f73 4f6d 2a73 696e  cosi']*cosOm*sin
+00047bb0: 7776 290a 2020 2020 2020 2020 7a20 3d20  wv).        z = 
+00047bc0: 722a 705b 2773 696e 6927 5d2a 7369 6e77  r*p['sini']*sinw
+00047bd0: 760a 2020 2020 2020 2020 0a20 2020 2020  v.        .     
+00047be0: 2020 2069 6620 6173 5f74 6162 6c65 3a0a     if as_table:.
+00047bf0: 2020 2020 2020 2020 2020 2020 7461 6220              tab 
+00047c00: 3d20 4754 6162 6c65 2829 0a20 2020 2020  = GTable().     
+00047c10: 2020 2020 2020 2074 6162 5b27 6474 275d         tab['dt']
+00047c20: 203d 2074 0a20 2020 2020 2020 2020 2020   = t.           
+00047c30: 2074 6162 5b27 7827 5d20 3d20 780a 2020   tab['x'] = x.  
+00047c40: 2020 2020 2020 2020 2020 7461 625b 2779            tab['y
+00047c50: 275d 203d 2079 0a20 2020 2020 2020 2020  '] = y.         
+00047c60: 2020 2074 6162 5b27 7a27 5d20 3d20 7a0a     tab['z'] = z.
+00047c70: 2020 2020 2020 2020 2020 2020 7461 625b              tab[
+00047c80: 2772 275d 203d 2072 0a20 2020 2020 2020  'r'] = r.       
+00047c90: 2020 2020 2072 6574 7572 6e20 7461 620a       return tab.
+00047ca0: 2020 2020 2020 2020 656c 7365 3a20 0a20          else: . 
+00047cb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00047cc0: 6e20 782c 2079 2c20 7a2c 2072 0a0a 0a20  n x, y, z, r... 
+00047cd0: 2020 2064 6566 2066 726f 6d5f 666c 7428     def from_flt(
+00047ce0: 7365 6c66 2c20 666c 745f 6669 6c65 2c20  self, flt_file, 
+00047cf0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00047d00: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00047d10: 6f6d 7075 7465 2070 6f73 6974 696f 6e73  ompute positions
+00047d20: 2061 7420 6578 7073 7461 7274 2c20 6578   at expstart, ex
+00047d30: 706d 6964 2c20 6578 7065 6e64 0a20 2020  pmid, expend.   
+00047d40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00047d50: 2069 6d70 6f72 7420 6173 7472 6f70 792e   import astropy.
+00047d60: 7469 6d65 0a20 2020 2020 2020 200a 2020  time.        .  
+00047d70: 2020 2020 2020 666c 7420 3d20 7079 6669        flt = pyfi
+00047d80: 7473 2e6f 7065 6e28 666c 745f 6669 6c65  ts.open(flt_file
+00047d90: 290a 2020 2020 2020 2020 6578 7073 7461  ).        expsta
+00047da0: 7274 203d 2066 6c74 5b30 5d2e 6865 6164  rt = flt[0].head
+00047db0: 6572 5b27 4558 5053 5441 5254 275d 0a20  er['EXPSTART']. 
+00047dc0: 2020 2020 2020 2065 7870 656e 6420 3d20         expend = 
+00047dd0: 666c 745b 305d 2e68 6561 6465 725b 2745  flt[0].header['E
+00047de0: 5850 454e 4427 5d0a 2020 2020 2020 2020  XPEND'].        
+00047df0: 6578 706d 6964 203d 2028 6578 7073 7461  expmid = (expsta
+00047e00: 7274 2b65 7870 656e 6429 2f32 2e0a 2020  rt+expend)/2..  
+00047e10: 2020 2020 2020 0a20 2020 2020 2020 2074        .        t
+00047e20: 5f69 6e20 3d20 6173 7472 6f70 792e 7469  _in = astropy.ti
+00047e30: 6d65 2e54 696d 6528 5b65 7870 7374 6172  me.Time([expstar
+00047e40: 742c 2065 7870 6d69 642c 2065 7870 656e  t, expmid, expen
+00047e50: 645d 2c20 666f 726d 6174 3d27 6d6a 6427  d], format='mjd'
+00047e60: 290a 2020 2020 2020 2020 666c 742e 636c  ).        flt.cl
+00047e70: 6f73 6528 290a 2020 2020 2020 2020 0a20  ose().        . 
+00047e80: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00047e90: 6c66 2874 5f69 6e2c 202a 2a6b 7761 7267  lf(t_in, **kwarg
+00047ea0: 7329 0a0a 0a20 2020 2064 6566 2064 656c  s)...    def del
+00047eb0: 7461 7428 7365 6c66 2c20 6474 293a 0a20  tat(self, dt):. 
+00047ec0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00047ed0: 2020 2043 6f6e 7665 7274 2061 2074 696d     Convert a tim
+00047ee0: 6520 6060 7460 6020 696e 2073 6563 6f6e  e ``t`` in secon
+00047ef0: 6473 2066 726f 6d20 312f 312f 3835 2074  ds from 1/1/85 t
+00047f00: 6f20 616e 2049 534f 2074 696d 650a 2020  o an ISO time.  
+00047f10: 2020 2020 2020 2222 2220 2020 200a 2020        """    .  
+00047f20: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
+00047f30: 6174 7472 2864 742c 2027 756e 6974 2729  attr(dt, 'unit')
+00047f40: 3a0a 2020 2020 2020 2020 2020 2020 6474  :.            dt
+00047f50: 7365 6320 3d20 6474 2a75 2e73 6563 6f6e  sec = dt*u.secon
+00047f60: 640a 2020 2020 2020 2020 656c 7365 3a0a  d.        else:.
+00047f70: 2020 2020 2020 2020 2020 2020 6474 7365              dtse
+00047f80: 6320 3d20 6474 0a20 2020 2020 2020 2020  c = dt.         
+00047f90: 2020 200a 2020 2020 2020 2020 7420 3d20     .        t = 
+00047fa0: 7365 6c66 2e5f 7431 3938 3520 2b20 6474  self._t1985 + dt
+00047fb0: 7365 630a 2020 2020 2020 2020 7265 7475  sec.        retu
+00047fc0: 726e 2074 0a0a 0a20 2020 2064 6566 2070  rn t...    def p
+00047fd0: 6172 7365 5f66 726f 6d5f 7370 7428 7365  arse_from_spt(se
+00047fe0: 6c66 2c20 7370 745f 6669 6c65 293a 0a20  lf, spt_file):. 
+00047ff0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00048000: 2020 2047 6574 206f 7262 6974 616c 2065     Get orbital e
+00048010: 6c65 6d65 6e74 7320 6672 6f6d 2053 5054  lements from SPT
+00048020: 2068 6561 6465 720a 2020 2020 2020 2020   header.        
+00048030: 2222 220a 2020 2020 2020 2020 696d 706f  """.        impo
+00048040: 7274 2061 7374 726f 7079 2e69 6f2e 6669  rt astropy.io.fi
+00048050: 7473 2061 7320 7079 6669 7473 0a20 2020  ts as pyfits.   
+00048060: 2020 2020 2069 6d70 6f72 7420 6173 7472       import astr
+00048070: 6f70 792e 7469 6d65 0a20 2020 2020 2020  opy.time.       
+00048080: 200a 2020 2020 2020 2020 7769 7468 2070   .        with p
+00048090: 7966 6974 732e 6f70 656e 2873 7074 5f66  yfits.open(spt_f
+000480a0: 696c 6529 2061 7320 5f69 6d3a 0a20 2020  ile) as _im:.   
+000480b0: 2020 2020 2020 2020 2073 7074 203d 205f           spt = _
+000480c0: 696d 5b30 5d2e 6865 6164 6572 2e63 6f70  im[0].header.cop
+000480d0: 7928 290a 2020 2020 2020 2020 0a20 2020  y().        .   
+000480e0: 2020 2020 2070 6172 616d 5f64 6963 7420       param_dict 
+000480f0: 3d20 7b7d 0a20 2020 2020 2020 2070 6172  = {}.        par
+00048100: 616d 5f64 6963 745b 2774 6175 275d 203d  am_dict['tau'] =
+00048110: 2073 7074 5b27 4550 4348 5449 4d45 275d   spt['EPCHTIME']
+00048120: 0a20 2020 2020 2020 2070 6172 616d 5f64  .        param_d
+00048130: 6963 745b 274d 3027 5d20 3d20 7370 745b  ict['M0'] = spt[
+00048140: 274d 4541 4e41 4e4f 4d27 5d0a 2020 2020  'MEANANOM'].    
+00048150: 2020 2020 7061 7261 6d5f 6469 6374 5b27      param_dict['
+00048160: 4d2e 275d 203d 2073 7074 5b27 4644 4d45  M.'] = spt['FDME
+00048170: 414e 414e 275d 0a20 2020 2020 2020 2070  ANAN'].        p
+00048180: 6172 616d 5f64 6963 745b 274d 2e2e 275d  aram_dict['M..']
+00048190: 203d 2073 7074 5b27 5344 4d45 414e 414e   = spt['SDMEANAN
+000481a0: 275d 0a20 2020 2020 2020 2070 6172 616d  '].        param
+000481b0: 5f64 6963 745b 2765 275d 203d 2073 7074  _dict['e'] = spt
+000481c0: 5b27 4543 4345 4e54 5259 275d 0a20 2020  ['ECCENTRY'].   
+000481d0: 2020 2020 2070 6172 616d 5f64 6963 745b       param_dict[
+000481e0: 2761 2831 2d65 2a2a 3229 275d 203d 2073  'a(1-e**2)'] = s
+000481f0: 7074 5b27 5345 4d49 4c52 4543 275d 0a20  pt['SEMILREC']. 
+00048200: 2020 2020 2020 2070 6172 616d 5f64 6963         param_dic
+00048210: 745b 2761 275d 203d 2070 6172 616d 5f64  t['a'] = param_d
+00048220: 6963 745b 2761 2831 2d65 2a2a 3229 275d  ict['a(1-e**2)']
+00048230: 202f 2028 312d 7061 7261 6d5f 6469 6374   / (1-param_dict
+00048240: 5b27 6527 5d2a 2a32 290a 2020 2020 2020  ['e']**2).      
+00048250: 2020 7061 7261 6d5f 6469 6374 5b27 4f6d    param_dict['Om
+00048260: 3027 5d20 3d20 7370 745b 2752 4153 4341  0'] = spt['RASCA
+00048270: 5343 4e27 5d0a 2020 2020 2020 2020 7061  SCN'].        pa
+00048280: 7261 6d5f 6469 6374 5b27 4f6d 2e27 5d20  ram_dict['Om.'] 
+00048290: 3d20 7370 745b 2752 4341 5343 4e52 5627  = spt['RCASCNRV'
+000482a0: 5d0a 2020 2020 2020 2020 7061 7261 6d5f  ].        param_
+000482b0: 6469 6374 5b27 7730 275d 203d 2073 7074  dict['w0'] = spt
+000482c0: 5b27 4152 4750 4552 4947 275d 0a20 2020  ['ARGPERIG'].   
+000482d0: 2020 2020 2070 6172 616d 5f64 6963 745b       param_dict[
+000482e0: 2777 2e27 5d20 3d20 7370 745b 2752 4341  'w.'] = spt['RCA
+000482f0: 5247 5045 5227 5d0a 2020 2020 2020 2020  RGPER'].        
+00048300: 7061 7261 6d5f 6469 6374 5b27 636f 7369  param_dict['cosi
+00048310: 275d 203d 2073 7074 5b27 434f 5349 4e43  '] = spt['COSINC
+00048320: 4c49 275d 0a20 2020 2020 2020 2070 6172  LI'].        par
+00048330: 616d 5f64 6963 745b 2773 696e 6927 5d20  am_dict['sini'] 
+00048340: 3d20 7370 745b 2753 494e 4549 4e43 4c27  = spt['SINEINCL'
+00048350: 5d0a 2020 2020 2020 2020 7061 7261 6d5f  ].        param_
+00048360: 6469 6374 5b27 5663 275d 203d 2073 7074  dict['Vc'] = spt
+00048370: 5b27 4349 5256 454c 4f43 275d 0a20 2020  ['CIRVELOC'].   
+00048380: 2020 2020 2070 6172 616d 5f64 6963 745b       param_dict[
+00048390: 2774 696d 6566 6665 6327 5d20 3d20 7370  'timeffec'] = sp
+000483a0: 745b 2754 494d 4546 4645 4327 5d0a 2020  t['TIMEFFEC'].  
+000483b0: 2020 2020 2020 7061 7261 6d5f 6469 6374        param_dict
+000483c0: 5b27 546f 7262 275d 203d 2073 7074 5b27  ['Torb'] = spt['
+000483d0: 4853 5448 4f52 4227 5d2a 320a 2020 2020  HSTHORB']*2.    
+000483e0: 2020 2020 7061 7261 6d5f 6469 6374 5b27      param_dict['
+000483f0: 7473 7461 7274 275d 203d 2073 7074 5b27  tstart'] = spt['
+00048400: 4f42 5353 5452 5454 275d 0a20 2020 2020  OBSSTRTT'].     
+00048410: 2020 200a 2020 2020 2020 2020 7061 7261     .        para
+00048420: 6d5f 6469 6374 5b27 7461 755f 7469 6d65  m_dict['tau_time
+00048430: 275d 203d 2073 656c 662e 6465 6c74 6174  '] = self.deltat
+00048440: 2870 6172 616d 5f64 6963 745b 2774 6175  (param_dict['tau
+00048450: 275d 290a 2020 2020 2020 2020 7061 7261  ']).        para
+00048460: 6d5f 6469 6374 5b27 7473 7461 7274 5f74  m_dict['tstart_t
+00048470: 696d 6527 5d20 3d20 7365 6c66 2e64 656c  ime'] = self.del
+00048480: 7461 7428 7061 7261 6d5f 6469 6374 5b27  tat(param_dict['
+00048490: 7473 7461 7274 275d 290a 2020 2020 2020  tstart']).      
+000484a0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+000484b0: 2020 2072 6574 7572 6e20 7061 7261 6d5f     return param_
+000484c0: 6469 6374 0a20 2020 200a 2020 2020 4073  dict.    .    @s
+000484d0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+000484e0: 6465 6620 7879 7a5f 746f 5f6c 6f6e 6c61  def xyz_to_lonla
+000484f0: 7428 7365 6c66 2c20 782c 2079 2c20 7a2c  t(self, x, y, z,
+00048500: 2072 6164 6961 6e73 3d46 616c 7365 293a   radians=False):
+00048510: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00048520: 2020 2020 2043 6f6d 7075 7465 2073 7562       Compute sub
+00048530: 6c6f 6e2c 2073 7562 6c61 742c 2061 6c74  lon, sublat, alt
+00048540: 2066 726f 6d20 7879 7a20 636f 6f72 6473   from xyz coords
+00048550: 2077 6974 6820 7079 7072 6f6a 0a20 2020   with pyproj.   
+00048560: 2020 2020 200a 2020 2020 2020 2020 7879       .        xy
+00048570: 7a20 6d75 7374 2062 6520 696e 206d 6574  z must be in met
+00048580: 6572 730a 2020 2020 2020 2020 0a20 2020  ers.        .   
+00048590: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000485a0: 2069 6d70 6f72 7420 7079 7072 6f6a 0a20   import pyproj. 
+000485b0: 2020 2020 2020 2065 6365 6620 3d20 7079         ecef = py
+000485c0: 7072 6f6a 2e50 726f 6a28 7072 6f6a 3d27  proj.Proj(proj='
+000485d0: 6765 6f63 656e 7427 2c20 656c 6c70 733d  geocent', ellps=
+000485e0: 2757 4753 3834 272c 2064 6174 756d 3d27  'WGS84', datum='
+000485f0: 5747 5338 3427 290a 2020 2020 2020 2020  WGS84').        
+00048600: 6c6c 6120 3d20 7079 7072 6f6a 2e50 726f  lla = pyproj.Pro
+00048610: 6a28 7072 6f6a 3d27 6c61 746c 6f6e 6727  j(proj='latlong'
+00048620: 2c20 656c 6c70 733d 2757 4753 3834 272c  , ellps='WGS84',
+00048630: 2064 6174 756d 3d27 5747 5338 3427 290a   datum='WGS84').
+00048640: 2020 2020 2020 2020 6c6f 6e2c 206c 6174          lon, lat
+00048650: 2c20 616c 7420 3d20 7079 7072 6f6a 2e74  , alt = pyproj.t
+00048660: 7261 6e73 666f 726d 2865 6365 662c 206c  ransform(ecef, l
+00048670: 6c61 2c20 782c 2079 2c20 7a2c 2072 6164  la, x, y, z, rad
+00048680: 6961 6e73 3d72 6164 6961 6e73 290a 2020  ians=radians).  
+00048690: 2020 2020 2020 7265 7475 726e 206c 6f6e        return lon
+000486a0: 2c20 6c61 742c 2061 6c74 0a0a 0a64 6566  , lat, alt...def
+000486b0: 2070 6174 6368 5f70 686f 7475 7469 6c73   patch_photutils
+000486c0: 2829 3a0a 2020 2020 2222 220a 2020 2020  ():.    """.    
+000486d0: 5061 7463 6820 746f 2066 6978 2069 6e63  Patch to fix inc
+000486e0: 6f6e 7369 7374 656e 6379 2077 6974 6820  onsistency with 
+000486f0: 6472 697a 7a6c 6570 6163 3d33 2e32 2e31  drizzlepac=3.2.1
+00048700: 2061 6e64 2070 686f 7475 7469 6c73 3e31   and photutils>1
+00048710: 2e30 2c20 7768 6572 6520 0a20 2020 2054  .0, where .    T
+00048720: 6865 206c 6174 7465 7220 6973 206e 6565  he latter is nee
+00048730: 6465 6420 666f 7220 6a77 7374 3d31 2e33  ded for jwst=1.3
+00048740: 2e32 0a20 2020 2022 2222 0a20 2020 2069  .2.    """.    i
+00048750: 6d70 6f72 7420 6f73 0a0a 2020 2020 7472  mport os..    tr
+00048760: 793a 0a20 2020 2020 2020 2069 6d70 6f72  y:.        impor
+00048770: 7420 6472 697a 7a6c 6570 6163 0a20 2020  t drizzlepac.   
+00048780: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
+00048790: 6545 7272 6f72 3a0a 2020 2020 0a20 2020  eError:.    .   
+000487a0: 2020 2020 2069 6d70 6f72 7420 7068 6f74       import phot
+000487b0: 7574 696c 730a 2020 2020 2020 2020 7369  utils.        si
+000487c0: 7465 5f70 6163 6b61 6765 7320 3d20 6f73  te_packages = os
+000487d0: 2e70 6174 682e 6469 726e 616d 6528 7068  .path.dirname(ph
+000487e0: 6f74 7574 696c 732e 5f5f 6669 6c65 5f5f  otutils.__file__
+000487f0: 290a 2020 2020 2020 2020 2320 6d61 6e75  ).        # manu
+00048800: 616c 2061 7070 6c79 2070 6174 6368 0a20  al apply patch. 
+00048810: 2020 2020 2020 2074 6865 5f66 696c 6520         the_file 
+00048820: 3d20 6627 7b73 6974 655f 7061 636b 6167  = f'{site_packag
+00048830: 6573 7d2f 2e2e 2f64 7269 7a7a 6c65 7061  es}/../drizzlepa
+00048840: 632f 6861 7075 7469 6c73 2f61 6c69 676e  c/haputils/align
+00048850: 5f75 7469 6c73 2e70 7927 0a20 2020 2020  _utils.py'.     
+00048860: 2020 2077 6974 6820 6f70 656e 2874 6865     with open(the
+00048870: 5f66 696c 652c 2772 2729 2061 7320 6670  _file,'r') as fp
+00048880: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
+00048890: 6e65 7320 3d20 6670 2e72 6561 646c 696e  nes = fp.readlin
+000488a0: 6573 2829 0a20 2020 200a 2020 2020 2020  es().    .      
+000488b0: 2020 7072 696e 7428 7369 7465 5f70 6163    print(site_pac
+000488c0: 6b61 6765 732c 206c 656e 286c 696e 6573  kages, len(lines
+000488d0: 2929 0a20 2020 2020 2020 2066 6f72 2069  )).        for i
+000488e0: 2c20 6c69 6e65 2069 6e20 656e 756d 6572  , line in enumer
+000488f0: 6174 6528 6c69 6e65 7329 3a0a 2020 2020  ate(lines):.    
+00048900: 2020 2020 2020 2020 6966 206c 696e 652e          if line.
+00048910: 7374 6172 7473 7769 7468 2827 4e6f 4465  startswith('NoDe
+00048920: 7465 6374 696f 6e73 5761 726e 696e 6727  tectionsWarning'
+00048930: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00048940: 2020 2062 7265 616b 0a20 2020 200a 2020     break.    .  
+00048950: 2020 2020 2020 6966 2027 6861 7361 7474        if 'hasatt
+00048960: 7228 7068 6f74 7574 696c 732e 6669 6e64  r(photutils.find
+00048970: 7374 6172 7327 2069 6e20 6c69 6e65 735b  stars' in lines[
+00048980: 692b 315d 3a0a 2020 2020 2020 2020 2020  i+1]:.          
+00048990: 2020 7072 696e 7428 6627 4920 666f 756e    print(f'I foun
+000489a0: 6420 7468 6520 7072 6f62 6c65 6d20 6f6e  d the problem on
+000489b0: 206c 696e 6573 207b 697d 2d7b 692b 327d   lines {i}-{i+2}
+000489c0: 3a20 2729 0a20 2020 2020 2020 2065 6c73  : ').        els
+000489d0: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
+000489e0: 7367 203d 2022 2222 0a4c 696e 6573 207b  sg = """.Lines {
+000489f0: 307d 2d7b 317d 2069 6e20 7b32 7d20 696d  0}-{1} in {2} im
+00048a00: 706f 7274 696e 6720 7068 6f74 7574 696c  porting photutil
+00048a10: 7320 7765 7265 206e 6f74 2061 7320 6578  s were not as ex
+00048a20: 7065 6374 6564 2e20 2049 2066 6f75 6e64  pected.  I found
+00048a30: 200a 0a7b 337d 0a0a 6275 7420 6578 7065   ..{3}..but expe
+00048a40: 6374 6564 200a 0a20 2020 4e6f 4465 7465  cted ..   NoDete
+00048a50: 6374 696f 6e73 5761 726e 696e 6720 3d20  ctionsWarning = 
+00048a60: 7068 6f74 7574 696c 732e 6669 6e64 7374  photutils.findst
+00048a70: 6172 732e 4e6f 4465 7465 6374 696f 6e73  ars.NoDetections
+00048a80: 5761 726e 696e 6720 6966 205c 5c0a 2020  Warning if \\.  
+00048a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00048aa0: 2020 2020 2020 2020 2068 6173 6174 7472           hasattr
+00048ab0: 2870 686f 7475 7469 6c73 2e66 696e 6473  (photutils.finds
+00048ac0: 7461 7273 2c20 274e 6f44 6574 6563 7469  tars, 'NoDetecti
+00048ad0: 6f6e 7357 6172 6e69 6e67 2729 2065 6c73  onsWarning') els
+00048ae0: 6520 5c5c 0a20 2020 2020 2020 2020 2020  e \\.           
+00048af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00048b00: 7068 6f74 7574 696c 732e 7574 696c 732e  photutils.utils.
+00048b10: 4e6f 4465 7465 6374 696f 6e73 5761 726e  NoDetectionsWarn
+00048b20: 696e 670a 0a0a 2020 2020 2222 222e 666f  ing...    """.fo
+00048b30: 726d 6174 2869 2c20 692b 322c 2074 6865  rmat(i, i+2, the
+00048b40: 5f66 696c 652c 206c 696e 6573 5b69 3a69  _file, lines[i:i
+00048b50: 2b33 5d29 0a20 2020 2020 2020 200a 2020  +3]).        .  
+00048b60: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00048b70: 5661 6c75 6545 7272 6f72 286d 7367 290a  ValueError(msg).
+00048b80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00048b90: 2062 6164 203d 205b 2720 2020 272b 6c69   bad = ['   '+li
+00048ba0: 6e65 732e 706f 7028 692b 322d 6a29 2066  nes.pop(i+2-j) f
+00048bb0: 6f72 206a 2069 6e20 7261 6e67 6528 3329  or j in range(3)
+00048bc0: 5d0a 2020 2020 2020 2020 7072 696e 7428  ].        print(
+00048bd0: 2727 2e6a 6f69 6e28 6261 645b 3a3a 2d31  ''.join(bad[::-1
+00048be0: 5d29 290a 0a20 2020 2020 2020 2023 2049  ]))..        # I
+00048bf0: 6e73 6572 7420 7468 6520 6669 780a 2020  nsert the fix.  
+00048c00: 2020 2020 2020 6c69 6e65 735b 695d 203d        lines[i] =
+00048c10: 2027 6672 6f6d 2070 686f 7475 7469 6c73   'from photutils
+00048c20: 2e75 7469 6c73 2e65 7863 6570 7469 6f6e  .utils.exception
+00048c30: 7320 696d 706f 7274 204e 6f44 6574 6563  s import NoDetec
+00048c40: 7469 6f6e 7357 6172 6e69 6e67 5c6e 5c6e  tionsWarning\n\n
+00048c50: 270a 2020 2020 2020 2020 2320 5265 7772  '.        # Rewr
+00048c60: 6974 6520 7468 6520 6669 650a 2020 2020  ite the fie.    
+00048c70: 2020 2020 7769 7468 206f 7065 6e28 6627      with open(f'
+00048c80: 7b73 6974 655f 7061 636b 6167 6573 7d2f  {site_packages}/
+00048c90: 2e2e 2f64 7269 7a7a 6c65 7061 632f 6861  ../drizzlepac/ha
+00048ca0: 7075 7469 6c73 2f61 6c69 676e 5f75 7469  putils/align_uti
+00048cb0: 6c73 2e70 7927 2c27 7727 2920 6173 2066  ls.py','w') as f
+00048cc0: 703a 0a20 2020 2020 2020 2020 2020 2066  p:.            f
+00048cd0: 702e 7772 6974 656c 696e 6573 286c 696e  p.writelines(lin
+00048ce0: 6573 290a 2020 2020 0a20 2020 2020 2020  es).    .       
+00048cf0: 2070 7269 6e74 2866 2750 6174 6368 2061   print(f'Patch a
+00048d00: 7070 6c69 6564 2074 6f20 7b74 6865 5f66  pplied to {the_f
+00048d10: 696c 657d 2127 290a                      ile}!').
```

### Comparing `grizli-1.8.5/grizli/utils_c/disperse.c` & `grizli-1.8.7/grizli/utils_c/disperse.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "grizli.utils_c.disperse",
         "sources": [
             "grizli/utils_c/disperse.pyx"
@@ -1051,195 +1051,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1320,42 +1320,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3498,15 +3498,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ysens.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3515,29 +3515,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3548,15 +3548,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3565,29 +3565,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3598,15 +3598,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3615,29 +3615,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3648,15 +3648,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3665,29 +3665,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3698,15 +3698,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3715,29 +3715,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3748,212 +3748,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3969,15 +3969,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3985,53 +3985,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -4039,30 +4039,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4077,15 +4077,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4101,15 +4101,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4117,53 +4117,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -4171,30 +4171,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4209,15 +4209,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4233,15 +4233,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4249,53 +4249,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -4303,30 +4303,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4341,176 +4341,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4625,26 +4625,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
@@ -5115,15 +5115,15 @@
  * import numpy as np
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `grizli-1.8.5/grizli/utils_c/disperse.pyx` & `grizli-1.8.7/grizli/utils_c/disperse.pyx`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli/utils_c/interp.c` & `grizli-1.8.7/grizli/utils_c/interp.c`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "grizli.utils_c.interp",
         "sources": [
             "grizli/utils_c/interp.pyx"
@@ -1051,195 +1051,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1293,42 +1293,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -9106,15 +9106,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_zgrid.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9123,29 +9123,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9156,15 +9156,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9173,29 +9173,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9206,15 +9206,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9223,29 +9223,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9256,15 +9256,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9273,29 +9273,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9306,15 +9306,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9323,29 +9323,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9356,212 +9356,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9577,15 +9577,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -9593,53 +9593,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -9647,30 +9647,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9685,15 +9685,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9709,15 +9709,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9725,53 +9725,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -9779,30 +9779,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9817,15 +9817,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9841,15 +9841,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9857,53 +9857,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -9911,30 +9911,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9949,176 +9949,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -10332,26 +10332,26 @@
   __pyx_slice_ = PySlice_New(__pyx_int_1, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
   __pyx_slice__2 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__2);
   __Pyx_GIVEREF(__pyx_slice__2);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 951, __pyx_L1_error)
@@ -11030,15 +11030,15 @@
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_run_nmf_line_454, __pyx_kp_u_run_nmf_flux_variance_templates) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../../../tmp/build-env-pd2mk51r/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-1andkqn4/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `grizli-1.8.5/grizli/utils_c/interp.pyx` & `grizli-1.8.7/grizli/utils_c/interp.pyx`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/grizli.egg-info/PKG-INFO` & `grizli-1.8.7/grizli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizli
-Version: 1.8.5
+Version: 1.8.7
 Summary: Grism redshift and line analysis software
 Home-page: https://github.com/gbrammer/grizli
 Author: G. Brammer
 Author-email: gbrammer@gmail.com
 License: MIT
 Project-URL: Documentation, https://grizli.readthedocs.io/
 Project-URL: Source, https://github.com/gbrammer/grizli
```

### Comparing `grizli-1.8.5/grizli.egg-info/SOURCES.txt` & `grizli-1.8.7/grizli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/setup.cfg` & `grizli-1.8.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/setup.py` & `grizli-1.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `grizli-1.8.5/test_pipeline_hst.py` & `grizli-1.8.7/test_pipeline_hst.py`

 * *Files identical despite different names*

