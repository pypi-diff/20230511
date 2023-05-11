# Comparing `tmp/adafruit-circuitpython-adafruitio-5.6.8.tar.gz` & `tmp/adafruit-circuitpython-adafruitio-5.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-adafruitio-5.6.8.tar", last modified: Thu Jun  9 18:37:18 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-adafruitio-5.6.9.tar", last modified: Wed Jul 13 19:50:59 2022, max compression
```

## Comparing `adafruit-circuitpython-adafruitio-5.6.8.tar` & `adafruit-circuitpython-adafruitio-5.6.9.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.142913 adafruit-circuitpython-adafruitio-5.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.134913 adafruit-circuitpython-adafruitio-5.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.134913 adafruit-circuitpython-adafruitio-5.6.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.138913 adafruit-circuitpython-adafruitio-5.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.138913 adafruit-circuitpython-adafruitio-5.6.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-06-09 18:37:18.142913 adafruit-circuitpython-adafruitio-5.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.138913 adafruit-circuitpython-adafruitio-5.6.8/adafruit_circuitpython_adafruitio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-06-09 18:37:18.000000 adafruit-circuitpython-adafruitio-5.6.8/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-06-09 18:37:18.000000 adafruit-circuitpython-adafruitio-5.6.8/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:37:18.000000 adafruit-circuitpython-adafruitio-5.6.8/adafruit_circuitpython_adafruitio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-09 18:37:18.000000 adafruit-circuitpython-adafruitio-5.6.8/adafruit_circuitpython_adafruitio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-09 18:37:18.000000 adafruit-circuitpython-adafruitio-5.6.8/adafruit_circuitpython_adafruitio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.138913 adafruit-circuitpython-adafruitio-5.6.8/adafruit_io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/adafruit_io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    28239 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/adafruit_io/adafruit_io.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      856 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/adafruit_io/adafruit_io_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.138913 adafruit-circuitpython-adafruitio-5.6.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.138913 adafruit-circuitpython-adafruitio-5.6.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5185 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.138913 adafruit-circuitpython-adafruitio-5.6.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.138913 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_analog_in.py
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_digital_out.py
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_feeds.py
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_randomizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_temperature.py
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_weather.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:18.142913 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4105 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4133 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (121)     3871 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3507 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4403 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_time.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4626 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:37:18.142913 adafruit-circuitpython-adafruitio-5.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-06-09 18:37:06.000000 adafruit-circuitpython-adafruitio-5.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.125214 adafruit-circuitpython-adafruitio-5.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.113214 adafruit-circuitpython-adafruitio-5.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.117214 adafruit-circuitpython-adafruitio-5.6.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.117214 adafruit-circuitpython-adafruitio-5.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.117214 adafruit-circuitpython-adafruitio-5.6.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-07-13 19:50:59.125214 adafruit-circuitpython-adafruitio-5.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.117214 adafruit-circuitpython-adafruitio-5.6.9/adafruit_circuitpython_adafruitio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-07-13 19:50:58.000000 adafruit-circuitpython-adafruitio-5.6.9/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-07-13 19:50:59.000000 adafruit-circuitpython-adafruitio-5.6.9/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-13 19:50:58.000000 adafruit-circuitpython-adafruitio-5.6.9/adafruit_circuitpython_adafruitio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-13 19:50:58.000000 adafruit-circuitpython-adafruitio-5.6.9/adafruit_circuitpython_adafruitio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-13 19:50:58.000000 adafruit-circuitpython-adafruitio-5.6.9/adafruit_circuitpython_adafruitio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.121214 adafruit-circuitpython-adafruitio-5.6.9/adafruit_io/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/adafruit_io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    28239 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/adafruit_io/adafruit_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      856 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/adafruit_io/adafruit_io_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.121214 adafruit-circuitpython-adafruitio-5.6.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.121214 adafruit-circuitpython-adafruitio-5.6.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5185 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.121214 adafruit-circuitpython-adafruitio-5.6.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.125214 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_analog_in.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_digital_out.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_randomizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2882 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:59.125214 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4105 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4133 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3871 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3624 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3507 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4403 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4626 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-13 19:50:59.125214 adafruit-circuitpython-adafruitio-5.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-07-13 19:50:44.000000 adafruit-circuitpython-adafruitio-5.6.9/setup.py
```

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-adafruitio-5.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/.github/workflows/build.yml` & `adafruit-circuitpython-adafruitio-5.6.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/.github/workflows/release.yml` & `adafruit-circuitpython-adafruitio-5.6.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/.gitignore` & `adafruit-circuitpython-adafruitio-5.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/.pre-commit-config.yaml` & `adafruit-circuitpython-adafruitio-5.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/.pylintrc` & `adafruit-circuitpython-adafruitio-5.6.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-adafruitio-5.6.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/LICENSE` & `adafruit-circuitpython-adafruitio-5.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-adafruitio-5.6.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/LICENSES/MIT.txt` & `adafruit-circuitpython-adafruitio-5.6.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-adafruitio-5.6.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/PKG-INFO` & `adafruit-circuitpython-adafruitio-5.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-adafruitio
-Version: 5.6.8
+Version: 5.6.9
 Summary: Adafruit IO for CircuitPython
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython adafruit_io adafruit-io rest api iot wifi
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/README.rst` & `adafruit-circuitpython-adafruitio-5.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO` & `adafruit-circuitpython-adafruitio-5.6.9/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-adafruitio
-Version: 5.6.8
+Version: 5.6.9
 Summary: Adafruit IO for CircuitPython
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython adafruit_io adafruit-io rest api iot wifi
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt` & `adafruit-circuitpython-adafruitio-5.6.9/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
+optional_requirements.txt
 requirements.txt
 setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
```

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/adafruit_io/adafruit_io.py` & `adafruit-circuitpython-adafruitio-5.6.9/adafruit_io/adafruit_io.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/adafruit_io/adafruit_io_errors.py` & `adafruit-circuitpython-adafruitio-5.6.9/adafruit_io/adafruit_io_errors.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/docs/_static/favicon.ico` & `adafruit-circuitpython-adafruitio-5.6.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/docs/conf.py` & `adafruit-circuitpython-adafruitio-5.6.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/docs/index.rst` & `adafruit-circuitpython-adafruitio-5.6.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_analog_in.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_analog_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_digital_out.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_digital_out.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_feeds.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_feeds.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_groups.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_groups.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_metadata.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_metadata.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_randomizer.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_randomizer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_simpletest.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_temperature.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_temperature.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_http/adafruit_io_weather.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_http/adafruit_io_weather.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_groups.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_groups.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_location.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_location.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_mqtt/adafruit_io_time.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_mqtt/adafruit_io_time.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/examples/adafruit_io_simpletest.py` & `adafruit-circuitpython-adafruitio-5.6.9/examples/adafruit_io_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.6.8/setup.py` & `adafruit-circuitpython-adafruitio-5.6.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     # The project's main homepage.
     url="https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO",
     # Author details
     author="Adafruit Industries",
     author_email="circuitpython@adafruit.com",
     install_requires=[
         "Adafruit-Blinka",
-        "Adafruit_CircuitPython_ESP32SPI",
-        "Adafruit-CircuitPython-MiniMQTT",
+        "adafruit-circuitpython-minimqtt",
     ],
     # Choose your license
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

