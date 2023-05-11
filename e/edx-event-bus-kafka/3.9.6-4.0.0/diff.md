# Comparing `tmp/edx_event_bus_kafka-3.9.6.tar.gz` & `tmp/edx_event_bus_kafka-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_kafka-3.9.6.tar", last modified: Tue Feb 28 20:46:40 2023, max compression
+gzip compressed data, was "edx_event_bus_kafka-4.0.0.tar", last modified: Wed May 10 20:41:56 2023, max compression
```

## Comparing `edx_event_bus_kafka-3.9.6.tar` & `edx_event_bus_kafka-4.0.0.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/
--rw-r--r--   0 runner    (1001) docker     (122)    10964 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    18358 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30625 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    14863 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30046 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    18435 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7613 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7386 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.601935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/templates/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18358 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5009 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.313124 edx_event_bus_kafka-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11962 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    19228 2023-05-10 20:41:56.313124 edx_event_bus_kafka-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6573 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.309124 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.309124 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30859 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14863 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.309124 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31454 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18435 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7678 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7386 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.309124 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.313124 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.305124 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.313124 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.309124 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    19228 2023-05-10 20:41:56.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-10 20:41:56.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 20:41:56.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 20:41:56.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-10 20:41:56.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-10 20:41:56.000000 edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.313124 edx_event_bus_kafka-4.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-10 20:41:56.313124 edx_event_bus_kafka-4.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5009 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 20:41:56.313124 edx_event_bus_kafka-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-10 20:41:48.000000 edx_event_bus_kafka-4.0.0/tests/test_models.py
```

### Comparing `edx_event_bus_kafka-3.9.6/CHANGELOG.rst` & `edx_event_bus_kafka-4.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,33 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[4.0.0] - 2023-05-10
+********************
+Changed
+=======
+* Implement openedx-events Event Bus Consumer API.
+* **BREAKING CHANGE**: Remove ``consume_events`` management command as this command will be provided by openedx_events. To replay events using the
+  openedx-events version of the management command, pass ``--extra '{"offset_time": "2023-01-08T06:46:22"}'`` instead of ``-o 2023-01-08T06:46:22``.
+* **BREAKING Change**: ``offset_timestamp`` argument has been removed from ``consume_indefinitely`` and ``reset_offsets_and_sleep_indefinitely`` methods.
+  It is now added as an optional argument named ``offset_time`` to ``KafkaEventConsumer`` constructor.
+
+[3.10.0] - 2023-05-05
+*********************
+Changed
+=======
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Refactored consumer to manually deserialize messages instead of using DeserializingConsumer
+* Make signal argument optional in consumer command (take signal from message headers)
+
 [3.9.6] - 2023-02-24
 ********************
 Added
 =====
 * Add function tracing to the event consumption workflow for better monitoring.
 
 [3.9.5] - 2023-02-24
```

### Comparing `edx_event_bus_kafka-3.9.6/LICENSE.txt` & `edx_event_bus_kafka-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/PKG-INFO` & `edx_event_bus_kafka-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_kafka
-Version: 3.9.6
+Version: 4.0.0
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -130,17 +130,15 @@
 
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 How To Contribute
 *****************
 
 Contributions are very welcome.
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for all Open edX projects.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <.github/ISSUE_TEMPLATE.md>`_.
 
@@ -199,14 +197,33 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[4.0.0] - 2023-05-10
+********************
+Changed
+=======
+* Implement openedx-events Event Bus Consumer API.
+* **BREAKING CHANGE**: Remove ``consume_events`` management command as this command will be provided by openedx_events. To replay events using the
+  openedx-events version of the management command, pass ``--extra '{"offset_time": "2023-01-08T06:46:22"}'`` instead of ``-o 2023-01-08T06:46:22``.
+* **BREAKING Change**: ``offset_timestamp`` argument has been removed from ``consume_indefinitely`` and ``reset_offsets_and_sleep_indefinitely`` methods.
+  It is now added as an optional argument named ``offset_time`` to ``KafkaEventConsumer`` constructor.
+
+[3.10.0] - 2023-05-05
+*********************
+Changed
+=======
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Refactored consumer to manually deserialize messages instead of using DeserializingConsumer
+* Make signal argument optional in consumer command (take signal from message headers)
+
 [3.9.6] - 2023-02-24
 ********************
 Added
 =====
 * Add function tracing to the event consumption workflow for better monitoring.
 
 [3.9.5] - 2023-02-24
```

### Comparing `edx_event_bus_kafka-3.9.6/README.rst` & `edx_event_bus_kafka-4.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -110,17 +110,15 @@
 
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 How To Contribute
 *****************
 
 Contributions are very welcome.
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for all Open edX projects.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <.github/ISSUE_TEMPLATE.md>`_.
```

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/config.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/consumer.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Core consumer and event-loop code.
 """
 import logging
 import time
-import warnings
 from datetime import datetime
+from functools import lru_cache
 
 from django.conf import settings
-from django.core.management.base import BaseCommand
 from django.db import connection
+from django.dispatch import receiver
+from django.test.signals import setting_changed
 from edx_django_utils.monitoring import function_trace, record_exception, set_custom_attribute
 from edx_toggles.toggles import SettingToggle
+from openedx_events.event_bus import EventBusConsumer
 from openedx_events.event_bus.avro.deserializer import AvroSignalDeserializer
-from openedx_events.tooling import OpenEdxPublicSignal, load_all_signals
+from openedx_events.tooling import OpenEdxPublicSignal
 
 from .config import get_full_topic, get_schema_registry_client, load_common_settings
 from .utils import (
     AUDIT_LOGGING_ENABLED,
     HEADER_EVENT_TYPE,
     HEADER_ID,
     _get_metadata_from_headers,
@@ -25,17 +27,18 @@
 )
 
 logger = logging.getLogger(__name__)
 
 # See https://github.com/openedx/event-bus-kafka/blob/main/docs/decisions/0005-optional-import-of-confluent-kafka.rst
 try:
     import confluent_kafka
-    from confluent_kafka import TIMESTAMP_NOT_AVAILABLE, DeserializingConsumer
+    from confluent_kafka import TIMESTAMP_NOT_AVAILABLE, Consumer
     from confluent_kafka.error import KafkaError
     from confluent_kafka.schema_registry.avro import AvroDeserializer
+    from confluent_kafka.serialization import MessageField, SerializationContext
 except ImportError:  # pragma: no cover
     confluent_kafka = None
 
 # .. toggle_name: EVENT_BUS_KAFKA_CONSUMERS_ENABLED
 # .. toggle_implementation: SettingToggle
 # .. toggle_default: True
 # .. toggle_description: If set to False, consumer will exit immediately. This can be used as an emergency kill-switch
@@ -93,105 +96,104 @@
     """
     has_connection = bool(connection.connection)
     requires_reconnect = has_connection and not connection.is_usable()
     if requires_reconnect:
         connection.connect()
 
 
