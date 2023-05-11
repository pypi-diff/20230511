# Comparing `tmp/llama_index-0.6.4.tar.gz` & `tmp/llama_index-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.6.4.tar", last modified: Wed May 10 00:11:41 2023, max compression
+gzip compressed data, was "llama_index-0.6.5.tar", last modified: Thu May 11 00:33:02 2023, max compression
```

## Comparing `llama_index-0.6.4.tar` & `llama_index-0.6.5.tar`

### file list

```diff
@@ -1,459 +1,464 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.991842 llama_index-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 00:11:27.000000 llama_index-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 00:11:27.000000 llama_index-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-10 00:11:41.991842 llama_index-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-10 00:11:27.000000 llama_index-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.939840 llama_index-0.6.4/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.939840 llama_index-0.6.4/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/callbacks/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.939840 llama_index-0.6.4/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.943840 llama_index-0.6.4/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/data_structs/document_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/data_structs/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/data_structs/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.943840 llama_index-0.6.4/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.943840 llama_index-0.6.4/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.943840 llama_index-0.6.4/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.943840 llama_index-0.6.4/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.943840 llama_index-0.6.4/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.947840 llama_index-0.6.4/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.947840 llama_index-0.6.4/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.947840 llama_index-0.6.4/llama_index/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/document_summary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.947840 llama_index-0.6.4/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.947840 llama_index-0.6.4/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.947840 llama_index-0.6.4/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.947840 llama_index-0.6.4/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.951840 llama_index-0.6.4/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.951840 llama_index-0.6.4/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.951840 llama_index-0.6.4/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.951840 llama_index-0.6.4/llama_index/indices/response/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24768 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/response/response_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/response/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.951840 llama_index-0.6.4/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/vector_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/llm_predictor/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/node_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.955840 llama_index-0.6.4/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/output_parsers/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.959841 llama_index-0.6.4/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.959841 llama_index-0.6.4/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.959841 llama_index-0.6.4/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.963841 llama_index-0.6.4/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.963841 llama_index-0.6.4/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.963841 llama_index-0.6.4/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/image_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/weaviate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/response/pprint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.967841 llama_index-0.6.4/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.971841 llama_index-0.6.4/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.971841 llama_index-0.6.4/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.971841 llama_index-0.6.4/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.971841 llama_index-0.6.4/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/token_counter/token_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.971841 llama_index-0.6.4/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/tools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.975841 llama_index-0.6.4/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.975841 llama_index-0.6.4/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-10 00:11:27.000000 llama_index-0.6.4/llama_index/vector_stores/weaviate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.939840 llama_index-0.6.4/llama_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-10 00:11:41.000000 llama_index-0.6.4/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-05-10 00:11:41.000000 llama_index-0.6.4/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:11:41.000000 llama_index-0.6.4/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 00:11:41.000000 llama_index-0.6.4/llama_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 00:11:41.000000 llama_index-0.6.4/llama_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-10 00:11:27.000000 llama_index-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 00:11:41.991842 llama_index-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-10 00:11:27.000000 llama_index-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.975841 llama_index-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.975841 llama_index-0.6.4/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.975841 llama_index-0.6.4/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/document_summary/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/postprocessor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.979841 llama_index-0.6.4/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.983842 llama_index-0.6.4/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.983842 llama_index-0.6.4/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/struct_store/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.983842 llama_index-0.6.4/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.983842 llama_index-0.6.4/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/test_lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/test_milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/test_weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.983842 llama_index-0.6.4/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.983842 llama_index-0.6.4/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/optimization/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/prompts/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.987842 llama_index-0.6.4/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.991842 llama_index-0.6.4/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/storage/test_storage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.991842 llama_index-0.6.4/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:41.991842 llama_index-0.6.4/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-10 00:11:27.000000 llama_index-0.6.4/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.292707 llama_index-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 00:32:40.000000 llama_index-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 00:32:40.000000 llama_index-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-11 00:33:02.292707 llama_index-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-11 00:32:40.000000 llama_index-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.236703 llama_index-0.6.5/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.236703 llama_index-0.6.5/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/callbacks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.236703 llama_index-0.6.5/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.240703 llama_index-0.6.5/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/data_structs/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.240703 llama_index-0.6.5/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.240703 llama_index-0.6.5/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.240703 llama_index-0.6.5/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.240703 llama_index-0.6.5/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.240703 llama_index-0.6.5/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.240703 llama_index-0.6.5/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.240703 llama_index-0.6.5/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.244703 llama_index-0.6.5/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.244703 llama_index-0.6.5/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.244703 llama_index-0.6.5/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.244703 llama_index-0.6.5/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.244703 llama_index-0.6.5/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.244703 llama_index-0.6.5/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.244703 llama_index-0.6.5/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.244703 llama_index-0.6.5/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.248704 llama_index-0.6.5/llama_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.248704 llama_index-0.6.5/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.248704 llama_index-0.6.5/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.248704 llama_index-0.6.5/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/vector_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.248704 llama_index-0.6.5/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.252704 llama_index-0.6.5/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.252704 llama_index-0.6.5/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/llm_predictor/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.252704 llama_index-0.6.5/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.252704 llama_index-0.6.5/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.252704 llama_index-0.6.5/llama_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.252704 llama_index-0.6.5/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/output_parsers/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.252704 llama_index-0.6.5/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.252704 llama_index-0.6.5/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.256704 llama_index-0.6.5/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.260705 llama_index-0.6.5/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.260705 llama_index-0.6.5/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.260705 llama_index-0.6.5/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.260705 llama_index-0.6.5/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.264705 llama_index-0.6.5/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.264705 llama_index-0.6.5/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.264705 llama_index-0.6.5/llama_index/readers/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.264705 llama_index-0.6.5/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.264705 llama_index-0.6.5/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.264705 llama_index-0.6.5/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.264705 llama_index-0.6.5/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.264705 llama_index-0.6.5/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.268705 llama_index-0.6.5/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.268705 llama_index-0.6.5/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.268705 llama_index-0.6.5/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.268705 llama_index-0.6.5/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.268705 llama_index-0.6.5/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.272706 llama_index-0.6.5/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.272706 llama_index-0.6.5/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/tools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.272706 llama_index-0.6.5/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.272706 llama_index-0.6.5/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-11 00:32:41.000000 llama_index-0.6.5/llama_index/vector_stores/weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.236703 llama_index-0.6.5/llama_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-11 00:33:02.000000 llama_index-0.6.5/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14219 2023-05-11 00:33:02.000000 llama_index-0.6.5/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:33:02.000000 llama_index-0.6.5/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 00:33:02.000000 llama_index-0.6.5/llama_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 00:33:02.000000 llama_index-0.6.5/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-11 00:32:41.000000 llama_index-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:33:02.292707 llama_index-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-11 00:32:41.000000 llama_index-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.276706 llama_index-0.6.5/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.280706 llama_index-0.6.5/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.280706 llama_index-0.6.5/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/postprocessor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.280706 llama_index-0.6.5/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.280706 llama_index-0.6.5/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.280706 llama_index-0.6.5/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.280706 llama_index-0.6.5/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.284706 llama_index-0.6.5/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/test_lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/test_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/test_weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.284706 llama_index-0.6.5/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.284706 llama_index-0.6.5/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.284706 llama_index-0.6.5/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.284706 llama_index-0.6.5/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.284706 llama_index-0.6.5/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.284706 llama_index-0.6.5/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.284706 llama_index-0.6.5/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.288707 llama_index-0.6.5/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.288707 llama_index-0.6.5/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.288707 llama_index-0.6.5/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.288707 llama_index-0.6.5/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.288707 llama_index-0.6.5/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.292707 llama_index-0.6.5/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:33:02.292707 llama_index-0.6.5/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-11 00:32:41.000000 llama_index-0.6.5/tests/vector_stores/test_weaviate.py
```

### Comparing `llama_index-0.6.4/LICENSE` & `llama_index-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/PKG-INFO` & `llama_index-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_index
-Version: 0.6.4
+Version: 0.6.5
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `llama_index-0.6.4/README.md` & `llama_index-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/__init__.py` & `llama_index-0.6.5/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/callbacks/base.py` & `llama_index-0.6.5/llama_index/callbacks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         event_id: str = "",
         **kwargs: Any
     ) -> None:
         """Run handlers when an event ends."""
         event_id = event_id or str(uuid.uuid4())
         for handler in self.handlers:
             if event_type not in handler.event_ends_to_ignore:
-                handler.on_event_start(event_type, payload, event_id=event_id, **kwargs)
+                handler.on_event_end(event_type, payload, event_id=event_id, **kwargs)
 
     def add_handler(self, handler: BaseCallbackHandler) -> None:
         """Add a handler to the callback manager."""
         self.handlers.append(handler)
 
     def remove_handler(self, handler: BaseCallbackHandler) -> None:
         """Remove a handler from the callback manager."""
```

### Comparing `llama_index-0.6.4/llama_index/callbacks/llama_debug.py` & `llama_index-0.6.5/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/composability/joint_qa_summary.py` & `llama_index-0.6.5/llama_index/composability/joint_qa_summary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Joint QA Summary graph."""
 
 
 from typing import Sequence, Optional
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.list.base import GPTListIndex
 from llama_index.indices.vector_store import GPTVectorStoreIndex
 from llama_index.readers.schema.base import Document
 from llama_index.selectors.llm_selectors import LLMSingleSelector
 from llama_index.storage.storage_context import StorageContext
 
