# Comparing `tmp/pyopencga-2.8.0.tar.gz` & `tmp/pyopencga-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencga-2.8.0.tar", last modified: Tue Apr 25 17:34:32 2023, max compression
+gzip compressed data, was "pyopencga-2.8.1.tar", last modified: Thu May 11 09:36:35 2023, max compression
```

## Comparing `pyopencga-2.8.0.tar` & `pyopencga-2.8.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:32.948865 pyopencga-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 17:34:01.000000 pyopencga-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-25 17:34:32.948865 pyopencga-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-25 17:34:01.000000 pyopencga-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:32.944865 pyopencga-2.8.0/pyopencga/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/opencga_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/opencga_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:32.948865 pyopencga-2.8.0/pyopencga/rest_clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/_parent_rest_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/alignment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52128 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/clinical_analysis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52556 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/clinical_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/cohort_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/disease_panel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/family_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26628 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/file_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/ga4gh_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/individual_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/job_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/project_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/sample_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/study_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/user_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61336 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/variant_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/variant_operation_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:32.944865 pyopencga-2.8.0/pyopencga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:34:32.948865 pyopencga-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-25 17:34:01.000000 pyopencga-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:35.872818 pyopencga-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 09:35:59.000000 pyopencga-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-11 09:36:35.872818 pyopencga-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-11 09:35:59.000000 pyopencga-2.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:35.868818 pyopencga-2.8.1/pyopencga/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/opencga_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/opencga_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:35.872818 pyopencga-2.8.1/pyopencga/rest_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/rest_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/rest_clients/_parent_rest_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/rest_clients/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/alignment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52128 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/clinical_analysis_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52556 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/clinical_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/cohort_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/disease_panel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/family_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26628 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/file_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/ga4gh_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/individual_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/job_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/sample_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/study_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/user_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61336 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/variant_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/variant_operation_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/rest_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:35.868818 pyopencga-2.8.1/pyopencga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:36:35.872818 pyopencga-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-11 09:35:59.000000 pyopencga-2.8.1/setup.py
```

### Comparing `pyopencga-2.8.0/LICENSE` & `pyopencga-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/PKG-INFO` & `pyopencga-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 2.8.0
+Version: 2.8.1
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
```

### Comparing `pyopencga-2.8.0/README.rst` & `pyopencga-2.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/commons.py` & `pyopencga-2.8.1/pyopencga/commons.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             else:
                 opts.append(k + '=' + str(v))
         if opts:
             url += '?' + '&'.join(opts)
     return url, header
 
 