-class KafkaEventConsumer:
+class KafkaEventConsumer(EventBusConsumer):
     """
-    Construct consumer for the given topic, group, and signal. The consumer can then
-    emit events from the event bus using the configured signal.
+    Construct consumer for the given topic and group. The consumer can then
+    emit events from the event bus using the signal from the message headers.
 
     Note that the topic should be specified here *without* the optional environment prefix.
 
     Can also consume messages indefinitely off the queue.
+
+    Attributes:
+        topic: Topic to consume (without environment prefix).
+        group_id: Consumer group id.
+        signal: Type of signal to emit from consumed messages.
+        consumer: Actual kafka consumer instance.
+        offset_time: The timestamp (in ISO format) that we would like to reset the consumers to. If this is used, the
+            consumers will only reset the offsets of the topic but will not actually consume and process any messages.
     """
 
-    def __init__(self, topic, group_id, signal):
+    def __init__(self, topic, group_id, offset_time=None):
         if confluent_kafka is None:  # pragma: no cover
             raise Exception('Library confluent-kafka not available. Cannot create event consumer.')
 
         self.topic = topic
         self.group_id = group_id
-        self.signal = signal
         self.consumer = self._create_consumer()
+        self.offset_time = None
+        if offset_time:
+            try:
+                self.offset_time = datetime.fromisoformat(str(offset_time))
+            except ValueError:
+                logger.exception('Could not parse the offset timestamp.')
+                raise
         self._shut_down_loop = False
+        self.schema_registry_client = get_schema_registry_client()
 
-    # return type (Optional[DeserializingConsumer]) removed from signature to avoid error on import
+    # return type Consumer removed from signature to avoid error on import
     def _create_consumer(self):
         """
-        Create a DeserializingConsumer for events of the given signal instance.
+        Create a Consumer in the correct consumer group
 
         Returns
-            None if confluent_kafka is not available.
-            DeserializingConsumer if it is.
+            Consumer in the configured consumer group
         """
 
-        schema_registry_client = get_schema_registry_client()
-
-        signal_deserializer = AvroSignalDeserializer(self.signal)
-
-        def inner_from_dict(event_data_dict, ctx=None):  # pylint: disable=unused-argument
-            return signal_deserializer.from_dict(event_data_dict)
-
         consumer_config = load_common_settings()
 
-        # We do not deserialize the key because we don't need it for anything yet.
-        # Also see https://github.com/openedx/openedx-events/issues/86 for some challenges on determining key schema.
         consumer_config.update({
             'group.id': self.group_id,
-            'value.deserializer': AvroDeserializer(schema_str=signal_deserializer.schema_string(),
-                                                   schema_registry_client=schema_registry_client,
-                                                   from_dict=inner_from_dict),
             # Turn off auto commit. Auto commit will commit offsets for the entire batch of messages received,
             # potentially resulting in data loss if some of those messages are not fully processed. See
             # https://newrelic.com/blog/best-practices/kafka-consumer-config-auto-commit-data-loss
             'enable.auto.commit': False,
         })
 
-        return DeserializingConsumer(consumer_config)
+        return Consumer(consumer_config)
 
     def _shut_down(self):
         """
         Test utility for shutting down the consumer loop.
         """
         self._shut_down_loop = True
 
-    def reset_offsets_and_sleep_indefinitely(self, offset_timestamp):
+    def reset_offsets_and_sleep_indefinitely(self):
         """
         Reset any assigned partitions to the given offset, and sleep indefinitely.
-
-        Arguments:
-            offset_timestamp (datetime): Reset the offsets of the consumer partitions to this timestamp.
         """
 
         def reset_offsets(consumer, partitions):
             # This is a callback method used on consumer assignment to handle offset reset logic.
             # We do not want to attempt to change offsets if the offset is None.
-            if offset_timestamp is None:
+            if self.offset_time is None:
                 return
 
             # Get the offset from the epoch. Kafka expects offsets in milliseconds for offsets_for_times. Although
             # this is undocumented in the libraries we're using (confluent-kafka and librdkafa), for reference
             # see the docs for kafka-python:
             # https://kafka-python.readthedocs.io/en/master/apidoc/KafkaConsumer.html#kafka.KafkaConsumer.offsets_for_times
-            offset_timestamp_ms = int(offset_timestamp.timestamp()*1000)
+            offset_timestamp_ms = int(self.offset_time.timestamp()*1000)
             # We set the epoch timestamp in the offset position.
             for partition in partitions:
                 partition.offset = offset_timestamp_ms
 
             partitions_with_offsets = consumer.offsets_for_times(partitions, timeout=1.0)
 
             # Partitions have an error field that may be set on return.
             errors = [p.error for p in partitions_with_offsets if p.error is not None]
             if len(errors) > 0:
                 raise Exception("Error getting offsets for timestamps: {errors}")
 
-            logger.info(f'Found offsets for timestamp {offset_timestamp}: {partitions_with_offsets}')
+            logger.info(f'Found offsets for timestamp {self.offset_time}: {partitions_with_offsets}')
 
             # We need to commit these offsets to Kafka in order to ensure these offsets are persisted.
             consumer.commit(offsets=partitions_with_offsets)
 
         full_topic = get_full_topic(self.topic)
         # Partition assignment will trigger the reset logic. This should happen on the first poll call,
         # but will also happen any time the broker needs to rebalance partitions among the consumer
@@ -219,16 +221,14 @@
             continue
 
     def _consume_indefinitely(self):
         """
         Consume events from a topic in an infinite loop.
         """
 
-        # This is already checked at the Command level, but it's possible this loop
-        # could get called some other way, so check it here too.
         if not KAFKA_CONSUMERS_ENABLED.is_enabled():
             logger.error("Kafka consumers not enabled, exiting.")
             return
 
         # .. setting_name: EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT
         # .. setting_default: None
         # .. setting_description: If the consumer encounters this many consecutive errors, exit with an
@@ -244,15 +244,14 @@
         CONSECUTIVE_ERRORS_LIMIT = getattr(settings, 'EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT', None)
 
         try:
             full_topic = get_full_topic(self.topic)
             run_context = {
                 'full_topic': full_topic,
                 'consumer_group': self.group_id,
-                'expected_signal': self.signal,
             }
             self.consumer.subscribe([full_topic])
             logger.info(f"Running consumer for {run_context!r}")
 
             # How many errors have we seen in a row? If this climbs too high, exit with error.
             # Any error counts, here — whether due to a polling failure or a message processing
             # failure. But only a successfully processed message clears the counter. Just
@@ -272,16 +271,17 @@
                 msg = None
                 try:
                     msg = self.consumer.poll(timeout=CONSUMER_POLL_TIMEOUT)
                     if msg is not None:
                         with function_trace('_consume_indefinitely_consume_single_message'):
                             # Before processing, make sure our db connection is still active
                             _reconnect_to_db_if_needed()
-
-                            self.emit_signals_from_message(msg)
+                            signal = self.determine_signal(msg)
+                            msg.set_value(self._deserialize_message_value(msg, signal))
+                            self.emit_signals_from_message(msg, signal)
                             consecutive_errors = 0
 
                     self._add_message_monitoring(run_context=run_context, message=msg)
                 except Exception as e:  # pylint: disable=broad-except
                     consecutive_errors += 1
                     self.record_event_consuming_error(run_context, e, msg)
                     # Kill the infinite loop if the error is fatal for the consumer
@@ -299,121 +299,160 @@
                     # to commit all this consumer's current offset across all partitions since we only process one
                     # message at a time, but limit it to just the offset/partition of the specified message
                     # to be super safe
                     self.consumer.commit(message=msg)
         finally:
             self.consumer.close()
 