@@ -55,21 +54,15 @@
     def build_from_documents(
         self,
         documents: Sequence[Document],
     ) -> RouterQueryEngine:
         """Build query engine."""
 
         # parse nodes
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.CHUNKING, payload={"documents": documents}
-        )
         nodes = self._service_context.node_parser.get_nodes_from_documents(documents)
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.CHUNKING, payload={"nodes": nodes}, event_id=event_id
-        )
 
         # ingest nodes
         self._storage_context.docstore.add_documents(nodes, allow_update=True)
 
         # build indices
         vector_index = GPTVectorStoreIndex(
             nodes,
```

### Comparing `llama_index-0.6.4/llama_index/data_structs/data_structs.py` & `llama_index-0.6.5/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/data_structs/document_summary.py` & `llama_index-0.6.5/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/data_structs/node.py` & `llama_index-0.6.5/llama_index/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/data_structs/registry.py` & `llama_index-0.6.5/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/data_structs/struct_type.py` & `llama_index-0.6.5/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/data_structs/table.py` & `llama_index-0.6.5/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/embeddings/base.py` & `llama_index-0.6.5/llama_index/embeddings/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import asyncio
 from abc import abstractmethod
 from enum import Enum
 from typing import Callable, Coroutine, List, Optional, Tuple
 
 import numpy as np
 
+from llama_index.callbacks.base import CallbackManager
+from llama_index.callbacks.schema import CBEventType
 from llama_index.utils import globals_helper
 
 # TODO: change to numpy array
 EMB_TYPE = List
 
 DEFAULT_EMBED_BATCH_SIZE = 10
 
@@ -48,34 +50,40 @@
 class BaseEmbedding:
     """Base class for embeddings."""
 
     def __init__(
         self,
         embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE,
         tokenizer: Optional[Callable] = None,
+        callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         """Init params."""
         self._total_tokens_used = 0
         self._last_token_usage: Optional[int] = None
         self._tokenizer = tokenizer or globals_helper.tokenizer
+        self.callback_manager = callback_manager or CallbackManager([])
         # list of tuples of id, text
         self._text_queue: List[Tuple[str, str]] = []
         if embed_batch_size <= 0:
             raise ValueError("embed_batch_size must be > 0")
         self._embed_batch_size = embed_batch_size
 
     @abstractmethod
     def _get_query_embedding(self, query: str) -> List[float]:
         """Get query embedding."""
 
     def get_query_embedding(self, query: str) -> List[float]:
         """Get query embedding."""
+        event_id = self.callback_manager.on_event_start(CBEventType.EMBEDDING)
         query_embedding = self._get_query_embedding(query)
         query_tokens_count = len(self._tokenizer(query))
         self._total_tokens_used += query_tokens_count
+        self.callback_manager.on_event_end(
+            CBEventType.EMBEDDING, payload={"num_nodes": 1}, event_id=event_id
+        )
         return query_embedding
 
     def get_agg_embedding_from_queries(
         self,
         queries: List[str],
         agg_fn: Optional[Callable[..., List[float]]] = None,
     ) -> List[float]:
@@ -117,17 +125,21 @@
         result = await asyncio.gather(
             *[self._aget_text_embedding(text) for text in texts]
         )
         return result
 
     def get_text_embedding(self, text: str) -> List[float]:
         """Get text embedding."""
+        event_id = self.callback_manager.on_event_start(CBEventType.EMBEDDING)
         text_embedding = self._get_text_embedding(text)
         text_tokens_count = len(self._tokenizer(text))
         self._total_tokens_used += text_tokens_count
+        self.callback_manager.on_event_end(
+            CBEventType.EMBEDDING, payload={"num_nodes": 1}, event_id=event_id
+        )
         return text_embedding
 
     def queue_text_for_embedding(self, text_id: str, text: str) -> None:
         """Queue text for embedding.
 
         Used for batching texts during embedding calls.
```

### Comparing `llama_index-0.6.4/llama_index/embeddings/google.py` & `llama_index-0.6.5/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/embeddings/langchain.py` & `llama_index-0.6.5/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/embeddings/openai.py` & `llama_index-0.6.5/llama_index/embeddings/openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """OpenAI embeddings file."""
 
 from enum import Enum
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Tuple
 
 import openai
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 from llama_index.embeddings.base import BaseEmbedding
 
 
@@ -86,53 +86,55 @@
     (OAEM.TEXT_SEARCH_MODE, "ada"): OAEMM.TEXT_SEARCH_ADA_DOC,
     (OAEM.TEXT_SEARCH_MODE, "text-embedding-ada-002"): OAEMM.TEXT_EMBED_ADA_002,
 }
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
 def get_embedding(
-    text: str,
-    engine: Optional[str] = None,
+    text: str, engine: Optional[str] = None, **kwargs: Any
 ) -> List[float]:
     """Get embedding.
 
     NOTE: Copied from OpenAI's embedding utils:
     https://github.com/openai/openai-python/blob/main/openai/embeddings_utils.py
 
     Copied here to avoid importing unnecessary dependencies
     like matplotlib, plotly, scipy, sklearn.
 
     """
     text = text.replace("\n", " ")
-    return openai.Embedding.create(input=[text], model=engine)["data"][0]["embedding"]
+    return openai.Embedding.create(input=[text], model=engine, **kwargs)["data"][0][
+        "embedding"
+    ]
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
-async def aget_embedding(text: str, engine: Optional[str] = None) -> List[float]:
+async def aget_embedding(
+    text: str, engine: Optional[str] = None, **kwargs: Any
+) -> List[float]:
     """Asynchronously get embedding.
 
     NOTE: Copied from OpenAI's embedding utils:
     https://github.com/openai/openai-python/blob/main/openai/embeddings_utils.py
 
     Copied here to avoid importing unnecessary dependencies
     like matplotlib, plotly, scipy, sklearn.
 
     """
     # replace newlines, which can negatively affect performance.
     text = text.replace("\n", " ")
 
-    return (await openai.Embedding.acreate(input=[text], model=engine))["data"][0][
-        "embedding"
-    ]
+    return (await openai.Embedding.acreate(input=[text], model=engine, **kwargs))[
+        "data"
+    ][0]["embedding"]
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
 def get_embeddings(
-    list_of_text: List[str],
-    engine: Optional[str] = None,
+    list_of_text: List[str], engine: Optional[str] = None, **kwargs: Any
 ) -> List[List[float]]:
     """Get embeddings.
 
     NOTE: Copied from OpenAI's embedding utils:
     https://github.com/openai/openai-python/blob/main/openai/embeddings_utils.py
 
     Copied here to avoid importing unnecessary dependencies
@@ -140,21 +142,21 @@
 
     """
     assert len(list_of_text) <= 2048, "The batch size should not be larger than 2048."
 
     # replace newlines, which can negatively affect performance.
     list_of_text = [text.replace("\n", " ") for text in list_of_text]
 
-    data = openai.Embedding.create(input=list_of_text, model=engine).data
+    data = openai.Embedding.create(input=list_of_text, model=engine, **kwargs).data
     return [d["embedding"] for d in data]
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
 async def aget_embeddings(
-    list_of_text: List[str], engine: Optional[str] = None
+    list_of_text: List[str], engine: Optional[str] = None, **kwargs: Any
 ) -> List[List[float]]:
     """Asynchronously get embeddings.
 
     NOTE: Copied from OpenAI's embedding utils:
     https://github.com/openai/openai-python/blob/main/openai/embeddings_utils.py
 
     Copied here to avoid importing unnecessary dependencies
@@ -162,18 +164,32 @@
 
     """
     assert len(list_of_text) <= 2048, "The batch size should not be larger than 2048."
 
     # replace newlines, which can negatively affect performance.
     list_of_text = [text.replace("\n", " ") for text in list_of_text]
 
-    data = (await openai.Embedding.acreate(input=list_of_text, model=engine)).data
+    data = (
+        await openai.Embedding.acreate(input=list_of_text, model=engine, **kwargs)
+    ).data
     return [d["embedding"] for d in data]
 
 
+def get_engine(
+    mode: str,
+    model: str,
+    mode_model_dict: Dict[Tuple[OpenAIEmbeddingMode, str], OpenAIEmbeddingModeModel],
+) -> OpenAIEmbeddingModeModel:
+    """Get engine."""
+    key = (OpenAIEmbeddingMode(mode), OpenAIEmbeddingModelType(model))
+    if key not in mode_model_dict:
+        raise ValueError(f"Invalid mode, model combination: {key}")
+    return mode_model_dict[key]
+
+
 class OpenAIEmbedding(BaseEmbedding):
     """OpenAI class for embeddings.
 
     Args:
         mode (str): Mode for embedding.
             Defaults to OpenAIEmbeddingMode.TEXT_SEARCH_MODE.
             Options are:
@@ -201,72 +217,45 @@
         mode: str = OpenAIEmbeddingMode.TEXT_SEARCH_MODE,
         model: str = OpenAIEmbeddingModelType.TEXT_EMBED_ADA_002,
         deployment_name: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """Init params."""
         super().__init__(**kwargs)
-        self.mode = OpenAIEmbeddingMode(mode)
-        self.model = OpenAIEmbeddingModelType(model)
         self.deployment_name = deployment_name
+        self.query_engine = get_engine(mode, model, _QUERY_MODE_MODEL_DICT)
+        self.text_engine = get_engine(mode, model, _TEXT_MODE_MODEL_DICT)
 
     def _get_query_embedding(self, query: str) -> List[float]:
         """Get query embedding."""
-        if self.deployment_name is not None:
-            engine = self.deployment_name
-        else:
-            key = (self.mode, self.model)
-            if key not in _QUERY_MODE_MODEL_DICT:
-                raise ValueError(f"Invalid mode, model combination: {key}")
-            engine = _QUERY_MODE_MODEL_DICT[key]
-        return get_embedding(query, engine=engine)
+        return get_embedding(
+            query, engine=self.query_engine, deployment_id=self.deployment_name
+        )
 
     def _get_text_embedding(self, text: str) -> List[float]:
         """Get text embedding."""
-        if self.deployment_name is not None:
-            engine = self.deployment_name
-        else:
-            key = (self.mode, self.model)
-            if key not in _TEXT_MODE_MODEL_DICT:
-                raise ValueError(f"Invalid mode, model combination: {key}")
-            engine = _TEXT_MODE_MODEL_DICT[key]
-        return get_embedding(text, engine=engine)
+        return get_embedding(
+            text, engine=self.text_engine, deployment_id=self.deployment_name
+        )
 
     async def _aget_text_embedding(self, text: str) -> List[float]:
         """Asynchronously get text embedding."""
-        if self.deployment_name is not None:
-            engine = self.deployment_name
-        else:
-            key = (self.mode, self.model)
-            if key not in _TEXT_MODE_MODEL_DICT:
-                raise ValueError(f"Invalid mode, model combination: {key}")
-            engine = _TEXT_MODE_MODEL_DICT[key]
-        return await aget_embedding(text, engine=engine)
+        return await aget_embedding(
+            text, engine=self.text_engine, deployment_id=self.deployment_name
+        )
 
     def _get_text_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Get text embeddings.
 
         By default, this is a wrapper around _get_text_embedding.
         Can be overriden for batch queries.
 
         """
-        if self.deployment_name is not None:
-            engine = self.deployment_name
-        else:
-            key = (self.mode, self.model)
-            if key not in _TEXT_MODE_MODEL_DICT:
-                raise ValueError(f"Invalid mode, model combination: {key}")
-            engine = _TEXT_MODE_MODEL_DICT[key]
-        embeddings = get_embeddings(texts, engine=engine)
-        return embeddings
+        return get_embeddings(
+            texts, engine=self.text_engine, deployment_id=self.deployment_name
+        )
 
     async def _aget_text_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Asynchronously get text embeddings."""
-        if self.deployment_name is not None:
-            engine = self.deployment_name
-        else:
-            key = (self.mode, self.model)
-            if key not in _TEXT_MODE_MODEL_DICT:
-                raise ValueError(f"Invalid mode, model combination: {key}")
-            engine = _TEXT_MODE_MODEL_DICT[key]
-        embeddings = await aget_embeddings(texts, engine=engine)
-        return embeddings
+        return await aget_embeddings(
+            texts, engine=self.text_engine, deployment_id=self.deployment_name
+        )
```

### Comparing `llama_index-0.6.4/llama_index/embeddings/utils.py` & `llama_index-0.6.5/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/evaluation/base.py` & `llama_index-0.6.5/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/evaluation/dataset_generation.py` & `llama_index-0.6.5/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/img_utils.py` & `llama_index-0.6.5/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/__init__.py` & `llama_index-0.6.5/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/base.py` & `llama_index-0.6.5/llama_index/indices/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Base index classes."""
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Generic, List, Optional, Sequence, Type, TypeVar
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs import IndexStruct
 from llama_index.data_structs.node import Node
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
 from llama_index.readers.schema.base import Document
 from llama_index.storage.docstore.types import BaseDocumentStore
@@ -85,21 +84,15 @@
         storage_context = storage_context or StorageContext.from_defaults()
         service_context = service_context or ServiceContext.from_defaults()
         docstore = storage_context.docstore
 
         for doc in documents:
             docstore.set_document_hash(doc.get_doc_id(), doc.get_doc_hash())
 
-        event_id = service_context.callback_manager.on_event_start(
-            CBEventType.CHUNKING, payload={"documents": documents}
-        )
         nodes = service_context.node_parser.get_nodes_from_documents(documents)
-        service_context.callback_manager.on_event_end(
-            CBEventType.CHUNKING, payload={"nodes": nodes}, event_id=event_id
-        )
 
         return cls(
             nodes=nodes,
             storage_context=storage_context,
             service_context=service_context,
             **kwargs,
         )
@@ -168,21 +161,15 @@
         """Insert nodes."""
         self.docstore.add_documents(nodes, allow_update=True)
         self._insert(nodes, **insert_kwargs)
         self._storage_context.index_store.add_index_struct(self._index_struct)
 
     def insert(self, document: Document, **insert_kwargs: Any) -> None:
         """Insert a document."""
-        event_id = self.service_context.callback_manager.on_event_start(
-            CBEventType.CHUNKING, payload={"documents": [document]}
-        )
         nodes = self.service_context.node_parser.get_nodes_from_documents([document])
-        self.service_context.callback_manager.on_event_end(
-            CBEventType.CHUNKING, payload={"nodes": nodes}, event_id=event_id
-        )
         self.insert_nodes(nodes, **insert_kwargs)
         self.docstore.set_document_hash(document.get_doc_id(), document.get_doc_hash())
 
     @abstractmethod
     def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document."""
```

### Comparing `llama_index-0.6.4/llama_index/indices/base_retriever.py` & `llama_index-0.6.5/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/common/struct_store/base.py` & `llama_index-0.6.5/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.6.5/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.6.5/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/common_tree/base.py` & `llama_index-0.6.5/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/composability/graph.py` & `llama_index-0.6.5/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/document_summary/base.py` & `llama_index-0.6.5/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/document_summary/retrievers.py` & `llama_index-0.6.5/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/empty/base.py` & `llama_index-0.6.5/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/empty/retrievers.py` & `llama_index-0.6.5/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.6.5/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/keyword_table/base.py` & `llama_index-0.6.5/llama_index/indices/keyword_table/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from abc import abstractmethod
 from enum import Enum
 from typing import Any, Optional, Sequence, Set, Union
 
 from llama_index.async_utils import run_async_tasks
-from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs import KeywordTable
 from llama_index.data_structs.node import Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.utils import extract_keywords_given_response
 from llama_index.indices.service_context import ServiceContext
 from llama_index.prompts.default_prompts import (
@@ -183,40 +182,22 @@
 
     This index uses a GPT model to extract keywords from the text.
 
     """
 
     def _extract_keywords(self, text: str) -> Set[str]:
         """Extract keywords from text."""
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM,
-            payload={"template": self.keyword_extract_template, "text": text},
-        )
         response, formatted_prompt = self._service_context.llm_predictor.predict(
             self.keyword_extract_template,
             text=text,
         )
         keywords = extract_keywords_given_response(response, start_token="KEYWORDS:")
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
-            event_id=event_id,
-        )
         return keywords
 
     async def _async_extract_keywords(self, text: str) -> Set[str]:
         """Extract keywords from text."""
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM,
-            payload={"template": self.keyword_extract_template, "text": text},
-        )
         response, formatted_prompt = await self._service_context.llm_predictor.apredict(
             self.keyword_extract_template,
             text=text,
         )
         keywords = extract_keywords_given_response(response, start_token="KEYWORDS:")
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
-            event_id=event_id,
-        )
         return keywords
```

### Comparing `llama_index-0.6.4/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.6.5/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.6.5/llama_index/indices/keyword_table/retrievers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Query for GPTKeywordTableIndex."""
 import logging
 from abc import abstractmethod
 from collections import defaultdict
 from typing import Any, Dict, List, Optional
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.base import (
     BaseGPTKeywordTableIndex,
 )
 from llama_index.indices.keyword_table.utils import (
     extract_keywords_given_response,
@@ -117,33 +116,20 @@
 
     See BaseGPTKeywordTableQuery for arguments.
 
     """
 
     def _get_keywords(self, query_str: str) -> List[str]:
         """Extract keywords."""
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM,
-            payload={
-                "template": self.query_keyword_extract_template,
-                "question": query_str,
-                "max_keywords": self.max_keywords_per_query,
-            },
-        )
         response, formatted_prompt = self._service_context.llm_predictor.predict(
             self.query_keyword_extract_template,
             max_keywords=self.max_keywords_per_query,
             question=query_str,
         )
         keywords = extract_keywords_given_response(response, start_token="KEYWORDS:")
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
-            event_id=event_id,
-        )
         return list(keywords)
 
 
 class KeywordTableSimpleRetriever(BaseKeywordTableRetriever):
     """Keyword Table Index Simple Retriever.
 
     Extracts keywords using simple regex-based keyword extractor.
```

### Comparing `llama_index-0.6.4/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.6.5/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/keyword_table/utils.py` & `llama_index-0.6.5/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.6.5/llama_index/indices/knowledge_graph/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 existing keywords in the table.
 
 """
 
 import logging
 from typing import Any, List, Optional, Sequence, Tuple
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs import KG
 from llama_index.data_structs.node import Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.prompts.default_prompts import (
     DEFAULT_KG_TRIPLET_EXTRACT_PROMPT,
     DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE,
@@ -79,27 +78,18 @@
         if len(self.index_struct.embedding_dict) > 0 and "retriever_mode" not in kwargs:
             kwargs["retriever_mode"] = KGRetrieverMode.HYBRID
 
         return KGTableRetriever(self, **kwargs)
 
     def _extract_triplets(self, text: str) -> List[Tuple[str, str, str]]:
         """Extract keywords from text."""
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM,
-            payload={"template": self.kg_triple_extract_template, "text": text},
-        )
-        response, formatted_prompt = self._service_context.llm_predictor.predict(
+        response, _ = self._service_context.llm_predictor.predict(
             self.kg_triple_extract_template,
             text=text,
         )
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={"response": response, "formatted_prompt": formatted_prompt},
-            event_id=event_id,
-        )
         return self._parse_triplet_response(response)
 
     @staticmethod
     def _parse_triplet_response(response: str) -> List[Tuple[str, str, str]]:
         knowledge_strs = response.strip().split("\n")
         results = []
         for text in knowledge_strs:
@@ -119,30 +109,22 @@
             logger.debug(f"> Extracted triplets: {triplets}")
             for triplet in triplets:
                 subj, _, obj = triplet
                 index_struct.upsert_triplet(triplet)
                 index_struct.add_node([subj, obj], n)
 
             if self.include_embeddings:
-                event_id = self._service_context.callback_manager.on_event_start(
-                    CBEventType.EMBEDDING
-                )
-                for i, triplet in enumerate(triplets):
+                for triplet in triplets:
                     self._service_context.embed_model.queue_text_for_embedding(
                         str(triplet), str(triplet)
                     )
 
                 embed_outputs = (
                     self._service_context.embed_model.get_queued_text_embeddings()
                 )
-                self._service_context.callback_manager.on_event_end(
-                    CBEventType.EMBEDDING,
-                    payload={"num_nodes": len(triplets)},
-                    event_id=event_id,
-                )
                 for rel_text, rel_embed in zip(*embed_outputs):
                     index_struct.add_to_embedding_dict(rel_text, rel_embed)
 
         return index_struct
 
     def _insert(self, nodes: Sequence[Node], **insert_kwargs: Any) -> None:
         """Insert a document."""
@@ -154,27 +136,19 @@
                 triplet_str = str(triplet)
                 self._index_struct.upsert_triplet(triplet)
                 self._index_struct.add_node([subj, obj], n)
                 if (
                     self.include_embeddings
                     and triplet_str not in self._index_struct.embedding_dict
                 ):
-                    event_id = self._service_context.callback_manager.on_event_start(
-                        CBEventType.EMBEDDING
-                    )
                     rel_embedding = (
                         self._service_context.embed_model.get_text_embedding(
                             triplet_str
                         )
                     )
-                    self._service_context.callback_manager.on_event_end(
-                        CBEventType.EMBEDDING,
-                        payload={"num_nodes": 1},
-                        event_id=event_id,
-                    )
                     self.index_struct.add_to_embedding_dict(triplet_str, rel_embedding)
 
     def upsert_triplet(self, triplet: Tuple[str, str, str]) -> None:
         """Insert triplets.
 
         Used for manual insertion of KG triplets (in the form
         of (subject, relationship, object)).
```

### Comparing `llama_index-0.6.4/llama_index/indices/knowledge_graph/retrievers.py` & `llama_index-0.6.5/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Query for GPTKGTableIndex."""
 import logging
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.utils import extract_keywords_given_response
 from llama_index.indices.knowledge_graph.base import GPTKnowledgeGraphIndex
 from llama_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
 )
@@ -90,35 +89,22 @@
         self.query_keyword_extract_template = query_keyword_extract_template or DQKET
         self.similarity_top_k = similarity_top_k
         self._include_text = include_text
         self._retriever_mode = KGRetrieverMode(retriever_mode)
 
     def _get_keywords(self, query_str: str) -> List[str]:
         """Extract keywords."""
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM,
-            payload={
-                "template": self.query_keyword_extract_template,
-                "question": query_str,
-                "max_keywords": self.max_keywords_per_query,
-            },
-        )
-        response, formatted_prompt = self._service_context.llm_predictor.predict(
+        response, _ = self._service_context.llm_predictor.predict(
             self.query_keyword_extract_template,
             max_keywords=self.max_keywords_per_query,
             question=query_str,
         )
         keywords = extract_keywords_given_response(
             response, start_token="KEYWORDS:", lowercase=False
         )
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
-            event_id=event_id,
-        )
         return list(keywords)
 
     def _extract_rel_text_keywords(self, rel_texts: List[str]) -> List[str]:
         """Find the keywords for given rel text triplets."""
         keywords = []
         for rel_text in rel_texts:
             keyword = rel_text.split(",")[0]
@@ -147,23 +133,17 @@
                     for node_id in self._index_struct.get_node_ids(keyword):
                         chunk_indices_count[node_id] += 1
 
         if (
             self._retriever_mode != KGRetrieverMode.KEYWORD
             and len(self._index_struct.embedding_dict) > 0
         ):
-            event_id = self._service_context.callback_manager.on_event_start(
-                CBEventType.EMBEDDING
-            )
             query_embedding = self._service_context.embed_model.get_text_embedding(
                 query_bundle.query_str
             )
-            self._service_context.callback_manager.on_event_end(
-                CBEventType.EMBEDDING, payload={"num_nodes": 1}, event_id=event_id
-            )
             all_rel_texts = list(self._index_struct.embedding_dict.keys())
 
             rel_text_embeddings = [
                 self._index_struct.embedding_dict[_id] for _id in all_rel_texts
             ]
             similarities, top_rel_texts = get_top_k_embeddings(
                 query_embedding,
```

### Comparing `llama_index-0.6.4/llama_index/indices/list/base.py` & `llama_index-0.6.5/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/list/retrievers.py` & `llama_index-0.6.5/llama_index/indices/list/retrievers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Default query for GPTListIndex."""
 import logging
 from typing import Any, List, Optional, Tuple
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
 )
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.list.base import GPTListIndex
@@ -87,40 +86,26 @@
         return node_with_scores
 
     def _get_embeddings(
         self, query_bundle: QueryBundle, nodes: List[Node]
     ) -> Tuple[List[float], List[List[float]]]:
         """Get top nodes by similarity to the query."""
         if query_bundle.embedding is None:
-            event_id = self._index._service_context.callback_manager.on_event_start(
-                CBEventType.EMBEDDING
-            )
             query_bundle.embedding = (
                 self._index._service_context.embed_model.get_agg_embedding_from_queries(
                     query_bundle.embedding_strs
                 )
             )
-            self._index._service_context.callback_manager.on_event_end(
-                CBEventType.EMBEDDING, payload={"num_nodes": 1}, event_id=event_id
-            )
-        node_embeddings: List[List[float]] = []
 
-        event_id = self._index._service_context.callback_manager.on_event_start(
-            CBEventType.EMBEDDING
-        )
+        node_embeddings: List[List[float]] = []
         nodes_embedded = 0
         for node in nodes:
             if node.embedding is None:
                 nodes_embedded += 1
                 node.embedding = (
                     self._index.service_context.embed_model.get_text_embedding(
                         node.get_text()
                     )
                 )
 
             node_embeddings.append(node.embedding)
-        self._index._service_context.callback_manager.on_event_end(
-            CBEventType.EMBEDDING,
-            payload={"num_nodes": nodes_embedded},
-            event_id=event_id,
-        )
         return query_bundle.embedding, node_embeddings
```

### Comparing `llama_index-0.6.4/llama_index/indices/loading.py` & `llama_index-0.6.5/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.6.5/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/postprocessor/cohere_rerank.py` & `llama_index-0.6.5/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/postprocessor/node.py` & `llama_index-0.6.5/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.6.5/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/postprocessor/pii.py` & `llama_index-0.6.5/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/prompt_helper.py` & `llama_index-0.6.5/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/query/base.py` & `llama_index-0.6.5/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/query/embedding_utils.py` & `llama_index-0.6.5/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/query/query_transform/base.py` & `llama_index-0.6.5/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.6.5/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/query/response_synthesis.py` & `llama_index-0.6.5/llama_index/indices/query/response_synthesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 import logging
-from typing import (
-    Any,
-    Dict,
-    Generator,
-    List,
-    Optional,
-    Sequence,
-)
+from typing import Any, Dict, Generator, List, Optional, Sequence
 
 from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.postprocessor.types import BaseNodePostprocessor
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.response.response_builder import (
     BaseResponseBuilder,
     ResponseMode,
@@ -19,19 +12,15 @@
 from llama_index.indices.service_context import ServiceContext
 from llama_index.optimization.optimizer import BaseTokenUsageOptimizer
 from llama_index.prompts.prompts import (
     QuestionAnswerPrompt,
     RefinePrompt,
     SimpleInputPrompt,
 )
-from llama_index.response.schema import (
-    RESPONSE_TYPE,
-    Response,
-    StreamingResponse,
-)
+from llama_index.response.schema import RESPONSE_TYPE, Response, StreamingResponse
 from llama_index.types import RESPONSE_TEXT_TYPE
 
 logger = logging.getLogger(__name__)
 
 
 class ResponseSynthesizer:
     """Response synthesize class.
```

### Comparing `llama_index-0.6.4/llama_index/indices/query/schema.py` & `llama_index-0.6.5/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/registry.py` & `llama_index-0.6.5/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/response/response_builder.py` & `llama_index-0.6.5/llama_index/indices/response/response_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 2) create and refine separately over each chunk, 3) tree summarization.
 
 """
 from abc import ABC, abstractmethod
 import logging
 from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, cast
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs import IndexGraph
 from llama_index.data_structs.node import Node
 from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.common_tree.base import GPTTreeIndexBuilder
 from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import get_sorted_node_list, truncate_text
@@ -66,51 +65,14 @@
             {"formatted_prompt_template": formatted_prompt}
         )
         logger.debug(f"> {log_prefix} response: {response}")
         self._service_context.llama_logger.add_log(
             {f"{log_prefix.lower()}_response": response or "Empty Response"}
         )
 
-    def _callback_llm_on_start(self) -> str:
-        """Call the callback manager on_start and return event id."""
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM
-        )
-        return event_id
-
-    def _callback_llm_on_end(
-        self,
-        formatted_prompt: str,
-        response: RESPONSE_TEXT_TYPE,
-        event_id: str,
-        stage: Optional[str] = "",
-    ) -> None:
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={
-                "stage": stage,
-                "response": response,
-                "formatted_prompt": formatted_prompt,
-            },
-            event_id=event_id,
-        )
-
-    def _callback_chunking_on_start(self, text: str) -> str:
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.CHUNKING, payload={"node": text}
-        )
-        return event_id
-
-    def _callback_chunking_on_end(
-        self, text_chunks: Sequence[str], event_id: str
-    ) -> None:
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.CHUNKING, payload={"chunks": text_chunks}, event_id=event_id
-        )
-
     @abstractmethod
     @llm_token_counter("get_response")
     def get_response(
         self,
         query_str: str,
         text_chunks: Sequence[str],
         prev_response: Optional[str] = None,
@@ -193,48 +155,38 @@
         """Give response given a query and a corresponding text chunk."""
         text_qa_template = self.text_qa_template.partial_format(query_str=query_str)
         qa_text_splitter = (
             self._service_context.prompt_helper.get_text_splitter_given_prompt(
                 text_qa_template, 1
             )
         )
-        event_id = self._callback_chunking_on_start(text_chunk)
         text_chunks = qa_text_splitter.split_text(text_chunk)
-        self._callback_chunking_on_end(text_chunk, event_id)
 
         response: Optional[RESPONSE_TEXT_TYPE] = None
         # TODO: consolidate with loop in get_response_default
         for cur_text_chunk in text_chunks:
             if response is None and not self._streaming:
-                event_id = self._callback_llm_on_start()
                 (
                     response,
                     formatted_prompt,
                 ) = self._service_context.llm_predictor.predict(
                     text_qa_template,
                     context_str=cur_text_chunk,
                 )
                 self._log_prompt_and_response(
                     formatted_prompt, response, log_prefix="Initial"
                 )
-                self._callback_llm_on_end(
-                    formatted_prompt, response, event_id, stage="Initial"
-                )
             elif response is None and self._streaming:
-                event_id = self._callback_llm_on_start()
                 response, formatted_prompt = self._service_context.llm_predictor.stream(
                     text_qa_template,
                     context_str=cur_text_chunk,
                 )
                 self._log_prompt_and_response(
                     formatted_prompt, response, log_prefix="Initial"
                 )
-                self._callback_llm_on_end(
-                    formatted_prompt, response, event_id, stage="Initial"
-                )
             else:
                 response = self._refine_response_single(
                     cast(RESPONSE_TEXT_TYPE, response),
                     query_str,
                     cur_text_chunk,
                 )
         if isinstance(response, str):
@@ -263,20 +215,17 @@
         )
         refine_text_splitter = (
             self._service_context.prompt_helper.get_text_splitter_given_prompt(
                 refine_template, 1
             )
         )
 
