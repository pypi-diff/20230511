# Comparing `tmp/adafruit-circuitpython-bitmap_font-1.5.8.tar.gz` & `tmp/adafruit-circuitpython-bitmap_font-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bitmap_font-1.5.8.tar", last modified: Thu Jun  9 18:33:34 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bitmap_font-1.5.9.tar", last modified: Tue Aug  9 19:57:17 2022, max compression
```

## Comparing `adafruit-circuitpython-bitmap_font-1.5.8.tar` & `adafruit-circuitpython-bitmap_font-1.5.9.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.310149 adafruit-circuitpython-bitmap_font-1.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.298149 adafruit-circuitpython-bitmap_font-1.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.302149 adafruit-circuitpython-bitmap_font-1.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.302149 adafruit-circuitpython-bitmap_font-1.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.302149 adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4310 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/OFL-1.1-RFN.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2022-06-09 18:33:34.310149 adafruit-circuitpython-bitmap_font-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3014 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.302149 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8273 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/bdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/bitmap_font.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/glyph_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    13683 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/pcf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/ttf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.306149 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_circuitpython_bitmap_font.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2022-06-09 18:33:34.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_circuitpython_bitmap_font.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-06-09 18:33:34.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_circuitpython_bitmap_font.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:33:34.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_circuitpython_bitmap_font.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-09 18:33:34.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_circuitpython_bitmap_font.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-09 18:33:34.000000 adafruit-circuitpython-bitmap_font-1.5.8/adafruit_circuitpython_bitmap_font.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.306149 adafruit-circuitpython-bitmap_font-1.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.306149 adafruit-circuitpython-bitmap_font-1.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.306149 adafruit-circuitpython-bitmap_font-1.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_displayio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)    17036 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_forkawesome_icons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_label_forkawesome.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_label_magtag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_label_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.310149 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    62897 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/Junction-regular-24.bdf
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/Junction-regular-24.bdf.license
--rw-r--r--   0 runner    (1001) docker     (121)   163036 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/Junction-regular-24.pcf
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/Junction-regular-24.pcf.license
--rw-r--r--   0 runner    (1001) docker     (121)    86848 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/LeagueSpartan-Bold-16.bdf
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/LeagueSpartan-Bold-16.bdf.license
--rw-r--r--   0 runner    (1001) docker     (121)   477640 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/forkawesome-42.pcf
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/forkawesome-42.pcf.license
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:33:34.310149 adafruit-circuitpython-bitmap_font-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:33:34.310149 adafruit-circuitpython-bitmap_font-1.5.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/test/displayio.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-06-09 18:33:22.000000 adafruit-circuitpython-bitmap_font-1.5.8/test/fontio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.221435 adafruit-circuitpython-bitmap_font-1.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.217435 adafruit-circuitpython-bitmap_font-1.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.217435 adafruit-circuitpython-bitmap_font-1.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.217435 adafruit-circuitpython-bitmap_font-1.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.217435 adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4310 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/OFL-1.1-RFN.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-08-09 19:57:17.221435 adafruit-circuitpython-bitmap_font-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.217435 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8266 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/bitmap_font.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/glyph_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13683 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/pcf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/ttf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.217435 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_circuitpython_bitmap_font.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-08-09 19:57:17.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_circuitpython_bitmap_font.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-08-09 19:57:17.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_circuitpython_bitmap_font.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:57:17.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_circuitpython_bitmap_font.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-09 19:57:17.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_circuitpython_bitmap_font.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-09 19:57:17.000000 adafruit-circuitpython-bitmap_font-1.5.9/adafruit_circuitpython_bitmap_font.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.221435 adafruit-circuitpython-bitmap_font-1.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.221435 adafruit-circuitpython-bitmap_font-1.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.221435 adafruit-circuitpython-bitmap_font-1.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_displayio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17036 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_forkawesome_icons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_label_forkawesome.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_label_magtag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_label_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.221435 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)    62897 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/Junction-regular-24.bdf
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/Junction-regular-24.bdf.license
+-rw-r--r--   0 runner    (1001) docker     (121)   163036 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/Junction-regular-24.pcf
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/Junction-regular-24.pcf.license
+-rw-r--r--   0 runner    (1001) docker     (121)    86848 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/LeagueSpartan-Bold-16.bdf
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/LeagueSpartan-Bold-16.bdf.license
+-rw-r--r--   0 runner    (1001) docker     (121)   477640 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/forkawesome-42.pcf
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/forkawesome-42.pcf.license
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-08-09 19:56:57.000000 adafruit-circuitpython-bitmap_font-1.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:57:17.221435 adafruit-circuitpython-bitmap_font-1.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:17.221435 adafruit-circuitpython-bitmap_font-1.5.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/test/displayio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-08-09 19:57:09.000000 adafruit-circuitpython-bitmap_font-1.5.9/test/fontio.py
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bitmap_font-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/.github/workflows/build.yml` & `adafruit-circuitpython-bitmap_font-1.5.9/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -43,33 +43,35 @@
       run: |
         source actions-ci/install.sh
     - name: Pip install Sphinx, pre-commit
       run: |
         pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
     - name: Archive bundles
       uses: actions/upload-artifact@v2
       with:
         name: bundles
         path: ${{ github.workspace }}/bundles/
     - name: Build docs
       working-directory: docs
       run: sphinx-build -E -W -b html . _build/html
-    - name: Check For setup.py
+    - name: Check For pyproject.toml
       id: need-pypi
       run: |
