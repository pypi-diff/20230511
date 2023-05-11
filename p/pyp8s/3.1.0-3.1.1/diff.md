# Comparing `tmp/pyp8s-3.1.0-py3-none-any.whl.zip` & `tmp/pyp8s-3.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19182 bytes, number of entries: 10
--rw-r--r--  2.0 unx      298 b- defN 23-May-02 00:01 pyp8s/__init__.py
--rw-r--r--  2.0 unx      250 b- defN 23-May-02 00:01 pyp8s/_version.py
--rw-r--r--  2.0 unx    12339 b- defN 23-May-02 00:01 pyp8s/metrics.py
--rw-r--r--  2.0 unx      226 b- defN 23-May-02 00:01 tests/__init__.py
--rw-r--r--  2.0 unx     1300 b- defN 23-May-02 00:01 tests/test_import.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2462 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      747 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/RECORD
-10 files, 52875 bytes uncompressed, 17928 bytes compressed:  66.1%
+Zip file size: 19046 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      298 b- defN 23-May-11 01:50 pyp8s/__init__.py
+-rw-r--r--  2.0 unx      250 b- defN 23-May-11 01:50 pyp8s/_version.py
+-rw-r--r--  2.0 unx    11426 b- defN 23-May-11 01:50 pyp8s/metrics.py
+-rw-r--r--  2.0 unx      226 b- defN 23-May-11 01:50 tests/__init__.py
+-rw-r--r--  2.0 unx     1300 b- defN 23-May-11 01:50 tests/test_import.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2462 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      747 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/RECORD
+10 files, 51962 bytes uncompressed, 17792 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_import.py
 Comment: 
 
-Filename: pyp8s-3.1.0.dist-info/LICENSE
+Filename: pyp8s-3.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyp8s-3.1.0.dist-info/METADATA
+Filename: pyp8s-3.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyp8s-3.1.0.dist-info/WHEEL
+Filename: pyp8s-3.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyp8s-3.1.0.dist-info/top_level.txt
+Filename: pyp8s-3.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyp8s-3.1.0.dist-info/RECORD
+Filename: pyp8s-3.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyp8s/_version.py

```diff
@@ -1,8 +1,8 @@
 #!/usr/bin/env python3
 # pylint: disable=line-too-long, missing-function-docstring, logging-fstring-interpolation
 # pylint: disable=too-many-locals, broad-except, too-many-arguments, raise-missing-from
 """
     pyp8s module
 """
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
```

## pyp8s/metrics.py