-        event_id = self._callback_chunking_on_start(text_chunk)
         text_chunks = refine_text_splitter.split_text(text_chunk)
-        self._callback_chunking_on_end(text_chunks, event_id)
 
         for cur_text_chunk in text_chunks:
-            event_id = self._callback_llm_on_start()
             if not self._streaming:
                 (
                     response,
                     formatted_prompt,
                 ) = self._service_context.llm_predictor.predict(
                     refine_template,
                     context_msg=cur_text_chunk,
@@ -289,17 +238,14 @@
             refine_template = self._refine_template.partial_format(
                 query_str=query_str, existing_answer=response
             )
 
             self._log_prompt_and_response(
                 formatted_prompt, response, log_prefix="Refined"
             )
-            self._callback_llm_on_end(
-                formatted_prompt, response, event_id, stage="Refined"
-            )
         return response
 
 
 class CompactAndRefine(Refine):
     def __init__(
         self,
         service_context: ServiceContext,
@@ -444,17 +390,15 @@
 
         # then get text splitter
         text_splitter = (
             self._service_context.prompt_helper.get_text_splitter_given_prompt(
                 summary_template, num_children
             )
         )
-        event_id = self._callback_chunking_on_start(all_text)
         text_chunks = text_splitter.split_text(all_text)
-        self._callback_chunking_on_end(text_chunks, event_id)
 
         new_nodes = [Node(text=t) for t in text_chunks]
 
         docstore = get_default_docstore()
         docstore.add_documents(new_nodes, allow_update=False)
         index_builder = GPTTreeIndexBuilder(
             num_children,
@@ -508,33 +452,29 @@
     ) -> RESPONSE_TEXT_TYPE:
         text_qa_template = self._text_qa_template.partial_format(query_str=query_str)
         node_text = self._service_context.prompt_helper.get_text_from_nodes(
             [Node(text=text) for text in text_chunks], prompt=text_qa_template
         )
 
         response: RESPONSE_TEXT_TYPE
-        event_id = self._callback_llm_on_start()
         if not self._streaming:
             (
                 response,
                 formatted_prompt,
             ) = await self._service_context.llm_predictor.apredict(
                 text_qa_template,
                 context_str=node_text,
             )
         else:
-            event_id = self._callback_llm_on_start()
             response, formatted_prompt = self._service_context.llm_predictor.stream(
                 text_qa_template,
                 context_str=node_text,
             )
         self._log_prompt_and_response(formatted_prompt, response)
-        self._callback_llm_on_end(
-            formatted_prompt, response, event_id, stage="summarize"
-        )
+
         if isinstance(response, str):
             response = response or "Empty Response"
         else:
             response = cast(Generator, response)
 
         return response
 
@@ -548,29 +488,26 @@
     ) -> RESPONSE_TEXT_TYPE:
         text_qa_template = self._text_qa_template.partial_format(query_str=query_str)
         node_text = self._service_context.prompt_helper.get_text_from_nodes(
             [Node(text=text) for text in text_chunks], prompt=text_qa_template
         )
 
         response: RESPONSE_TEXT_TYPE
-        event_id = self._callback_llm_on_start()
         if not self._streaming:
             (response, formatted_prompt,) = self._service_context.llm_predictor.predict(
                 text_qa_template,
                 context_str=node_text,
             )
         else:
             response, formatted_prompt = self._service_context.llm_predictor.stream(
                 text_qa_template,
                 context_str=node_text,
             )
         self._log_prompt_and_response(formatted_prompt, response)
-        self._callback_llm_on_end(
-            formatted_prompt, response, event_id, stage="summarize"
-        )
+
         if isinstance(response, str):
             response = response or "Empty Response"
         else:
             response = cast(Generator, response)
 
         return response
 
@@ -594,23 +531,21 @@
         **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         # NOTE: ignore text chunks and previous response
         del text_chunks
         del prev_response
 
         if not self._streaming:
-            event_id = self._callback_llm_on_start()
             (
                 response,
                 formatted_prompt,
             ) = await self._service_context.llm_predictor.apredict(
                 self._input_prompt,
                 query_str=query_str,
             )
-            self._callback_llm_on_end(formatted_prompt, response, event_id)
             return response
         else:
             stream_response, _ = self._service_context.llm_predictor.stream(
                 self._input_prompt,
                 query_str=query_str,
             )
             return stream_response
@@ -624,20 +559,18 @@
         **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         # NOTE: ignore text chunks and previous response
         del text_chunks
         del prev_response
 
         if not self._streaming:
-            event_id = self._callback_llm_on_start()
             response, formatted_prompt = self._service_context.llm_predictor.predict(
                 self._input_prompt,
                 query_str=query_str,
             )
-            self._callback_llm_on_end(formatted_prompt, response, event_id)
             return response
         else:
             stream_response, _ = self._service_context.llm_predictor.stream(
                 self._input_prompt,
                 query_str=query_str,
             )
             return stream_response
```

### Comparing `llama_index-0.6.4/llama_index/indices/service_context.py` & `llama_index-0.6.5/llama_index/indices/service_context.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,21 +8,31 @@
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.text_splitter import TokenTextSplitter
 from llama_index.logger import LlamaLogger
 from llama_index.node_parser.interface import NodeParser
 from llama_index.node_parser.simple import SimpleNodeParser
 
 
-def _get_default_node_parser(chunk_size_limit: Optional[int] = None) -> NodeParser:
+def _get_default_node_parser(
+    chunk_size_limit: Optional[int] = None,
+    callback_manager: Optional[CallbackManager] = None,
+) -> NodeParser:
     """Get default node parser."""
+    callback_manager = callback_manager or CallbackManager([])
     if chunk_size_limit is None:
-        token_text_splitter = TokenTextSplitter()  # use default chunk size
+        token_text_splitter = TokenTextSplitter(
+            callback_manager=callback_manager
+        )  # use default chunk size
     else:
-        token_text_splitter = TokenTextSplitter(chunk_size=chunk_size_limit)
-    return SimpleNodeParser(text_splitter=token_text_splitter)
+        token_text_splitter = TokenTextSplitter(
+            chunk_size=chunk_size_limit, callback_manager=callback_manager
+        )
+    return SimpleNodeParser(
+        text_splitter=token_text_splitter, callback_manager=callback_manager
+    )
 
 
 @dataclass
 class ServiceContext:
     """Service Context container.
 
     The service context container is a utility container for LlamaIndex
@@ -67,22 +77,28 @@
             node_parser (Optional[NodeParser]): NodeParser
             llama_logger (Optional[LlamaLogger]): LlamaLogger (deprecated)
             chunk_size_limit (Optional[int]): chunk_size_limit
 
         """
         callback_manager = callback_manager or CallbackManager([])
         llm_predictor = llm_predictor or LLMPredictor()
+        llm_predictor.callback_manager = callback_manager
+
         # NOTE: the embed_model isn't used in all indices
         embed_model = embed_model or OpenAIEmbedding()
+        embed_model.callback_manager = callback_manager
+
         prompt_helper = prompt_helper or PromptHelper.from_llm_predictor(
             llm_predictor, chunk_size_limit=chunk_size_limit
         )
+
         node_parser = node_parser or _get_default_node_parser(
-            chunk_size_limit=chunk_size_limit
+            chunk_size_limit=chunk_size_limit, callback_manager=callback_manager
         )
+
         llama_logger = llama_logger or LlamaLogger()
 
         return cls(
             llm_predictor=llm_predictor,
             embed_model=embed_model,
             prompt_helper=prompt_helper,
             node_parser=node_parser,
```

### Comparing `llama_index-0.6.4/llama_index/indices/struct_store/__init__.py` & `llama_index-0.6.5/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/struct_store/base.py` & `llama_index-0.6.5/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.6.5/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/struct_store/pandas.py` & `llama_index-0.6.5/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/struct_store/pandas_query.py` & `llama_index-0.6.5/llama_index/indices/struct_store/pandas_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 from typing import Any, Callable, Optional
 
 import pandas as pd
 from langchain.input import print_text
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.struct_store.pandas import GPTPandasIndex
 from llama_index.prompts.default_prompts import DEFAULT_PANDAS_PROMPT
 from llama_index.prompts.prompts import PandasPrompt
 from llama_index.response.schema import Response
 
@@ -107,40 +106,24 @@
         """Get table context."""
         return str(self.df.head(self._head))
 
     def _query(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         context = self._get_table_context()
 
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM,
-            payload={
-                "template": self._pandas_prompt,
-                "df_str": context,
-                "query_str": query_bundle.query_str,
-                "instruction_str": self._instruction_str,
-            },
-        )
         (
             pandas_response_str,
             formatted_prompt,
         ) = self._service_context.llm_predictor.predict(
             self._pandas_prompt,
             df_str=context,
             query_str=query_bundle.query_str,
             instruction_str=self._instruction_str,
         )
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={
-                "response": pandas_response_str,
-                "formatted_prompt": formatted_prompt,
-            },
-            event_id=event_id,
-        )
+
         if self._verbose:
             print_text(f"> Pandas Instructions:\n" f"```\n{pandas_response_str}\n```\n")
         pandas_output = self._output_processor(
             pandas_response_str,
             self.df,
             **self._output_kwargs,
         )
```

### Comparing `llama_index-0.6.4/llama_index/indices/struct_store/sql.py` & `llama_index-0.6.5/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.6.5/llama_index/indices/struct_store/sql_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Default query for GPTSQLStructStoreIndex."""
 import logging
 from typing import Any, Optional
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.struct_store.container_builder import (
     SQLContextContainerBuilder,
 )
 from llama_index.indices.struct_store.sql import GPTSQLStructStoreIndex
 from llama_index.prompts.default_prompts import DEFAULT_TEXT_TO_SQL_PROMPT
@@ -106,34 +105,21 @@
         return tables_desc_str
 
     @llm_token_counter("query")
     def _query(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         table_desc_str = self._get_table_context(query_bundle)
         logger.info(f"> Table desc str: {table_desc_str}")
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM,
-            payload={
-                "template": self._text_to_sql_prompt,
-                "query_str": query_bundle.query_str,
-                "schema": table_desc_str,
-                "dialect": self._sql_database.dialect,
-            },
-        )
-        response_str, formatted_prompt = self._service_context.llm_predictor.predict(
+
+        response_str, _ = self._service_context.llm_predictor.predict(
             self._text_to_sql_prompt,
             query_str=query_bundle.query_str,
             schema=table_desc_str,
             dialect=self._sql_database.dialect,
         )
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={"response": response_str, "formatted_prompt": formatted_prompt},
-            event_id=event_id,
-        )
 
         sql_query_str = self._parse_response_to_sql(response_str)
         # assume that it's a valid SQL query
         logger.debug(f"> Predicted SQL query: {sql_query_str}")
 
         response_str, extra_info = self._sql_database.run_sql(sql_query_str)
         extra_info["sql_query"] = sql_query_str
@@ -141,37 +127,24 @@
         return response
 
     @llm_token_counter("aquery")
     async def _aquery(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         table_desc_str = self._get_table_context(query_bundle)
         logger.info(f"> Table desc str: {table_desc_str}")
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.LLM,
-            payload={
-                "template": self._text_to_sql_prompt,
-                "query_str": query_bundle.query_str,
-                "schema": table_desc_str,
-                "dialect": self._sql_database.dialect,
-            },
-        )
+
         (
             response_str,
             formatted_prompt,
         ) = await self._service_context.llm_predictor.apredict(
             self._text_to_sql_prompt,
             query_str=query_bundle.query_str,
             schema=table_desc_str,
             dialect=self._sql_database.dialect,
         )
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.LLM,
-            payload={"response": response_str, "formatted_prompt": formatted_prompt},
-            event_id=event_id,
-        )
 
         sql_query_str = self._parse_response_to_sql(response_str)
         # assume that it's a valid SQL query
         logger.debug(f"> Predicted SQL query: {sql_query_str}")
 
         response_str, extra_info = self._sql_database.run_sql(sql_query_str)
         extra_info["sql_query"] = sql_query_str
```

### Comparing `llama_index-0.6.4/llama_index/indices/tree/__init__.py` & `llama_index-0.6.5/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.6.5/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/tree/base.py` & `llama_index-0.6.5/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/tree/inserter.py` & `llama_index-0.6.5/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.6.5/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.6.5/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.6.5/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/utils.py` & `llama_index-0.6.5/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/indices/vector_store/base.py` & `llama_index-0.6.5/llama_index/indices/vector_store/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 An index that that is built on top of an existing vector store.
 
 """
 
 from typing import Any, Dict, List, Optional, Sequence, Tuple
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.async_utils import run_async_tasks
 from llama_index.data_structs.data_structs import IndexDict
 from llama_index.data_structs.node import ImageNode, IndexNode, Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
 from llama_index.storage.storage_context import StorageContext
@@ -74,28 +73,19 @@
             if n.embedding is None:
                 self._service_context.embed_model.queue_text_for_embedding(
                     n.get_doc_id(), n.get_text()
                 )
             else:
                 id_to_embed_map[n.get_doc_id()] = n.embedding
 
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.EMBEDDING
-        )
-
         # call embedding model to get embeddings
         (
             result_ids,
             result_embeddings,
         ) = self._service_context.embed_model.get_queued_text_embeddings()
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.EMBEDDING,
-            payload={"num_nodes": len(result_ids)},
-            event_id=event_id,
-        )
         for new_id, text_embedding in zip(result_ids, result_embeddings):
             id_to_embed_map[new_id] = text_embedding
 
         results = []
         for node in nodes:
             embedding = id_to_embed_map[node.get_doc_id()]
             result = NodeWithEmbedding(node=node, embedding=embedding)
