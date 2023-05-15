# Comparing `tmp/dcicsnovault-8.0.1.1b5.tar.gz` & `tmp/dcicsnovault-8.0.1.2b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.0.1.1b5.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.1.2b4.tar", max compression
```

## Comparing `dcicsnovault-8.0.1.1b5.tar` & `dcicsnovault-8.0.1.2b4.tar`

### file list

```diff
@@ -1,163 +1,165 @@
--rw-r--r--   0        0        0     1135 2023-05-03 20:04:05.642902 dcicsnovault-8.0.1.1b5/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-05-03 20:04:05.642902 dcicsnovault-8.0.1.1b5/README.rst
--rw-r--r--   0        0        0     5506 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/pyproject.toml
--rw-r--r--   0        0        0     4675 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/snovault/aggregated_items.py
--rw-r--r--   0        0        0     8799 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/snovault/app.py
--rw-r--r--   0        0        0      358 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/snovault/appdefs.py
--rw-r--r--   0        0        0    11879 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/snovault/attachment.py
--rw-r--r--   0        0        0    25502 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/snovault/authentication.py
--rw-r--r--   0        0        0     4467 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-05-03 20:04:05.646902 dcicsnovault-8.0.1.1b5/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6813 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     5764 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/list_db_tables.py
--rw-r--r--   0        0        0     6212 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2402 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     5155 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/prepare_template.py
--rw-r--r--   0        0        0     4350 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/custom_embed.py
--rw-r--r--   0        0        0     7228 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/jsonld_context.py
--rw-r--r--   0        0        0    30350 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/loadxl.py
--rw-r--r--   0        0        0     2425 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/memlimit.py
--rw-r--r--   0        0        0      895 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/nginx-dev.conf
--rw-r--r--   0        0        0     1165 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/parallel.py
--rw-r--r--   0        0        0      846 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/predicates.py
--rw-r--r--   0        0        0     2174 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/project.py
--rw-r--r--   0        0        0       95 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22128 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/resource_views.py
--rw-r--r--   0        0        0    23243 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/resources.py
--rw-r--r--   0        0        0     9867 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/root.py
--rw-r--r--   0        0        0      986 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/schema_formats.py
--rw-r--r--   0        0        0     3450 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/schema_graph.py
--rw-r--r--   0        0        0    14547 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-05-03 20:04:05.650902 dcicsnovault-8.0.1.1b5/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0    18744 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/search/search.py
--rw-r--r--   0        0        0    17901 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/search/search_utils.py
--rw-r--r--   0        0        0     4577 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/server_defaults.py
--rw-r--r--   0        0        0      522 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/settings.py
--rw-r--r--   0        0        0     1769 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/sqlalchemy_tools.py
--rw-r--r--   0        0        0     1498 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2210 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0        0 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/data/inserts/README.rst
--rw-r--r--   0        0        0        0 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/data/master-inserts/README.rst
--rw-r--r--   0        0        0     3086 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3173 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-05-03 20:04:05.654902 dcicsnovault-8.0.1.1b5/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     6782 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/test_types_access_key.py
--rw-r--r--   0        0        0     1291 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/test_util.py
--rw-r--r--   0        0        0    18612 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4578 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/types/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/types/access_key.py
--rw-r--r--   0        0        0    16288 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/types/filter_set.py
--rw-r--r--   0        0        0     5536 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/upgrader.py
--rw-r--r--   0        0        0    52799 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-05-03 20:04:05.658902 dcicsnovault-8.0.1.1b5/snovault/validators.py
--rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-05-15 19:34:11.093843 dcicsnovault-8.0.1.2b4/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-05-15 19:34:11.093843 dcicsnovault-8.0.1.2b4/README.rst
+-rw-r--r--   0        0        0     5276 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/pyproject.toml
+-rw-r--r--   0        0        0     4907 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/app.py
+-rw-r--r--   0        0        0      358 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/appdefs.py
+-rw-r--r--   0        0        0    11879 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/attachment.py
+-rw-r--r--   0        0        0    25327 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/authentication.py
+-rw-r--r--   0        0        0     4467 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6813 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     5806 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/list_db_tables.py
+-rw-r--r--   0        0        0     6212 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2402 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     5155 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/prepare_template.py
+-rw-r--r--   0        0        0     4350 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7271 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8249 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    30350 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/loadxl.py
+-rw-r--r--   0        0        0     2425 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/memlimit.py
+-rw-r--r--   0        0        0      895 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/nginx-dev.conf
+-rw-r--r--   0        0        0     1165 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/predicates.py
+-rw-r--r--   0        0        0     9251 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/project.py
+-rw-r--r--   0        0        0      259 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/project_defs.py
+-rw-r--r--   0        0        0       84 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/project_start.py
+-rw-r--r--   0        0        0       95 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22128 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/resource_views.py
+-rw-r--r--   0        0        0    24112 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/resources.py
+-rw-r--r--   0        0        0     9867 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/root.py
+-rw-r--r--   0        0        0      986 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schema_formats.py
+-rw-r--r--   0        0        0     3450 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schema_graph.py
+-rw-r--r--   0        0        0    14547 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4358 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schema_views.py
+-rw-r--r--   0        0        0     1855 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5098 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0    18744 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19600 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/search/search.py
+-rw-r--r--   0        0        0    17915 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     4409 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/server_defaults.py
+-rw-r--r--   0        0        0      522 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/settings.py
+-rw-r--r--   0        0        0     1769 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/sqlalchemy_tools.py
+-rw-r--r--   0        0        0     1498 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      697 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/data/inserts/README.rst
+-rw-r--r--   0        0        0        0 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/data/master-inserts/README.rst
+-rw-r--r--   0        0        0     3086 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3186 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     6782 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_types_access_key.py
+-rw-r--r--   0        0        0     1291 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    19246 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4620 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34107 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/access_key.py
+-rw-r--r--   0        0        0    16288 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/filter_set.py
+-rw-r--r--   0        0        0     5583 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/upgrader.py
+-rw-r--r--   0        0        0    52343 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/validators.py
+-rw-r--r--   0        0        0     9196 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.2b4/PKG-INFO
```

### Comparing `dcicsnovault-8.0.1.1b5/LICENSE.txt` & `dcicsnovault-8.0.1.2b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/README.rst` & `dcicsnovault-8.0.1.2b4/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/pyproject.toml` & `dcicsnovault-8.0.1.2b4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.0.1.1b5"  # to become 8.1.0
+version = "8.0.1.2b4"  # to become 8.1.0
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
@@ -33,16 +33,16 @@
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 aws_requests_auth = "^0.4.1"
-botocore = ">=1.19.119"  # no particular version required, but this speeds up search
-boto3 = ">=1.26.119"  # no particular version required, but this speeds up search
+boto3 = "^1.26.124"  # no particular version required, but this speeds up search
+botocore = "^1.19.124"  # no particular version required, but this speeds up search
 elasticsearch = "7.13.4"  # versions >= 7.14.0 lock out AWS ES
 elasticsearch_dsl = "^7.4.0"
 dcicutils = "^7.0.0"
 future = ">=0.15.2,<1"
 html5lib = ">=1.1"  # experimental, should be OK now that we're not using moto server
 humanfriendly = "^1.44.9"
 jsonschema_serialize_fork = "^2.1.1"
