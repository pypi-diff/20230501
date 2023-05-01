# Comparing `tmp/llama_index-0.6.0a4.tar.gz` & `tmp/llama_index-0.6.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.6.0a4.tar", last modified: Mon May  1 00:23:44 2023, max compression
+gzip compressed data, was "llama_index-0.6.0a5.tar", last modified: Mon May  1 06:33:46 2023, max compression
```

## Comparing `llama_index-0.6.0a4.tar` & `llama_index-0.6.0a5.tar`

### file list

```diff
@@ -1,304 +1,312 @@
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.744300 llama_index-0.6.0a4/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1064 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/LICENSE
--rw-r--r--   0 jerryliu   (501) staff       (20)       73 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/MANIFEST.in
--rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-01 00:23:44.744196 llama_index-0.6.0a4/PKG-INFO
--rw-r--r--   0 jerryliu   (501) staff       (20)     4124 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/README.md
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.719994 llama_index-0.6.0a4/llama_index/
--rw-r--r--   0 jerryliu   (501) staff       (20)       13 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/VERSION
--rw-r--r--   0 jerryliu   (501) staff       (20)     4719 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      322 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/async_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.720713 llama_index-0.6.0a4/llama_index/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)      220 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      171 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/composability/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2739 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      219 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/constants.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.721507 llama_index-0.6.0a4/llama_index/data_structs/
--rw-r--r--   0 jerryliu   (501) staff       (20)      409 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    12377 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/data_structs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9476 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/data_structs_v2.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      264 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/node_mapping.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6221 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/node_v2.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      779 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3256 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/struct_type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/table.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1032 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/data_structs/table_v2.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.721940 llama_index-0.6.0a4/llama_index/embeddings/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/embeddings/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7721 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/embeddings/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1109 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/embeddings/langchain.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10103 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/embeddings/openai.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      559 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/embeddings/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.722201 llama_index-0.6.0a4/llama_index/evaluation/
--rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/evaluation/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11972 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/evaluation/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5344 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      544 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/img_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.722922 llama_index-0.6.0a4/llama_index/indices/
--rw-r--r--   0 jerryliu   (501) staff       (20)      542 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9024 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      897 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.723008 llama_index-0.6.0a4/llama_index/indices/common/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.723373 llama_index-0.6.0a4/llama_index/indices/common/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8114 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      776 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2676 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.723550 llama_index-0.6.0a4/llama_index/indices/common_tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7244 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.723729 llama_index-0.6.0a4/llama_index/indices/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)      180 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3962 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.723997 llama_index-0.6.0a4/llama_index/indices/empty/
--rw-r--r--   0 jerryliu   (501) staff       (20)      198 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/empty/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2151 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/empty/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1176 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.724537 llama_index-0.6.0a4/llama_index/indices/keyword_table/
--rw-r--r--   0 jerryliu   (501) staff       (20)      656 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7652 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      650 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5891 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      844 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2264 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.724806 llama_index-0.6.0a4/llama_index/indices/knowledge_graph/
--rw-r--r--   0 jerryliu   (501) staff       (20)      254 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7816 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9543 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.725074 llama_index-0.6.0a4/llama_index/indices/list/
--rw-r--r--   0 jerryliu   (501) staff       (20)      295 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/list/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3305 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/list/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3455 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/list/retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3608 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/loading.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.725525 llama_index-0.6.0a4/llama_index/indices/postprocessor/
--rw-r--r--   0 jerryliu   (501) staff       (20)      888 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)       83 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/postprocessor/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11695 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8778 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4896 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8492 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.725975 llama_index-0.6.0a4/llama_index/indices/query/
--rw-r--r--   0 jerryliu   (501) staff       (20)      137 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/query/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1975 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/query/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3386 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.726249 llama_index-0.6.0a4/llama_index/indices/query/query_transform/
--rw-r--r--   0 jerryliu   (501) staff       (20)      281 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8928 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5920 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8098 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1203 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/query/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1811 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/registry.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.726544 llama_index-0.6.0a4/llama_index/indices/response/
--rw-r--r--   0 jerryliu   (501) staff       (20)      419 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/response/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    22074 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/response/response_builder.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/response/type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3296 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/service_context.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.727223 llama_index-0.6.0a4/llama_index/indices/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      622 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2115 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/struct_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5802 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2214 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4688 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6139 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5887 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.727982 llama_index-0.6.0a4/llama_index/indices/tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)      616 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1612 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5834 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/tree/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7181 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/tree/inserter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4663 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15299 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1402 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2005 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.728301 llama_index-0.6.0a4/llama_index/indices/vector_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      260 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8183 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/vector_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3987 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.728914 llama_index-0.6.0a4/llama_index/langchain_helpers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       39 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.729401 llama_index-0.6.0a4/llama_index/langchain_helpers/agents/
--rw-r--r--   0 jerryliu   (501) staff       (20)      514 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2989 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      837 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2211 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      252 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7675 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3287 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    17585 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.729987 llama_index-0.6.0a4/llama_index/llm_predictor/
--rw-r--r--   0 jerryliu   (501) staff       (20)      330 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10593 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/llm_predictor/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4275 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4732 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/llm_predictor/stable_lm.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2274 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.730234 llama_index-0.6.0a4/llama_index/logger/
--rw-r--r--   0 jerryliu   (501) staff       (20)       95 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/logger/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      995 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/logger/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.730699 llama_index-0.6.0a4/llama_index/node_parser/
--rw-r--r--   0 jerryliu   (501) staff       (20)      184 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/node_parser/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      530 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/node_parser/interface.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3585 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/node_parser/node_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1821 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/node_parser/simple.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.730932 llama_index-0.6.0a4/llama_index/optimization/
--rw-r--r--   0 jerryliu   (501) staff       (20)      144 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/optimization/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4301 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.731361 llama_index-0.6.0a4/llama_index/output_parsers/
--rw-r--r--   0 jerryliu   (501) staff       (20)      230 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/output_parsers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      611 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/output_parsers/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2742 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1828 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/output_parsers/langchain.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.731581 llama_index-0.6.0a4/llama_index/playground/
--rw-r--r--   0 jerryliu   (501) staff       (20)      202 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/playground/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6471 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/playground/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.732350 llama_index-0.6.0a4/llama_index/prompts/
--rw-r--r--   0 jerryliu   (501) staff       (20)       87 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/prompts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6626 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/prompts/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1969 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1134 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10843 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/prompts/default_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      992 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/prompts/prompt_type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7685 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/prompts/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/py.typed
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.732871 llama_index-0.6.0a4/llama_index/query_engine/
--rw-r--r--   0 jerryliu   (501) staff       (20)      460 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/query_engine/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3572 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5814 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5322 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2967 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.735208 llama_index-0.6.0a4/llama_index/readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)     2974 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      659 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.735447 llama_index-0.6.0a4/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 jerryliu   (501) staff       (20)      145 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2111 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3755 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/chroma.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3308 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/database.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3457 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/deeplake.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4981 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/discord_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7775 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/download.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2392 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/elasticsearch.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2510 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/faiss.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.737312 llama_index-0.6.0a4/llama_index/readers/file/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8535 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1342 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/base_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1629 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1318 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3180 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4106 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/image_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3222 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1027 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3616 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3162 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3945 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3357 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1770 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.737825 llama_index-0.6.0a4/llama_index/readers/github_readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11730 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15928 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5473 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.738206 llama_index-0.6.0a4/llama_index/readers/google_readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5659 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4989 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3708 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/json.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.738454 llama_index-0.6.0a4/llama_index/readers/make_com/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1696 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1261 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/mbox.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4588 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2608 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/mongo.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5541 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5679 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/notion.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1601 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/obsidian.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2766 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3909 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/qdrant.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.738711 llama_index-0.6.0a4/llama_index/readers/schema/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/schema/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1214 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/schema/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7892 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/slack.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.738943 llama_index-0.6.0a4/llama_index/readers/steamship/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3498 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1042 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/string_iterable.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1918 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/twitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.739305 llama_index-0.6.0a4/llama_index/readers/weaviate/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7766 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/weaviate/client.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3986 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1867 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7987 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/web.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      981 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/wikipedia.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1255 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.739668 llama_index-0.6.0a4/llama_index/response/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/response/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2039 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/response/notebook_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3071 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/response/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/response/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.739843 llama_index-0.6.0a4/llama_index/retrievers/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1258 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/retrievers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1066 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2768 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/schema.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.740026 llama_index-0.6.0a4/llama_index/storage/
--rw-r--r--   0 jerryliu   (501) staff       (20)      124 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.740652 llama_index-0.6.0a4/llama_index/storage/docstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)      536 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4825 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1408 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      762 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/docstore/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2294 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2532 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/docstore/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      918 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.741258 llama_index-0.6.0a4/llama_index/storage/index_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      301 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2224 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1341 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1508 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      884 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/index_store/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      644 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.741675 llama_index-0.6.0a4/llama_index/storage/kvstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)      187 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4061 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2330 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      973 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/kvstore/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3114 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/storage/storage_context.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.742191 llama_index-0.6.0a4/llama_index/token_counter/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/token_counter/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4664 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      722 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2874 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/token_counter/token_counter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/token_counter/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.742401 llama_index-0.6.0a4/llama_index/tools/
--rw-r--r--   0 jerryliu   (501) staff       (20)       13 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/tools/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      723 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/tools/file_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.742781 llama_index-0.6.0a4/llama_index/tts/
--rw-r--r--   0 jerryliu   (501) staff       (20)      154 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/tts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2589 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/tts/bark.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      631 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/tts/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1282 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/tts/elevenlabs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)       81 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5847 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.744051 llama_index-0.6.0a4/llama_index/vector_stores/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1132 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5240 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3947 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/chroma.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8631 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4365 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/faiss.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15768 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8344 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7186 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11419 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6505 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1973 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5084 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/simple.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2210 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3385 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index/vector_stores/weaviate.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 00:23:44.720439 llama_index-0.6.0a4/llama_index.egg-info/
--rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 jerryliu   (501) staff       (20)     9661 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)        1 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       96 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index.egg-info/requires.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       12 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/llama_index.egg-info/top_level.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       38 2023-05-01 00:23:44.744331 llama_index-0.6.0a4/setup.cfg
--rw-r--r--   0 jerryliu   (501) staff       (20)     1130 2023-05-01 00:23:44.000000 llama_index-0.6.0a4/setup.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.759964 llama_index-0.6.0a5/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1064 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/LICENSE
+-rw-r--r--   0 jerryliu   (501) staff       (20)       73 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/MANIFEST.in
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-01 06:33:46.759859 llama_index-0.6.0a5/PKG-INFO
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4124 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/README.md
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.735778 llama_index-0.6.0a5/llama_index/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       13 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/VERSION
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4719 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      322 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/async_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.736499 llama_index-0.6.0a5/llama_index/composability/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      220 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/composability/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      171 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/composability/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2739 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      219 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/constants.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.737321 llama_index-0.6.0a5/llama_index/data_structs/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      409 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    12377 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9476 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/data_structs_v2.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      264 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/node_mapping.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6221 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/node_v2.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      779 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3256 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/table.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1032 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/table_v2.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.737770 llama_index-0.6.0a5/llama_index/embeddings/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7721 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1109 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/langchain.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10103 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/openai.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      559 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.738038 llama_index-0.6.0a5/llama_index/evaluation/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/evaluation/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11972 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/evaluation/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5344 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      544 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/img_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.738744 llama_index-0.6.0a5/llama_index/indices/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      542 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9112 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      859 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.738830 llama_index-0.6.0a5/llama_index/indices/common/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.739191 llama_index-0.6.0a5/llama_index/indices/common/struct_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8114 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      776 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2676 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.739371 llama_index-0.6.0a5/llama_index/indices/common_tree/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7244 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.739552 llama_index-0.6.0a5/llama_index/indices/composability/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      180 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3962 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.739819 llama_index-0.6.0a5/llama_index/indices/empty/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      198 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2151 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/empty/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1176 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.740370 llama_index-0.6.0a5/llama_index/indices/keyword_table/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      656 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7652 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      650 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5891 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      844 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2264 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.740638 llama_index-0.6.0a5/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      254 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7816 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9543 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.740906 llama_index-0.6.0a5/llama_index/indices/list/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      295 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/list/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3305 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/list/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3455 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3608 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/loading.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.741353 llama_index-0.6.0a5/llama_index/indices/postprocessor/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      888 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)       83 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11695 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8778 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4896 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8492 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.741801 llama_index-0.6.0a5/llama_index/indices/query/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      137 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1937 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3386 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.742080 llama_index-0.6.0a5/llama_index/indices/query/query_transform/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      281 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8904 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5920 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8098 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1248 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1811 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/registry.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.742383 llama_index-0.6.0a5/llama_index/indices/response/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      419 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/response/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    21995 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/response/type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3296 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/service_context.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.743013 llama_index-0.6.0a5/llama_index/indices/struct_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      622 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2115 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5765 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2214 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4688 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6139 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5887 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.743641 llama_index-0.6.0a5/llama_index/indices/tree/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      616 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1612 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5834 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7181 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4663 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15299 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1402 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2005 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.743907 llama_index-0.6.0a5/llama_index/indices/vector_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      260 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8183 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/vector_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3987 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.744466 llama_index-0.6.0a5/llama_index/langchain_helpers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       39 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.744858 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      514 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2994 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      837 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2211 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      252 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7675 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3287 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    18172 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.745310 llama_index-0.6.0a5/llama_index/llm_predictor/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      330 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10838 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4282 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4732 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/stable_lm.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2274 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.745503 llama_index-0.6.0a5/llama_index/logger/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       95 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/logger/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      995 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/logger/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.745882 llama_index-0.6.0a5/llama_index/node_parser/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      184 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/node_parser/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      530 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/node_parser/interface.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3585 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1821 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/node_parser/simple.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.746079 llama_index-0.6.0a5/llama_index/optimization/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      144 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/optimization/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4301 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.746603 llama_index-0.6.0a5/llama_index/output_parsers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      230 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      611 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2742 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1828 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1345 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/selection.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.746817 llama_index-0.6.0a5/llama_index/playground/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      202 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/playground/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6471 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/playground/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.747555 llama_index-0.6.0a5/llama_index/prompts/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       87 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6633 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1969 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1134 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10843 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1120 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7685 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/py.typed
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.748194 llama_index-0.6.0a5/llama_index/query_engine/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      560 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3572 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5814 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5322 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2449 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2967 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.750991 llama_index-0.6.0a5/llama_index/readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2974 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      659 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.751232 llama_index-0.6.0a5/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      145 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2111 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3755 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/chroma.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3308 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/database.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3457 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/deeplake.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4981 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/discord_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7775 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/download.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2392 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2510 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/faiss.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.752745 llama_index-0.6.0a5/llama_index/readers/file/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8535 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1342 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1629 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1318 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3180 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4106 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3222 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1027 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3616 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3162 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3945 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3357 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1770 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.753140 llama_index-0.6.0a5/llama_index/readers/github_readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11730 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15928 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5473 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.753402 llama_index-0.6.0a5/llama_index/readers/google_readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5659 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4989 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3708 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/json.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.753626 llama_index-0.6.0a5/llama_index/readers/make_com/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1696 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1261 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/mbox.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4588 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/milvus.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2608 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/mongo.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5541 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/myscale.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5679 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/notion.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1601 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/obsidian.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2766 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/pinecone.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3909 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/qdrant.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.753847 llama_index-0.6.0a5/llama_index/readers/schema/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1214 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/schema/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7892 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/slack.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.754066 llama_index-0.6.0a5/llama_index/readers/steamship/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3498 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1042 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/string_iterable.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1918 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/twitter.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.754507 llama_index-0.6.0a5/llama_index/readers/weaviate/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7766 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3986 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1867 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7987 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/web.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      981 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/wikipedia.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1255 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.754942 llama_index-0.6.0a5/llama_index/response/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/response/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2039 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/response/notebook_utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3071 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/response/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/response/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.755177 llama_index-0.6.0a5/llama_index/retrievers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1258 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/retrievers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1066 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2768 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/schema.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.755576 llama_index-0.6.0a5/llama_index/selectors/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/selectors/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7055 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2438 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/selectors/prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2006 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/selectors/types.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.755752 llama_index-0.6.0a5/llama_index/storage/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      124 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.756385 llama_index-0.6.0a5/llama_index/storage/docstore/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      536 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4825 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1408 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      762 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2294 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2532 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      918 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.756931 llama_index-0.6.0a5/llama_index/storage/index_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      301 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2224 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1341 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1508 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      884 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      644 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.757287 llama_index-0.6.0a5/llama_index/storage/kvstore/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      187 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4061 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2330 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      973 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3114 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/storage_context.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.757727 llama_index-0.6.0a5/llama_index/token_counter/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4664 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      722 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2874 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.758015 llama_index-0.6.0a5/llama_index/tools/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      162 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tools/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1557 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tools/query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      366 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tools/types.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.758403 llama_index-0.6.0a5/llama_index/tts/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      154 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tts/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2589 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tts/bark.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      631 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tts/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1282 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)       81 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5847 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.759711 llama_index-0.6.0a5/llama_index/vector_stores/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1132 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5240 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3947 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8631 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4365 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15768 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8344 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7186 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11419 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6505 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1973 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5084 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/simple.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2210 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3385 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/weaviate.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.736230 llama_index-0.6.0a5/llama_index.egg-info/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9915 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)        1 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       96 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/requires.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       12 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       38 2023-05-01 06:33:46.759993 llama_index-0.6.0a5/setup.cfg
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1130 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/setup.py
```

### Comparing `llama_index-0.6.0a4/LICENSE` & `llama_index-0.6.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/PKG-INFO` & `llama_index-0.6.0a5/llama_index.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: llama_index
-Version: 0.6.0a4
+Name: llama-index
+Version: 0.6.0a5
 Summary: Interface between LLMs and your data.
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `llama_index-0.6.0a4/README.md` & `llama_index-0.6.0a5/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/__init__.py` & `llama_index-0.6.0a5/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/composability/joint_qa_summary.py` & `llama_index-0.6.0a5/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/data_structs/data_structs.py` & `llama_index-0.6.0a5/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/data_structs/data_structs_v2.py` & `llama_index-0.6.0a5/llama_index/data_structs/data_structs_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/data_structs/node_v2.py` & `llama_index-0.6.0a5/llama_index/data_structs/node_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/data_structs/registry.py` & `llama_index-0.6.0a5/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/data_structs/struct_type.py` & `llama_index-0.6.0a5/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/data_structs/table.py` & `llama_index-0.6.0a5/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/data_structs/table_v2.py` & `llama_index-0.6.0a5/llama_index/data_structs/table_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/embeddings/base.py` & `llama_index-0.6.0a5/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/embeddings/langchain.py` & `llama_index-0.6.0a5/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/embeddings/openai.py` & `llama_index-0.6.0a5/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/embeddings/utils.py` & `llama_index-0.6.0a5/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/evaluation/base.py` & `llama_index-0.6.0a5/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/evaluation/dataset_generation.py` & `llama_index-0.6.0a5/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/img_utils.py` & `llama_index-0.6.0a5/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/__init__.py` & `llama_index-0.6.0a5/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/base.py` & `llama_index-0.6.0a5/llama_index/indices/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
         self._insert(nodes, **insert_kwargs)
         self._storage_context.index_store.add_index_struct(self._index_struct)
 
     def insert(self, document: Document, **insert_kwargs: Any) -> None:
         """Insert a document."""
         nodes = self.service_context.node_parser.get_nodes_from_documents([document])
         self.insert_nodes(nodes, **insert_kwargs)
+        self.docstore.set_document_hash(document.get_doc_id(), document.get_doc_hash())
 
     @abstractmethod
     def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document."""
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document from the index.
```

