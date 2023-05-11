# Comparing `tmp/marqo-0.9.4.tar.gz` & `tmp/marqo-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-0.9.4.tar", last modified: Mon Apr 24 07:58:52 2023, max compression
+gzip compressed data, was "marqo-0.9.5.tar", last modified: Thu May 11 01:14:14 2023, max compression
```

## Comparing `marqo-0.9.4.tar` & `marqo-0.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:58:52.644319 marqo-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-24 07:58:35.000000 marqo-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-24 07:58:52.644319 marqo-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-24 07:58:35.000000 marqo-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 07:58:35.000000 marqo-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:58:52.644319 marqo-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-24 07:58:35.000000 marqo-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:58:52.636319 marqo-0.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:58:52.644319 marqo-0.9.4/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/marqo_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-24 07:58:35.000000 marqo-0.9.4/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:58:52.644319 marqo-0.9.4/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-24 07:58:52.000000 marqo-0.9.4/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-24 07:58:52.000000 marqo-0.9.4/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:58:52.000000 marqo-0.9.4/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-24 07:58:52.000000 marqo-0.9.4/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 07:58:52.000000 marqo-0.9.4/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:14:14.271015 marqo-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-05-11 01:14:00.000000 marqo-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-05-11 01:14:14.267015 marqo-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21052 2023-05-11 01:14:00.000000 marqo-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 01:14:00.000000 marqo-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:14:14.271015 marqo-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-11 01:14:00.000000 marqo-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:14:14.263015 marqo-0.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:14:14.267015 marqo-0.9.5/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/marqo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:14:14.267015 marqo-0.9.5/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-0.9.4/LICENSE` & `marqo-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-0.9.4/setup.py` & `marqo-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "pydantic"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="0.9.4",
+    version="0.9.5",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-0.9.4/src/marqo/_httprequests.py` & `marqo-0.9.5/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.4/src/marqo/client.py` & `marqo-0.9.5/src/marqo/client.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.4/src/marqo/config.py` & `marqo-0.9.5/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.4/src/marqo/defaults.py` & `marqo-0.9.5/src/marqo/defaults.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.4/src/marqo/errors.py` & `marqo-0.9.5/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.4/src/marqo/index.py` & `marqo-0.9.5/src/marqo/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         return self.http.post(path=F"indexes/{self.index_name}/refresh")
 
     def search(self, q: Union[str, dict], searchable_attributes: Optional[List[str]] = None,
                limit: int = 10, offset: int = 0, search_method: Union[SearchMethods.TENSOR, str] = SearchMethods.TENSOR,
                highlights=None, device: Optional[str] = None, filter_string: str = None,
                show_highlights=True, reranker=None, image_download_headers: Optional[Dict] = None,
                attributes_to_retrieve: Optional[List[str]] = None, boost: Optional[Dict[str,List[Union[float, int]]]] = None,
-               context: Optional[dict] = None, score_modifiers: Optional[dict] = None,
+               context: Optional[dict] = None, score_modifiers: Optional[dict] = None, model_auth: Optional[dict] = None
                ) -> Dict[str, Any]:
         """Search the index.
 
         Args:
             q: String to search, or a dictionary of weighted strings to search
                 (with the structure <search string>:<weight float>). Strings
                 to search are text or a pointer/url to an image if the index
@@ -141,14 +141,15 @@
             filter_string: a filter string, used to prefilter documents during the
                 search. For example: "car_colour:blue"
             attributes_to_retrieve: a list of document attributes to be
                 retrieved. If left as None, then all attributes will be
                 retrieved.
             context: a dictionary to allow you to bring your own vectors and more into search.
             score_modifiers: a dictionary to modify the score based on field values, for tensor search only
+            model_auth: authorisation that lets Marqo download a private model, if required
         Returns:
             Dictionary with hits and other metadata
         """
 
         start_time_client_request = timer()
         if highlights is not None:
             logging.warning("Deprecation warning for parameter 'highlights'. "
@@ -176,14 +177,16 @@
             body["filter"] = filter_string
         if image_download_headers is not None:
             body["image_download_headers"] = image_download_headers
         if context is not None:
             body["context"] = context
         if score_modifiers is not None:
             body["scoreModifiers"] = score_modifiers
+        if model_auth is not None:
+            body["modelAuth"] = model_auth
         res = self.http.post(
             path=path_with_query_str,
             body=body
         )
 
         num_results = len(res["hits"])
         end_time_client_request = timer()
@@ -242,14 +245,15 @@
         client_batch_size: int = None,
         processes: int = None,
         device: str = None,
         non_tensor_fields: List[str] = None,
         use_existing_tensors: bool = False,
         image_download_headers: dict = None,
         mappings: dict = None,
+        model_auth: dict = None
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """Add documents to this index. Does a partial update on existing documents,
         based on their ID. Adds unseen documents to the index.
 
         Args:
             documents: List of documents. Each document should be a dictionary.
             auto_refresh: Automatically refresh the index. If you are making
@@ -265,27 +269,28 @@
             device: the device used to index the data. Examples include "cpu",
                 "cuda" and "cuda:2"
             non_tensor_fields: fields within documents to not create and store tensors against.
             use_existing_tensors: use vectors that already exist in the docs.
             image_download_headers: a dictionary of headers to be passed while downloading images,
                 for URLs found in documents
             mappings: a dictionary to help handle the object fields. e.g., multimodal_combination field
-
+            model_auth: used to authorise a private model
         Returns:
             Response body outlining indexing result
         """
         if non_tensor_fields is None:
             non_tensor_fields = []
         if image_download_headers is None:
             image_download_headers = dict()
         return self._generic_add_update_docs(
             update_method="replace",
             documents=documents, auto_refresh=auto_refresh, server_batch_size=server_batch_size,
             client_batch_size=client_batch_size, processes=processes, device=device, non_tensor_fields=non_tensor_fields,
-            use_existing_tensors=use_existing_tensors, image_download_headers=image_download_headers, mappings = mappings
+            use_existing_tensors=use_existing_tensors, image_download_headers=image_download_headers, mappings=mappings,
+            model_auth=model_auth
         )
 
     def update_documents(
         self,
         documents: List[Dict[str, Any]],
         auto_refresh=True,
         server_batch_size: int = None,
@@ -338,15 +343,16 @@
         server_batch_size: int = None,
         client_batch_size: int = None,
         processes: int = None,
         device: str = None,
         non_tensor_fields: List = None,
         use_existing_tensors: bool = False,
         image_download_headers: dict = None,
-        mappings: dict = None
+        mappings: dict = None,
+        model_auth: dict = None
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
 
         error_detected_message = ('Errors detected in add documents call. '
                                   'Please examine the returned result object for more information.')
         if non_tensor_fields is None:
             non_tensor_fields = []
 
@@ -356,23 +362,25 @@
         # ADD DOCS TIMER-LOGGER (1)
         t0 = timer()
         start_time_client_process = timer()
         base_path = f"indexes/{self.index_name}/documents"
         non_tensor_fields_query_param = utils.convert_list_to_query_params("non_tensor_fields", non_tensor_fields)
         image_download_headers_param = (utils.convert_dict_to_url_params(image_download_headers)
                                         if image_download_headers else '')
+        model_auth_param = (utils.convert_dict_to_url_params(model_auth) if model_auth else '')
         mappings_param = (utils.convert_dict_to_url_params(mappings) if mappings else '')
         query_str_params = (
             f"{f'&device={utils.translate_device_string_for_url(selected_device)}'}"
             f"{f'&processes={processes}' if processes is not None else ''}"
             f"{f'&batch_size={server_batch_size}' if server_batch_size is not None else ''}"
             f"{f'&use_existing_tensors={str(use_existing_tensors).lower()}' if use_existing_tensors is not None else ''}"
             f"{f'&{non_tensor_fields_query_param}' if len(non_tensor_fields) > 0 else ''}"
             f"{f'&image_download_headers={image_download_headers_param}' if image_download_headers else ''}"
             f"{f'&mappings={mappings_param}' if mappings else ''}"
+            f"{f'&model_auth={model_auth_param}' if model_auth_param else ''}"
         )
         end_time_client_process = timer()
         total_client_process_time = end_time_client_process - start_time_client_process
         mq_logger.debug(f"add_documents pre-processing: took {(total_client_process_time):.3f}s for {num_docs} docs, "
                        f"for an average of {(total_client_process_time / num_docs):.3f}s per doc.")
 
         if client_batch_size is not None:
```

### Comparing `marqo-0.9.4/src/marqo/models.py` & `marqo-0.9.5/src/marqo/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     reRanker: str = None
     filter: str = None
     attributesToRetrieve: Union[None, List[str]] = None
     boost: Optional[Dict] = None
     image_download_headers: Optional[Dict] = None
     context: Optional[Dict] = None
     scoreModifiers: Optional[Dict] = None
-
+    modelAuth: Optional[Dict] = None
 
 class BulkSearchBody(SearchBody):
     index: str
     # Attributes that are not supported in bulk search
     context: None = None
     scoreModifiers: None = None
```

### Comparing `marqo-0.9.4/src/marqo/utils.py` & `marqo-0.9.5/src/marqo/utils.py`

 * *Files identical despite different names*