-    def consume_indefinitely(self, offset_timestamp=None):
+    def consume_indefinitely(self):
         """
-        Consume events from a topic in an infinite loop.
-
-        Arguments:
-            offset_timestamp (datetime): Optional and deprecated; if supplied, calls
-                ``reset_offsets_and_sleep_indefinitely`` instead. Relying code should
-                switch to calling that method directly.
-        """
-        # TODO: Once this deprecated argument can be removed, just
-        # remove this delegation method entirely and rename
-        # `_consume_indefinitely` to no longer have the `_` prefix.
-        if offset_timestamp is None:
+        Consume events from a topic in an infinite loop if offset_time is not set else reset any assigned partitions to
+        the given offset, and sleep indefinitely.
+        """
+        if self.offset_time is None:
             self._consume_indefinitely()
         else:
-            warnings.warn(
-                "Calling consume_indefinitely with offset_timestamp is deprecated; "
-                "please call reset_offsets_and_sleep_indefinitely directly instead."
-            )
-            self.reset_offsets_and_sleep_indefinitely(offset_timestamp)
+            self.reset_offsets_and_sleep_indefinitely()
 
     @function_trace('emit_signals_from_message')
-    def emit_signals_from_message(self, msg):
+    def emit_signals_from_message(self, msg, signal):
         """
-        Determine the correct signal and send the event from the message.
+        Send the event from the message via the given signal.
+
+        Assumes the message has been deserialized and the signal matches the event_type of the message header.
 
         Arguments:
-            msg (Message): Consumed message.
+            msg (Message): Deserialized message.
+            signal (OpenEdxPublicSignal): Signal - must match the event_type of the message header.
         """
         self._log_message_received(msg)
 
-        # DeserializingConsumer.poll() always returns either a valid message
-        # or None, and raises an exception in all other cases. This means
-        # we don't need to check msg.error() ourselves. But... check it here
-        # anyway for robustness against code changes.
         if msg.error() is not None:
             raise UnusableMessageError(
-                f"Polled message had error object (shouldn't happen): {msg.error()!r}"
+                f"Polled message had error object: {msg.error()!r}"
             )
 
-        headers = msg.headers() or []  # treat None as []
-
-        event_types = get_message_header_values(headers, HEADER_EVENT_TYPE)
-        if len(event_types) == 0:
-            raise UnusableMessageError(
-                "Missing ce_type header on message, cannot determine signal"
-            )
-        if len(event_types) > 1:
-            raise UnusableMessageError(
-                "Multiple ce_type headers found on message, cannot determine signal"
-            )
-        event_type = event_types[0]
+        # This should also never happen since the signal should be determined from the message
+        # but it's here to prevent misuse of the method
+        msg_event_type = self._get_event_type_from_message(msg)
+        if signal.event_type != msg_event_type:
+            raise Exception(f"Error emitting event from Kafka: (UNEXPECTED) message event type {msg_event_type}"
+                            f" does not match signal {signal.event_type}")
 
-        if event_type != self.signal.event_type:
-            raise UnusableMessageError(
-                f"Signal types do not match. Expected {self.signal.event_type}. "
-                f"Received message of type {event_type}."
-            )
         try:
-            event_metadata = _get_metadata_from_headers(headers)
+            event_metadata = _get_metadata_from_headers(msg.headers())
         except Exception as e:
             raise UnusableMessageError(f"Error determining metadata from message headers: {e}") from e
 
         with function_trace('emit_signals_from_message_send_event_with_custom_metadata'):
-            send_results = self.signal.send_event_with_custom_metadata(event_metadata, **msg.value())
+            send_results = signal.send_event_with_custom_metadata(event_metadata, **msg.value())
 
         # Raise an exception if any receivers errored out. This allows logging of the receivers
         # along with partition, offset, etc. in record_event_consuming_error. Hopefully the
         # receiver code is idempotent and we can just replay any messages that were involved.
-        self._check_receiver_results(send_results)
+        self._check_receiver_results(send_results, signal)
 
         # At the very end, log that a message was processed successfully.
         # Since we're single-threaded, no other information is needed;
         # we just need the logger to spit this out with a timestamp.
         # See ADR: docs/decisions/0010_audit_logging.rst
         if AUDIT_LOGGING_ENABLED.is_enabled():
             logger.info('Message from Kafka processed successfully')
 
-    def _check_receiver_results(self, send_results: list):
+    def determine_signal(self, msg) -> OpenEdxPublicSignal:
+        """
+        Determine which OpenEdxPublicSignal should be used to emit the event data in a message
+
+        Arguments:
+            msg (Message): Consumed message
+
+        Returns:
+            The OpenEdxPublicSignal instance corresponding to the ce_type header on the message
+        """
+        event_type = self._get_event_type_from_message(msg)
+        try:
+            return OpenEdxPublicSignal.get_signal_by_type(event_type)
+        except KeyError as ke:
+            raise UnusableMessageError(
+                f"Unrecognized type {event_type} found on message, cannot determine signal"
+            ) from ke
+
+    def _get_event_type_from_message(self, msg):
+        """
+        Return the event type from the ce_type header
+
+        Arguments:
+            msg (Message): the consumed message
+
+        Returns
+            The associated event type as a string
+        """
+        headers = msg.headers() or []  # treat None as []
+        event_types = get_message_header_values(headers, HEADER_EVENT_TYPE)
+        if len(event_types) == 0:
+            raise UnusableMessageError(
+                "Missing ce_type header on message, cannot determine signal"
+            )
+        if len(event_types) > 1:
+            raise UnusableMessageError(
+                "Multiple ce_type headers found on message, cannot determine signal"
+            )
+        return event_types[0]
+
+    def _deserialize_message_value(self, msg, signal: OpenEdxPublicSignal):
+        """
+        Deserialize an Avro message value
+
+        The signal is expected to match the ce_type header on the message
+
+        Arguments:
+            msg (Message): the raw message from the consumer
+            signal (OpenEdxPublicSignal): The instance of OpenEdxPublicSignal corresponding to the ce_type header on msg
+
+        Returns:
+            The deserialized message value
+        """
+        msg_event_type = self._get_event_type_from_message(msg)
+        if signal.event_type != msg_event_type:
+            # This should never happen but it's here to prevent misuse of the method
+            raise Exception(f"Error deserializing event from Kafka: (UNEXPECTED) message event type {msg_event_type}"
+                            f" does not match signal {signal.event_type}")
+        signal_deserializer = get_deserializer(signal, self.schema_registry_client)
+        ctx = SerializationContext(msg.topic(), MessageField.VALUE, msg.headers())
+        return signal_deserializer(msg.value(), ctx)
+
+    def _check_receiver_results(self, send_results: list, signal: OpenEdxPublicSignal):
         """
         Raises exception if any of the receivers produced an exception.
 
         Arguments:
             send_results: Output of ``send_events``, a list of ``(receiver, response)`` tuples.
         """
         error_descriptions = []
         errors = []
-        for receiver, response in send_results:
+        for signal_receiver, response in send_results:
             if not isinstance(response, BaseException):
                 continue
 
             # Probably every receiver will be a regular function or even a lambda with
             # these attrs, so this check is just to be safe.
             try:
-                receiver_name = f"{receiver.__module__}.{receiver.__qualname__}"
+                receiver_name = f"{signal_receiver.__module__}.{signal_receiver.__qualname__}"
             except AttributeError:
-                receiver_name = str(receiver)
+                receiver_name = str(signal_receiver)
 
             # The stack traces are already logged by django.dispatcher, so just the error message is fine.
             error_descriptions.append(f"{receiver_name}={response!r}")
             errors.append(response)
 
         if len(error_descriptions) > 0:
             raise ReceiverError(
                 f"{len(error_descriptions)} receiver(s) out of {len(send_results)} "
                 "produced errors (stack trace elsewhere in logs) "
-                f"when handling signal {self.signal}: {', '.join(error_descriptions)}",
+                f"when handling signal {signal}: {', '.join(error_descriptions)}",
                 errors
             )
 
     def _log_message_received(self, msg):
         """
         Log that a message was received, for audit log purposes.
 