### Comparing `llama_index-0.6.0a4/llama_index/indices/base_retriever.py` & `llama_index-0.6.0a5/llama_index/indices/base_retriever.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from abc import ABC, abstractmethod
-from typing import List, Union
+from typing import List
 from llama_index.data_structs.node_v2 import NodeWithScore
 
-from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.query.schema import QueryBundle, QueryType
 
 
 class BaseRetriever(ABC):
     """Base retriever."""
 
-    def retrieve(
-        self, str_or_query_bundle: Union[str, QueryBundle]
-    ) -> List[NodeWithScore]:
+    def retrieve(self, str_or_query_bundle: QueryType) -> List[NodeWithScore]:
         """Retrieve nodes given query.
 
         Args:
-            str_or_query_bundle (Union[str, QueryBundle]): Either a query string or
+            str_or_query_bundle (QueryType): Either a query string or
                 a QueryBundle object.
 
         """
         if isinstance(str_or_query_bundle, str):
             str_or_query_bundle = QueryBundle(str_or_query_bundle)
         return self._retrieve(str_or_query_bundle)
```

### Comparing `llama_index-0.6.0a4/llama_index/indices/common/struct_store/base.py` & `llama_index-0.6.0a5/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.6.0a5/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.6.0a5/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/common_tree/base.py` & `llama_index-0.6.0a5/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/composability/graph.py` & `llama_index-0.6.0a5/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/empty/base.py` & `llama_index-0.6.0a5/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/empty/retrievers.py` & `llama_index-0.6.0a5/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.6.0a5/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/keyword_table/base.py` & `llama_index-0.6.0a5/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.6.0a5/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.6.0a5/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.6.0a5/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/keyword_table/utils.py` & `llama_index-0.6.0a5/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.6.0a5/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/knowledge_graph/retrievers.py` & `llama_index-0.6.0a5/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/list/base.py` & `llama_index-0.6.0a5/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/list/retrievers.py` & `llama_index-0.6.0a5/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/loading.py` & `llama_index-0.6.0a5/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.6.0a5/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/postprocessor/node.py` & `llama_index-0.6.0a5/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.6.0a5/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/postprocessor/pii.py` & `llama_index-0.6.0a5/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/prompt_helper.py` & `llama_index-0.6.0a5/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/query/base.py` & `llama_index-0.6.0a5/llama_index/indices/query/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """Base query engine."""
 
 import logging
 from abc import ABC, abstractmethod