@@ -117,31 +107,22 @@
         text_queue: List[Tuple[str, str]] = []
         for n in nodes:
             if n.embedding is None:
                 text_queue.append((n.get_doc_id(), n.get_text()))
             else:
                 id_to_embed_map[n.get_doc_id()] = n.embedding
 
-        event_id = self._service_context.callback_manager.on_event_start(
-            CBEventType.EMBEDDING
-        )
-
         # call embedding model to get embeddings
         (
             result_ids,
             result_embeddings,
         ) = await self._service_context.embed_model.aget_queued_text_embeddings(
             text_queue
         )
 
-        self._service_context.callback_manager.on_event_end(
-            CBEventType.EMBEDDING,
-            payload={"num_nodes": len(text_queue)},
-            event_id=event_id,
-        )
         for new_id, text_embedding in zip(result_ids, result_embeddings):
             id_to_embed_map[new_id] = text_embedding
 
         results = []
         for node in nodes:
             embedding = id_to_embed_map[node.get_doc_id()]
             result = NodeWithEmbedding(node=node, embedding=embedding)
```

### Comparing `llama_index-0.6.4/llama_index/indices/vector_store/retrievers.py` & `llama_index-0.6.5/llama_index/indices/vector_store/retrievers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Base vector store index query."""
 
 
 from typing import Any, List, Optional
 from llama_index.constants import DEFAULT_SIMILARITY_TOP_K
 
-from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs import IndexDict
 from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.utils import log_vector_store_query_result
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
 from llama_index.token_counter.token_counter import llm_token_counter
@@ -51,25 +50,19 @@
     @llm_token_counter("retrieve")
     def _retrieve(
         self,
         query_bundle: QueryBundle,
     ) -> List[NodeWithScore]:
         if self._vector_store.is_embedding_query:
             if query_bundle.embedding is None:
-                event_id = self._service_context.callback_manager.on_event_start(
-                    CBEventType.EMBEDDING
-                )
                 query_bundle.embedding = (
                     self._service_context.embed_model.get_agg_embedding_from_queries(
                         query_bundle.embedding_strs
                     )
                 )
-                self._service_context.callback_manager.on_event_end(
-                    CBEventType.EMBEDDING, payload={"num_nodes": 1}, event_id=event_id
-                )
 
         query = VectorStoreQuery(
             query_embedding=query_bundle.embedding,
             similarity_top_k=self._similarity_top_k,
             doc_ids=self._doc_ids,
             query_str=query_bundle.query_str,
             mode=self._vector_store_query_mode,
```

### Comparing `llama_index-0.6.4/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.6.5/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.6.5/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.6.5/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.6.5/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.6.5/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.6.5/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.6.5/llama_index/langchain_helpers/text_splitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Text splitter implementations."""
 from dataclasses import dataclass
 from typing import Callable, List, Optional
 
 from langchain.text_splitter import TextSplitter
 from llama_index.constants import DEFAULT_CHUNK_OVERLAP, DEFAULT_CHUNK_SIZE
 