@@ -567,85 +606,41 @@
                          f" -- event message={message!r}, error event message={kafka_message!r}.")
         # give priority to the passed message, although in theory, it should be the same message if not None
         kafka_message = message or kafka_message
 
         return kafka_message, kafka_error
 
 
-class ConsumeEventsCommand(BaseCommand):
+# argument type SchemaRegistryClient for schema_registry_client removed from signature to avoid error on import
+@lru_cache
+def get_deserializer(signal: OpenEdxPublicSignal, schema_registry_client):
     """
-    Management command for Kafka consumer workers in the event bus.
-    """
-    help = """
-    Consume messages of specified signal type from a Kafka topic and send their data to that signal.
+    Get the value deserializer for a signal.
+
+    This is cached in order to save work re-transforming classes into Avro schemas.
+    We do not deserialize the key because we don't need it for anything yet.
+    Also see https://github.com/openedx/openedx-events/issues/86 for some challenges on determining key schema.
 
-    Example::
+    Arguments:
+        signal: The OpenEdxPublicSignal to make a deserializer for.
+        schema_registry_client: The SchemaRegistryClient instance for the consumer
 
-        python3 manage.py cms consume_events -t user-login -g user-activity-service \
-            -s org.openedx.learning.auth.session.login.completed.v1
+    Returns:
+        AvroSignalDeserializer for event value
     """
+    if schema_registry_client is None:
+        raise Exception('Cannot create Kafka deserializer -- missing library or settings')
 
-    def add_arguments(self, parser):
+    signal_deserializer = AvroSignalDeserializer(signal)
 
-        parser.add_argument(
-            '-t', '--topic',
-            nargs=1,
-            required=True,
-            help='Topic to consume (without environment prefix)'
-        )
-
-        parser.add_argument(
-            '-g', '--group_id',
-            nargs=1,
-            required=True,
-            help='Consumer group id'
-        )
-        parser.add_argument(
-            '-s', '--signal',
-            nargs=1,
-            required=True,
-            help='Type of signal to emit from consumed messages.'
-        )
-        parser.add_argument(
-            '-o', '--offset_time',
-            nargs=1,
-            required=False,
-            default=None,
-            help='The timestamp (in ISO format) that we would like to reset the consumers to. '
-                 'If this is used, the consumers will only reset the offsets of the topic '
-                 'but will not actually consume and process any messages.'
-        )
-
-    def handle(self, *args, **options):
-        if confluent_kafka is None:
-            logger.error(
-                "Cannot consume events because confluent_kafka dependency (or one of its extras) was not installed"
-            )
-            return
+    def inner_from_dict(event_data_dict, ctx=None):  # pylint: disable=unused-argument
+        return signal_deserializer.from_dict(event_data_dict)
 
-        if not KAFKA_CONSUMERS_ENABLED.is_enabled():
-            logger.error("Kafka consumers not enabled, exiting.")
-            return
+    return AvroDeserializer(schema_str=signal_deserializer.schema_string(),
+                            schema_registry_client=schema_registry_client,
+                            from_dict=inner_from_dict)
 
-        try:
-            load_all_signals()
-            signal = OpenEdxPublicSignal.get_signal_by_type(options['signal'][0])
-            if options['offset_time'] and options['offset_time'][0] is not None:
-                try:
-                    offset_timestamp = datetime.fromisoformat(options['offset_time'][0])
-                except ValueError:
-                    logger.exception('Could not parse the offset timestamp.')
-                    raise
-            else:
-                offset_timestamp = None
 
