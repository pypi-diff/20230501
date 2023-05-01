# Comparing `tmp/gpt_index-0.6.0a3.tar.gz` & `tmp/gpt_index-0.6.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_index-0.6.0a3.tar", last modified: Sun Apr 30 08:48:55 2023, max compression
+gzip compressed data, was "gpt_index-0.6.0a4.tar", last modified: Mon May  1 00:22:28 2023, max compression
```

## Comparing `gpt_index-0.6.0a3.tar` & `gpt_index-0.6.0a4.tar`

### file list

```diff
@@ -1,418 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.813879 gpt_index-0.6.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-30 08:48:55.813879 gpt_index-0.6.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.741878 gpt_index-0.6.0a3/gpt_index/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.741878 gpt_index-0.6.0a3/gpt_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.741878 gpt_index-0.6.0a3/gpt_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/data_structs/data_structs_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/data_structs/node_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/data_structs/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/data_structs/table_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.741878 gpt_index-0.6.0a3/gpt_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.745878 gpt_index-0.6.0a3/gpt_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.749878 gpt_index-0.6.0a3/gpt_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/postprocessor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.749878 gpt_index-0.6.0a3/gpt_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.749878 gpt_index-0.6.0a3/gpt_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/query/response_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.749878 gpt_index-0.6.0a3/gpt_index/indices/response/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22046 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/response/response_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/response/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.749878 gpt_index-0.6.0a3/gpt_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.749878 gpt_index-0.6.0a3/gpt_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.749878 gpt_index-0.6.0a3/gpt_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/vector_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/llm_predictor/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/llm_predictor/stable_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/llm_predictor/structured.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/node_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/output_parsers/langchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.753878 gpt_index-0.6.0a3/gpt_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.757878 gpt_index-0.6.0a3/gpt_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.761878 gpt_index-0.6.0a3/gpt_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.761878 gpt_index-0.6.0a3/gpt_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.765878 gpt_index-0.6.0a3/gpt_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/docs_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/epub_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/image_caption_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/image_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/ipynb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/mbox_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/slides_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/tabular_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/file/video_audio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.765878 gpt_index-0.6.0a3/gpt_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.765878 gpt_index-0.6.0a3/gpt_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.769878 gpt_index-0.6.0a3/gpt_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.769878 gpt_index-0.6.0a3/gpt_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.769878 gpt_index-0.6.0a3/gpt_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.769878 gpt_index-0.6.0a3/gpt_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/weaviate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/weaviate/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.773878 gpt_index-0.6.0a3/gpt_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.773878 gpt_index-0.6.0a3/gpt_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.773878 gpt_index-0.6.0a3/gpt_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.773878 gpt_index-0.6.0a3/gpt_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.777878 gpt_index-0.6.0a3/gpt_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.777878 gpt_index-0.6.0a3/gpt_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.781878 gpt_index-0.6.0a3/gpt_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/token_counter/token_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.781878 gpt_index-0.6.0a3/gpt_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/tools/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.785879 gpt_index-0.6.0a3/gpt_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/gpt_index/vector_stores/weaviate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.741878 gpt_index-0.6.0a3/gpt_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-30 08:48:55.000000 gpt_index-0.6.0a3/gpt_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-04-30 08:48:55.000000 gpt_index-0.6.0a3/gpt_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:48:55.000000 gpt_index-0.6.0a3/gpt_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-30 08:48:55.000000 gpt_index-0.6.0a3/gpt_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 08:48:55.000000 gpt_index-0.6.0a3/gpt_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 08:48:55.813879 gpt_index-0.6.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.785879 gpt_index-0.6.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.785879 gpt_index-0.6.0a3/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.789878 gpt_index-0.6.0a3/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.789878 gpt_index-0.6.0a3/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.789878 gpt_index-0.6.0a3/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.793878 gpt_index-0.6.0a3/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.793878 gpt_index-0.6.0a3/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.793878 gpt_index-0.6.0a3/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.793878 gpt_index-0.6.0a3/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/postprocessor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.797879 gpt_index-0.6.0a3/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.797879 gpt_index-0.6.0a3/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.797879 gpt_index-0.6.0a3/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/struct_store/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.801879 gpt_index-0.6.0a3/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.805879 gpt_index-0.6.0a3/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/test_milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/test_weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.805879 gpt_index-0.6.0a3/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.805879 gpt_index-0.6.0a3/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.805879 gpt_index-0.6.0a3/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.809879 gpt_index-0.6.0a3/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.809879 gpt_index-0.6.0a3/tests/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/optimization/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.809879 gpt_index-0.6.0a3/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/output_parsers/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.809879 gpt_index-0.6.0a3/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.809879 gpt_index-0.6.0a3/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/prompts/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.813879 gpt_index-0.6.0a3/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.813879 gpt_index-0.6.0a3/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.813879 gpt_index-0.6.0a3/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.813879 gpt_index-0.6.0a3/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:55.813879 gpt_index-0.6.0a3/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-30 08:48:42.000000 gpt_index-0.6.0a3/tests/vector_stores/test_qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.342674 gpt_index-0.6.0a4/gpt_index/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.342674 gpt_index-0.6.0a4/gpt_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/data_structs/data_structs_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/data_structs/node_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/data_structs/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/data_structs/table_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.346675 gpt_index-0.6.0a4/gpt_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.350675 gpt_index-0.6.0a4/gpt_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.350675 gpt_index-0.6.0a4/gpt_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.350675 gpt_index-0.6.0a4/gpt_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.350675 gpt_index-0.6.0a4/gpt_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/postprocessor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.350675 gpt_index-0.6.0a4/gpt_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.350675 gpt_index-0.6.0a4/gpt_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.354675 gpt_index-0.6.0a4/gpt_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22046 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.354675 gpt_index-0.6.0a4/gpt_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.354675 gpt_index-0.6.0a4/gpt_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.354675 gpt_index-0.6.0a4/gpt_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/vector_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.354675 gpt_index-0.6.0a4/gpt_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.358675 gpt_index-0.6.0a4/gpt_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.358675 gpt_index-0.6.0a4/gpt_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/llm_predictor/stable_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.358675 gpt_index-0.6.0a4/gpt_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.358675 gpt_index-0.6.0a4/gpt_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.358675 gpt_index-0.6.0a4/gpt_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.358675 gpt_index-0.6.0a4/gpt_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/output_parsers/langchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.358675 gpt_index-0.6.0a4/gpt_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.358675 gpt_index-0.6.0a4/gpt_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.362676 gpt_index-0.6.0a4/gpt_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.362676 gpt_index-0.6.0a4/gpt_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.366676 gpt_index-0.6.0a4/gpt_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.366676 gpt_index-0.6.0a4/gpt_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/docs_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/epub_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/image_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/mbox_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/slides_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/tabular_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/file/video_audio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.366676 gpt_index-0.6.0a4/gpt_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.366676 gpt_index-0.6.0a4/gpt_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.366676 gpt_index-0.6.0a4/gpt_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.370676 gpt_index-0.6.0a4/gpt_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.370676 gpt_index-0.6.0a4/gpt_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.370676 gpt_index-0.6.0a4/gpt_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.370676 gpt_index-0.6.0a4/gpt_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.370676 gpt_index-0.6.0a4/gpt_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.370676 gpt_index-0.6.0a4/gpt_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.370676 gpt_index-0.6.0a4/gpt_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.374677 gpt_index-0.6.0a4/gpt_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.374677 gpt_index-0.6.0a4/gpt_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.374677 gpt_index-0.6.0a4/gpt_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.374677 gpt_index-0.6.0a4/gpt_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/tools/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.374677 gpt_index-0.6.0a4/gpt_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.378677 gpt_index-0.6.0a4/gpt_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/gpt_index/vector_stores/weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.342674 gpt_index-0.6.0a4/gpt_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-01 00:22:28.000000 gpt_index-0.6.0a4/gpt_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-01 00:22:28.000000 gpt_index-0.6.0a4/gpt_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:22:28.000000 gpt_index-0.6.0a4/gpt_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 00:22:28.000000 gpt_index-0.6.0a4/gpt_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 00:22:28.000000 gpt_index-0.6.0a4/gpt_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.378677 gpt_index-0.6.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.378677 gpt_index-0.6.0a4/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.378677 gpt_index-0.6.0a4/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.378677 gpt_index-0.6.0a4/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.378677 gpt_index-0.6.0a4/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.378677 gpt_index-0.6.0a4/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.382677 gpt_index-0.6.0a4/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.382677 gpt_index-0.6.0a4/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.382677 gpt_index-0.6.0a4/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/postprocessor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.382677 gpt_index-0.6.0a4/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.382677 gpt_index-0.6.0a4/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.382677 gpt_index-0.6.0a4/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.382677 gpt_index-0.6.0a4/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.386677 gpt_index-0.6.0a4/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/test_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/test_weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.386677 gpt_index-0.6.0a4/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.386677 gpt_index-0.6.0a4/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.386677 gpt_index-0.6.0a4/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.386677 gpt_index-0.6.0a4/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.386677 gpt_index-0.6.0a4/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.386677 gpt_index-0.6.0a4/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/output_parsers/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.386677 gpt_index-0.6.0a4/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:28.390678 gpt_index-0.6.0a4/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-01 00:22:12.000000 gpt_index-0.6.0a4/tests/vector_stores/test_qdrant.py
```

### Comparing `gpt_index-0.6.0a3/LICENSE` & `gpt_index-0.6.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/PKG-INFO` & `gpt_index-0.6.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_index
-Version: 0.6.0a3
+Version: 0.6.0a4
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.0a3/README.md` & `gpt_index-0.6.0a4/README.md`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/__init__.py` & `gpt_index-0.6.0a4/gpt_index/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/composability/joint_qa_summary.py` & `gpt_index-0.6.0a4/gpt_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/data_structs/data_structs.py` & `gpt_index-0.6.0a4/gpt_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/data_structs/data_structs_v2.py` & `gpt_index-0.6.0a4/gpt_index/data_structs/data_structs_v2.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/data_structs/node_v2.py` & `gpt_index-0.6.0a4/gpt_index/data_structs/node_v2.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/data_structs/registry.py` & `gpt_index-0.6.0a4/gpt_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/data_structs/struct_type.py` & `gpt_index-0.6.0a4/gpt_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/data_structs/table.py` & `gpt_index-0.6.0a4/gpt_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/data_structs/table_v2.py` & `gpt_index-0.6.0a4/gpt_index/data_structs/table_v2.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/embeddings/base.py` & `gpt_index-0.6.0a4/gpt_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/embeddings/langchain.py` & `gpt_index-0.6.0a4/gpt_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/embeddings/openai.py` & `gpt_index-0.6.0a4/gpt_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/embeddings/utils.py` & `gpt_index-0.6.0a4/gpt_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/evaluation/base.py` & `gpt_index-0.6.0a4/gpt_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/evaluation/dataset_generation.py` & `gpt_index-0.6.0a4/gpt_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/img_utils.py` & `gpt_index-0.6.0a4/gpt_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/__init__.py` & `gpt_index-0.6.0a4/gpt_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/base_retriever.py` & `gpt_index-0.6.0a4/gpt_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/common/struct_store/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/common/struct_store/schema.py` & `gpt_index-0.6.0a4/gpt_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/common/struct_store/sql.py` & `gpt_index-0.6.0a4/gpt_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/common_tree/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/composability/graph.py` & `gpt_index-0.6.0a4/gpt_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/empty/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/empty/retrievers.py` & `gpt_index-0.6.0a4/gpt_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/keyword_table/__init__.py` & `gpt_index-0.6.0a4/gpt_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/keyword_table/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/keyword_table/rake_base.py` & `gpt_index-0.6.0a4/gpt_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/keyword_table/retrievers.py` & `gpt_index-0.6.0a4/gpt_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/keyword_table/simple_base.py` & `gpt_index-0.6.0a4/gpt_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/keyword_table/utils.py` & `gpt_index-0.6.0a4/gpt_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/knowledge_graph/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/knowledge_graph/retrievers.py` & `gpt_index-0.6.0a4/gpt_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/list/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/list/retrievers.py` & `gpt_index-0.6.0a4/gpt_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/loading.py` & `gpt_index-0.6.0a4/gpt_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/postprocessor/__init__.py` & `gpt_index-0.6.0a4/gpt_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/postprocessor/node.py` & `gpt_index-0.6.0a4/gpt_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/postprocessor/node_recency.py` & `gpt_index-0.6.0a4/gpt_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/postprocessor/pii.py` & `gpt_index-0.6.0a4/gpt_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/prompt_helper.py` & `gpt_index-0.6.0a4/gpt_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/query/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/query/embedding_utils.py` & `gpt_index-0.6.0a4/gpt_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/query/query_transform/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/query/query_transform/prompts.py` & `gpt_index-0.6.0a4/gpt_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/query/response_synthesis.py` & `gpt_index-0.6.0a4/gpt_index/indices/query/response_synthesis.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/query/schema.py` & `gpt_index-0.6.0a4/gpt_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/registry.py` & `gpt_index-0.6.0a4/gpt_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/response/response_builder.py` & `gpt_index-0.6.0a4/gpt_index/indices/response/response_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/service_context.py` & `gpt_index-0.6.0a4/gpt_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/struct_store/__init__.py` & `gpt_index-0.6.0a4/gpt_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/struct_store/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/struct_store/container_builder.py` & `gpt_index-0.6.0a4/gpt_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/struct_store/pandas.py` & `gpt_index-0.6.0a4/gpt_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/struct_store/pandas_query.py` & `gpt_index-0.6.0a4/gpt_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/struct_store/sql.py` & `gpt_index-0.6.0a4/gpt_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/struct_store/sql_query.py` & `gpt_index-0.6.0a4/gpt_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/tree/__init__.py` & `gpt_index-0.6.0a4/gpt_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/tree/all_leaf_retriever.py` & `gpt_index-0.6.0a4/gpt_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/tree/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/tree/inserter.py` & `gpt_index-0.6.0a4/gpt_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/tree/select_leaf_embedding_retriever.py` & `gpt_index-0.6.0a4/gpt_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/tree/select_leaf_retriever.py` & `gpt_index-0.6.0a4/gpt_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/tree/tree_root_retriever.py` & `gpt_index-0.6.0a4/gpt_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/utils.py` & `gpt_index-0.6.0a4/gpt_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/vector_store/base.py` & `gpt_index-0.6.0a4/gpt_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/indices/vector_store/retrievers.py` & `gpt_index-0.6.0a4/gpt_index/indices/vector_store/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/langchain_helpers/agents/agents.py` & `gpt_index-0.6.0a4/gpt_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/langchain_helpers/agents/toolkits.py` & `gpt_index-0.6.0a4/gpt_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/langchain_helpers/agents/tools.py` & `gpt_index-0.6.0a4/gpt_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/langchain_helpers/memory_wrapper.py` & `gpt_index-0.6.0a4/gpt_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/langchain_helpers/sql_wrapper.py` & `gpt_index-0.6.0a4/gpt_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/langchain_helpers/text_splitter.py` & `gpt_index-0.6.0a4/gpt_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/llm_predictor/base.py` & `gpt_index-0.6.0a4/gpt_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/llm_predictor/chatgpt.py` & `gpt_index-0.6.0a4/gpt_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/llm_predictor/stable_lm.py` & `gpt_index-0.6.0a4/gpt_index/llm_predictor/stable_lm.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/llm_predictor/structured.py` & `gpt_index-0.6.0a4/gpt_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/logger/base.py` & `gpt_index-0.6.0a4/gpt_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/node_parser/interface.py` & `gpt_index-0.6.0a4/gpt_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/node_parser/node_utils.py` & `gpt_index-0.6.0a4/gpt_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/node_parser/simple.py` & `gpt_index-0.6.0a4/gpt_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/optimization/optimizer.py` & `gpt_index-0.6.0a4/gpt_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/output_parsers/base.py` & `gpt_index-0.6.0a4/gpt_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/output_parsers/guardrails.py` & `gpt_index-0.6.0a4/gpt_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/output_parsers/langchain.py` & `gpt_index-0.6.0a4/gpt_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/playground/base.py` & `gpt_index-0.6.0a4/gpt_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/prompts/base.py` & `gpt_index-0.6.0a4/gpt_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/prompts/chat_prompts.py` & `gpt_index-0.6.0a4/gpt_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/prompts/default_prompt_selectors.py` & `gpt_index-0.6.0a4/gpt_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/prompts/default_prompts.py` & `gpt_index-0.6.0a4/gpt_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/prompts/prompt_type.py` & `gpt_index-0.6.0a4/gpt_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/prompts/prompts.py` & `gpt_index-0.6.0a4/gpt_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/query_engine/graph_query_engine.py` & `gpt_index-0.6.0a4/gpt_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/query_engine/multistep_query_engine.py` & `gpt_index-0.6.0a4/gpt_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/query_engine/retriever_query_engine.py` & `gpt_index-0.6.0a4/gpt_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/query_engine/transform_query_engine.py` & `gpt_index-0.6.0a4/gpt_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/__init__.py` & `gpt_index-0.6.0a4/gpt_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/base.py` & `gpt_index-0.6.0a4/gpt_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/chatgpt_plugin/base.py` & `gpt_index-0.6.0a4/gpt_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/chroma.py` & `gpt_index-0.6.0a4/gpt_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/database.py` & `gpt_index-0.6.0a4/gpt_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/deeplake.py` & `gpt_index-0.6.0a4/gpt_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/discord_reader.py` & `gpt_index-0.6.0a4/gpt_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/download.py` & `gpt_index-0.6.0a4/gpt_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/elasticsearch.py` & `gpt_index-0.6.0a4/gpt_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/faiss.py` & `gpt_index-0.6.0a4/gpt_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/base.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/base_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/docs_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/epub_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/image_caption_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/image_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/image_vision_llm_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/ipynb_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/markdown_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/mbox_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/slides_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/tabular_parser.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/file/video_audio.py` & `gpt_index-0.6.0a4/gpt_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/github_readers/github_api_client.py` & `gpt_index-0.6.0a4/gpt_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/github_readers/github_repository_reader.py` & `gpt_index-0.6.0a4/gpt_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/github_readers/utils.py` & `gpt_index-0.6.0a4/gpt_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/google_readers/gdocs.py` & `gpt_index-0.6.0a4/gpt_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/google_readers/gsheets.py` & `gpt_index-0.6.0a4/gpt_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/json.py` & `gpt_index-0.6.0a4/gpt_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/make_com/wrapper.py` & `gpt_index-0.6.0a4/gpt_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/mbox.py` & `gpt_index-0.6.0a4/gpt_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/milvus.py` & `gpt_index-0.6.0a4/gpt_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/mongo.py` & `gpt_index-0.6.0a4/gpt_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/myscale.py` & `gpt_index-0.6.0a4/gpt_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/notion.py` & `gpt_index-0.6.0a4/gpt_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/obsidian.py` & `gpt_index-0.6.0a4/gpt_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/pinecone.py` & `gpt_index-0.6.0a4/gpt_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/qdrant.py` & `gpt_index-0.6.0a4/gpt_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/schema/base.py` & `gpt_index-0.6.0a4/gpt_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/slack.py` & `gpt_index-0.6.0a4/gpt_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/steamship/file_reader.py` & `gpt_index-0.6.0a4/gpt_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/string_iterable.py` & `gpt_index-0.6.0a4/gpt_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/twitter.py` & `gpt_index-0.6.0a4/gpt_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/weaviate/client.py` & `gpt_index-0.6.0a4/gpt_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/weaviate/reader.py` & `gpt_index-0.6.0a4/gpt_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/weaviate/utils.py` & `gpt_index-0.6.0a4/gpt_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/web.py` & `gpt_index-0.6.0a4/gpt_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/wikipedia.py` & `gpt_index-0.6.0a4/gpt_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/readers/youtube_transcript.py` & `gpt_index-0.6.0a4/gpt_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/response/notebook_utils.py` & `gpt_index-0.6.0a4/gpt_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/response/schema.py` & `gpt_index-0.6.0a4/gpt_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/retrievers/__init__.py` & `gpt_index-0.6.0a4/gpt_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/retrievers/transform_retriever.py` & `gpt_index-0.6.0a4/gpt_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/schema.py` & `gpt_index-0.6.0a4/gpt_index/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/docstore/__init__.py` & `gpt_index-0.6.0a4/gpt_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/docstore/keyval_docstore.py` & `gpt_index-0.6.0a4/gpt_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/docstore/mongo_docstore.py` & `gpt_index-0.6.0a4/gpt_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/docstore/registry.py` & `gpt_index-0.6.0a4/gpt_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/docstore/simple_docstore.py` & `gpt_index-0.6.0a4/gpt_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/docstore/types.py` & `gpt_index-0.6.0a4/gpt_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/docstore/utils.py` & `gpt_index-0.6.0a4/gpt_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/index_store/keyval_index_store.py` & `gpt_index-0.6.0a4/gpt_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/index_store/mongo_index_store.py` & `gpt_index-0.6.0a4/gpt_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/index_store/simple_index_store.py` & `gpt_index-0.6.0a4/gpt_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/index_store/types.py` & `gpt_index-0.6.0a4/gpt_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/index_store/utils.py` & `gpt_index-0.6.0a4/gpt_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/kvstore/mongodb_kvstore.py` & `gpt_index-0.6.0a4/gpt_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/kvstore/simple_kvstore.py` & `gpt_index-0.6.0a4/gpt_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/kvstore/types.py` & `gpt_index-0.6.0a4/gpt_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/storage/storage_context.py` & `gpt_index-0.6.0a4/gpt_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/token_counter/mock_chain_wrapper.py` & `gpt_index-0.6.0a4/gpt_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/token_counter/mock_embed_model.py` & `gpt_index-0.6.0a4/gpt_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/token_counter/token_counter.py` & `gpt_index-0.6.0a4/gpt_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/token_counter/utils.py` & `gpt_index-0.6.0a4/gpt_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/tools/file_utils.py` & `gpt_index-0.6.0a4/gpt_index/tools/file_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/utils.py` & `gpt_index-0.6.0a4/gpt_index/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/__init__.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/chatgpt_plugin.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/chroma.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/deeplake.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/faiss.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/milvus.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/myscale.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/opensearch.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/pinecone.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/qdrant.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/registry.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/simple.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/types.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index/vector_stores/weaviate.py` & `gpt_index-0.6.0a4/gpt_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/gpt_index.egg-info/PKG-INFO` & `gpt_index-0.6.0a4/gpt_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-index
-Version: 0.6.0a3
+Version: 0.6.0a4
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.0a3/gpt_index.egg-info/SOURCES.txt` & `gpt_index-0.6.0a4/gpt_index.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,18 @@
 gpt_index/token_counter/__init__.py
 gpt_index/token_counter/mock_chain_wrapper.py
 gpt_index/token_counter/mock_embed_model.py
 gpt_index/token_counter/token_counter.py
 gpt_index/token_counter/utils.py
 gpt_index/tools/__init__.py
 gpt_index/tools/file_utils.py
+gpt_index/tts/__init__.py
+gpt_index/tts/bark.py
+gpt_index/tts/base.py
+gpt_index/tts/elevenlabs.py
 gpt_index/vector_stores/__init__.py
 gpt_index/vector_stores/chatgpt_plugin.py
 gpt_index/vector_stores/chroma.py
 gpt_index/vector_stores/deeplake.py
 gpt_index/vector_stores/faiss.py
 gpt_index/vector_stores/milvus.py
 gpt_index/vector_stores/myscale.py
```