+from llama_index.callbacks.base import CallbackManager
+from llama_index.callbacks.schema import CBEventType
 from llama_index.utils import globals_helper
 
 
 @dataclass
 class TextSplit:
     """Text split with overlap.
 
@@ -27,26 +29,28 @@
     def __init__(
         self,
         separator: str = " ",
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         chunk_overlap: int = DEFAULT_CHUNK_OVERLAP,
         tokenizer: Optional[Callable] = None,
         backup_separators: Optional[List[str]] = ["\n"],
+        callback_manager: Optional[CallbackManager] = None,
     ):
         """Initialize with parameters."""
         if chunk_overlap > chunk_size:
             raise ValueError(
                 f"Got a larger chunk overlap ({chunk_overlap}) than chunk size "
                 f"({chunk_size}), should be smaller."
             )
         self._separator = separator
         self._chunk_size = chunk_size
         self._chunk_overlap = chunk_overlap
         self.tokenizer = tokenizer or globals_helper.tokenizer
         self._backup_separators = backup_separators
+        self.callback_manager = callback_manager or CallbackManager([])
 
     def _reduce_chunk_size(
         self, start_idx: int, cur_idx: int, splits: List[str]
     ) -> int:
         """Reduce the chunk size by reducing cur_idx.
 
         Return the new cur_idx.
@@ -120,23 +124,33 @@
             if doc.text_chunk.replace(" ", "") == "":
                 continue
             new_docs.append(doc)
         return new_docs
 
     def split_text(self, text: str, extra_info_str: Optional[str] = None) -> List[str]:
         """Split incoming text and return chunks."""
+        event_id = self.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"text": text}
+        )
         text_splits = self.split_text_with_overlaps(text, extra_info_str=extra_info_str)
