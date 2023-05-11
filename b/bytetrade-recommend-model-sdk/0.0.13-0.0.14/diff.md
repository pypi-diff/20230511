# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.13.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.13.tar", last modified: Wed May 10 04:09:41 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.14.tar", last modified: Thu May 11 19:47:28 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.13.tar` & `bytetrade-recommend-model-sdk-0.0.14.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 04:09:41.503509 bytetrade-recommend-model-sdk-0.0.13/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       75 2023-05-10 04:08:43.000000 bytetrade-recommend-model-sdk-0.0.13/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-10 04:09:41.503509 bytetrade-recommend-model-sdk-0.0.13/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-04-24 08:15:48.000000 bytetrade-recommend-model-sdk-0.0.13/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 04:09:41.499509 bytetrade-recommend-model-sdk-0.0.13/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-10 04:09:41.000000 bytetrade-recommend-model-sdk-0.0.13/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      983 2023-05-10 04:09:41.000000 bytetrade-recommend-model-sdk-0.0.13/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-10 04:09:41.000000 bytetrade-recommend-model-sdk-0.0.13/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-05-10 04:09:41.000000 bytetrade-recommend-model-sdk-0.0.13/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-10 04:09:41.000000 bytetrade-recommend-model-sdk-0.0.13/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 04:09:41.499509 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 08:07:33.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 04:09:41.499509 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 15:19:49.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-04-21 15:20:39.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2518 2023-04-22 09:06:18.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 04:09:41.503509 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-23 00:13:23.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-04-28 08:19:07.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 04:09:41.503509 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/rank/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:16:24.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/rank/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:17:41.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/rank/faiss_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7781 2023-05-07 22:18:42.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/rank/rank_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-07 06:11:48.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/rank/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 04:09:41.503509 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 01:30:23.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      740 2023-04-21 13:49:04.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 04:09:41.503509 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 12:41:52.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3456 2023-04-22 22:25:24.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3652 2023-05-06 12:19:45.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26424 2023-05-08 01:15:21.000000 bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-10 04:09:41.503509 bytetrade-recommend-model-sdk-0.0.13/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-05-08 01:27:22.000000 bytetrade-recommend-model-sdk-0.0.13/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-10 04:37:58.000000 bytetrade-recommend-model-sdk-0.0.14/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-04-24 08:15:48.000000 bytetrade-recommend-model-sdk-0.0.14/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.380156 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      983 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.380156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 08:07:33.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 15:19:49.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-04-21 15:20:39.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2518 2023-04-22 09:06:18.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-23 00:13:23.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-04-28 08:19:07.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:16:24.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:17:41.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/faiss_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9462 2023-05-11 19:36:12.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/rank_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-07 06:11:48.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 01:30:23.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      740 2023-04-21 13:49:04.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 12:41:52.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3456 2023-04-22 22:25:24.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3652 2023-05-06 12:19:45.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26424 2023-05-08 01:15:21.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-05-11 19:46:20.000000 bytetrade-recommend-model-sdk-0.0.14/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.13/README.md` & `bytetrade-recommend-model-sdk-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/rank/rank_tool.py` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/rank_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 class RankTool:
     def __init__(self,base_document_id_to_embedding) -> None:
         """_summary_
 
         Args:
             base_document_id_to_embedding (_type_): _description_
             {
-                "document_id":[],numpy
+                "document_id":{
+                    "embedding":[],numpy
+                    "created_at": datetime
+                }
             }
 
         Raises:
             ValueError: _description_
             ValueError: _description_
             ValueError: _description_
             ValueError: _description_
@@ -31,40 +34,57 @@
         list_current_embedding = list()
         self.__base_length = len(base_document_id_to_embedding)
         self.__base_index_to_document_id = dict()
         self.__base_document_id_to_index = dict()
         self.__common_tool = CommonTool()
         self.__logger = self.__common_tool.get_logger()
         current_index = 0
-        for current_document_id, current_embedding in base_document_id_to_embedding.items():
+        self.__base_document_id_to_created_at_tuple_list = list()
+        for current_document_id, current_embedding_info in base_document_id_to_embedding.items():
             if isinstance(current_document_id,str) is False:
                 raise ValueError(f"current_document_id {current_document_id} is not str")
+            if isinstance(current_embedding_info,dict) is False:
+                raise ValueError("current_embedding_info is not dict")
+            if "embedding" not in current_embedding_info:
+                raise ValueError("embedding not in current_embedding_info")
+            current_embedding = current_embedding_info["embedding"]
             # if isinstance(current_embedding,np.array)
             if isinstance(current_embedding,np.ndarray) is False:
                 raise ValueError('there is embedding is not np.ndarray')
             if current_embedding.dtype != np.float32:
                 raise ValueError("embedding_value is not float32")
+            if "created_at" not in current_embedding_info:
+                raise ValueError("created_at not in current_embedding_info")
+            created_at = current_embedding_info["created_at"]
+            if isinstance(created_at,datetime) is False:
+                raise ValueError("created_at is not datetime")
+            self.__base_document_id_to_created_at_tuple_list.append((current_document_id,created_at))
+            
             set_shape.add(current_embedding.shape)
             list_current_embedding.append(current_embedding)
             self.__base_index_to_document_id[current_index] = current_document_id
             self.__base_document_id_to_index[current_document_id] = current_index
             
             current_index = current_index + 1
-            
+        self.__base_document_id_to_created_at_tuple_list.sort(key=lambda tup: tup[1],reverse=True)
+        self.__logger.debug(self.__base_document_id_to_created_at_tuple_list)
         if len(set_shape) > 1:
             raise ValueError(f'have different shape embeddings')
         self.__embedding_shape = set_shape.pop()
         self.__original_base_embedding = np.stack(list_current_embedding)
         self.__normalized_base_embedding = np.copy(self.__original_base_embedding)
         faiss.normalize_L2(self.__normalized_base_embedding)
         # self.__original_base_embedding_index =  faiss.IndexFlatL2(self.__original_base_embedding)
         self.__cosin_index = faiss.index_factory(self.__embedding_shape[0], "Flat", faiss.METRIC_INNER_PRODUCT)
         self.__cosin_index.add(self.__normalized_base_embedding)
         self.__time_weight_decay_tool = TimeWeightDecayTool()
     
+    def get_latest_article(self,rank_limit=100):
+        
+        pass
     
     def rank(self,document_id_to_document_info,rank_limit = 100):
         # https://github.com/facebookresearch/faiss/issues/396
         # 
         """_summary_
         {
             "document_id":{
@@ -76,20 +96,28 @@
         Args:
             document_id_to_document_info (_type_): _description_
         """
         query_document_length = len(document_id_to_document_info)
         self.__logger.debug(f'query_document_length {query_document_length}')
         if rank_limit > self.__base_length:
             raise ValueError("rank_limit is bigger than base length")
+        full_weight = 50
+
+        if len(document_id_to_document_info) == 0:
+            current_tuple_list = self.__base_document_id_to_created_at_tuple_list[:rank_limit]
+            document_id_to_weight_tuple_list = list()
+            for current_document_id, current_created_at in current_tuple_list:
+                document_id_to_weight_tuple_list.append((current_document_id,self.__time_weight_decay_tool.compute(full_weight,current_created_at,datetime.now())))
+            return document_id_to_weight_tuple_list
+            
         search_k = 3
         while(query_document_length*search_k < 2 * rank_limit):
             search_k = search_k + 1
         self.__logger.debug(f"search_k {search_k}")
         # previous review weight
-        full_weight = 50
         
         # currently weight
         query_index_to_query_document_id = dict()
         query_document_id_to_query_index = dict()
         query_index = 0
         list_query_embedding = list()
         query_document_id_to_weight = dict()
```

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/rank/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/resources/model_management.json`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/model_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.13/setup.py` & `bytetrade-recommend-model-sdk-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.13",
+    version="0.0.14",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==4.21.8",
         "nltk==3.8.1",
         "boto3"
```