### Comparing `gpt_index-0.6.0a3/setup.py` & `gpt_index-0.6.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/conftest.py` & `gpt_index-0.6.0a4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/embeddings/test_base.py` & `gpt_index-0.6.0a4/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/composability/test_utils.py` & `gpt_index-0.6.0a4/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/conftest.py` & `gpt_index-0.6.0a4/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/empty/test_base.py` & `gpt_index-0.6.0a4/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/keyword_table/test_base.py` & `gpt_index-0.6.0a4/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/keyword_table/test_retrievers.py` & `gpt_index-0.6.0a4/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/keyword_table/test_utils.py` & `gpt_index-0.6.0a4/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/knowledge_graph/test_base.py` & `gpt_index-0.6.0a4/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/knowledge_graph/test_retrievers.py` & `gpt_index-0.6.0a4/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/list/test_index.py` & `gpt_index-0.6.0a4/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/list/test_retrievers.py` & `gpt_index-0.6.0a4/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/postprocessor/test_base.py` & `gpt_index-0.6.0a4/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/query/conftest.py` & `gpt_index-0.6.0a4/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/query/query_transform/test_base.py` & `gpt_index-0.6.0a4/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/query/test_compose.py` & `gpt_index-0.6.0a4/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/query/test_compose_vector.py` & `gpt_index-0.6.0a4/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/query/test_query_bundle.py` & `gpt_index-0.6.0a4/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/struct_store/conftest.py` & `gpt_index-0.6.0a4/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/struct_store/test_base.py` & `gpt_index-0.6.0a4/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/struct_store/test_pandas.py` & `gpt_index-0.6.0a4/tests/indices/struct_store/test_pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/struct_store/test_sql_query.py` & `gpt_index-0.6.0a4/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/test_loading.py` & `gpt_index-0.6.0a4/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/test_loading_graph.py` & `gpt_index-0.6.0a4/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/test_node_utils.py` & `gpt_index-0.6.0a4/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/test_prompt_helper.py` & `gpt_index-0.6.0a4/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/tree/conftest.py` & `gpt_index-0.6.0a4/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/tree/test_embedding_retriever.py` & `gpt_index-0.6.0a4/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/tree/test_index.py` & `gpt_index-0.6.0a4/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/tree/test_retrievers.py` & `gpt_index-0.6.0a4/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/conftest.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/mock_faiss.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/mock_services.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/test_faiss.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/test_milvus.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/test_milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/test_myscale.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/test_pinecone.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/test_retrievers.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/test_simple.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/test_weaviate.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/test_weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/indices/vector_store/utils.py` & `gpt_index-0.6.0a4/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/langchain_helpers/test_text_splitter.py` & `gpt_index-0.6.0a4/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/llm_predictor/test_base.py` & `gpt_index-0.6.0a4/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/logger/test_base.py` & `gpt_index-0.6.0a4/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/mock_utils/mock_predict.py` & `gpt_index-0.6.0a4/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/mock_utils/mock_prompts.py` & `gpt_index-0.6.0a4/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/mock_utils/mock_text_splitter.py` & `gpt_index-0.6.0a4/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/mock_utils/mock_utils.py` & `gpt_index-0.6.0a4/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/optimization/test_base.py` & `gpt_index-0.6.0a4/tests/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/output_parsers/test_base.py` & `gpt_index-0.6.0a4/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/playground/test_base.py` & `gpt_index-0.6.0a4/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/prompts/test_base.py` & `gpt_index-0.6.0a4/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/readers/test_file.py` & `gpt_index-0.6.0a4/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/readers/test_json.py` & `gpt_index-0.6.0a4/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/readers/test_mongo.py` & `gpt_index-0.6.0a4/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/storage/conftest.py` & `gpt_index-0.6.0a4/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/storage/docstore/test_mongo_docstore.py` & `gpt_index-0.6.0a4/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/storage/docstore/test_simple_docstore.py` & `gpt_index-0.6.0a4/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/test_utils.py` & `gpt_index-0.6.0a4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/token_predictor/test_base.py` & `gpt_index-0.6.0a4/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a3/tests/vector_stores/test_qdrant.py` & `gpt_index-0.6.0a4/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