-        echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
+        echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
-      if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
+      if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
-        pip install --upgrade setuptools wheel twine readme_renderer testresources
-        python setup.py sdist
-        python setup.py bdist_wheel --universal
+        pip install --upgrade build twine
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+        done;
+        python -m build
         twine check dist/*
-    - name: Setup problem matchers
-      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/.gitignore` & `adafruit-circuitpython-bitmap_font-1.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bitmap_font-1.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/.pylintrc` & `adafruit-circuitpython-bitmap_font-1.5.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bitmap_font-1.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/LICENSE` & `adafruit-circuitpython-bitmap_font-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/OFL-1.1-RFN.txt` & `adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/OFL-1.1-RFN.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bitmap_font-1.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/PKG-INFO` & `adafruit-circuitpython-bitmap_font-1.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bitmap_font
-Version: 1.5.8
+Version: 1.5.9
 Summary: Loads bitmap fonts into CircuitPython displayio.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython font text displayio bitmap
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font
+Keywords: adafruit,blinka,circuitpython,micropython,font,text,displayio,bitmap
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bitmap_font/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/bitmap-font/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 Loads bitmap fonts into CircuitPython's displayio. BDF and PCF files are well supported. TTF
 support is not yet complete.
 
 Dependencies
 =============
 This driver depends on:
 
@@ -61,16 +64,16 @@
     sudo pip3 install adafruit-circuitpython-bitmap_font
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-bitmap_font
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -98,9 +101,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/README.rst` & `adafruit-circuitpython-bitmap_font-1.5.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 Loads bitmap fonts into CircuitPython's displayio. BDF and PCF files are well supported. TTF
 support is not yet complete.
 
 Dependencies
 =============
 This driver depends on:
 
@@ -42,16 +46,16 @@
     sudo pip3 install adafruit-circuitpython-bitmap_font
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-bitmap_font
 
 Usage Example
 =============
 
 .. code-block:: python
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/bdf.py` & `adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/bdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     pass
 
 import gc
 from fontio import Glyph
 from .glyph_cache import GlyphCache
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font.git"
 
 
 class BDF(GlyphCache):
     """Loads glyphs from a BDF file in the given bitmap_class."""
 
     def __init__(self, f: FileIO, bitmap_class: Bitmap) -> None:
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/bitmap_font.py` & `adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/bitmap_font.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from displayio import Bitmap
     from . import bdf
     from . import pcf
     from . import ttf
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font.git"
 
 
 def load_font(
     filename: str, bitmap: Optional[Bitmap] = None
 ) -> Union[bdf.BDF, pcf.PCF, ttf.TTF]:
     """Loads a font file. Returns None if unsupported."""
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/glyph_cache.py` & `adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/glyph_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     from typing import Union, Iterable
     from fontio import Glyph
 except ImportError:
     pass
 
 import gc
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font.git"
 
 
 class GlyphCache:
     """Caches glyphs loaded by a subclass."""
 
     def __init__(self) -> None:
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/pcf.py` & `adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/pcf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/adafruit_bitmap_font/ttf.py` & `adafruit-circuitpython-bitmap_font-1.5.9/adafruit_bitmap_font/ttf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/adafruit_circuitpython_bitmap_font.egg-info/PKG-INFO` & `adafruit-circuitpython-bitmap_font-1.5.9/adafruit_circuitpython_bitmap_font.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bitmap-font
-Version: 1.5.8
+Version: 1.5.9
 Summary: Loads bitmap fonts into CircuitPython displayio.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython font text displayio bitmap
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font
+Keywords: adafruit,blinka,circuitpython,micropython,font,text,displayio,bitmap
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bitmap_font/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/bitmap-font/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 Loads bitmap fonts into CircuitPython's displayio. BDF and PCF files are well supported. TTF
 support is not yet complete.
 
 Dependencies
 =============
 This driver depends on:
 
@@ -61,16 +64,16 @@
     sudo pip3 install adafruit-circuitpython-bitmap_font
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-bitmap_font
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -98,9 +101,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/adafruit_circuitpython_bitmap_font.egg-info/SOURCES.txt` & `adafruit-circuitpython-bitmap_font-1.5.9/adafruit_circuitpython_bitmap_font.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/OFL-1.1-RFN.txt
```

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bitmap_font-1.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/docs/api.rst` & `adafruit-circuitpython-bitmap_font-1.5.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/docs/conf.py` & `adafruit-circuitpython-bitmap_font-1.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/docs/examples.rst` & `adafruit-circuitpython-bitmap_font-1.5.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/docs/index.rst` & `adafruit-circuitpython-bitmap_font-1.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_displayio_simpletest.py` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_displayio_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_forkawesome_icons.py` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_forkawesome_icons.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_label_forkawesome.py` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_label_forkawesome.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_label_magtag.py` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_label_magtag.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_label_simpletest.py` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_label_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/bitmap_font_simpletest.py` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/bitmap_font_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/Junction-regular-24.bdf` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/Junction-regular-24.bdf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/Junction-regular-24.pcf` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/Junction-regular-24.pcf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/LeagueSpartan-Bold-16.bdf` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/LeagueSpartan-Bold-16.bdf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/examples/fonts/forkawesome-42.pcf` & `adafruit-circuitpython-bitmap_font-1.5.9/examples/fonts/forkawesome-42.pcf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-1.5.8/test/displayio.py` & `adafruit-circuitpython-bitmap_font-1.5.9/test/displayio.py`

 * *Files identical despite different names*