```diff
@@ -69,46 +69,34 @@
     def __repr__(self):
         return self.__str__()
 
     def __format_labels(self, **kwargs):
         return ["=".join([f"{pair[0]}", f'"{pair[1]}"']) for pair in kwargs.items()]
 
     def __craft_labelset_key(self, **kwargs):
-
-        logging.debug(f"Crafting a metric key from kwargs='{kwargs}'")
-
         kwargs_items_sorted = sorted(kwargs.items(), key=lambda x: x[0].casefold())
-        logging.debug(f"Crafting a metric key kwargs_items_sorted='{kwargs_items_sorted}'")
-
         kwargs_items_joined_pairs = ["_".join([str(pair[0]), str(pair[1])]) for pair in kwargs_items_sorted]
-        logging.debug(f"Crafting a metric key kwargs_items_joined_pairs='{kwargs_items_joined_pairs}'")
-
         kwargs_items_joined_full = "_".join(kwargs_items_joined_pairs)
-        logging.debug(f"Crafting a metric key kwargs_items_joined_full='{kwargs_items_joined_full}'")
 
         return kwargs_items_joined_full
 
     def __get_labelset_item(self, *args, **kwargs):
 
         labelset_key = self.__craft_labelset_key(**kwargs)
 
         if labelset_key not in self.data:
 
-            logging.debug(f"Initialising metric '{labelset_key}'")
-
             self.data[labelset_key] = {
                 "value": 0,
                 "labels": {
                     **kwargs  # TODO: Validate kwargs before saving them
                 },
                 "labels_formatted": self.__format_labels(**kwargs)
             }
 
-            logging.debug(f"New metric initialised: '{self.data[labelset_key]}'")
-
         return self.data[labelset_key]
 
     def set_name(self, metric_name):
         self.metric_name = metric_name
 
     def set_type(self, metric_type):
         self.metric_type = metric_type
@@ -139,15 +127,14 @@
         :type **kwargs: dict[str]
 
         :return: None
         :rtype: None
         """
 
         metric = self.__get_labelset_item(**kwargs)
-        logging.debug(f"Incrementing metric '{metric}' (current {metric['value']})")
         metric["value"] += increment
         logging.debug(f"Incremented metric '{metric}' (new {metric['value']})")
 
     def set(self, value, *args, **kwargs):
         """Sets metric value to a given number
 
         :param value: New value for the metric to set
@@ -158,15 +145,14 @@
         :type **kwargs: dict[str]
 
         :return: None
         :rtype: None
         """
 
         metric = self.__get_labelset_item(**kwargs)
-        logging.debug(f"Incrementing metric '{metric}' (current {metric['value']})")
         metric["value"] = value
         logging.debug(f"Incremented metric '{metric}' (new {metric['value']})")
 
 
 class MetricsHandler(metaclass=Singleton):
 
     def __init__(self):
@@ -179,50 +165,48 @@
 
     @staticmethod
     def serve(listen_address="127.0.0.1", listen_port=19001):
         self = MetricsHandler()
 
         if not self.__is_serving():
 
-            logging.debug(f"UUID={self.uuid} Starting the metrics server on {listen_address} port {listen_port}")
+            logging.debug(f"Starting the metrics server on {listen_address} port {listen_port}")
 
             self.server = ThreadedHTTPServer((listen_address, listen_port), ReqHandlerMetrics)
             self.server_thread = threading.Thread(target=self.server.serve_forever)
 
             self.server_thread.daemon = True
 
-            logging.info(f"UUID={self.uuid} Starting metrics server")
+            logging.info(f"Starting metrics server")
             self.server_thread.start()
-            logging.info(f"UUID={self.uuid} Metrics server started")
+            logging.info(f"Metrics server started")
 
         else:
-            logging.error(f"UUID={self.uuid} Tried to start the metrics server twice")
-            raise Exception(f"UUID={self.uuid} Server already started: {self.server}")
+            logging.error(f"Tried to start the metrics server twice")
+            raise Exception(f"Server already started: {self.server}")
 
     @staticmethod
     def shutdown():
         self = MetricsHandler()
-        logging.debug(f"UUID={self.uuid} Shutting down the metrics server")
+        logging.debug(f"Shutting down the metrics server")
 
         try:
             self.server.shutdown()
         except Exception as e:
-            logging.error(f"UUID={self.uuid} Couldn't shutdown the metrics server: {e}")
+            logging.error(f"Couldn't shutdown the metrics server: {e}")
             raise e
 
     @staticmethod
     def get_metrics():
         self = MetricsHandler()
-        logging.debug("Returning metrics")
         return self.metrics
 
     @staticmethod
     def get_metric(metric_name):
         self = MetricsHandler()
-        logging.debug(f"Returning metric {metric_name}")
         return self.metrics[metric_name]
 
     @staticmethod
     def __get_metric_obj(metric_name):
         self = MetricsHandler()
 
         if metric_name not in self.metrics:
```

## Comparing `pyp8s-3.1.0.dist-info/LICENSE` & `pyp8s-3.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyp8s-3.1.0.dist-info/METADATA` & `pyp8s-3.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp8s
-Version: 3.1.0
+Version: 3.1.1
 Summary: Customisable prometheus exporter for your python application
 Home-page: https://github.com/pyp8s/pyp8s
 Author: Pavel Kim
 Author-email: hello@pavelkim.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