-            event_consumer = KafkaEventConsumer(
-                topic=options['topic'][0],
-                group_id=options['group_id'][0],
-                signal=signal,
-            )
-            if offset_timestamp is None:
-                event_consumer.consume_indefinitely()
-            else:
-                event_consumer.reset_offsets_and_sleep_indefinitely(offset_timestamp=offset_timestamp)
-        except Exception:  # pylint: disable=broad-except
-            logger.exception("Error consuming Kafka events")
+@receiver(setting_changed)
+def _reset_caches(sender, **kwargs):  # pylint: disable=unused-argument
+    """Reset caches when settings change during unit tests."""
+    get_deserializer.cache_clear()
```

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/producer.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_config.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_consumer.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/test_consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 import copy
 from datetime import datetime
 from unittest.mock import Mock, call, patch
 from uuid import uuid1
 
 import ddt
 import pytest
-from django.core.management import call_command
 from django.test import TestCase
 from django.test.utils import override_settings
 from openedx_events.learning.data import UserData, UserPersonalData
 from openedx_events.learning.signals import SESSION_LOGIN_COMPLETED
+from openedx_events.tooling import OpenEdxPublicSignal
 
-from edx_event_bus_kafka.internal.consumer import KafkaEventConsumer, ReceiverError, UnusableMessageError
+from edx_event_bus_kafka.internal.consumer import (
+    KafkaEventConsumer,
+    ReceiverError,
+    UnusableMessageError,
+    get_deserializer,
+)
 from edx_event_bus_kafka.internal.tests.test_utils import FakeMessage, side_effects
-from edx_event_bus_kafka.management.commands.consume_events import Command
 
 # See https://github.com/openedx/event-bus-kafka/blob/main/docs/decisions/0005-optional-import-of-confluent-kafka.rst
 try:
     from confluent_kafka import (
         TIMESTAMP_CREATE_TIME,
         TIMESTAMP_NOT_AVAILABLE,
         KafkaError,
@@ -42,14 +46,15 @@
 
 
 @override_settings(
     EVENT_BUS_KAFKA_SCHEMA_REGISTRY_URL='https://test-url',
     EVENT_BUS_KAFKA_BOOTSTRAP_SERVERS='bootstrap-servers',
     EVENT_BUS_KAFKA_API_KEY='test-key',
     EVENT_BUS_KAFKA_API_SECRET='test-secret',
+    EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT=10,  # prevent infinite looping if tests are broken
 )
 @ddt.ddt
 class TestEmitSignals(TestCase):
     """
     Tests for message parsing and signal-sending.
     """
 
@@ -62,38 +67,41 @@
                 pii=UserPersonalData(
                     username='foobob',
                     email='bob@foo.example',
                     name='Bob Foo'
                 )
             )
         }
+        # determined by manual testing
+        self.normal_event_data_bytes = b'\x00\x00\x01\x86\xb3\xf6\x01\x01\x0cfoobob\x1ebob@foo.example\x0eBob Foo'
+
         self.message_id = uuid1()
         self.message_id_bytes = str(self.message_id).encode('utf-8')
 
         self.signal_type_bytes = b'org.openedx.learning.auth.session.login.completed.v1'
         self.signal_type = self.signal_type_bytes.decode('utf-8')
         self.normal_message = FakeMessage(
             topic='local-some-topic',
             partition=2,
             offset=12345,
             headers=[
                 ('ce_id', self.message_id_bytes),
                 ('ce_type', self.signal_type_bytes),
             ],
             key=b'\x00\x00\x00\x00\x01\x0cfoobob',  # Avro, as observed in manual test
-            value=self.normal_event_data,
+            value=self.normal_event_data_bytes,
             error=None,
             timestamp=(TIMESTAMP_CREATE_TIME, 1675114920123),
         )
         self.mock_receiver = Mock()
         self.signal = SESSION_LOGIN_COMPLETED
         self.signal.connect(fake_receiver_returns_quietly)
         self.signal.connect(fake_receiver_raises_error)
         self.signal.connect(self.mock_receiver)
-        self.event_consumer = KafkaEventConsumer('some-topic', 'test_group_id', self.signal)
+        self.event_consumer = KafkaEventConsumer('some-topic', 'test_group_id')
 
     def tearDown(self):
         self.signal.disconnect(fake_receiver_returns_quietly)
         self.signal.disconnect(fake_receiver_raises_error)
         self.signal.disconnect(self.mock_receiver)
 
     def assert_signal_sent_with(self, signal, data):
@@ -122,15 +130,16 @@
         self.event_consumer.consume_indefinitely()  # returns at all
         mock_logger.error.assert_called_once_with("Kafka consumers not enabled, exiting.")
 
     def test_reset_offsets_and_sleep_indefinitely(self):
         test_time = datetime.now()
         self.event_consumer.consumer = Mock()
         self.event_consumer._shut_down()  # pylint: disable=protected-access
-        self.event_consumer.reset_offsets_and_sleep_indefinitely(offset_timestamp=test_time)
+        self.event_consumer.offset_time = test_time
+        self.event_consumer.reset_offsets_and_sleep_indefinitely()
         reset_offsets = self.event_consumer.consumer.subscribe.call_args[1]['on_assign']
         partitions = [TopicPartition('dummy_topic', 0, 0), TopicPartition('dummy_topic', 1, 0)]
         self.event_consumer.consumer.offsets_for_times.return_value = partitions
 
         # This is usually called by Kafka after assignment of partitions. For testing, we are calling
         # it directly.
         reset_offsets(self.event_consumer.consumer, partitions)
@@ -144,14 +153,26 @@
         assert partition_0.topic == 'dummy_topic'
         assert partition_0.partition == 0
 
         assert partition_1.offset == test_time_ms
         assert partition_1.topic == 'dummy_topic'
         assert partition_1.partition == 1
 
+    def test_reset_offsets_and_sleep_indefinitely_with_none_offset(self):
+        self.event_consumer.consumer = Mock()
+        self.event_consumer._shut_down()  # pylint: disable=protected-access
+        self.event_consumer.offset_time = None
+        self.event_consumer.reset_offsets_and_sleep_indefinitely()
+        reset_offsets = self.event_consumer.consumer.subscribe.call_args[1]['on_assign']
+
+        # This is usually called by Kafka after assignment of partitions. For testing, we are calling
+        # it directly.
+        reset_offsets(self.event_consumer.consumer, [])
+        self.event_consumer.consumer.offsets_for_times.assert_not_called()
+
     @override_settings(
         EVENT_BUS_KAFKA_SCHEMA_REGISTRY_URL='http://localhost:12345',
         EVENT_BUS_KAFKA_BOOTSTRAP_SERVERS='localhost:54321',
         EVENT_BUS_TOPIC_PREFIX='local',
     )
     @patch('edx_event_bus_kafka.internal.consumer.set_custom_attribute', autospec=True)
     @patch('edx_event_bus_kafka.internal.consumer.logger', autospec=True)
@@ -173,32 +194,32 @@
             self.event_consumer._shut_down  # pylint: disable=protected-access
         ]
 
         with patch.object(
                 self.event_consumer, 'emit_signals_from_message',
                 side_effect=side_effects(mock_emit_side_effects),
         ) as mock_emit:
-            mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
-            self.event_consumer.consumer = mock_consumer
-            self.event_consumer.consume_indefinitely()
+            with patch('edx_event_bus_kafka.internal.consumer.AvroDeserializer',
+                       return_value=lambda _x, _y: self.normal_event_data):
+                mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
+                self.event_consumer.consumer = mock_consumer
+                self.event_consumer.consume_indefinitely()
 
         # Check that each of the mocked out methods got called as expected.
         mock_consumer.subscribe.assert_called_once_with(['local-some-topic'])
         # Check that emit was called the expected number of times
-        assert mock_emit.call_args_list == [call(self.normal_message)] * len(mock_emit_side_effects)
+        assert mock_emit.call_args_list == [call(self.normal_message, self.signal)] * len(mock_emit_side_effects)
 
         # Check that there was one error log message and that it contained all the right parts,
         # in some order.
         mock_logger.exception.assert_called_once()
         (exc_log_msg,) = mock_logger.exception.call_args.args
         assert "Error consuming event from Kafka: Exception('something broke') in context" in exc_log_msg
         assert "full_topic='local-some-topic'" in exc_log_msg
         assert "consumer_group='test_group_id'" in exc_log_msg
-        assert ("expected_signal=<OpenEdxPublicSignal: "
-                "org.openedx.learning.auth.session.login.completed.v1>") in exc_log_msg
         assert "-- event details: " in exc_log_msg
         assert "'partition': 2" in exc_log_msg
         assert "'offset': 12345" in exc_log_msg
         assert f"'headers': [('ce_id', b'{self.message_id}'), " \
                "('ce_type', b'org.openedx.learning.auth.session.login.completed.v1')]" in exc_log_msg
         assert "'key': b'\\x00\\x00\\x00\\x00\\x01\\x0cfoobob'" in exc_log_msg
         assert "email='bob@foo.example'" in exc_log_msg
@@ -232,20 +253,22 @@
 
         exception_count = 4
 
         with patch.object(
                 self.event_consumer, 'emit_signals_from_message',
                 side_effect=side_effects([raise_exception] * exception_count)
         ) as mock_emit:
-            mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
-            self.event_consumer.consumer = mock_consumer
-            with pytest.raises(Exception) as exc_info:
-                self.event_consumer.consume_indefinitely()
+            with patch('edx_event_bus_kafka.internal.consumer.AvroDeserializer',
+                       return_value=lambda _x, _y: self.normal_event_data):
+                mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
+                self.event_consumer.consumer = mock_consumer
+                with pytest.raises(Exception) as exc_info:
+                    self.event_consumer.consume_indefinitely()
 
-        assert mock_emit.call_args_list == [call(self.normal_message)] * exception_count
+        assert mock_emit.call_args_list == [call(self.normal_message, self.signal)] * exception_count
         assert exc_info.value.args == ("Too many consecutive errors, exiting (4 in a row)",)
 
     @override_settings(
         EVENT_BUS_KAFKA_SCHEMA_REGISTRY_URL='http://localhost:12345',
         EVENT_BUS_KAFKA_BOOTSTRAP_SERVERS='localhost:54321',
     )
     @patch('edx_event_bus_kafka.internal.consumer.connection')
@@ -261,17 +284,19 @@
             mock_connection.connection = None
         mock_connection.is_usable.return_value = is_usable
 
         with patch.object(
                 self.event_consumer, 'emit_signals_from_message',
                 side_effect=side_effects([self.event_consumer._shut_down])  # pylint: disable=protected-access
         ):
-            mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
-            self.event_consumer.consumer = mock_consumer
-            self.event_consumer.consume_indefinitely()
+            with patch('edx_event_bus_kafka.internal.consumer.AvroDeserializer',
+                       return_value=lambda _x, _y: self.normal_event_data):
+                mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
+                self.event_consumer.consumer = mock_consumer
+                self.event_consumer.consume_indefinitely()
 
         if reconnect_expected:
             mock_connection.connect.assert_called_once()
         else:
             mock_connection.connect.assert_not_called()
 
     @override_settings(
@@ -280,24 +305,37 @@
         EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT=4,
     )
     @patch('edx_event_bus_kafka.internal.consumer.logger', autospec=True)
     @patch('edx_event_bus_kafka.internal.consumer.time.sleep', autospec=True)
     def test_no_consume_with_offsets(self, mock_sleep, mock_logger):
         mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
         self.event_consumer.consumer = mock_consumer
+        self.event_consumer.offset_time = datetime.now()
         mock_sleep.side_effect = side_effects([self.event_consumer._shut_down])  # pylint: disable=protected-access
-        self.event_consumer.consume_indefinitely(offset_timestamp=0)
+        self.event_consumer.consume_indefinitely()
         mock_sleep.assert_called_with(30)
         mock_logger.info.assert_any_call('Offsets are being reset. Sleeping instead of consuming events.')
 
     @override_settings(
         EVENT_BUS_KAFKA_SCHEMA_REGISTRY_URL='http://localhost:12345',
         EVENT_BUS_KAFKA_BOOTSTRAP_SERVERS='localhost:54321',
         EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT=4,
     )
+    @patch('edx_event_bus_kafka.internal.consumer.logger', autospec=True)
+    def test_no_consume_with_bad_offset_timestamp(self, mock_logger):
+        with pytest.raises(Exception) as exc_info:
+            KafkaEventConsumer('some-topic', 'test_group_id', offset_time="12345")
+        assert exc_info.value.args == ("Invalid isoformat string: '12345'",)
+        mock_logger.exception.assert_any_call('Could not parse the offset timestamp.')
+
+    @override_settings(
+        EVENT_BUS_KAFKA_SCHEMA_REGISTRY_URL='http://localhost:12345',
+        EVENT_BUS_KAFKA_BOOTSTRAP_SERVERS='localhost:54321',
+        EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT=4,
+    )
     def test_non_consecutive_errors(self):
         """Confirm that non-consecutive errors may not break out of loop."""
         def raise_exception():
             raise Exception("something broke")
 
         mock_emit_side_effects = [
             raise_exception, raise_exception,
@@ -307,19 +345,21 @@
             self.event_consumer._shut_down,  # pylint: disable=protected-access
         ]
 
         with patch.object(
                 self.event_consumer, 'emit_signals_from_message',
                 side_effect=side_effects(mock_emit_side_effects)
         ) as mock_emit:
-            mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
-            self.event_consumer.consumer = mock_consumer
-            self.event_consumer.consume_indefinitely()  # exits normally
+            with patch('edx_event_bus_kafka.internal.consumer.AvroDeserializer',
+                       return_value=lambda _x, _y: self.normal_event_data):
+                mock_consumer = Mock(**{'poll.return_value': self.normal_message}, autospec=True)
+                self.event_consumer.consumer = mock_consumer
+                self.event_consumer.consume_indefinitely()  # exits normally
 
-        assert mock_emit.call_args_list == [call(self.normal_message)] * len(mock_emit_side_effects)
+        assert mock_emit.call_args_list == [call(self.normal_message, self.signal)] * len(mock_emit_side_effects)
 
     TEST_FAILED_MESSAGE = FakeMessage(
         partition=7,
         offset=6789,
         headers=[
             ('ce_id', b'1111-1111'),
             ('ce_type', b'org.openedx.learning.auth.session.login.completed.v1'),
@@ -375,16 +415,14 @@
         # in some order.
         mock_logger.error.assert_not_called()
         mock_logger.exception.assert_called_once()
         (exc_log_msg,) = mock_logger.exception.call_args.args
         assert f"Error consuming event from Kafka: {repr(exception)} in context" in exc_log_msg
         assert "full_topic='local-some-topic'" in exc_log_msg
         assert "consumer_group='test_group_id'" in exc_log_msg
-        assert ("expected_signal=<OpenEdxPublicSignal: "
-                "org.openedx.learning.auth.session.login.completed.v1>") in exc_log_msg
         if has_message:
             assert "-- event details" in exc_log_msg
         else:
             assert "-- no event available" in exc_log_msg
 
         expected_custom_attribute_calls = [
             call("kafka_topic", "local-some-topic"),
@@ -404,42 +442,42 @@
         # For non-fatal errors, "no-event" sleep branch was triggered
         if not is_fatal:
             mock_sleep.assert_called_once_with(1)
 
         mock_consumer.commit.assert_not_called()
 
     def test_check_event_error(self):
-        """
-        DeserializingConsumer.poll() should never return a Message with an error() object,
-        but we check it anyway as a safeguard. This test exercises that branch.
-        """
         with pytest.raises(Exception) as exc_info:
             self.event_consumer.emit_signals_from_message(
                 FakeMessage(
                     partition=2,
                     error=KafkaError(123, "done broke"),
-                )
+                    headers=[{'ce_type': 'org.openedx.learning.auth.session.login.completed.v1'}]
+                ),
+                self.signal
             )
 
         assert exc_info.value.args == (
-            "Polled message had error object (shouldn't happen): "
+            "Polled message had error object: "
             "KafkaError{code=ERR_123?,val=123,str=\"done broke\"}",
         )
 
     @override_settings(
         EVENT_BUS_TOPIC_PREFIX='local',
     )
     @patch('edx_event_bus_kafka.internal.consumer.set_custom_attribute', autospec=True)
     @patch('edx_event_bus_kafka.internal.consumer.logger', autospec=True)
     @ddt.data(True, False)
     def test_emit_success(self, audit_logging, mock_logger, mock_set_attribute):
         self.signal.disconnect(fake_receiver_raises_error)  # just successes for this one!
+        # assume we've already deserialized the data
+        self.normal_message.set_value(self.normal_event_data)
 
         with override_settings(EVENT_BUS_KAFKA_AUDIT_LOGGING_ENABLED=audit_logging):
-            self.event_consumer.emit_signals_from_message(self.normal_message)
+            self.event_consumer.emit_signals_from_message(self.normal_message, self.signal)
         self.assert_signal_sent_with(self.signal, self.normal_event_data)
         # Specifically, not called with 'kafka_logging_error'
         mock_set_attribute.assert_not_called()
         if audit_logging:
             mock_logger.info.assert_has_calls([
                 call(
                     "Message received from Kafka: topic=local-some-topic, partition=2, "
@@ -454,33 +492,37 @@
     @override_settings(
         EVENT_BUS_TOPIC_PREFIX='local',
     )
     @patch('edx_event_bus_kafka.internal.consumer.set_custom_attribute', autospec=True)
     @patch('edx_event_bus_kafka.internal.consumer.logger', autospec=True)
     def test_emit_success_tolerates_missing_timestamp(self, mock_logger, mock_set_attribute):
         self.signal.disconnect(fake_receiver_raises_error)  # just successes for this one!
+        # assume we've already deserialized the data
+        self.normal_message.set_value(self.normal_event_data)
         self.normal_message._timestamp = (TIMESTAMP_NOT_AVAILABLE, None)  # pylint: disable=protected-access
 
-        self.event_consumer.emit_signals_from_message(self.normal_message)
+        self.event_consumer.emit_signals_from_message(self.normal_message, self.signal)
         self.assert_signal_sent_with(self.signal, self.normal_event_data)
         # Specifically, not called with 'kafka_logging_error'
         mock_set_attribute.assert_not_called()
         mock_logger.info.assert_has_calls([
             call(
                 "Message received from Kafka: topic=local-some-topic, partition=2, "
                 f"offset=12345, message_id={self.message_id}, "
                 "key=b'\\x00\\x00\\x00\\x00\\x01\\x0cfoobob', event_timestamp_ms=none"
             ),
             call('Message from Kafka processed successfully'),
         ])
 
     @patch('django.dispatch.dispatcher.logger', autospec=True)
     def test_emit(self, mock_logger):
+        # assume we've already deserialized the data
+        self.normal_message.set_value(self.normal_event_data)
         with pytest.raises(ReceiverError) as exc_info:
-            self.event_consumer.emit_signals_from_message(self.normal_message)
+            self.event_consumer.emit_signals_from_message(self.normal_message, self.signal)
         self.assert_signal_sent_with(self.signal, self.normal_event_data)
         assert exc_info.value.args == (
             "1 receiver(s) out of 3 produced errors (stack trace elsewhere in logs) "
             "when handling signal <OpenEdxPublicSignal: "
             "org.openedx.learning.auth.session.login.completed.v1>: "
             "edx_event_bus_kafka.internal.tests.test_consumer.fake_receiver_raises_error="
             "Exception('receiver whoops')",
@@ -493,73 +535,111 @@
         mock_logger.error.assert_called_once_with(
             "Error calling %s in Signal.send_robust() (%s)",
             'fake_receiver_raises_error',
             receiver_error,
             exc_info=receiver_error,
         )
 
+    def test_emit_type_mismatch(self):
+        # assume we've already deserialized the data
+        self.normal_message.set_value(self.normal_event_data)
+        self.normal_message._headers = [('ce_type', b'xxxx')]  # pylint: disable=protected-access
+
+        with pytest.raises(Exception) as excinfo:
+            self.event_consumer.emit_signals_from_message(self.normal_message, self.signal)
+
+        assert excinfo.value.args == (
+            "Error emitting event from Kafka: (UNEXPECTED) message event type xxxx "
+            "does not match signal org.openedx.learning.auth.session.login.completed.v1",
+        )
+        assert not self.mock_receiver.called
+
+    def test_deserialize_type_mismatch(self):
+        self.normal_message._headers = [('ce_type', b'xxxx')]  # pylint: disable=protected-access
+
+        with pytest.raises(Exception) as excinfo:
+            self.event_consumer._deserialize_message_value(  # pylint: disable=protected-access
+                                                           self.normal_message, self.signal
+                                                          )
+
+        assert excinfo.value.args == (
+            "Error deserializing event from Kafka: (UNEXPECTED) message event type xxxx "
+            "does not match signal org.openedx.learning.auth.session.login.completed.v1",
+        )
+        assert not self.mock_receiver.called
+
     def test_malformed_receiver_errors(self):
         """
         Ensure that even a really messed-up receiver is still reported correctly.
         """
         with pytest.raises(ReceiverError) as exc_info:
             self.event_consumer._check_receiver_results([  # pylint: disable=protected-access
                 (lambda x:x, Exception("for lambda")),
                 # This would actually raise an error inside send_robust(), but it will serve well enough for testing...
                 ("not even a function", Exception("just plain bad")),
-            ])
+            ], self.signal)
         assert exc_info.value.args == (
             "2 receiver(s) out of 2 produced errors (stack trace elsewhere in logs) "
             "when handling signal <OpenEdxPublicSignal: "
             "org.openedx.learning.auth.session.login.completed.v1>: "
 
             "edx_event_bus_kafka.internal.tests.test_consumer.TestEmitSignals."
             "test_malformed_receiver_errors.<locals>.<lambda>=Exception('for lambda'), "
 
             "not even a function=Exception('just plain bad')",
         )
 
+    def test_determine_signal_success(self):
+        determined_signal = self.event_consumer.determine_signal(self.normal_message)
+        assert isinstance(determined_signal, OpenEdxPublicSignal)
+        assert determined_signal.event_type == self.signal_type
+
     def test_no_type(self):
         msg = copy.copy(self.normal_message)
+        # assume we've already deserialized the data
+        msg.set_value(self.normal_event_data)
         msg._headers = []  # pylint: disable=protected-access
 
         with pytest.raises(UnusableMessageError) as excinfo:
-            self.event_consumer.emit_signals_from_message(msg)
+            self.event_consumer.determine_signal(msg)
 
         assert excinfo.value.args == (
             "Missing ce_type header on message, cannot determine signal",
         )
         assert not self.mock_receiver.called
 
     def test_multiple_types(self):
         """
         Very unlikely case, but this gets us coverage.
         """
         msg = copy.copy(self.normal_message)
+        # assume we've already deserialized the data
+        msg.set_value(self.normal_event_data)
         msg._headers = [['ce_type', b'abc'], ['ce_type', b'def']]  # pylint: disable=protected-access
 
         with pytest.raises(UnusableMessageError) as excinfo:
-            self.event_consumer.emit_signals_from_message(msg)
+            self.event_consumer.determine_signal(msg)
 
         assert excinfo.value.args == (
             "Multiple ce_type headers found on message, cannot determine signal",
         )
         assert not self.mock_receiver.called
 
     def test_unexpected_signal_type_in_header(self):
         msg = copy.copy(self.normal_message)
+        # assume we've already deserialized the data
+        msg.set_value(self.normal_event_data)
         msg._headers = [  # pylint: disable=protected-access
             ['ce_type', b'xxxx']
         ]
         with pytest.raises(UnusableMessageError) as excinfo:
-            self.event_consumer.emit_signals_from_message(msg)
+            self.event_consumer.determine_signal(msg)
 
         assert excinfo.value.args == (
-            "Signal types do not match. Expected org.openedx.learning.auth.session.login.completed.v1. "
-            "Received message of type xxxx.",
+            "Unrecognized type xxxx found on message, cannot determine signal",
         )
         assert not self.mock_receiver.called
 
     def test_no_commit_if_no_error_logged(self):
         """
         Check that if there is an error that we fail to log, we do not commit the offset
         """
@@ -577,79 +657,29 @@
 
     def test_bad_headers(self):
         """
         Check that if we cannot process the message headers, we raise an UnusableMessageError
 
         The various kinds of bad headers are more fully tested in test_utils
         """
-        self.normal_message._headers = [  # pylint: disable=protected-access
+        msg = copy.copy(self.normal_message)
+        # assume we've already deserialized the data
+        msg.set_value(self.normal_event_data)
+        msg._headers = [  # pylint: disable=protected-access
             ('ce_type', b'org.openedx.learning.auth.session.login.completed.v1'),
             ('ce_id', b'bad_id')
         ]
         with pytest.raises(UnusableMessageError) as excinfo:
-            self.event_consumer.emit_signals_from_message(self.normal_message)
+            self.event_consumer.emit_signals_from_message(msg, self.signal)
 
         assert excinfo.value.args == (
             "Error determining metadata from message headers: badly formed hexadecimal UUID string",
         )
 
         assert not self.mock_receiver.called
 
-
-class TestCommand(TestCase):
-    """
-    Tests for the consume_events management command
-    """
-
-    @override_settings(EVENT_BUS_KAFKA_CONSUMERS_ENABLED=False)
-    @patch('edx_event_bus_kafka.internal.consumer.logger', autospec=True)
-    @patch('edx_event_bus_kafka.internal.consumer.KafkaEventConsumer._create_consumer')
-    def test_kafka_consumers_disabled(self, mock_create_consumer, mock_logger):
-        call_command(Command(), topic='test', group_id='test', signal='')
-        assert not mock_create_consumer.called
-        mock_logger.error.assert_called_once_with("Kafka consumers not enabled, exiting.")
-
-    @patch.dict('edx_event_bus_kafka.internal.consumer.__dict__', {'confluent_kafka': None})
-    @patch('edx_event_bus_kafka.internal.consumer.logger', autospec=True)
-    @patch('edx_event_bus_kafka.internal.consumer.KafkaEventConsumer._create_consumer')
-    def test_kafka_consumers_no_lib(self, mock_create_consumer, mock_logger):
-        call_command(Command(), topic='test', group_id='test', signal='')
-        assert not mock_create_consumer.called
-        mock_logger.error.assert_called_once_with(
-            "Cannot consume events because confluent_kafka dependency (or one of its extras) was not installed"
-        )
-
-    @patch('edx_event_bus_kafka.internal.consumer.OpenEdxPublicSignal.get_signal_by_type')
-    @patch('edx_event_bus_kafka.internal.consumer.KafkaEventConsumer._create_consumer')
-    @patch('edx_event_bus_kafka.internal.consumer.KafkaEventConsumer.consume_indefinitely')
-    def test_kafka_consumers_normal(self, mock_consume, mock_create_consumer, _gsbt):
-        call_command(
-            Command(),
-            topic='test',
-            group_id='test',
-            signal='openedx',
-        )
-        assert mock_create_consumer.called
-        assert mock_consume.called
-
-    @patch('edx_event_bus_kafka.internal.consumer.OpenEdxPublicSignal.get_signal_by_type')
-    @patch('edx_event_bus_kafka.internal.consumer.KafkaEventConsumer._create_consumer')
-    @patch('edx_event_bus_kafka.internal.consumer.KafkaEventConsumer.reset_offsets_and_sleep_indefinitely')
-    def test_kafka_consumers_with_timestamp(self, mock_reset_offsets, mock_create_consumer, _gsbt):
-        call_command(
-            Command(),
-            topic='test',
-            group_id='test',
-            signal='openedx',
-            offset_time=['2019-05-18T15:17:08.132263']
+    def test_no_deserializer_if_no_registry_client(self):
+        with pytest.raises(Exception) as excinfo:
+            get_deserializer(self.signal, None)
+        assert excinfo.value.args == (
+            "Cannot create Kafka deserializer -- missing library or settings",
         )
-        assert mock_create_consumer.called
-        assert mock_reset_offsets.called
-
-    @patch('edx_event_bus_kafka.internal.consumer.logger', autospec=True)
-    @patch('edx_event_bus_kafka.internal.consumer.OpenEdxPublicSignal.get_signal_by_type')
-    @patch('edx_event_bus_kafka.internal.consumer.KafkaEventConsumer._create_consumer')
-    @patch('edx_event_bus_kafka.internal.consumer.KafkaEventConsumer.consume_indefinitely')
-    def test_kafka_consumers_with_bad_timestamp(self, _ci, _cc, _gsbt, mock_logger):
-        call_command(Command(), topic='test', group_id='test', signal='openedx', offset_time=['notatimestamp'])
-        mock_logger.exception.assert_any_call("Could not parse the offset timestamp.")
-        mock_logger.exception.assert_called_with("Error consuming Kafka events")
```

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_producer.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_utils.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,20 @@
         return self._headers
 
     def key(self) -> Optional[bytes]:
         """Bytes (Avro)."""
         return self._key
 
     def value(self):