@@ -81,21 +81,18 @@
 WSGIProxy2 = "0.4.2"
 xlrd = "^1.0.0"
 "zope.deprecation" = "^4.4.0"
 "zope.interface" = ">=4.7.2,<6"
 "zope.sqlalchemy" = "1.6"
 
 [tool.poetry.dev-dependencies]
-botocore-stubs = ">=1.29.119"  # no particular version required, but this speeds up search
-boto3-stubs = ">=1.26.119"  # no particular version required, but this speeds up search
+boto3-stubs = "^1.26.124"  # no particular version required, but this speeds up search
+botocore-stubs = "^1.29.124"  # no particular version required, but this speeds up search
 coverage = ">=6.2"
 codacy-coverage = ">=1.3.11"
-# When we add coverage, this must be loaded manually in GA workflow for coverage because a dependency on 2to3
-# in its docopts dependency makes a problem for laoding it here in poetry. -kmp 25-Apr-2023
-# coveralls = ">=3.3.1"
 docutils = ">=0.16,<1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
 moto = "^4.0.3"
 PasteDeploy = "1.5.2"
 plaster = "1.0"
 plaster-pastedeploy = "0.6"
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/__init__.py` & `dcicsnovault-8.0.1.2b4/snovault/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,43 +17,43 @@
 from .schema_utils import load_schema  # noqa
 from .upgrader import upgrade_step  # noqa
 
 
 def includeme(config):
     config.include('pyramid_retry')
     config.include('pyramid_tm')
