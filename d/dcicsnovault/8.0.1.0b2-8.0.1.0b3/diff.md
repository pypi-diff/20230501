# Comparing `tmp/dcicsnovault-8.0.1.0b2.tar.gz` & `tmp/dcicsnovault-8.0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.0.1.0b2.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.1.0b3.tar", max compression
```

## Comparing `dcicsnovault-8.0.1.0b2.tar` & `dcicsnovault-8.0.1.0b3.tar`

### file list

```diff
@@ -1,160 +1,163 @@
--rw-r--r--   0        0        0     1135 2023-04-28 17:25:54.473943 dcicsnovault-8.0.1.0b2/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-04-28 17:25:54.473943 dcicsnovault-8.0.1.0b2/README.rst
--rw-r--r--   0        0        0     5506 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     4586 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/aggregated_items.py
--rw-r--r--   0        0        0     8799 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/app.py
--rw-r--r--   0        0        0    11879 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/attachment.py
--rw-r--r--   0        0        0    25327 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/authentication.py
--rw-r--r--   0        0        0     4467 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6813 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     5764 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/list_db_tables.py
--rw-r--r--   0        0        0     6212 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2402 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     5155 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/prepare_template.py
--rw-r--r--   0        0        0     4350 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/custom_embed.py
--rw-r--r--   0        0        0     7228 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/jsonld_context.py
--rw-r--r--   0        0        0    30350 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/loadxl.py
--rw-r--r--   0        0        0     2425 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/memlimit.py
--rw-r--r--   0        0        0      895 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/nginx-dev.conf
--rw-r--r--   0        0        0     1165 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/parallel.py
--rw-r--r--   0        0        0      846 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/predicates.py
--rw-r--r--   0        0        0     1095 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/project.py
--rw-r--r--   0        0        0       95 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22128 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/resource_views.py
--rw-r--r--   0        0        0    21863 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/resources.py
--rw-r--r--   0        0        0     3450 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/schema_graph.py
--rw-r--r--   0        0        0    14547 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0    18744 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/search/search.py
--rw-r--r--   0        0        0    17901 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/search/search_utils.py
--rw-r--r--   0        0        0     4541 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/server_defaults.py
--rw-r--r--   0        0        0      522 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/settings.py
--rw-r--r--   0        0        0     1769 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/sqlalchemy_tools.py
--rw-r--r--   0        0        0     1498 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2210 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0        0 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/data/inserts/README.rst
--rw-r--r--   0        0        0        0 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/data/master-inserts/README.rst
--rw-r--r--   0        0        0     3086 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3173 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     6782 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_types_access_key.py
--rw-r--r--   0        0        0     1291 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_util.py
--rw-r--r--   0        0        0    18612 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4578 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/__init__.py
--rw-r--r--   0        0        0     5101 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/access_key.py
--rw-r--r--   0        0        0    16288 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/filter_set.py
--rw-r--r--   0        0        0     5536 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/upgrader.py
--rw-r--r--   0        0        0    51788 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/validators.py
--rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-05-01 17:31:15.503177 dcicsnovault-8.0.1.0b3/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-05-01 17:31:15.503177 dcicsnovault-8.0.1.0b3/README.rst
+-rw-r--r--   0        0        0     5506 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     4636 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/app.py
+-rw-r--r--   0        0        0      358 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/appdefs.py
+-rw-r--r--   0        0        0    11879 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/attachment.py
+-rw-r--r--   0        0        0    25327 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/authentication.py
+-rw-r--r--   0        0        0     4467 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-05-01 17:31:15.507177 dcicsnovault-8.0.1.0b3/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6813 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     5764 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/list_db_tables.py
+-rw-r--r--   0        0        0     6212 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2402 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     5155 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/prepare_template.py
+-rw-r--r--   0        0        0     4350 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7228 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8249 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    30350 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/loadxl.py
+-rw-r--r--   0        0        0     2425 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/memlimit.py
+-rw-r--r--   0        0        0      895 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/nginx-dev.conf
+-rw-r--r--   0        0        0     1165 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/predicates.py
+-rw-r--r--   0        0        0     1095 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/project.py
+-rw-r--r--   0        0        0       95 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22128 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/resource_views.py
+-rw-r--r--   0        0        0    21863 2023-05-01 17:31:15.511177 dcicsnovault-8.0.1.0b3/snovault/resources.py
+-rw-r--r--   0        0        0     9874 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/root.py
+-rw-r--r--   0        0        0      986 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/schema_formats.py
+-rw-r--r--   0        0        0     3450 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/schema_graph.py
+-rw-r--r--   0        0        0    14547 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4358 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/schema_views.py
+-rw-r--r--   0        0        0     1855 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5098 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0    18744 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19600 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/search/search.py
+-rw-r--r--   0        0        0    17901 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     4541 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/server_defaults.py
+-rw-r--r--   0        0        0      522 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/settings.py
+-rw-r--r--   0        0        0     1769 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/sqlalchemy_tools.py
+-rw-r--r--   0        0        0     1498 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      697 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0        0 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/data/inserts/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/data/master-inserts/README.rst
+-rw-r--r--   0        0        0     3086 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3173 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-05-01 17:31:15.515177 dcicsnovault-8.0.1.0b3/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     6782 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_types_access_key.py
+-rw-r--r--   0        0        0     1291 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    18612 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4578 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34107 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/types/access_key.py
+-rw-r--r--   0        0        0    16288 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/types/filter_set.py
+-rw-r--r--   0        0        0     5536 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/upgrader.py
+-rw-r--r--   0        0        0    52799 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-05-01 17:31:15.519177 dcicsnovault-8.0.1.0b3/snovault/validators.py
+-rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b3/PKG-INFO
```

### Comparing `dcicsnovault-8.0.1.0b2/LICENSE.txt` & `dcicsnovault-8.0.1.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/README.rst` & `dcicsnovault-8.0.1.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/pyproject.toml` & `dcicsnovault-8.0.1.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.0.1.0b2"  # to become 8.1.0
+version = "8.0.1.0b3"  # to become 8.1.0
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
```

### Comparing `dcicsnovault-8.0.1.0b2/snovault/__init__.py` & `dcicsnovault-8.0.1.0b3/snovault/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,16 @@
     # only include this stuff if we're testing
     if asbool(settings.get('testing', False)):
         config.include('snovault.tests.testing_views')
         config.include('snovault.tests.root')
 
         # in addition, enable invalidation scope for testing - but NOT by default
         settings[INVALIDATION_SCOPE_ENABLED] = True