-        return [text_split.text_chunk for text_split in text_splits]
+        chunks = [text_split.text_chunk for text_split in text_splits]
+        self.callback_manager.on_event_end(
+            CBEventType.CHUNKING, payload={"chunks": chunks}, event_id=event_id
+        )
+        return chunks
 
     def split_text_with_overlaps(
         self, text: str, extra_info_str: Optional[str] = None
     ) -> List[TextSplit]:
         """Split incoming text and return chunks with overlap size."""
         if text == "":
             return []
+        event_id = self.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"text": text}
+        )
 
         # NOTE: Consider extra info str that will be added to the chunk at query time
         #       This reduces the effective chunk size that we can have
         if extra_info_str is not None:
             # NOTE: extra 2 newline chars for formatting when prepending in query
             num_extra_tokens = len(self.tokenizer(f"{extra_info_str}\n\n")) + 1
             effective_chunk_size = self._chunk_size - num_extra_tokens
@@ -217,14 +231,19 @@
             overlap = sum([len(splits[i]) for i in range(start_idx, prev_idx)]) + len(
                 range(start_idx, prev_idx)
             )
         docs.append(TextSplit(self._separator.join(splits[start_idx:cur_idx]), overlap))
 
         # run postprocessing to remove blank spaces
         docs = self._postprocess_splits(docs)
+        self.callback_manager.on_event_end(
+            CBEventType.CHUNKING,
+            payload={"chunks": [x.text_chunk for x in docs]},
+            event_id=event_id,
+        )
         return docs
 
     def truncate_text(self, text: str) -> str:
         """Truncate text in order to fit the underlying chunk size."""
         if text == "":
             return ""
         # First we naively split the large input into a bunch of smaller ones.
@@ -259,26 +278,28 @@
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         chunk_overlap: int = 200,
         tokenizer: Optional[Callable] = None,
         backup_separators: Optional[List[str]] = ["\n"],
         paragraph_separator: Optional[str] = "\n\n\n",
         chunking_tokenizer_fn: Optional[Callable[[str], List[str]]] = None,
         secondary_chunking_regex: Optional[str] = "[^,.;。]+[,.;。]?",
+        callback_manager: Optional[CallbackManager] = None,
     ):
         """Initialize with parameters."""
         if chunk_overlap > chunk_size:
             raise ValueError(
                 f"Got a larger chunk overlap ({chunk_overlap}) than chunk size "
                 f"({chunk_size}), should be smaller."
             )
         self._separator = separator
         self._chunk_size = chunk_size
         self._chunk_overlap = chunk_overlap
         self.tokenizer = tokenizer or globals_helper.tokenizer
         self._backup_separators = backup_separators
+        self.callback_manager = callback_manager or CallbackManager([])
         if chunking_tokenizer_fn is None:
             import nltk.tokenize.punkt as pkt
 
             class CustomLanguageVars(pkt.PunktLanguageVars):
                 _period_context_fmt = r"""
                     %(SentEndChars)s             # a potential sentence ending
                     (\)\"\s)\s*                  # other end chars and
@@ -320,14 +341,17 @@
         """
         Split incoming text and return chunks with overlap size.
 
         Has a preference for complete sentences, phrases, and minimal overlap.
         """
         if text == "":
             return []
+        event_id = self.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"text": text}
+        )
 
         # NOTE: Consider extra info str that will be added to the chunk at query time
         #       This reduces the effective chunk size that we can have
         if extra_info_str is not None:
             # NOTE: extra 2 newline chars for formatting when prepending in query
             num_extra_tokens = len(self.tokenizer(f"{extra_info_str}\n\n")) + 1
             effective_chunk_size = self._chunk_size - num_extra_tokens
@@ -412,16 +436,29 @@
                     cur_doc_list = []
                     cur_tokens = 0
 
         docs.append(TextSplit("".join(cur_doc_list).strip()))
 
         # run postprocessing to remove blank spaces
         docs = self._postprocess_splits(docs)
+
+        self.callback_manager.on_event_end(
+            CBEventType.CHUNKING,
+            payload={"chunks": [x.text_chunk for x in docs]},
+            event_id=event_id,
+        )
         return docs
 
     def split_text(self, text: str, extra_info_str: Optional[str] = None) -> List[str]:
         """Split incoming text and return chunks."""
+        event_id = self.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"text": text}
+        )
         text_splits = self.split_text_with_overlaps(text, extra_info_str=extra_info_str)
-        return [text_split.text_chunk for text_split in text_splits]
+        chunks = [text_split.text_chunk for text_split in text_splits]
+        self.callback_manager.on_event_end(
+            CBEventType.CHUNKING, payload={"chunks": chunks}, event_id=event_id
+        )
+        return chunks
 
 
 __all__ = ["TextSplitter", "TokenTextSplitter", "SentenceSplitter"]
```

### Comparing `llama_index-0.6.4/llama_index/llm_predictor/base.py` & `llama_index-0.6.5/llama_index/llm_predictor/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Wrapper functions around an LLM chain."""
 
 import logging
 from abc import abstractmethod
 from dataclasses import dataclass
+from threading import Thread
 from typing import Any, Generator, Optional, Protocol, Tuple
 
 import langchain
 import openai
-from langchain import Cohere, LLMChain, OpenAI, BaseCache
+from langchain import BaseCache, Cohere, LLMChain, OpenAI
+from langchain.base_language import BaseLanguageModel
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import AI21
-from langchain.base_language import BaseLanguageModel
 
+from llama_index.callbacks.base import CallbackManager
+from llama_index.callbacks.schema import CBEventType
 from llama_index.constants import MAX_CHUNK_SIZE, NUM_OUTPUTS
+from llama_index.langchain_helpers.streaming import StreamingGeneratorCallbackHandler
 from llama_index.prompts.base import Prompt
 from llama_index.utils import (
     ErrorToRetry,
     globals_helper,
     retry_on_exceptions_with_backoff,
 )
 
@@ -160,19 +164,21 @@
     """
 
     def __init__(
         self,
         llm: Optional[BaseLanguageModel] = None,
         retry_on_throttling: bool = True,
         cache: Optional[BaseCache] = None,
+        callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         """Initialize params."""
         self._llm = llm or OpenAI(temperature=0, model_name="text-davinci-003")
         if cache is not None:
             langchain.llm_cache = cache
+        self.callback_manager = callback_manager or CallbackManager([])
         self.retry_on_throttling = retry_on_throttling
         self._total_tokens_used = 0
         self.flag = True
         self._last_token_usage: Optional[int] = None
 
     @property
     def llm(self) -> BaseLanguageModel:
@@ -222,23 +228,34 @@
         Args:
             prompt (Prompt): Prompt to use for prediction.
 
         Returns:
             Tuple[str, str]: Tuple of the predicted answer and the formatted prompt.
 
         """
+        llm_payload = {**prompt_args}
+        llm_payload["template"] = prompt
+        event_id = self.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload=llm_payload,
+        )
         formatted_prompt = prompt.format(llm=self._llm, **prompt_args)
         llm_prediction = self._predict(prompt, **prompt_args)
         logger.debug(llm_prediction)
 
         # We assume that the value of formatted_prompt is exactly the thing
         # eventually sent to OpenAI, or whatever LLM downstream
         prompt_tokens_count = self._count_tokens(formatted_prompt)
         prediction_tokens_count = self._count_tokens(llm_prediction)
         self._total_tokens_used += prompt_tokens_count + prediction_tokens_count
+        self.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"response": llm_prediction, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
         return llm_prediction, formatted_prompt
 
     def stream(self, prompt: Prompt, **prompt_args: Any) -> Tuple[Generator, str]:
         """Stream the answer to a query.
 
         NOTE: this is a beta feature. Will try to build or use
         better abstractions about response handling.
@@ -246,19 +263,31 @@
         Args:
             prompt (Prompt): Prompt to use for prediction.
 
         Returns:
             str: The predicted answer.
 
         """
-        if not isinstance(self._llm, OpenAI):
-            raise ValueError("stream is only supported for OpenAI LLMs")
         formatted_prompt = prompt.format(llm=self._llm, **prompt_args)
-        raw_response_gen = self._llm.stream(formatted_prompt)
-        response_gen = _get_response_gen(raw_response_gen)
+
+        handler = StreamingGeneratorCallbackHandler()
+
+        if not hasattr(self._llm, "callbacks"):
+            raise ValueError("LLM must support callbacks to use streaming.")
+
+        self._llm.callbacks = [handler]
+
+        if not getattr(self._llm, "streaming", False):
+            raise ValueError("LLM must support streaming and set streaming=True.")
+
+        thread = Thread(target=self._predict, args=[prompt], kwargs=prompt_args)
+        thread.start()
+
+        response_gen = handler.get_response_gen()
+
         # NOTE/TODO: token counting doesn't work with streaming
         return response_gen, formatted_prompt
 
     @property
     def total_tokens_used(self) -> int:
         """Get the total tokens used so far."""
         return self._total_tokens_used
@@ -302,17 +331,27 @@
         Args:
             prompt (Prompt): Prompt to use for prediction.
 
         Returns:
             Tuple[str, str]: Tuple of the predicted answer and the formatted prompt.
 
         """
+        llm_payload = {**prompt_args}
+        llm_payload["template"] = prompt
+        event_id = self.callback_manager.on_event_start(
+            CBEventType.LLM, payload=prompt_args
+        )
         formatted_prompt = prompt.format(llm=self._llm, **prompt_args)
         llm_prediction = await self._apredict(prompt, **prompt_args)
         logger.debug(llm_prediction)
 
         # We assume that the value of formatted_prompt is exactly the thing
         # eventually sent to OpenAI, or whatever LLM downstream
         prompt_tokens_count = self._count_tokens(formatted_prompt)
         prediction_tokens_count = self._count_tokens(llm_prediction)
         self._total_tokens_used += prompt_tokens_count + prediction_tokens_count
+        self.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"response": llm_prediction, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
         return llm_prediction, formatted_prompt
```

### Comparing `llama_index-0.6.4/llama_index/llm_predictor/chatgpt.py` & `llama_index-0.6.5/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/llm_predictor/huggingface.py` & `llama_index-0.6.5/llama_index/llm_predictor/huggingface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Huggingface LLM Wrapper."""
 
 import logging
 from threading import Thread
 from typing import Any, List, Generator, Optional, Tuple
 
+from llama_index.callbacks.base import CallbackManager
+from llama_index.callbacks.schema import CBEventType
 from llama_index.llm_predictor.base import BaseLLMPredictor, LLMMetadata
 from llama_index.prompts.base import Prompt
 from llama_index.prompts.default_prompts import DEFAULT_SIMPLE_INPUT_PROMPT
 from llama_index.prompts.prompts import SimpleInputPrompt
 
 logger = logging.getLogger(__name__)
 
@@ -41,24 +43,27 @@
         model_name: str = "StabilityAI/stablelm-tuned-alpha-3b",
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
         device_map: str = "auto",
         stopping_ids: Optional[List[int]] = None,
         tokenizer_kwargs: Optional[dict] = None,
         model_kwargs: Optional[dict] = None,
+        callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         """Initialize params."""
         import torch
         from transformers import (
             AutoModelForCausalLM,
             AutoTokenizer,
             StoppingCriteria,
             StoppingCriteriaList,
         )
 
+        self.callback_manager = callback_manager or CallbackManager([])
+
         model_kwargs = model_kwargs or {}
         self.model = model or AutoModelForCausalLM.from_pretrained(
             model_name, device_map=device_map, **model_kwargs
         )
 
         # check max_input_size
         config_dict = self.model.config.to_dict()