-        """Deserialized event value."""
+        """Event value (bytes or object)"""
         return self._value
 
+    def set_value(self, value):
+        self._value = value
+
     def error(self):
         return self._error
 
     def timestamp(self):
         return self._timestamp
```

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/utils.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/produce_event.py` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/PKG-INFO` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-bus-kafka
-Version: 3.9.6
+Version: 4.0.0
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -130,17 +130,15 @@
 
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 How To Contribute
 *****************
 
 Contributions are very welcome.
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for all Open edX projects.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <.github/ISSUE_TEMPLATE.md>`_.
 
@@ -199,14 +197,33 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[4.0.0] - 2023-05-10
+********************
+Changed
+=======
+* Implement openedx-events Event Bus Consumer API.
+* **BREAKING CHANGE**: Remove ``consume_events`` management command as this command will be provided by openedx_events. To replay events using the
+  openedx-events version of the management command, pass ``--extra '{"offset_time": "2023-01-08T06:46:22"}'`` instead of ``-o 2023-01-08T06:46:22``.
+* **BREAKING Change**: ``offset_timestamp`` argument has been removed from ``consume_indefinitely`` and ``reset_offsets_and_sleep_indefinitely`` methods.
+  It is now added as an optional argument named ``offset_time`` to ``KafkaEventConsumer`` constructor.
+
+[3.10.0] - 2023-05-05
+*********************
+Changed
+=======
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Refactored consumer to manually deserialize messages instead of using DeserializingConsumer
+* Make signal argument optional in consumer command (take signal from message headers)
+
 [3.9.6] - 2023-02-24
 ********************
 Added
 =====
 * Add function tracing to the event consumption workflow for better monitoring.
 
 [3.9.5] - 2023-02-24
```

### Comparing `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/SOURCES.txt` & `edx_event_bus_kafka-4.0.0/edx_event_bus_kafka.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,13 +22,12 @@
 edx_event_bus_kafka/internal/tests/__init__.py
 edx_event_bus_kafka/internal/tests/test_config.py
 edx_event_bus_kafka/internal/tests/test_consumer.py
 edx_event_bus_kafka/internal/tests/test_producer.py
 edx_event_bus_kafka/internal/tests/test_utils.py
 edx_event_bus_kafka/management/__init__.py
 edx_event_bus_kafka/management/commands/__init__.py
-edx_event_bus_kafka/management/commands/consume_events.py
 edx_event_bus_kafka/management/commands/produce_event.py
 edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
 requirements/base.in
 requirements/constraints.txt
 tests/test_models.py
```

### Comparing `edx_event_bus_kafka-3.9.6/requirements/constraints.txt` & `edx_event_bus_kafka-4.0.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.6/setup.py` & `edx_event_bus_kafka-4.0.0/setup.py`

 * *Files identical despite different names*