-from typing import List, Optional, Sequence, Union
+from typing import List, Optional, Sequence
 from llama_index.data_structs.node_v2 import NodeWithScore
 
-from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.query.schema import QueryBundle, QueryType
 from llama_index.response.schema import (
     RESPONSE_TYPE,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class BaseQueryEngine(ABC):
-    def query(self, str_or_query_bundle: Union[str, QueryBundle]) -> RESPONSE_TYPE:
+    def query(self, str_or_query_bundle: QueryType) -> RESPONSE_TYPE:
         if isinstance(str_or_query_bundle, str):
             str_or_query_bundle = QueryBundle(str_or_query_bundle)
         return self._query(str_or_query_bundle)
 
-    async def aquery(
-        self, str_or_query_bundle: Union[str, QueryBundle]
-    ) -> RESPONSE_TYPE:
+    async def aquery(self, str_or_query_bundle: QueryType) -> RESPONSE_TYPE:
         if isinstance(str_or_query_bundle, str):
             str_or_query_bundle = QueryBundle(str_or_query_bundle)
         return await self._aquery(str_or_query_bundle)
 
     def retrieve(self, query_bundle: QueryBundle) -> List[NodeWithScore]:
         raise NotImplementedError(
             "This query engine does not support retrieve, use query directly"
```

### Comparing `llama_index-0.6.0a4/llama_index/indices/query/embedding_utils.py` & `llama_index-0.6.0a5/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/query/query_transform/base.py` & `llama_index-0.6.0a5/llama_index/indices/query/query_transform/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Query transform."""
 
 import dataclasses
 from abc import abstractmethod
-from typing import Dict, Optional, Union, cast
+from typing import Dict, Optional, cast
 
 from langchain.input import print_text
 
 from llama_index.indices.query.query_transform.prompts import (
     DEFAULT_DECOMPOSE_QUERY_TRANSFORM_PROMPT,
     DEFAULT_IMAGE_OUTPUT_PROMPT,
     DEFAULT_STEP_DECOMPOSE_QUERY_TRANSFORM_PROMPT,
     DecomposeQueryTransformPrompt,
     ImageOutputQueryTransformPrompt,
     StepDecomposeQueryTransformPrompt,
 )
-from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.query.schema import QueryBundle, QueryType
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.prompts.base import Prompt
 from llama_index.prompts.default_prompts import DEFAULT_HYDE_PROMPT
 from llama_index.response.schema import Response
 
 
 class BaseQueryTransform:
@@ -33,15 +33,15 @@
 
     @abstractmethod
     def _run(self, query_bundle: QueryBundle, extra_info: Dict) -> QueryBundle:
         """Run query transform."""
 
     def run(
         self,
-        query_bundle_or_str: Union[str, QueryBundle],
+        query_bundle_or_str: QueryType,
         extra_info: Optional[Dict] = None,
     ) -> QueryBundle:
         """Run query transform."""
         extra_info = extra_info or {}
         if isinstance(query_bundle_or_str, str):
             query_bundle = QueryBundle(
                 query_str=query_bundle_or_str,
@@ -50,15 +50,15 @@
         else:
             query_bundle = query_bundle_or_str
 
         return self._run(query_bundle, extra_info=extra_info)
 
     def __call__(
         self,
-        query_bundle_or_str: Union[str, QueryBundle],
+        query_bundle_or_str: QueryType,
         extra_info: Optional[Dict] = None,
     ) -> QueryBundle:
         """Run query processor."""
         return self.run(query_bundle_or_str, extra_info=extra_info)
 
 
 class IdentityQueryTransform(BaseQueryTransform):
```

### Comparing `llama_index-0.6.0a4/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.6.0a5/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/query/response_synthesis.py` & `llama_index-0.6.0a5/llama_index/indices/query/response_synthesis.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/query/schema.py` & `llama_index-0.6.0a5/llama_index/indices/query/schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This schema is used under the hood for all queries, but is primarily
 exposed for recursive queries over composable indices.
 
 """
 
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Union
 
 from dataclasses_json import DataClassJsonMixin
 
 
 @dataclass
 class QueryBundle(DataClassJsonMixin):
     """
@@ -33,7 +33,10 @@
     @property
     def embedding_strs(self) -> List[str]:
         """Use custom embedding strs if specified, otherwise use query str."""
         if self.custom_embedding_strs is None:
             return [self.query_str]
         else:
             return self.custom_embedding_strs
+
+
+QueryType = Union[str, QueryBundle]
```

### Comparing `llama_index-0.6.0a4/llama_index/indices/registry.py` & `llama_index-0.6.0a5/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/response/response_builder.py` & `llama_index-0.6.0a5/llama_index/indices/response/response_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,25 +253,23 @@
         super().__init__(
             service_context=service_context,
             text_qa_template=text_qa_template,
             refine_template=refine_template,
             streaming=streaming,
         )
 
-    @llm_token_counter("aget_response")
     async def aget_response(
         self,
         query_str: str,
         text_chunks: Sequence[str],
         prev_response: Optional[str] = None,
         **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         return self.get_response(query_str, text_chunks, prev_response)
 
-    @llm_token_counter("get_response")
     def get_response(
         self,
         query_str: str,
         text_chunks: Sequence[str],
         prev_response: Optional[str] = None,
         **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
```

### Comparing `llama_index-0.6.0a4/llama_index/indices/service_context.py` & `llama_index-0.6.0a5/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/struct_store/__init__.py` & `llama_index-0.6.0a5/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/struct_store/base.py` & `llama_index-0.6.0a5/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.6.0a5/llama_index/indices/struct_store/container_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """SQL Container builder."""
 
 
-from typing import Any, Dict, List, Optional, Type, Union
+from typing import Any, Dict, List, Optional, Type
 
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.common.struct_store.base import SQLDocumentContextBuilder
 from llama_index.indices.common.struct_store.schema import SQLContextContainer
-from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.query.schema import QueryType
 from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
 from llama_index.readers.base import Document
 from llama_index.schema import BaseDocument
 
 DEFAULT_CONTEXT_QUERY_TMPL = (
     "Please return the relevant tables (including the full schema) "
     "for the following query: {orig_query_str}"
@@ -112,28 +112,28 @@
             **index_kwargs,
         )
         return index
 
     def query_index_for_context(
         self,
         index: BaseGPTIndex,
-        query_str: Union[str, QueryBundle],
+        query_str: QueryType,
         query_tmpl: Optional[str] = DEFAULT_CONTEXT_QUERY_TMPL,
         store_context_str: bool = True,
         **index_kwargs: Any,
     ) -> str:
         """Query index for context.
 
         A simple wrapper around the index.query call which
         injects a query template to specifically fetch table information,
         and can store a context_str.
 
         Args:
             index (BaseGPTIndex): index data structure
-            query_str (Union[str, QueryBundle]): query string
+            query_str (QueryType): query string
             query_tmpl (Optional[str]): query template
             store_context_str (bool): store context_str
 
         """
         if query_tmpl is None:
             context_query_str = query_str
         else:
```

### Comparing `llama_index-0.6.0a4/llama_index/indices/struct_store/pandas.py` & `llama_index-0.6.0a5/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/struct_store/pandas_query.py` & `llama_index-0.6.0a5/llama_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/struct_store/sql.py` & `llama_index-0.6.0a5/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.6.0a5/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/tree/__init__.py` & `llama_index-0.6.0a5/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.6.0a5/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/tree/base.py` & `llama_index-0.6.0a5/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/tree/inserter.py` & `llama_index-0.6.0a5/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.6.0a5/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.6.0a5/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.6.0a5/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/utils.py` & `llama_index-0.6.0a5/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/vector_store/base.py` & `llama_index-0.6.0a5/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/indices/vector_store/retrievers.py` & `llama_index-0.6.0a5/llama_index/indices/vector_store/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.6.0a5/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.6.0a5/llama_index/langchain_helpers/agents/agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Create LlamaIndex agents."""
 
 from typing import Any, Optional
 
 from langchain.agents import AgentExecutor, initialize_agent
-from langchain.callbacks import BaseCallbackManager
+from langchain.callbacks.base import BaseCallbackManager
 from langchain.llms.base import BaseLLM
 from langchain.agents.agent_types import AgentType
 
 from llama_index.langchain_helpers.agents.toolkits import LlamaToolkit
 
 
 def create_llama_agent(
```

### Comparing `llama_index-0.6.0a4/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.6.0a5/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.6.0a5/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.6.0a5/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.6.0a5/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.6.0a5/llama_index/langchain_helpers/text_splitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,18 +91,26 @@
 
                 cur_splits2 = []
                 for cur_split in cur_splits:
                     num_cur_tokens = len(self.tokenizer(cur_split))
                     if num_cur_tokens <= chunk_size:
                         cur_splits2.extend([cur_split])
                     else:
-                        cur_split_chunks = [
-                            cur_split[i : i + chunk_size]
-                            for i in range(0, len(cur_split), chunk_size)
-                        ]
+                        # split cur_split according to chunk size of the token numbers
+                        cur_split_chunks = []
+                        end_idx = len(cur_split)
+                        while len(self.tokenizer(cur_split[0:end_idx])) > chunk_size:
+                            for i in range(1, end_idx):
+                                tmp_split = cur_split[0 : end_idx - i]
+                                if len(self.tokenizer(tmp_split)) <= chunk_size:
+                                    cur_split_chunks.append(tmp_split)
+                                    cur_split = cur_split[end_idx - i : end_idx]
+                                    end_idx = len(cur_split)
+                                    break
+                        cur_split_chunks.append(cur_split)
                         cur_splits2.extend(cur_split_chunks)
 
                 new_splits.extend(cur_splits2)
         return new_splits
 
     def _postprocess_splits(self, docs: List[TextSplit]) -> List[TextSplit]:
         """Post-process splits."""
```

### Comparing `llama_index-0.6.0a4/llama_index/llm_predictor/base.py` & `llama_index-0.6.0a5/llama_index/llm_predictor/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Wrapper functions around an LLM chain."""
 
 import logging
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import Any, Generator, Optional, Protocol, Tuple
 
+import langchain
 import openai
-from langchain import Cohere, LLMChain, OpenAI
+from langchain import Cohere, LLMChain, OpenAI, BaseCache
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import AI21
-from langchain.schema import BaseLanguageModel
+from langchain.base_language import BaseLanguageModel
 
 from llama_index.constants import MAX_CHUNK_SIZE, NUM_OUTPUTS
 from llama_index.prompts.base import Prompt
 from llama_index.utils import (
     ErrorToRetry,
     globals_helper,
     retry_on_exceptions_with_backoff,
@@ -151,21 +152,27 @@
             Please see `Langchain's LLM Page
             <https://langchain.readthedocs.io/en/latest/modules/llms.html>`_
             for more details.
 
         retry_on_throttling (bool): Whether to retry on rate limit errors.
             Defaults to true.
 
+        cache (Optional[langchain.cache.BaseCache]) : use cached result for LLM
     """
 
     def __init__(
-        self, llm: Optional[BaseLanguageModel] = None, retry_on_throttling: bool = True
+        self,
+        llm: Optional[BaseLanguageModel] = None,
+        retry_on_throttling: bool = True,
+        cache: Optional[BaseCache] = None,
     ) -> None:
         """Initialize params."""
         self._llm = llm or OpenAI(temperature=0, model_name="text-davinci-003")
+        if cache is not None:
+            langchain.llm_cache = cache
         self.retry_on_throttling = retry_on_throttling
         self._total_tokens_used = 0
         self.flag = True
         self._last_token_usage: Optional[int] = None
 
     @property
     def llm(self) -> BaseLanguageModel:
```

### Comparing `llama_index-0.6.0a4/llama_index/llm_predictor/chatgpt.py` & `llama_index-0.6.0a5/llama_index/llm_predictor/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from langchain.prompts.base import BasePromptTemplate
 from langchain.prompts.chat import (
     BaseMessagePromptTemplate,
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
 )
 from langchain.prompts.prompt import PromptTemplate
-from langchain.schema import BaseLanguageModel, BaseMessage
+from langchain.base_language import BaseLanguageModel, BaseMessage
 
 from llama_index.llm_predictor.base import LLMPredictor
 from llama_index.prompts.base import Prompt
 from llama_index.utils import ErrorToRetry, retry_on_exceptions_with_backoff
 
 logger = logging.getLogger(__name__)
```

### Comparing `llama_index-0.6.0a4/llama_index/llm_predictor/stable_lm.py` & `llama_index-0.6.0a5/llama_index/llm_predictor/stable_lm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/llm_predictor/structured.py` & `llama_index-0.6.0a5/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/logger/base.py` & `llama_index-0.6.0a5/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/node_parser/interface.py` & `llama_index-0.6.0a5/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/node_parser/node_utils.py` & `llama_index-0.6.0a5/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/node_parser/simple.py` & `llama_index-0.6.0a5/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/optimization/optimizer.py` & `llama_index-0.6.0a5/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/output_parsers/base.py` & `llama_index-0.6.0a5/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/output_parsers/guardrails.py` & `llama_index-0.6.0a5/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/output_parsers/langchain.py` & `llama_index-0.6.0a5/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/playground/base.py` & `llama_index-0.6.0a5/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/prompts/base.py` & `llama_index-0.6.0a5/llama_index/prompts/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 from string import Formatter
 from typing import Any, Dict, List, Optional, Type, TypeVar
 
 from langchain import BasePromptTemplate as BaseLangchainPrompt
 from langchain import PromptTemplate as LangchainPrompt
 from langchain.chains.prompt_selector import ConditionalPromptSelector
-from langchain.schema import BaseLanguageModel
+from langchain.base_language import BaseLanguageModel
 
 from llama_index.output_parsers.base import BaseOutputParser
 from llama_index.prompts.prompt_type import PromptType
 
 PMT = TypeVar("PMT", bound="Prompt")
```

### Comparing `llama_index-0.6.0a4/llama_index/prompts/chat_prompts.py` & `llama_index-0.6.0a5/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.6.0a5/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/prompts/default_prompts.py` & `llama_index-0.6.0a5/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/prompts/prompt_type.py` & `llama_index-0.6.0a5/llama_index/prompts/prompt_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,9 +37,15 @@
 
     # Simple Input prompt
     SIMPLE_INPUT = "simple_input"
 
     # Pandas prompt
     PANDAS = "pandas"
 
+    # Single select prompt
+    SINGLE_SELECT = "single_select"
+
+    # Multiple select prompt
+    MULTI_SELECT = "multi_select"
+
     # custom (by default)
     CUSTOM = "custom"
```

### Comparing `llama_index-0.6.0a4/llama_index/prompts/prompts.py` & `llama_index-0.6.0a5/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.6.0a5/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.6.0a5/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.6.0a5/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.6.0a5/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/__init__.py` & `llama_index-0.6.0a5/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/base.py` & `llama_index-0.6.0a5/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.6.0a5/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/chroma.py` & `llama_index-0.6.0a5/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/database.py` & `llama_index-0.6.0a5/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/deeplake.py` & `llama_index-0.6.0a5/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/discord_reader.py` & `llama_index-0.6.0a5/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/download.py` & `llama_index-0.6.0a5/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/elasticsearch.py` & `llama_index-0.6.0a5/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/faiss.py` & `llama_index-0.6.0a5/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/base.py` & `llama_index-0.6.0a5/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/base_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/docs_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/epub_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/image_caption_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/image_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/image_vision_llm_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/ipynb_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/markdown_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/mbox_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/slides_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/tabular_parser.py` & `llama_index-0.6.0a5/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/file/video_audio.py` & `llama_index-0.6.0a5/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.6.0a5/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.6.0a5/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/github_readers/utils.py` & `llama_index-0.6.0a5/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.6.0a5/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.6.0a5/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/json.py` & `llama_index-0.6.0a5/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/make_com/wrapper.py` & `llama_index-0.6.0a5/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/mbox.py` & `llama_index-0.6.0a5/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/milvus.py` & `llama_index-0.6.0a5/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/mongo.py` & `llama_index-0.6.0a5/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/myscale.py` & `llama_index-0.6.0a5/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/notion.py` & `llama_index-0.6.0a5/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/obsidian.py` & `llama_index-0.6.0a5/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/pinecone.py` & `llama_index-0.6.0a5/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/qdrant.py` & `llama_index-0.6.0a5/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/schema/base.py` & `llama_index-0.6.0a5/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/slack.py` & `llama_index-0.6.0a5/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/steamship/file_reader.py` & `llama_index-0.6.0a5/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/string_iterable.py` & `llama_index-0.6.0a5/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/twitter.py` & `llama_index-0.6.0a5/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/weaviate/client.py` & `llama_index-0.6.0a5/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/weaviate/reader.py` & `llama_index-0.6.0a5/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/weaviate/utils.py` & `llama_index-0.6.0a5/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/web.py` & `llama_index-0.6.0a5/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/wikipedia.py` & `llama_index-0.6.0a5/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/readers/youtube_transcript.py` & `llama_index-0.6.0a5/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/response/notebook_utils.py` & `llama_index-0.6.0a5/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/response/schema.py` & `llama_index-0.6.0a5/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/retrievers/__init__.py` & `llama_index-0.6.0a5/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/retrievers/transform_retriever.py` & `llama_index-0.6.0a5/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/schema.py` & `llama_index-0.6.0a5/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/docstore/__init__.py` & `llama_index-0.6.0a5/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.6.0a5/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.6.0a5/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/docstore/registry.py` & `llama_index-0.6.0a5/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.6.0a5/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/docstore/types.py` & `llama_index-0.6.0a5/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/docstore/utils.py` & `llama_index-0.6.0a5/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.6.0a5/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.6.0a5/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.6.0a5/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/index_store/types.py` & `llama_index-0.6.0a5/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/index_store/utils.py` & `llama_index-0.6.0a5/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.6.0a5/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.6.0a5/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/kvstore/types.py` & `llama_index-0.6.0a5/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/storage/storage_context.py` & `llama_index-0.6.0a5/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index-0.6.0a5/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.6.0a5/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/token_counter/token_counter.py` & `llama_index-0.6.0a5/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/token_counter/utils.py` & `llama_index-0.6.0a5/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/tts/bark.py` & `llama_index-0.6.0a5/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/tts/base.py` & `llama_index-0.6.0a5/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/tts/elevenlabs.py` & `llama_index-0.6.0a5/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/utils.py` & `llama_index-0.6.0a5/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/__init__.py` & `llama_index-0.6.0a5/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.6.0a5/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/chroma.py` & `llama_index-0.6.0a5/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/deeplake.py` & `llama_index-0.6.0a5/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/faiss.py` & `llama_index-0.6.0a5/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/milvus.py` & `llama_index-0.6.0a5/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/myscale.py` & `llama_index-0.6.0a5/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/opensearch.py` & `llama_index-0.6.0a5/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/pinecone.py` & `llama_index-0.6.0a5/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/qdrant.py` & `llama_index-0.6.0a5/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/registry.py` & `llama_index-0.6.0a5/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/simple.py` & `llama_index-0.6.0a5/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/types.py` & `llama_index-0.6.0a5/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index/vector_stores/weaviate.py` & `llama_index-0.6.0a5/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a4/llama_index.egg-info/PKG-INFO` & `llama_index-0.6.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: llama-index
-Version: 0.6.0a4
+Name: llama_index
+Version: 0.6.0a5
 Summary: Interface between LLMs and your data.
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `llama_index-0.6.0a4/llama_index.egg-info/SOURCES.txt` & `llama_index-0.6.0a5/llama_index.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -123,27 +123,29 @@
 llama_index/node_parser/simple.py
 llama_index/optimization/__init__.py
 llama_index/optimization/optimizer.py
 llama_index/output_parsers/__init__.py
 llama_index/output_parsers/base.py
 llama_index/output_parsers/guardrails.py
 llama_index/output_parsers/langchain.py
+llama_index/output_parsers/selection.py
 llama_index/playground/__init__.py
 llama_index/playground/base.py
 llama_index/prompts/__init__.py
 llama_index/prompts/base.py
 llama_index/prompts/chat_prompts.py
 llama_index/prompts/default_prompt_selectors.py
 llama_index/prompts/default_prompts.py
 llama_index/prompts/prompt_type.py
 llama_index/prompts/prompts.py
 llama_index/query_engine/__init__.py
 llama_index/query_engine/graph_query_engine.py
 llama_index/query_engine/multistep_query_engine.py
 llama_index/query_engine/retriever_query_engine.py
+llama_index/query_engine/router_query_engine.py
 llama_index/query_engine/transform_query_engine.py
 llama_index/readers/__init__.py
 llama_index/readers/base.py
 llama_index/readers/chroma.py
 llama_index/readers/database.py
 llama_index/readers/deeplake.py
 llama_index/readers/discord_reader.py
@@ -200,14 +202,18 @@
 llama_index/readers/weaviate/utils.py
 llama_index/response/__init__.py
 llama_index/response/notebook_utils.py
 llama_index/response/schema.py
 llama_index/response/utils.py
 llama_index/retrievers/__init__.py
 llama_index/retrievers/transform_retriever.py
+llama_index/selectors/__init__.py
+llama_index/selectors/llm_selectors.py
+llama_index/selectors/prompts.py
+llama_index/selectors/types.py
 llama_index/storage/__init__.py
 llama_index/storage/storage_context.py
 llama_index/storage/docstore/__init__.py
 llama_index/storage/docstore/keyval_docstore.py
 llama_index/storage/docstore/mongo_docstore.py
 llama_index/storage/docstore/registry.py
 llama_index/storage/docstore/simple_docstore.py
@@ -225,15 +231,16 @@
 llama_index/storage/kvstore/types.py
 llama_index/token_counter/__init__.py
 llama_index/token_counter/mock_chain_wrapper.py
 llama_index/token_counter/mock_embed_model.py
 llama_index/token_counter/token_counter.py
 llama_index/token_counter/utils.py
 llama_index/tools/__init__.py
-llama_index/tools/file_utils.py
+llama_index/tools/query_engine.py
+llama_index/tools/types.py
 llama_index/tts/__init__.py
 llama_index/tts/bark.py
 llama_index/tts/base.py
 llama_index/tts/elevenlabs.py
 llama_index/vector_stores/__init__.py
 llama_index/vector_stores/chatgpt_plugin.py
 llama_index/vector_stores/chroma.py
```

### Comparing `llama_index-0.6.0a4/setup.py` & `llama_index-0.6.0a5/setup.py`

 * *Files identical despite different names*