@@ -191,14 +196,20 @@
 
         Returns:
             Tuple[str, str]: Tuple of the predicted answer and the formatted prompt.
 
         """
         import torch
 
+        llm_payload = {**prompt_args}
+        llm_payload["template"] = prompt
+        event_id = self.callback_manager.on_event_start(
+            CBEventType.LLM, payload=llm_payload
+        )
+
         formatted_prompt = prompt.format(**prompt_args)
         full_prompt = self._query_wrapper_prompt.format(query_str=formatted_prompt)
         if self._system_prompt:
             full_prompt = f"{self._system_prompt} {full_prompt}"
 
         inputs = self.tokenizer(full_prompt, return_tensors="pt")
         if "cuda" == self._device_map or (
@@ -212,14 +223,20 @@
             temperature=self._temperature,
             do_sample=self._do_sample,
             stopping_criteria=self._stopping_criteria,
         )
         completion_tokens = tokens[0][inputs["input_ids"].size(1) :]
         self._total_tokens_used += len(completion_tokens) + inputs["input_ids"].size(1)
         completion = self.tokenizer.decode(completion_tokens, skip_special_tokens=True)
+
+        self.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"response": completion, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
         return completion, formatted_prompt
 
     async def apredict(self, prompt: Prompt, **prompt_args: Any) -> Tuple[str, str]:
         """Async predict the answer to a query.
 
         Args:
             prompt (Prompt): Prompt to use for prediction.