+    else:
+        config.include('snovault.root')
 
     if 'elasticsearch.server' in config.registry.settings:
         config.include('snovault.elasticsearch')
 
     # configure redis server in production.ini
     if 'redis.server' in config.registry.settings:
         config.include('snovault.redis')
```

### Comparing `dcicsnovault-8.0.1.0b2/snovault/aggregated_items.py` & `dcicsnovault-8.0.1.0b3/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/app.py` & `dcicsnovault-8.0.1.0b3/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/attachment.py` & `dcicsnovault-8.0.1.0b3/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/authentication.py` & `dcicsnovault-8.0.1.0b3/snovault/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/authorization.py` & `dcicsnovault-8.0.1.0b3/snovault/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/batchupgrade.py` & `dcicsnovault-8.0.1.0b3/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/cache.py` & `dcicsnovault-8.0.1.0b3/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/calculated.py` & `dcicsnovault-8.0.1.0b3/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/clear_db_es_contents.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/create_mapping_on_deploy.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/create_mapping_on_deploy.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/list_db_tables.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/list_db_tables.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/load_access_keys.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/load_access_keys.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/load_data.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/load_data_by_type.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/load_data_by_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/prepare_template.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/prepare_template.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/profile.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/purge_item_type.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/purge_item_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/run_upgrader_on_inserts.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/run_upgrader_on_inserts.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/update_inserts_from_server.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/update_inserts_from_server.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.1.0b3/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/config.py` & `dcicsnovault-8.0.1.0b3/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/connection.py` & `dcicsnovault-8.0.1.0b3/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/crud_views.py` & `dcicsnovault-8.0.1.0b3/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/custom_embed.py` & `dcicsnovault-8.0.1.0b3/snovault/custom_embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/dev_servers.py` & `dcicsnovault-8.0.1.0b3/snovault/dev_servers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/drs.py` & `dcicsnovault-8.0.1.0b3/snovault/drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/edw_hash.py` & `dcicsnovault-8.0.1.0b3/snovault/edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.1.0b3/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/embed.py` & `dcicsnovault-8.0.1.0b3/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/etag.py` & `dcicsnovault-8.0.1.0b3/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/indexing_views.py` & `dcicsnovault-8.0.1.0b3/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/interfaces.py` & `dcicsnovault-8.0.1.0b3/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/invalidation.py` & `dcicsnovault-8.0.1.0b3/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/json_renderer.py` & `dcicsnovault-8.0.1.0b3/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/jsongraph.py` & `dcicsnovault-8.0.1.0b3/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/jsonld_context.py` & `dcicsnovault-8.0.1.0b3/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/loadxl.py` & `dcicsnovault-8.0.1.0b3/snovault/loadxl.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/memlimit.py` & `dcicsnovault-8.0.1.0b3/snovault/memlimit.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/nginx-dev.conf` & `dcicsnovault-8.0.1.0b3/snovault/nginx-dev.conf`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/parallel.py` & `dcicsnovault-8.0.1.0b3/snovault/parallel.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/predicates.py` & `dcicsnovault-8.0.1.0b3/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/project.py` & `dcicsnovault-8.0.1.0b3/snovault/project.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.1.0b3/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/renderers.py` & `dcicsnovault-8.0.1.0b3/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/resource_views.py` & `dcicsnovault-8.0.1.0b3/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/resources.py` & `dcicsnovault-8.0.1.0b3/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/schema_graph.py` & `dcicsnovault-8.0.1.0b3/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/schema_utils.py` & `dcicsnovault-8.0.1.0b3/snovault/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/schema_views.py` & `dcicsnovault-8.0.1.0b3/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/schemas/access_key.json` & `dcicsnovault-8.0.1.0b3/snovault/schemas/access_key.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/schemas/filter_set.json` & `dcicsnovault-8.0.1.0b3/snovault/schemas/filter_set.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/schemas/mixins.json` & `dcicsnovault-8.0.1.0b3/snovault/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/schemas/user.json` & `dcicsnovault-8.0.1.0b3/snovault/schemas/user.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/search/compound_search.py` & `dcicsnovault-8.0.1.0b3/snovault/search/compound_search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/search/lucene_builder.py` & `dcicsnovault-8.0.1.0b3/snovault/search/lucene_builder.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/search/search.py` & `dcicsnovault-8.0.1.0b3/snovault/search/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/search/search_utils.py` & `dcicsnovault-8.0.1.0b3/snovault/search/search_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/server_defaults.py` & `dcicsnovault-8.0.1.0b3/snovault/server_defaults.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/settings.py` & `dcicsnovault-8.0.1.0b3/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/sqlalchemy_tools.py` & `dcicsnovault-8.0.1.0b3/snovault/sqlalchemy_tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/standalone_dev.py` & `dcicsnovault-8.0.1.0b3/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/stats.py` & `dcicsnovault-8.0.1.0b3/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/storage.py` & `dcicsnovault-8.0.1.0b3/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/test_schemas/mixins.json` & `dcicsnovault-8.0.1.0b3/snovault/test_schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/conftest.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/root.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_clear_db_es_contents.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_drs.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_edw_hash.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_key.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_link.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_logging.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_misc.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_stats.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_storage.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_types_access_key.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_types_access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_util.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/test_views.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/testing_views.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.1.0b3/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/tools.py` & `dcicsnovault-8.0.1.0b3/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/typedsheets.py` & `dcicsnovault-8.0.1.0b3/snovault/typedsheets.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/typeinfo.py` & `dcicsnovault-8.0.1.0b3/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/types/access_key.py` & `dcicsnovault-8.0.1.0b3/snovault/types/access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/types/base.py` & `dcicsnovault-8.0.1.0b3/snovault/types/base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/types/filter_set.py` & `dcicsnovault-8.0.1.0b3/snovault/types/filter_set.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/types/user.py` & `dcicsnovault-8.0.1.0b3/snovault/types/user.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/upgrader.py` & `dcicsnovault-8.0.1.0b3/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/util.py` & `dcicsnovault-8.0.1.0b3/snovault/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1220,7 +1220,36 @@
     """ Helper function that builds a presigned URL. """
     s3_client = make_s3_client()
     return s3_client.generate_presigned_url(
         ClientMethod='get_object',
         Params=params,
         ExpiresIn=36 * 60 * 60
     )
+
+
+class SettingsKey:
+    APPLICATION_BUCKET_PREFIX = 'application_bucket_prefix'
+    BLOB_BUCKET = 'blob_bucket'
+    EB_APP_VERSION = 'eb_app_version'
+    ELASTICSEARCH_SERVER = 'elasticsearch.server'
+    ENCODED_VERSION = 'encoded_version'
+    FILE_UPLOAD_BUCKET = 'file_upload_bucket'
+    FILE_WFOUT_BUCKET = 'file_wfout_bucket'
+    FOURSIGHT_BUCKET_PREFIX = 'foursight_bucket_prefix'
+    IDENTITY = 'identity'
+    INDEXER = 'indexer'
+    INDEXER_NAMESPACE = 'indexer.namespace'
+    INDEX_SERVER = 'index_server'
+    LOAD_TEST_DATA = 'load_test_data'
+    METADATA_BUNDLES_BUCKET = 'metadata_bundles_bucket'
+    S3_ENCRYPT_KEY_ID = 's3_encrypt_key_id'
+    SNOVAULT_VERSION = 'snovault_version'
+    SQLALCHEMY_URL = 'sqlalchemy.url'
+    SYSTEM_BUCKET = 'system_bucket'
+    TIBANNA_CWLS_BUCKET = 'tibanna_cwls_bucket'
+    TIBANNA_OUTPUT_BUCKET = 'tibanna_output_bucket'
+    UTILS_VERSION = 'utils_version'
+
+
+class ExtraArgs:
+    SERVER_SIDE_ENCRYPTION = "ServerSideEncryption"
+    SSE_KMS_KEY_ID = "SSEKMSKeyId"
```

### Comparing `dcicsnovault-8.0.1.0b2/snovault/validation.py` & `dcicsnovault-8.0.1.0b3/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/snovault/validators.py` & `dcicsnovault-8.0.1.0b3/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b2/PKG-INFO` & `dcicsnovault-8.0.1.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.0.1.0b2
+Version: 8.0.1.0b3
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
```