-    config.include('.authentication')
-    config.include('.util')
-    config.include('.drs')
-    config.include('.stats')
-    config.include('.batchupgrade')
-    config.include('.calculated')
-    config.include('.config')
-    config.include('.connection')
-    config.include('.custom_embed')
-    config.include('.embed')
-    config.include('.json_renderer')
-    config.include('.validation')
-    config.include('.predicates')
-    config.include('.invalidation')
-    config.include('.upgrader')
-    config.include('.aggregated_items')
-    config.include('.storage')
-    config.include('.typeinfo')
-    config.include('.types')
-    config.include('.resources')
-    config.include('.attachment')
-    config.include('.schema_graph')
-    config.include('.jsonld_context')
-    config.include('.schema_views')
-    config.include('.crud_views')
-    config.include('.indexing_views')
-    config.include('.resource_views')
-    config.include('.settings')
-    config.include('.server_defaults')
+    config.include('snovault.authentication')
+    config.include('snovault.util')
+    config.include('snovault.drs')
+    config.include('snovault.stats')
+    config.include('snovault.batchupgrade')
+    config.include('snovault.calculated')
+    config.include('snovault.config')
+    config.include('snovault.connection')
+    config.include('snovault.custom_embed')
+    config.include('snovault.embed')
+    config.include('snovault.json_renderer')
+    config.include('snovault.validation')
+    config.include('snovault.predicates')
+    config.include('snovault.invalidation')
+    config.include('snovault.upgrader')
+    config.include('snovault.aggregated_items')
+    config.include('snovault.storage')
+    config.include('snovault.typeinfo')
+    config.include('snovault.types')
+    config.include('snovault.resources')
+    config.include('snovault.attachment')
+    config.include('snovault.schema_graph')
+    config.include('snovault.jsonld_context')
+    config.include('snovault.schema_views')
+    config.include('snovault.crud_views')
+    config.include('snovault.indexing_views')
+    config.include('snovault.resource_views')
+    config.include('snovault.settings')
+    config.include('snovault.server_defaults')
 
 
 def main(global_config, **local_config):
     """
     This function returns a Pyramid WSGI application.
     """
     settings = global_config
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/aggregated_items.py` & `dcicsnovault-8.0.1.2b4/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/app.py` & `dcicsnovault-8.0.1.2b4/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/attachment.py` & `dcicsnovault-8.0.1.2b4/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/authentication.py` & `dcicsnovault-8.0.1.2b4/snovault/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 # envs where the back-end will accept automated user registration
 # TODO: move to dcicutils
 AUTO_REGISTRATION_ENVS = ['cgap-training']
 
 
 def includeme(config):
-    config.include('snovault.edw_hash')
+    config.include('.edw_hash')
     setting_prefix = 'passlib.'
     passlib_settings = {
         k[len(setting_prefix):]: v
         for k, v in config.registry.settings.items()
         if k.startswith(setting_prefix)
     }
     if not passlib_settings:
@@ -544,22 +544,20 @@
     }
 
     id_token = jwt.encode(
         jwt_contents,
         auth0_secret,
         algorithm=JWT_ENCODING_ALGORITHM
     )