```

### Comparing `llama_index-0.6.4/llama_index/llm_predictor/structured.py` & `llama_index-0.6.5/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/logger/base.py` & `llama_index-0.6.5/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/node_parser/interface.py` & `llama_index-0.6.5/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/node_parser/node_utils.py` & `llama_index-0.6.5/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/node_parser/simple.py` & `llama_index-0.6.5/llama_index/node_parser/simple.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Simple node parser."""
 from typing import List, Optional, Sequence
 
+from llama_index.callbacks.base import CallbackManager
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node import Node
 from llama_index.langchain_helpers.text_splitter import TextSplitter, TokenTextSplitter
 from llama_index.node_parser.node_utils import get_nodes_from_document
 from llama_index.readers.schema.base import Document
 from llama_index.node_parser.interface import NodeParser
 
 
@@ -21,34 +23,44 @@
     """
 
     def __init__(
         self,
         text_splitter: Optional[TextSplitter] = None,
         include_extra_info: bool = True,
         include_prev_next_rel: bool = True,
+        callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         """Init params."""
-        self._text_splitter = text_splitter or TokenTextSplitter()
+        self.callback_manager = callback_manager or CallbackManager([])
+        self._text_splitter = text_splitter or TokenTextSplitter(
+            callback_manager=self.callback_manager
+        )
         self._include_extra_info = include_extra_info
         self._include_prev_next_rel = include_prev_next_rel
 
     def get_nodes_from_documents(
         self,
         documents: Sequence[Document],
     ) -> List[Node]:
         """Parse document into nodes.
 
         Args:
             documents (Sequence[Document]): documents to parse
             include_extra_info (bool): whether to include extra info in nodes
 
         """
+        event_id = self.callback_manager.on_event_start(
+            CBEventType.NODE_PARSING, payload={"documents": documents}
+        )
         all_nodes: List[Node] = []
         for document in documents:
             nodes = get_nodes_from_document(
                 document,
                 self._text_splitter,
                 self._include_extra_info,
                 include_prev_next_rel=self._include_prev_next_rel,
             )
             all_nodes.extend(nodes)
+        self.callback_manager.on_event_end(
+            CBEventType.NODE_PARSING, payload={"nodes": all_nodes}, event_id=event_id
+        )
         return all_nodes
```

### Comparing `llama_index-0.6.4/llama_index/optimization/optimizer.py` & `llama_index-0.6.5/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/output_parsers/base.py` & `llama_index-0.6.5/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/output_parsers/guardrails.py` & `llama_index-0.6.5/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/output_parsers/langchain.py` & `llama_index-0.6.5/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/output_parsers/selection.py` & `llama_index-0.6.5/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/playground/base.py` & `llama_index-0.6.5/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/prompts/base.py` & `llama_index-0.6.5/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/prompts/chat_prompts.py` & `llama_index-0.6.5/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.6.5/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/prompts/default_prompts.py` & `llama_index-0.6.5/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/prompts/prompt_type.py` & `llama_index-0.6.5/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/prompts/prompts.py` & `llama_index-0.6.5/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/query_engine/__init__.py` & `llama_index-0.6.5/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.6.5/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.6.5/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.6.5/llama_index/query_engine/retriever_query_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         response_synthesizer: Optional[ResponseSynthesizer] = None,
         callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         self._retriever = retriever
         self._response_synthesizer = (
             response_synthesizer or ResponseSynthesizer.from_args()
         )
-        self._callback_manager = callback_manager or CallbackManager([])
+        self.callback_manager = callback_manager or CallbackManager([])
 
     @classmethod
     def from_args(
         cls,
         retriever: BaseRetriever,
         service_context: Optional[ServiceContext] = None,
         node_postprocessors: Optional[List[BaseNodePostprocessor]] = None,
@@ -129,48 +129,48 @@
             query_bundle=query_bundle,
             nodes=nodes,
             additional_source_nodes=additional_source_nodes,
         )
 
     def _query(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
         """Answer a query."""
-        query_id = self._callback_manager.on_event_start(CBEventType.QUERY)
+        query_id = self.callback_manager.on_event_start(CBEventType.QUERY)
 
-        retrieve_id = self._callback_manager.on_event_start(CBEventType.RETRIEVE)
+        retrieve_id = self.callback_manager.on_event_start(CBEventType.RETRIEVE)
         nodes = self._retriever.retrieve(query_bundle)
-        self._callback_manager.on_event_end(
+        self.callback_manager.on_event_end(
             CBEventType.RETRIEVE, payload={"nodes": nodes}, event_id=retrieve_id
         )
 
-        synth_id = self._callback_manager.on_event_start(CBEventType.SYNTHESIZE)
+        synth_id = self.callback_manager.on_event_start(CBEventType.SYNTHESIZE)
         response = self._response_synthesizer.synthesize(
             query_bundle=query_bundle,
             nodes=nodes,
         )
-        self._callback_manager.on_event_end(
+        self.callback_manager.on_event_end(
             CBEventType.SYNTHESIZE, payload={"response": response}, event_id=synth_id
         )
 
-        self._callback_manager.on_event_end(CBEventType.QUERY, event_id=query_id)
+        self.callback_manager.on_event_end(CBEventType.QUERY, event_id=query_id)
         return response
 
     async def _aquery(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
         """Answer a query."""
-        query_id = self._callback_manager.on_event_start(CBEventType.QUERY)
+        query_id = self.callback_manager.on_event_start(CBEventType.QUERY)
 
-        retrieve_id = self._callback_manager.on_event_start(CBEventType.RETRIEVE)
+        retrieve_id = self.callback_manager.on_event_start(CBEventType.RETRIEVE)
         nodes = self._retriever.retrieve(query_bundle)
-        self._callback_manager.on_event_end(
+        self.callback_manager.on_event_end(
             CBEventType.RETRIEVE, payload={"nodes": nodes}, event_id=retrieve_id
         )
 
-        synth_id = self._callback_manager.on_event_start(CBEventType.SYNTHESIZE)
+        synth_id = self.callback_manager.on_event_start(CBEventType.SYNTHESIZE)
         response = await self._response_synthesizer.asynthesize(
             query_bundle=query_bundle,
             nodes=nodes,
         )
-        self._callback_manager.on_event_end(
+        self.callback_manager.on_event_end(
             CBEventType.SYNTHESIZE, payload={"response": response}, event_id=synth_id
         )
 
-        self._callback_manager.on_event_end(CBEventType.QUERY, event_id=query_id)
+        self.callback_manager.on_event_end(CBEventType.QUERY, event_id=query_id)
         return response
```

### Comparing `llama_index-0.6.4/llama_index/query_engine/router_query_engine.py` & `llama_index-0.6.5/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.6.5/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/__init__.py` & `llama_index-0.6.5/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/base.py` & `llama_index-0.6.5/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.6.5/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/chroma.py` & `llama_index-0.6.5/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/database.py` & `llama_index-0.6.5/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/deeplake.py` & `llama_index-0.6.5/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/discord_reader.py` & `llama_index-0.6.5/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/download.py` & `llama_index-0.6.5/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/elasticsearch.py` & `llama_index-0.6.5/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/faiss.py` & `llama_index-0.6.5/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/base.py` & `llama_index-0.6.5/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/base_parser.py` & `llama_index-0.6.5/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/docs_parser.py` & `llama_index-0.6.5/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/epub_parser.py` & `llama_index-0.6.5/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/image_caption_parser.py` & `llama_index-0.6.5/llama_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/image_parser.py` & `llama_index-0.6.5/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/image_vision_llm_parser.py` & `llama_index-0.6.5/llama_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/ipynb_parser.py` & `llama_index-0.6.5/llama_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/markdown_parser.py` & `llama_index-0.6.5/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/mbox_parser.py` & `llama_index-0.6.5/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/slides_parser.py` & `llama_index-0.6.5/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/tabular_parser.py` & `llama_index-0.6.5/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/file/video_audio.py` & `llama_index-0.6.5/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.6.5/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.6.5/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/github_readers/utils.py` & `llama_index-0.6.5/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.6.5/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.6.5/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/json.py` & `llama_index-0.6.5/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/make_com/wrapper.py` & `llama_index-0.6.5/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/mbox.py` & `llama_index-0.6.5/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/metal.py` & `llama_index-0.6.5/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/milvus.py` & `llama_index-0.6.5/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/mongo.py` & `llama_index-0.6.5/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/myscale.py` & `llama_index-0.6.5/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/notion.py` & `llama_index-0.6.5/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/obsidian.py` & `llama_index-0.6.5/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/pinecone.py` & `llama_index-0.6.5/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/qdrant.py` & `llama_index-0.6.5/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/schema/base.py` & `llama_index-0.6.5/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/slack.py` & `llama_index-0.6.5/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/steamship/file_reader.py` & `llama_index-0.6.5/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/string_iterable.py` & `llama_index-0.6.5/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/twitter.py` & `llama_index-0.6.5/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/weaviate/client.py` & `llama_index-0.6.5/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/weaviate/reader.py` & `llama_index-0.6.5/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/weaviate/utils.py` & `llama_index-0.6.5/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/web.py` & `llama_index-0.6.5/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/wikipedia.py` & `llama_index-0.6.5/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/readers/youtube_transcript.py` & `llama_index-0.6.5/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/response/notebook_utils.py` & `llama_index-0.6.5/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/response/pprint_utils.py` & `llama_index-0.6.5/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/response/schema.py` & `llama_index-0.6.5/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/retrievers/__init__.py` & `llama_index-0.6.5/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/retrievers/transform_retriever.py` & `llama_index-0.6.5/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/schema.py` & `llama_index-0.6.5/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/selectors/llm_selectors.py` & `llama_index-0.6.5/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/selectors/prompts.py` & `llama_index-0.6.5/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/selectors/types.py` & `llama_index-0.6.5/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/docstore/__init__.py` & `llama_index-0.6.5/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.6.5/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.6.5/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/docstore/registry.py` & `llama_index-0.6.5/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.6.5/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/docstore/types.py` & `llama_index-0.6.5/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/docstore/utils.py` & `llama_index-0.6.5/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.6.5/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.6.5/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.6.5/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/index_store/types.py` & `llama_index-0.6.5/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/index_store/utils.py` & `llama_index-0.6.5/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.6.5/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.6.5/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/kvstore/types.py` & `llama_index-0.6.5/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/storage/storage_context.py` & `llama_index-0.6.5/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index-0.6.5/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.6.5/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/token_counter/token_counter.py` & `llama_index-0.6.5/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/token_counter/utils.py` & `llama_index-0.6.5/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/tools/query_engine.py` & `llama_index-0.6.5/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/tts/bark.py` & `llama_index-0.6.5/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/tts/base.py` & `llama_index-0.6.5/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/tts/elevenlabs.py` & `llama_index-0.6.5/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/utils.py` & `llama_index-0.6.5/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/__init__.py` & `llama_index-0.6.5/llama_index/vector_stores/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Vector stores."""
 
 from llama_index.vector_stores.chatgpt_plugin import ChatGPTRetrievalPluginClient
 from llama_index.vector_stores.chroma import ChromaVectorStore
 from llama_index.vector_stores.deeplake import DeepLakeVectorStore
 from llama_index.vector_stores.faiss import FaissVectorStore
-from llama_index.vector_stores.milvus import MilvusVectorStore
 from llama_index.vector_stores.lancedb import LanceDBVectorStore
 from llama_index.vector_stores.metal import MetalVectorStore
+from llama_index.vector_stores.milvus import MilvusVectorStore
 from llama_index.vector_stores.myscale import MyScaleVectorStore
 from llama_index.vector_stores.opensearch import (
     OpensearchVectorClient,
     OpensearchVectorStore,
 )
 from llama_index.vector_stores.pinecone import PineconeVectorStore
 from llama_index.vector_stores.qdrant import QdrantVectorStore
+from llama_index.vector_stores.redis import RedisVectorStore
 from llama_index.vector_stores.simple import SimpleVectorStore
 from llama_index.vector_stores.weaviate import WeaviateVectorStore
 
 __all__ = [
     "SimpleVectorStore",
+    "RedisVectorStore",
     "FaissVectorStore",
     "PineconeVectorStore",
     "WeaviateVectorStore",
     "QdrantVectorStore",
     "ChromaVectorStore",
     "MetalVectorStore",
     "OpensearchVectorStore",
```

### Comparing `llama_index-0.6.4/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.6.5/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/chroma.py` & `llama_index-0.6.5/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/deeplake.py` & `llama_index-0.6.5/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/faiss.py` & `llama_index-0.6.5/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/lancedb.py` & `llama_index-0.6.5/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/metal.py` & `llama_index-0.6.5/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/milvus.py` & `llama_index-0.6.5/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/myscale.py` & `llama_index-0.6.5/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/opensearch.py` & `llama_index-0.6.5/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/pinecone.py` & `llama_index-0.6.5/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/qdrant.py` & `llama_index-0.6.5/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/registry.py` & `llama_index-0.6.5/llama_index/vector_stores/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from enum import Enum
 from typing import Dict, Type
 
 from llama_index.vector_stores.chatgpt_plugin import ChatGPTRetrievalPluginClient
 from llama_index.vector_stores.chroma import ChromaVectorStore
 from llama_index.vector_stores.deeplake import DeepLakeVectorStore
 from llama_index.vector_stores.faiss import FaissVectorStore
-from llama_index.vector_stores.milvus import MilvusVectorStore
 from llama_index.vector_stores.lancedb import LanceDBVectorStore
+from llama_index.vector_stores.milvus import MilvusVectorStore
 from llama_index.vector_stores.myscale import MyScaleVectorStore
 from llama_index.vector_stores.opensearch import OpensearchVectorStore
 from llama_index.vector_stores.pinecone import PineconeVectorStore
 from llama_index.vector_stores.qdrant import QdrantVectorStore
+from llama_index.vector_stores.redis import RedisVectorStore
 from llama_index.vector_stores.simple import SimpleVectorStore
 from llama_index.vector_stores.types import VectorStore
 from llama_index.vector_stores.weaviate import WeaviateVectorStore
 
 
 class VectorStoreType(str, Enum):
     SIMPLE = "simple"
+    REDIS = "redis"
     WEAVIATE = "weaviate"
     QDRANT = "qdrant"
     PINECONE = "pinecone"
     OPENSEARCH = "opensearch"
     FAISS = "faiss"
     CHROMA = "chroma"
     CHATGPT_PLUGIN = "chatgpt_plugin"
@@ -29,14 +31,15 @@
     MILVUS = "milvus"
     DEEPLAKE = "deeplake"
     MYSCALE = "myscale"
 
 
 VECTOR_STORE_TYPE_TO_VECTOR_STORE_CLASS: Dict[VectorStoreType, Type[VectorStore]] = {
     VectorStoreType.SIMPLE: SimpleVectorStore,
+    VectorStoreType.REDIS: RedisVectorStore,
     VectorStoreType.WEAVIATE: WeaviateVectorStore,
     VectorStoreType.QDRANT: QdrantVectorStore,
     VectorStoreType.LANCEDB: LanceDBVectorStore,
     VectorStoreType.MILVUS: MilvusVectorStore,
     VectorStoreType.PINECONE: PineconeVectorStore,
     VectorStoreType.OPENSEARCH: OpensearchVectorStore,
     VectorStoreType.FAISS: FaissVectorStore,
```

### Comparing `llama_index-0.6.4/llama_index/vector_stores/simple.py` & `llama_index-0.6.5/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/types.py` & `llama_index-0.6.5/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index/vector_stores/weaviate.py` & `llama_index-0.6.5/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/llama_index.egg-info/PKG-INFO` & `llama_index-0.6.5/llama_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index
-Version: 0.6.4
+Version: 0.6.5
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `llama_index-0.6.4/llama_index.egg-info/SOURCES.txt` & `llama_index-0.6.5/llama_index.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 llama_index/indices/vector_store/__init__.py
 llama_index/indices/vector_store/base.py
 llama_index/indices/vector_store/retrievers.py
 llama_index/langchain_helpers/__init__.py
 llama_index/langchain_helpers/chain_wrapper.py
 llama_index/langchain_helpers/memory_wrapper.py
 llama_index/langchain_helpers/sql_wrapper.py
+llama_index/langchain_helpers/streaming.py
 llama_index/langchain_helpers/text_splitter.py
 llama_index/langchain_helpers/agents/__init__.py
 llama_index/langchain_helpers/agents/agents.py
 llama_index/langchain_helpers/agents/toolkits.py
 llama_index/langchain_helpers/agents/tools.py
 llama_index/llm_predictor/__init__.py
 llama_index/llm_predictor/base.py
@@ -197,14 +198,16 @@
 llama_index/readers/github_readers/github_repository_reader.py
 llama_index/readers/github_readers/utils.py
 llama_index/readers/google_readers/__init__.py
 llama_index/readers/google_readers/gdocs.py
 llama_index/readers/google_readers/gsheets.py
 llama_index/readers/make_com/__init__.py
 llama_index/readers/make_com/wrapper.py
+llama_index/readers/redis/__init__.py
+llama_index/readers/redis/utils.py
 llama_index/readers/schema/__init__.py
 llama_index/readers/schema/base.py
 llama_index/readers/steamship/__init__.py
 llama_index/readers/steamship/file_reader.py
 llama_index/readers/weaviate/__init__.py
 llama_index/readers/weaviate/client.py
 llama_index/readers/weaviate/reader.py
@@ -259,14 +262,15 @@
 llama_index/vector_stores/lancedb.py
 llama_index/vector_stores/metal.py
 llama_index/vector_stores/milvus.py
 llama_index/vector_stores/myscale.py
 llama_index/vector_stores/opensearch.py
 llama_index/vector_stores/pinecone.py
 llama_index/vector_stores/qdrant.py
+llama_index/vector_stores/redis.py
 llama_index/vector_stores/registry.py
 llama_index/vector_stores/simple.py
 llama_index/vector_stores/types.py
 llama_index/vector_stores/weaviate.py
 tests/__init__.py
 tests/conftest.py
 tests/test_utils.py
```

### Comparing `llama_index-0.6.4/setup.py` & `llama_index-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/callbacks/test_llama_debug.py` & `llama_index-0.6.5/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/conftest.py` & `llama_index-0.6.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/embeddings/test_base.py` & `llama_index-0.6.5/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/composability/test_utils.py` & `llama_index-0.6.5/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/conftest.py` & `llama_index-0.6.5/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/document_summary/test_index.py` & `llama_index-0.6.5/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/empty/test_base.py` & `llama_index-0.6.5/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/keyword_table/test_base.py` & `llama_index-0.6.5/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/keyword_table/test_retrievers.py` & `llama_index-0.6.5/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/keyword_table/test_utils.py` & `llama_index-0.6.5/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/knowledge_graph/test_base.py` & `llama_index-0.6.5/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/knowledge_graph/test_retrievers.py` & `llama_index-0.6.5/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/list/test_index.py` & `llama_index-0.6.5/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/list/test_retrievers.py` & `llama_index-0.6.5/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/postprocessor/test_base.py` & `llama_index-0.6.5/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/query/conftest.py` & `llama_index-0.6.5/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/query/query_transform/test_base.py` & `llama_index-0.6.5/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/query/test_compose.py` & `llama_index-0.6.5/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/query/test_compose_vector.py` & `llama_index-0.6.5/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/query/test_query_bundle.py` & `llama_index-0.6.5/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/struct_store/conftest.py` & `llama_index-0.6.5/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/struct_store/test_base.py` & `llama_index-0.6.5/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/struct_store/test_pandas.py` & `llama_index-0.6.5/tests/indices/struct_store/test_pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/struct_store/test_sql_query.py` & `llama_index-0.6.5/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/test_loading.py` & `llama_index-0.6.5/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/test_loading_graph.py` & `llama_index-0.6.5/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/test_node_utils.py` & `llama_index-0.6.5/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/test_prompt_helper.py` & `llama_index-0.6.5/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/tree/conftest.py` & `llama_index-0.6.5/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/tree/test_embedding_retriever.py` & `llama_index-0.6.5/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/tree/test_index.py` & `llama_index-0.6.5/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/tree/test_retrievers.py` & `llama_index-0.6.5/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/conftest.py` & `llama_index-0.6.5/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/mock_faiss.py` & `llama_index-0.6.5/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/mock_services.py` & `llama_index-0.6.5/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/test_faiss.py` & `llama_index-0.6.5/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/test_lancedb.py` & `llama_index-0.6.5/tests/indices/vector_store/test_lancedb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/test_milvus.py` & `llama_index-0.6.5/tests/indices/vector_store/test_milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/test_myscale.py` & `llama_index-0.6.5/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/test_pinecone.py` & `llama_index-0.6.5/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/test_retrievers.py` & `llama_index-0.6.5/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/test_simple.py` & `llama_index-0.6.5/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/test_weaviate.py` & `llama_index-0.6.5/tests/indices/vector_store/test_weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/indices/vector_store/utils.py` & `llama_index-0.6.5/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/langchain_helpers/test_text_splitter.py` & `llama_index-0.6.5/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/llm_predictor/test_base.py` & `llama_index-0.6.5/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/logger/test_base.py` & `llama_index-0.6.5/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/mock_utils/mock_predict.py` & `llama_index-0.6.5/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/mock_utils/mock_prompts.py` & `llama_index-0.6.5/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/mock_utils/mock_text_splitter.py` & `llama_index-0.6.5/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/mock_utils/mock_utils.py` & `llama_index-0.6.5/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/optimization/test_base.py` & `llama_index-0.6.5/tests/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/output_parsers/test_base.py` & `llama_index-0.6.5/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/output_parsers/test_selection.py` & `llama_index-0.6.5/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/playground/test_base.py` & `llama_index-0.6.5/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/prompts/test_base.py` & `llama_index-0.6.5/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/readers/test_file.py` & `llama_index-0.6.5/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/readers/test_json.py` & `llama_index-0.6.5/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/readers/test_mongo.py` & `llama_index-0.6.5/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/selectors/test_llm_selectors.py` & `llama_index-0.6.5/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/storage/conftest.py` & `llama_index-0.6.5/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/storage/docstore/test_mongo_docstore.py` & `llama_index-0.6.5/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/storage/docstore/test_simple_docstore.py` & `llama_index-0.6.5/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/storage/test_storage_context.py` & `llama_index-0.6.5/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/test_utils.py` & `llama_index-0.6.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/token_predictor/test_base.py` & `llama_index-0.6.5/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/vector_stores/test_qdrant.py` & `llama_index-0.6.5/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.4/tests/vector_stores/test_weaviate.py` & `llama_index-0.6.5/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