-def _fetch(host, version, sid, category, resource, method, subcategory=None, query_id=None,
+def _fetch(config, sid, category, resource, method, subcategory=None, query_id=None,
            second_query_id=None, data=None, options=None):
     """Queries the REST service retrieving results until exhaustion or limit"""
     # HERE BE DRAGONS
     final_response = None
 
     # Setting up skip and limit default parameters
     call_skip = 0
@@ -124,16 +124,16 @@
                 current_id_indexes = range(len(total_id_list))
             else:
                 current_query_id = ','.join(next_id_list)
                 current_id_list = next_id_list
                 current_id_indexes = next_id_indexes
 
         # Retrieving url
-        url, header = _create_rest_url(host=host,
-                                       version=version,
+        url, header = _create_rest_url(host=config.host,
+                                       version=config.version,
                                        category=category,
                                        sid=sid,
                                        subcategory=subcategory,
                                        query_id=current_query_id,
                                        second_query_id=second_query_id,
                                        resource=resource,
                                        options=opts)
@@ -141,30 +141,30 @@
         # DEBUG param
         if opts is not None and 'debug' in opts and opts['debug']:
             sys.stderr.write(url + '\n')
 
         # Getting REST response
         if method == 'get':
             try:
-                r = requests.get(url, headers=header)
+                r = requests.get(url, headers=header, cookies=config.cookies)
             except requests.exceptions.ConnectionError:
                 sleep(1)
-                r = requests.get(url, headers=header)
+                r = requests.get(url, headers=header, cookies=config.cookies)
         elif method == 'post':
             try:
-                r = requests.post(url, json=data, headers=header)
+                r = requests.post(url, json=data, headers=header, cookies=config.cookies)
             except requests.exceptions.ConnectionError:
                 sleep(1)
-                r = requests.post(url, json=data, headers=header)
+                r = requests.post(url, json=data, headers=header, cookies=config.cookies)
         elif method == 'delete':
             try:
-                r = requests.delete(url, headers=header)
+                r = requests.delete(url, headers=header, cookies=config.cookies)
             except requests.exceptions.ConnectionError:
                 sleep(1)
-                r = requests.delete(url, headers=header)
+                r = requests.delete(url, headers=header, cookies=config.cookies)
         else:
             raise NotImplementedError('method: ' + method + ' not implemented.')
 
         if r.status_code == 504:  # Gateway Time-out
             if time_out_counter == 99:
                 msg = 'Server not responding in time'
                 raise requests.ConnectionError(msg)
@@ -231,22 +231,22 @@
             # When 'limit' is 0 returns all the results. So, break the loop if 0
             if max_limit == 0:
                 break
 
     return final_response
 
 
-def _worker(queue, results, host, version, sid, category, resource, method, subcategory=None,
+def _worker(queue, results, config, sid, category, resource, method, subcategory=None,
             second_query_id=None, data=None, options=None):
 
     """Manages the queue system for the threads"""
     while True:
         # Fetching new element from the queue
         index, query_id = queue.get()
-        response = _fetch(host=host, version=version, sid=sid, category=category, subcategory=subcategory,
+        response = _fetch(config=config, sid=sid, category=category, subcategory=subcategory,
                           resource=resource, method=method, data=data, query_id=query_id,
                           second_query_id=second_query_id, options=options)
         # Store data in results at correct index
         results[index] = response
         # Signaling to the queue that task has been processed
         queue.task_done()
 
@@ -271,28 +271,28 @@
                         final_response['responses'][j][key] = query_result[key]
                     else:
                         if isinstance(query_result[key], (int, list)):
                             final_response['responses'][j][key] += query_result[key]
     return final_response
 
 
-def execute(host, version, sid, category, resource, method, subcategory=None, query_id=None,
+def execute(config, sid, category, resource, method, subcategory=None, query_id=None,
             second_query_id=None, data=None, options=None):
     """Queries the REST service using multiple threads if needed"""
 
     # If query_id is an array, convert to comma-separated string
     if query_id is not None:
         if isinstance(query_id, list):
             query_id = ','.join([str(item) for item in query_id])
         else:
             query_id = str(query_id)  # convert to string so we can call this method with int ids
 
     # Multithread if the number of queries is greater than _CALL_BATCH_SIZE
     if query_id is None or len(query_id.split(',')) <= _CALL_BATCH_SIZE:
-        response = _fetch(host=host, version=version, sid=sid, category=category, subcategory=subcategory,
+        response = _fetch(config=config, sid=sid, category=category, subcategory=subcategory,
                           resource=resource, method=method, data=data, query_id=query_id,
                           second_query_id=second_query_id, options=options)
         return response
     else:
         if options is not None and 'num_threads' in options:
             num_threads = options['num_threads']
         else:
@@ -309,16 +309,15 @@
         res = [''] * len(id_batches)
 
         # Setting up the threads
         for thread in range(num_threads):
             t = threading.Thread(target=_worker,
                                  kwargs={'queue': q,
                                          'results': res,
-                                         'host': host,
-                                         'version': version,
+                                         'config': config,
                                          'sid': sid,
                                          'category': category,
                                          'subcategory': subcategory,
                                          'second_query_id': second_query_id,
                                          'resource': resource,
                                          'method': method,
                                          'data': data,
```

### Comparing `pyopencga-2.8.0/pyopencga/opencga_client.py` & `pyopencga-2.8.1/pyopencga/opencga_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/opencga_config.py` & `pyopencga-2.8.1/pyopencga/opencga_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
+import os
 import json
 import requests
 import yaml
 
 
 class ClientConfiguration(object):
     """
     Configuration class shared between OpenCGA python clients
-
-    usage:     
-        >>> from pyopencga.opencga_config import ClientConfiguration
-        >>> config_file = "/opt/opencga/conf/client-configuration.yml" # it can accept .json
-        >>> ClientConfiguration(configuration)
     """
     
     def __init__(self, config_input):
         """
         :param config_input: a dict, or a yaml/json file containing an OpenCGA valid client configuration.
         """
 
@@ -25,25 +21,21 @@
         if isinstance(config_input, dict):
             self._config = config_input
         else:
             self._config = self._get_dictionary_from_file(config_input)
 
         self._validate_configuration(self._config)
 
-    def _get_dictionary_from_file(self, config_fpath):
-        try:
-            config_fhand = open(config_fpath, 'r')
-        except:
-            msg = 'Unable to read file "' + config_fpath + '"'
-            raise IOError(msg)
+    @staticmethod
+    def _get_dictionary_from_file(config_fpath):
+        config_fhand = open(config_fpath, 'r')
 
         config_dict = None
         if config_fpath.endswith('.yml') or config_fpath.endswith('.yaml'):
             config_dict = yaml.safe_load(config_fhand)
-
         if config_fpath.endswith('.json'):
             config_dict = json.loads(config_fhand.read())
 
         config_fhand.close()
 
         return config_dict
 
@@ -55,15 +47,16 @@
             raise ValueError('Missing "rest" field from configuration dictionary. Please, pass a valid OpenCGA configuration dictionary')
 
         if 'host' not in config['rest'] or not config['rest']['host']:
             raise ValueError('Missing or empty "host" in OpenCGA configuration')
 
         self._validate_host(config['rest']['host'])
 
-    def _validate_host(self, host):
+    @staticmethod
+    def _validate_host(host):
         if not (host.startswith('http://') or host.startswith('https://')):
             host = 'http://' + host
         try:
             r = requests.head(host, timeout=2)
             if r.status_code == 302:
                 return
         except requests.ConnectionError:
@@ -77,15 +70,24 @@
     def host(self, new_host):
         if not (new_host.startswith('http://') or new_host.startswith('https://')):
             new_host = 'http://' + new_host
         self._config['rest']['host'] = new_host
 
     @property
     def version(self):
-        return 'v2'
+        return self._config['version'] if 'version' in self._config else 'v2'
+
+    @property
+    def cookies(self):
+        if 'cookies' in self._config and self._config['cookies']:
+            python_session_fhand = open(os.path.expanduser("~/.opencga/python_session.json"), 'r')
+            session_info = json.loads(python_session_fhand.read())
+            return session_info['cookies']
+        else:
+            return None
 
     @property
     def configuration(self):
         return self._config
 
     @property
     def max_attempts(self):
```

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/_parent_rest_clients.py` & `pyopencga-2.8.1/pyopencga/rest_clients/_parent_rest_clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     def _rest_retry(self, method, category, resource, query_id=None, subcategory=None,
                     second_query_id=None, data=None, dont_retry=None,
                     **options):
 
         query_ids_str = self._get_query_id_str(query_id)
 
         def exec_retry():
-            return execute(host=self._cfg.host,
-                           version=self._cfg.version,
+            return execute(config=self._cfg,
                            sid=self.token,
                            category=category,
                            subcategory=subcategory,
                            method=method,
                            query_id=query_ids_str,
                            second_query_id=second_query_id,
                            resource=resource,
```

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/admin_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/admin_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/alignment_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/alignment_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/clinical_analysis_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/clinical_analysis_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/clinical_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/clinical_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/cohort_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/cohort_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/disease_panel_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/disease_panel_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/family_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/family_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/file_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/file_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/ga4gh_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/ga4gh_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/individual_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/individual_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/job_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/job_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/meta_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/meta_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/project_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/project_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/sample_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/sample_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/study_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/study_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/user_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/user_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/variant_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/variant_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_clients/variant_operation_client.py` & `pyopencga-2.8.1/pyopencga/rest_clients/variant_operation_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/rest_response.py` & `pyopencga-2.8.1/pyopencga/rest_response.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga/retry.py` & `pyopencga-2.8.1/pyopencga/retry.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/pyopencga.egg-info/PKG-INFO` & `pyopencga-2.8.1/pyopencga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 2.8.0
+Version: 2.8.1
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
```

### Comparing `pyopencga-2.8.0/pyopencga.egg-info/SOURCES.txt` & `pyopencga-2.8.1/pyopencga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.0/setup.py` & `pyopencga-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyopencga',
-    version='2.8.0',
+    version='2.8.1',
     description='A REST client for OpenCGA REST web services',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga',
     packages=['pyopencga', 'pyopencga.rest_clients'],
     license='Apache Software License',
     author='David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil',
```