-    # In PyJWT v1, the id_token was bytes. In v2, it's a string. This insulates us.
-    id_token_string = id_token.decode('utf-8') if isinstance(id_token, bytes) else id_token
 
     is_https = request.scheme == "https"
 
     request.response.set_cookie(
         "jwtToken",
-        value=id_token_string,
+        value=id_token.decode('utf-8'),
         domain=request.domain,
         path="/",
         httponly=True,
         samesite="strict",
         overwrite=True,
         secure=is_https
     )
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/authorization.py` & `dcicsnovault-8.0.1.2b4/snovault/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/batchupgrade.py` & `dcicsnovault-8.0.1.2b4/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/cache.py` & `dcicsnovault-8.0.1.2b4/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/calculated.py` & `dcicsnovault-8.0.1.2b4/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/clear_db_es_contents.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/create_mapping_on_deploy.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/create_mapping_on_deploy.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/list_db_tables.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/list_db_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # from snovault.storage import Base
 # from snovault.elasticsearch.create_mapping import run as run_create_mapping
 # from sqlalchemy import MetaData
 from typing import Optional, List
 # from zope.sqlalchemy import mark_changed
 from .. import configure_dbsession
 from ..sqlalchemy_tools import PyramidAppManager
-from ..project import PROJECT_NAME
+from ..project import app_project
 
 
 logger = structlog.getLogger(__name__)
 
 
 EPILOG = __doc__
 
@@ -111,19 +111,20 @@
     app_name = args.app_name
     config_uri = args.config_uri
     only_envs = args.only_envs
     allow_prod = args.allow_prod
     log = args.log
 
     logging.basicConfig()
+    project = app_project(initialize=True)
     # Loading app will have configured from config file. Reconfigure here:
     if log:
-        logging.getLogger(PROJECT_NAME).setLevel(logging.DEBUG)
+        logging.getLogger(project.NAME).setLevel(logging.DEBUG)
     else:
-        logging.getLogger(PROJECT_NAME).setLevel(logging.ERROR)
+        logging.getLogger(project.NAME).setLevel(logging.ERROR)
 
     if confirm is None:
         confirm = False   # not only_envs  # If only_envs is supplied, we have better protection so don't need to confirm
 
     # get the pyramids app
     app = get_app(config_uri, app_name)
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/load_access_keys.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/load_access_keys.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/load_data.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/load_data_by_type.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/load_data_by_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/prepare_template.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/prepare_template.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/profile.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/purge_item_type.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/purge_item_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/run_upgrader_on_inserts.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/run_upgrader_on_inserts.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/update_inserts_from_server.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/update_inserts_from_server.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.1.2b4/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/config.py` & `dcicsnovault-8.0.1.2b4/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/connection.py` & `dcicsnovault-8.0.1.2b4/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/crud_views.py` & `dcicsnovault-8.0.1.2b4/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/custom_embed.py` & `dcicsnovault-8.0.1.2b4/snovault/custom_embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/dev_servers.py` & `dcicsnovault-8.0.1.2b4/snovault/dev_servers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import subprocess
 import sys
 
 from dcicutils.misc_utils import PRINT
 from pyramid.paster import get_app, get_appsettings
 from pyramid.path import DottedNameResolver
 from .elasticsearch import create_mapping
-from .project import PROJECT_NAME, project_filename
+from .project import app_project, project_filename
 from .tests import elasticsearch_fixture, postgresql_fixture
 
 
 EPILOG = __doc__
 
 logger = logging.getLogger(__name__)
 
@@ -110,17 +110,19 @@
     run(app_name=args.app_name, config_uri=args.config_uri, datadir=args.datadir,
         # Ingestion is disabled. snovault has no such concept. -kmp 17-Feb-2023
         clear=args.clear, init=args.init, load=args.load, ingest=False)  # ingest=not args.no_ingest
 
 
 def run(app_name, config_uri, datadir, clear=False, init=False, load=False, ingest=True):
 
+    project = app_project(initialize=True)
+
     logging.basicConfig(format='')
     # Loading app will have configured from config file. Reconfigure here:
-    logging.getLogger(PROJECT_NAME).setLevel(logging.INFO)
+    logging.getLogger(project.NAME).setLevel(logging.INFO)
 
     # get the config and see if we want to connect to non-local servers
     # TODO: This variable seems to not get used? -kmp 25-Jul-2020
     config = get_appsettings(config_uri, app_name)
 
     datadir = os.path.abspath(datadir)
     pgdata = os.path.join(datadir, 'pgdata')
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/drs.py` & `dcicsnovault-8.0.1.2b4/snovault/drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/edw_hash.py` & `dcicsnovault-8.0.1.2b4/snovault/edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/embed.py` & `dcicsnovault-8.0.1.2b4/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/etag.py` & `dcicsnovault-8.0.1.2b4/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/indexing_views.py` & `dcicsnovault-8.0.1.2b4/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/interfaces.py` & `dcicsnovault-8.0.1.2b4/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/invalidation.py` & `dcicsnovault-8.0.1.2b4/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/json_renderer.py` & `dcicsnovault-8.0.1.2b4/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/jsongraph.py` & `dcicsnovault-8.0.1.2b4/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/jsonld_context.py` & `dcicsnovault-8.0.1.2b4/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/loadxl.py` & `dcicsnovault-8.0.1.2b4/snovault/loadxl.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/memlimit.py` & `dcicsnovault-8.0.1.2b4/snovault/memlimit.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/nginx-dev.conf` & `dcicsnovault-8.0.1.2b4/snovault/nginx-dev.conf`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/parallel.py` & `dcicsnovault-8.0.1.2b4/snovault/parallel.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/predicates.py` & `dcicsnovault-8.0.1.2b4/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.1.2b4/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/renderers.py` & `dcicsnovault-8.0.1.2b4/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/resource_views.py` & `dcicsnovault-8.0.1.2b4/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/resources.py` & `dcicsnovault-8.0.1.2b4/snovault/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from .util import add_default_embeds, IndexSettings
 
 logger = logging.getLogger(__name__)
 
 
 def includeme(config):
     config.include(auth0_config)
+    config.include(recaptcha_config)
     config.scan(__name__)
 
 
 def acl_from_settings(settings):
     # XXX Unsure if any of the demo instance still need this
     acl = []
     for k, v in settings.items():
@@ -191,14 +192,39 @@
             callback = f'{request.host_url}/callback'
             response_dict['auth0Options']['auth']['redirectUrl'] = callback
         return response_dict
 
     config.add_view(auth0_config_view, route_name='auth0-config')
 
 
+def recaptcha_config(config):
+    """ Route that exposes the recaptcha site key """
+    config.add_route(
+        'recaptcha-config',
+        '/recaptcha_config'
+    )
+    recaptcha_config_values = {  # determines which values are echoed
+        'g.recaptcha.key': 'RecaptchaKey',
+    }
+
+    def recaptcha_config_view(request):
+        response = request.response
+        response.content_type = 'application/json; charset=utf-8'
+        response_dict = {
+            'title': 'Recaptcha Config',
+        }
+        settings = config.registry.settings
+        for config_key, result_key in recaptcha_config_values.items():
+            if config_key in settings:
+                response_dict[result_key] = settings[config_key]
+        return response_dict
+
+    config.add_view(recaptcha_config_view, route_name='recaptcha-config')
+
+
 class AbstractCollection(Resource, Mapping):
     """
     Collection for a certain type of resource that stores the following info:
     - registry (pyramid registry)
     - type_info (TypeInfo for a certain item type, see snovault.typeinfo.py)
     - __acl__
     - uniqueKey for the collection (e.g. item_name:key)
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/root.py` & `dcicsnovault-8.0.1.2b4/snovault/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/schema_formats.py` & `dcicsnovault-8.0.1.2b4/snovault/schema_formats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/schema_graph.py` & `dcicsnovault-8.0.1.2b4/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/schema_utils.py` & `dcicsnovault-8.0.1.2b4/snovault/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/schema_views.py` & `dcicsnovault-8.0.1.2b4/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/schemas/access_key.json` & `dcicsnovault-8.0.1.2b4/snovault/schemas/access_key.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/schemas/filter_set.json` & `dcicsnovault-8.0.1.2b4/snovault/schemas/filter_set.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/schemas/mixins.json` & `dcicsnovault-8.0.1.2b4/snovault/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/schemas/user.json` & `dcicsnovault-8.0.1.2b4/snovault/schemas/user.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/search/compound_search.py` & `dcicsnovault-8.0.1.2b4/snovault/search/compound_search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/search/lucene_builder.py` & `dcicsnovault-8.0.1.2b4/snovault/search/lucene_builder.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/search/search.py` & `dcicsnovault-8.0.1.2b4/snovault/search/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/search/search_utils.py` & `dcicsnovault-8.0.1.2b4/snovault/search/search_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from pyramid.httpexceptions import HTTPBadRequest
 from snovault import TYPES
 from snovault.util import crawl_schema, find_collection_subtypes
 from snovault.embed import make_subrequest
 from snovault.elasticsearch.indexer_utils import get_namespaced_index
 from snovault.elasticsearch.create_mapping import determine_if_is_date_field
-from ..util import deduplicate_list
+from dcicutils.misc_utils import deduplicate_list
 
 
 log = structlog.getLogger(__name__)
 
 # Constants
 
 # from now on, use these constants when referring to elastic search
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/server_defaults.py` & `dcicsnovault-8.0.1.2b4/snovault/server_defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import random
 import uuid
 
-from datetime import datetime
+from dcicutils.misc_utils import utc_now_str
 from jsonschema_serialize_fork import NO_DEFAULT
 from pyramid.path import DottedNameResolver
 from pyramid.threadlocal import get_current_request
 from snovault.schema_utils import server_default
 from snovault import COLLECTIONS  # , ROOT
 from string import digits  # , ascii_uppercase
-from .project import PROJECT_ACCESSION_PREFIX
 
 
 ACCESSION_FACTORY = __name__ + ':accession_factory'
-ACCESSION_PREFIX = PROJECT_ACCESSION_PREFIX
+ACCESSION_PREFIX = 'SNO'  # Can be changed downstream
 ACCESSION_TEST_PREFIX = 'TST'
 
 
 def includeme(config):
     accession_factory = config.registry.settings.get('accession_factory')
     if accession_factory:
         factory = DottedNameResolver().resolve(accession_factory)
@@ -43,19 +42,14 @@
 
 
 @server_default
 def now(instance, subschema):  # args required by jsonschema-serialize-fork
     return utc_now_str()
 
 
-def utc_now_str():
-    # from jsonschema_serialize_fork date-time format requires a timezone
-    return datetime.utcnow().isoformat() + '+00:00'
-
-
 @server_default
 def uuid4(instance, subschema):
     return str(uuid.uuid4())
 
 
 @server_default
 def accession(instance, subschema):
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/settings.py` & `dcicsnovault-8.0.1.2b4/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/sqlalchemy_tools.py` & `dcicsnovault-8.0.1.2b4/snovault/sqlalchemy_tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/standalone_dev.py` & `dcicsnovault-8.0.1.2b4/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/stats.py` & `dcicsnovault-8.0.1.2b4/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/storage.py` & `dcicsnovault-8.0.1.2b4/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/test_schemas/mixins.json` & `dcicsnovault-8.0.1.2b4/snovault/test_schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/conftest.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/root.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_clear_db_es_contents.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_drs.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_drs.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from ..drs import REQUIRED_FIELDS
 
 
 class TestDRSAPI:
     """ Class for testing the DRS implementation - uses TestingDownload as it implements
         the @@download scheme
     """
+    BASE_URL = 'http://localhost:80/'
 
     def test_drs_get_object(self, testapp, testing_download):  # noQA fixture
         """ Tests basic structure about a drs object """
         res = testapp.get(testing_download)
         drs_object_uri = res.json['uuid']
         drs_object_1 = testapp.get(f'/ga4gh/drs/v1/objects/{drs_object_uri}').json
         for key in REQUIRED_FIELDS:
             assert key in drs_object_1
         assert drs_object_1['self_uri'] == f'drs://localhost:80/ga4gh/drs/v1/objects/{drs_object_uri}'
         assert (drs_object_1['access_methods'][0]['access_url']['url']
-                == f'http://localhost:80/{drs_object_uri}/@@download')
+                == f'{self.BASE_URL}{drs_object_uri}/@@download')
 
         # failure cases
         testapp.get(f'/ga4gh/drs/v1/objects/not_a_uri', status=404)
 
         # @@drs case
         drs_object_2 = testapp.get(f'/{drs_object_uri}/@@drs')
         for key in REQUIRED_FIELDS:
@@ -31,33 +32,33 @@
         """ Tests extracting URL through ga4gh pathway """
         res = testapp.get(testing_download)
         drs_object_uri = res.json['uuid']
 
         # standard URI with meaningful access_id, discarded
         drs_object_download = testapp.get(f'/ga4gh/drs/v1/objects/{drs_object_uri}/access/https').json
         assert drs_object_download == {
-            'url': f'http://localhost:80/{drs_object_uri}/@@download'
+            'url': f'{self.BASE_URL}{drs_object_uri}/@@download'
         }
 
         # /access/ method
         drs_object_download = testapp.get(f'/ga4gh/drs/v1/objects/{drs_object_uri}/access/').json
         assert drs_object_download == {
-            'url': f'http://localhost:80/{drs_object_uri}/@@download'
+            'url': f'{self.BASE_URL}{drs_object_uri}/@@download'
         }
 
         # standard URI with nonsense access id, still discarded
         drs_object_download = testapp.get(f'/ga4gh/drs/v1/objects/{drs_object_uri}/access/blah').json
         assert drs_object_download == {
-            'url': f'http://localhost:80/{drs_object_uri}/@@download'
+            'url': f'{self.BASE_URL}{drs_object_uri}/@@download'
         }
 
         # /access method
         drs_object_download = testapp.get(f'/ga4gh/drs/v1/objects/{drs_object_uri}/access').json
         assert drs_object_download == {
-            'url': f'http://localhost:80/{drs_object_uri}/@@download'
+            'url': f'{self.BASE_URL}{drs_object_uri}/@@download'
         }
 
     def test_drs_get_object_failure(self, testapp, testing_download):  # noQA fixture
         """ Tests a bunch of bunk URLs """
         res = testapp.get(testing_download)
         drs_object_uri = res.json['uuid']
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_edw_hash.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_key.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_link.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_logging.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_misc.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_stats.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_storage.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_types_access_key.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_types_access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_util.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/test_views.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/test_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -429,7 +429,23 @@
     """ Tests that acquiring auth0 config gives the expected values from settings for admins. """
     _test_auth_config(testapp, registry)
 
 
 def test_auth0_config_anon(anontestapp, registry):
     """ Tests that acquiring auth0 config gives the expected values from settings for anonymous users. """
     _test_auth_config(anontestapp, registry)
+
+
+def _test_recaptcha_config(testapp, registry):
+    cfg = testapp.get('/recaptcha_config').json
+    assert cfg['title'] == 'Recaptcha Config'
+    assert cfg['RecaptchaKey'] == registry.settings['g.recaptcha.key']
+
+
+def test_recaptcha_config_admin(testapp, registry):
+    """ Tests that acquiring recaptcha config gives the expected values from settings for admins. """
+    _test_recaptcha_config(testapp, registry)
+
+
+def test_recaptcha_config_anon(anontestapp, registry):
+    """ Tests that acquiring recaptcha config gives the expected values from settings for anonymous users. """
+    _test_recaptcha_config(anontestapp, registry)
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/testappfixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     'testing': True,
     'mpindexer': False,
     'pyramid.debug_authorization': True,
     'postgresql.statement_timeout': 20,
     'retry.attempts': 3,
     'production': True,
     'structlog.dir': '/tmp/',
+    'g.recaptcha.key': 'dummy-recaptcha',
     'auth0.client': 'dummy-client',
     'auth0.domain': 'dummy.domain',
     'auth0.options': {
         'auth': {
             'sso': False,
             'redirect': False,
             'responseType': 'token',
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/testing_views.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.1.2b4/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/tools.py` & `dcicsnovault-8.0.1.2b4/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/typedsheets.py` & `dcicsnovault-8.0.1.2b4/snovault/typedsheets.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/typeinfo.py` & `dcicsnovault-8.0.1.2b4/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/types/access_key.py` & `dcicsnovault-8.0.1.2b4/snovault/types/access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/types/base.py` & `dcicsnovault-8.0.1.2b4/snovault/types/base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/types/filter_set.py` & `dcicsnovault-8.0.1.2b4/snovault/types/filter_set.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/types/user.py` & `dcicsnovault-8.0.1.2b4/snovault/types/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 ] + ONLY_ADMIN_VIEW_USER_DETAILS_ACL
 
 
 @collection(
     name='users',
     unique_key='user:email',
     properties={
-        'title': 'CGAP Users',
-        'description': 'Listing of current CGAP users',
+        'title': 'Users',
+        'description': f'Listing of current users',
     },
 )
 class User(Item):
     """The user class."""
 
     item_type = 'user'
     schema = load_schema('snovault:schemas/user.json')
@@ -100,22 +100,25 @@
 
     def __ac_local_roles__(self):
         """return the owner user."""
         owner = 'userid.%s' % self.uuid
         return {owner: 'role.owner'}
 
 
+USER_PAGE_VIEW_ATTRIBUTES = ['@id', '@type', 'uuid', 'title', 'display_title']
+
+
 @view_config(context=User, permission='view', request_method='GET', name='page')
 @debug_log
 def user_page_view(context, request):
     """smth."""
     properties = item_view_page(context, request)
     if not request.has_permission('view_details'):
         filtered = {}
-        for key in ['@id', '@type', 'uuid', 'title', 'display_title']:
+        for key in USER_PAGE_VIEW_ATTRIBUTES:
             try:
                 filtered[key] = properties[key]
             except KeyError:
                 pass
         return filtered
     return properties
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/upgrader.py` & `dcicsnovault-8.0.1.2b4/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/util.py` & `dcicsnovault-8.0.1.2b4/snovault/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,28 +136,14 @@
         log.error('Got dictionary KeyError with %s and %s' % (dictionary, key))
         return None
         # raise DictionaryKeyError(dictionary=dictionary, key=key)  this causes MPIndexer exception - will 3/10/2020
     else:
         return dictionary[key]
 
 
-def deduplicate_list(lst):
-    """ De-duplicates the given list by converting it to a set then back to a list.
-
-    NOTES:
-    * The list must contain 'hashable' type elements that can be used in sets.
-    * The result list might not be ordered the same as the input list.
-    * This will also take tuples as input, though the result will be a list.
-
-    :param lst: list to de-duplicate
-    :return: de-duplicated list
-    """
-    return list(set(lst))
-
-
 _skip_fields = ['@type', 'principals_allowed']  # globally accessible if need be in the future
 
 
 # TODO: This is a priority candidate for unit testing. -kmp 27-Jul-2020
 def filter_embedded(embedded, effective_principals):
     """
     Filter the embedded items by principals_allowed, replacing them with
```

### Comparing `dcicsnovault-8.0.1.1b5/snovault/validation.py` & `dcicsnovault-8.0.1.2b4/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/snovault/validators.py` & `dcicsnovault-8.0.1.2b4/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.1b5/PKG-INFO` & `dcicsnovault-8.0.1.2b4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.0.1.1b5
+Version: 8.0.1.2b4
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
@@ -21,16 +21,16 @@
 Requires-Dist: PyBrowserID (>=0.10.0,<1)
 Requires-Dist: SPARQLWrapper (>=1.8.5,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: WSGIProxy2 (==0.4.2)
 Requires-Dist: WebOb (>=1.8.7,<2.0.0)
 Requires-Dist: WebTest (>=2.0.35,<3.0.0)
 Requires-Dist: aws_requests_auth (>=0.4.1,<0.5.0)
-Requires-Dist: boto3 (>=1.26.119)
-Requires-Dist: botocore (>=1.19.119)
+Requires-Dist: boto3 (>=1.26.124,<2.0.0)
+Requires-Dist: botocore (>=1.19.124,<2.0.0)
 Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch_dsl (>=7.4.0,<8.0.0)
 Requires-Dist: future (>=0.15.2,<1)
 Requires-Dist: html5lib (>=1.1)
 Requires-Dist: humanfriendly (>=1.44.9,<2.0.0)
 Requires-Dist: jsonschema_serialize_fork (>=2.1.1,<3.0.0)
```

