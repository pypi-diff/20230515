# Comparing `tmp/mitzu-0.6.0rc8.tar.gz` & `tmp/mitzu-0.6.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.0rc8.tar", max compression
+gzip compressed data, was "mitzu-0.6.0rc9.tar", max compression
```

## Comparing `mitzu-0.6.0rc8.tar` & `mitzu-0.6.0rc9.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     1082 2023-05-12 18:27:50.573348 mitzu-0.6.0rc8/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-05-12 18:27:50.573348 mitzu-0.6.0rc8/README.md
--rw-r--r--   0        0        0     6148 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/.DS_Store
--rw-r--r--   0        0        0      865 2023-05-12 18:28:50.717186 mitzu-0.6.0rc8/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1918 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5148 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     3390 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/bigquery_adapter.py
--rw-r--r--   0        0        0     6026 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2533 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3733 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3298 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39624 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     4963 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6614 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/helper.py
--rw-r--r--   0        0        0    53963 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     3306 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11926 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7022 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1278 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-12 18:27:50.997354 mitzu-0.6.0rc8/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    20802 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/bigquery.png
--rw-r--r--   0        0        0    10321 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    13445 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1594 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2920 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1462 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3088 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8375 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/model.py
--rw-r--r--   0        0        0      408 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5435 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    16230 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4527 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    20885 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9787 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/dashboards_page.py
--rw-r--r--   0        0        0    14654 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:51.001355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5724 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    21781 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0     9604 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1347 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     4107 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5027 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1387 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10191 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11953 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9629 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    36159 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5155 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3185 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5302 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     2105 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     4719 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    21490 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25781 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     4899 2023-05-12 18:27:51.005355 mitzu-0.6.0rc8/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     3055 2023-05-12 18:28:50.717186 mitzu-0.6.0rc8/pyproject.toml
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 mitzu-0.6.0rc8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-15 19:57:09.432988 mitzu-0.6.0rc9/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-05-15 19:57:09.432988 mitzu-0.6.0rc9/README.md
+-rw-r--r--   0        0        0     6148 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/.DS_Store
+-rw-r--r--   0        0        0      865 2023-05-15 19:58:06.717343 mitzu-0.6.0rc9/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1918 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5148 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     3390 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/bigquery_adapter.py
+-rw-r--r--   0        0        0     6026 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2533 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     3733 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3298 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39624 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     4963 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6614 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/helper.py
+-rw-r--r--   0        0        0    53963 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     3306 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11926 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7022 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1278 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    20802 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/bigquery.png
+-rw-r--r--   0        0        0    10321 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    13716 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1594 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2920 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1462 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3088 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8375 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      408 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5435 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    16230 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4527 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    20885 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9787 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards_page.py
+-rw-r--r--   0        0        0    14654 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5724 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    21781 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0     9604 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1347 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     4107 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5027 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1387 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10191 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11953 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9629 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    36159 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5155 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3185 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5302 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     4719 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    23896 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25781 2023-05-15 19:57:09.836990 mitzu-0.6.0rc9/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4744 2023-05-15 19:57:09.836990 mitzu-0.6.0rc9/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     3055 2023-05-15 19:58:06.717343 mitzu-0.6.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 mitzu-0.6.0rc9/PKG-INFO
```

### Comparing `mitzu-0.6.0rc8/LICENSE.txt` & `mitzu-0.6.0rc9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/README.md` & `mitzu-0.6.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/.DS_Store` & `mitzu-0.6.0rc9/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/__init__.py` & `mitzu-0.6.0rc9/mitzu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.0-rc.8"
+__version__ = "0.6.0-rc.9"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.0rc9/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/bigquery_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/file_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/helper.py` & `mitzu-0.6.0rc9/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.0rc9/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/helper.py` & `mitzu-0.6.0rc9/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/model.py` & `mitzu-0.6.0rc9/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/notebook/model_loader.py` & `mitzu-0.6.0rc9/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/project_discovery.py` & `mitzu-0.6.0rc9/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/project_serialization.py` & `mitzu-0.6.0rc9/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/samples/__init__.py` & `mitzu-0.6.0rc9/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/samples/data_ingestion.py` & `mitzu-0.6.0rc9/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.0rc9/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/serialization.py` & `mitzu-0.6.0rc9/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/visualization/charts.py` & `mitzu-0.6.0rc9/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/visualization/common.py` & `mitzu-0.6.0rc9/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/visualization/labels.py` & `mitzu-0.6.0rc9/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/visualization/plot.py` & `mitzu-0.6.0rc9/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/visualization/titles.py` & `mitzu-0.6.0rc9/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/visualization/tooltips.py` & `mitzu-0.6.0rc9/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/visualization/transform_conv.py` & `mitzu-0.6.0rc9/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/visualization/transform_retention.py` & `mitzu-0.6.0rc9/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/.DS_Store` & `mitzu-0.6.0rc9/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.0rc9/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.0rc9/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/logo.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.0rc9/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/bigquery.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/bigquery.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.0rc9/mitzu/webapp/auth/authorizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 class AuthConfig:
     user_service: U.UserService
 
     token_cookie_name: str = "auth-token"
     redirect_cookie_name: str = "redirect-to"
 
     session_timeout: int = 7 * 24 * 60 * 60
+    token_refresh_threshold: int = 60
     token_signing_key: str = configs.AUTH_JWT_SECRET
 
     oauth: Optional[OAuthConfig] = None
     token_validator: Optional[TokenValidator] = None
 
 
 @dataclass(frozen=True)
@@ -106,14 +107,15 @@
     )
     _ignore_token_refresh_prefixes: List[str] = field(
         default_factory=lambda: [
             P.UNAUTHORIZED_URL,
             P.SIGN_OUT_URL,
             P.HEALTHCHECK_PATH,
             "/assets/",
+            "/_dash-component-suites/",
         ]
     )
 
     @classmethod
     def create(cls, config: AuthConfig) -> OAuthAuthorizer:
         return OAuthAuthorizer(
             _config=config,
@@ -301,14 +303,21 @@
             if request.path.startswith(prefix):
                 return resp
 
         auth_token = flask.request.cookies.get(self._config.token_cookie_name)
         if auth_token is not None:
             token_claims = self._validate_token(auth_token)
             if token_claims is not None:
+
+                if (
+                    token_claims["iat"]
+                    >= int(time.time()) - self._config.token_refresh_threshold
+                ):
+                    return resp
+
                 new_token = self._generate_new_token_with_claims(token_claims)
                 self.set_cookie(resp, self._config.token_cookie_name, new_token)
         return resp
 
     def is_request_authorized(self, request: flask.Request) -> bool:
         auth_token = request.cookies.get(self._config.token_cookie_name)
         return auth_token is not None and self._validate_token(auth_token) is not None
```

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.0rc9/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.0rc9/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/auth/google.py` & `mitzu-0.6.0rc9/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/cache.py` & `mitzu-0.6.0rc9/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.0rc9/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/configs.py` & `mitzu-0.6.0rc9/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/dependencies.py` & `mitzu-0.6.0rc9/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/helper.py` & `mitzu-0.6.0rc9/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/model.py` & `mitzu-0.6.0rc9/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/offcanvas.py` & `mitzu-0.6.0rc9/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/dashboards_page.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/home.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/login.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/paths.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/pages/users.py` & `mitzu-0.6.0rc9/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/service/events_service.py` & `mitzu-0.6.0rc9/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.0rc9/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.0rc9/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.0rc9/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/service/user_service.py` & `mitzu-0.6.0rc9/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/storage.py` & `mitzu-0.6.0rc9/mitzu/webapp/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         self,
         connection_string: str = "sqlite://?check_same_thread=False",
     ) -> None:
         self.__pid = None
         self.__is_sqlite = connection_string.startswith("sqlite")
         self.__connection_string = connection_string
 
-    def __create_new_db_session(self) -> Session:
+    def _new_db_session(self) -> Session:
+        self.__create_engine_when_needed()
         session = SA.orm.sessionmaker(bind=self._engine)()
         if self.__is_sqlite:
             session.execute("PRAGMA foreign_keys = ON;")
             session.commit()
         return session
 
     def __create_engine_when_needed(self):
@@ -97,27 +98,14 @@
             LOGGER.debug(
                 f"Engine needs to be recreated, previous instance created by pid: {self.__pid}, current pid: {pid}"
             )
             self._engine = SA.create_engine(
                 self.__connection_string, pool_pre_ping=True
             )
             self.__pid = pid
-            if flask.has_app_context() and "request_session_cache" in flask.g:
-                flask.g.request_session_cache = self.__create_new_db_session()
-
-    @property
-    def _session(self) -> Session:
-        self.__create_engine_when_needed()
-        if flask.has_app_context():
-            if "request_session_cache" not in flask.g:
-                flask.g.request_session_cache = self.__create_new_db_session()
-
-            return flask.g.request_session_cache
-        else:
-            return self.__create_new_db_session()
 
     def init_db_schema(self):
         LOGGER.debug("Initializing the database schema")
         self.__create_engine_when_needed()
         tables = []
         for storage_record in [
             SM.UserStorageRecord,
@@ -132,222 +120,239 @@
             SM.DashboardMetricStorageRecord,
         ]:
             tables.append(SM.Base.metadata.tables[storage_record.__tablename__])
 
         SM.Base.metadata.create_all(self._engine, tables=tables)
 
     def set_project(self, project_id: str, project: M.Project):
-        self.set_connection(project.connection.id, project.connection)
-        self.set_discovery_settings(
-            project.discovery_settings.id, project.discovery_settings
-        )
-        self.set_webapp_settings(project.webapp_settings.id, project.webapp_settings)
-
-        current_edt_ids = [edt.id for edt in project.event_data_tables]
-        self._remove_unreferenced_event_data_tables(project.id, current_edt_ids)
-
-        record = (
-            self._session.query(SM.ProjectStorageRecord)
-            .filter(SM.ProjectStorageRecord.project_id == project_id)
-            .first()
-        )
+        with self._new_db_session() as session:
+            self._set_connection(project.connection.id, project.connection, session)
+            self._set_discovery_settings(
+                project.discovery_settings.id, project.discovery_settings, session
+            )
+            self._set_webapp_settings(
+                project.webapp_settings.id, project.webapp_settings, session
+            )
 
-        if record is None:
-            self._session.add(SM.ProjectStorageRecord.from_model_instance(project))
-        else:
-            record.update(project)
+            current_edt_ids = [edt.id for edt in project.event_data_tables]
+            self._remove_unreferenced_event_data_tables(
+                project.id, current_edt_ids, session
+            )
 
-        for edt in project.event_data_tables:
-            self._set_event_data_table(project.id, edt)
+            record = (
+                session.query(SM.ProjectStorageRecord)
+                .filter(SM.ProjectStorageRecord.project_id == project_id)
+                .first()
+            )
 
-        discovered_project = project._discovered_project.get_value()
-        if discovered_project:
-            self.populate_discovered_project(discovered_project)
-            for edt, vals in discovered_project.definitions.items():
-                self.set_event_data_table_definition(edt, vals)
+            if record is None:
+                session.add(SM.ProjectStorageRecord.from_model_instance(project))
+            else:
+                record.update(project)
+
+            for edt in project.event_data_tables:
+                self._set_event_data_table(project.id, edt, session)
+
+            discovered_project = project._discovered_project.get_value()
+            if discovered_project:
+                self._populate_discovered_project(discovered_project, session)
+                for edt, vals in discovered_project.definitions.items():
+                    self._set_event_data_table_definition(edt, vals, session)
 
-        self._session.commit()
+            session.commit()
 
     def project_exists(self, project_id: str) -> bool:
-        return (
-            self._session.query(SM.ProjectStorageRecord)
-            .filter(SM.ProjectStorageRecord.project_id == project_id)
-            .first()
-        ) is not None
+        with self._new_db_session() as session:
+            return (
+                session.query(SM.ProjectStorageRecord)
+                .filter(SM.ProjectStorageRecord.project_id == project_id)
+                .first()
+            ) is not None
 
     def get_project(self, project_id: str) -> M.Project:
-        record = (
-            self._session.query(SM.ProjectStorageRecord)
-            .filter(SM.ProjectStorageRecord.project_id == project_id)
-            .first()
-        )
-        if record is None:
-            raise ValueError(f"Project not found with project_id={project_id}")
-
-        connection = self.get_connection(record.connection_id)
-        discovery_settings = self.get_discovery_settings(record.discovery_settings_id)
-        webapp_settings = self.get_webapp_settings(record.webapp_settings_id)
-        edts = self._get_event_data_tables_for_project(record.project_id)
-        project = record.as_model_instance(
-            connection, edts, discovery_settings, webapp_settings
-        )
-
-        discovered_definitions: Dict[
-            M.EventDataTable, Dict[str, M.Reference[M.EventDef]]
-        ] = {}
-        for edt in edts:
-            discovered_fields = (
-                self._session.query(
-                    SM.EventDefStorageRecord.event_name, SM.EventDefStorageRecord.id
-                )
-                .filter(SM.EventDefStorageRecord.event_data_table_id == edt.id)
-                .all()
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.ProjectStorageRecord)
+                .filter(SM.ProjectStorageRecord.project_id == project_id)
+                .first()
             )
-            definitions: Dict[str, M.Reference[M.EventDef]] = {}
-            for field in discovered_fields:
-                definitions[field.event_name] = StorageEventDefReference(
-                    id=field.id, value=None, event_data_table=edt
-                )
-            if len(definitions) > 0:
-                discovered_definitions[edt] = definitions
+            if record is None:
+                raise ValueError(f"Project not found with project_id={project_id}")
 
-        if len(discovered_definitions) > 0:
-            # it may seems a bit od but the constructor will put the reference of the discovered project into the project
-            M.DiscoveredProject(discovered_definitions, project)
-        return project
+            connection = self._get_connection(record.connection_id, session)
+            discovery_settings = self._get_discovery_settings(
+                record.discovery_settings_id, session
+            )
+            webapp_settings = self._get_webapp_settings(
+                record.webapp_settings_id, session
+            )
+            edts = self._get_event_data_tables_for_project(record.project_id, session)
+            project = record.as_model_instance(
+                connection, edts, discovery_settings, webapp_settings
+            )
+
+            discovered_definitions: Dict[
+                M.EventDataTable, Dict[str, M.Reference[M.EventDef]]
+            ] = {}
+            for edt in edts:
+                discovered_fields = (
+                    session.query(
+                        SM.EventDefStorageRecord.event_name, SM.EventDefStorageRecord.id
+                    )
+                    .filter(SM.EventDefStorageRecord.event_data_table_id == edt.id)
+                    .all()
+                )
+                definitions: Dict[str, M.Reference[M.EventDef]] = {}
+                for field in discovered_fields:
+                    definitions[field.event_name] = StorageEventDefReference(
+                        id=field.id, value=None, event_data_table=edt
+                    )
+                if len(definitions) > 0:
+                    discovered_definitions[edt] = definitions
+
+            if len(discovered_definitions) > 0:
+                # it may seems a bit od but the constructor will put the reference of the discovered project into the project
+                M.DiscoveredProject(discovered_definitions, project)
+            return project
 
     def delete_project(self, project_id: str):
-        session = self._session
-        record = (
-            session.query(SM.ProjectStorageRecord)
-            .filter(SM.ProjectStorageRecord.project_id == project_id)
-            .first()
-        )
-        if record is not None:
-            session.delete(record)
-            session.commit()
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.ProjectStorageRecord)
+                .filter(SM.ProjectStorageRecord.project_id == project_id)
+                .first()
+            )
+            if record is not None:
+                session.delete(record)
+                session.commit()
 
-    def _set_event_data_table(self, project_id: str, edt: M.EventDataTable):
+    def _set_event_data_table(
+        self, project_id: str, edt: M.EventDataTable, session: SA.orm.Session
+    ):
         if edt.discovery_settings:
-            self.set_discovery_settings(
-                edt.discovery_settings.id, edt.discovery_settings
+            self._set_discovery_settings(
+                edt.discovery_settings.id, edt.discovery_settings, session
             )
         record = (
-            self._session.query(SM.EventDataTableStorageRecord)
+            session.query(SM.EventDataTableStorageRecord)
             .filter(
                 (SM.EventDataTableStorageRecord.project_id == project_id)
                 & (SM.EventDataTableStorageRecord.table_name == edt.table_name)
             )
             .first()
         )
         if record is not None:
-            self._session.delete(record)
+            session.delete(record)
 
         rec = SM.EventDataTableStorageRecord.from_model_instance(
             project_id=project_id, edt=edt
         )
-        self._session.add(rec)
-
-        self._session.commit()
+        session.add(rec)
 
     def _get_event_data_tables_for_project(
-        self, project_id: str
+        self, project_id: str, session: SA.orm.Session
     ) -> List[M.EventDataTable]:
-        records = self._session.query(SM.EventDataTableStorageRecord).filter(
+        records = session.query(SM.EventDataTableStorageRecord).filter(
             SM.EventDataTableStorageRecord.project_id == project_id
         )
         result = []
         for edt_record in records.all():
-            discovery_settings = self.get_discovery_settings(
-                edt_record.discovery_settings_id
+            discovery_settings = self._get_discovery_settings(
+                edt_record.discovery_settings_id, session
             )
             result.append(edt_record.as_model_instance(discovery_settings))
         return result
 
     def _remove_unreferenced_event_data_tables(
-        self, project_id: str, referenced_edts: List[str]
+        self, project_id: str, referenced_edts: List[str], session: SA.orm.Session
     ):
         records = (
-            self._session.query(SM.EventDataTableStorageRecord)
+            session.query(SM.EventDataTableStorageRecord)
             .filter(
                 (SM.EventDataTableStorageRecord.project_id == project_id)
                 & (
                     SM.EventDataTableStorageRecord.event_data_table_id
                     not in referenced_edts
                 )
             )
             .all()
         )
         for record in records:
-            self._session.delete(record)
+            session.delete(record)
 
-    def set_discovery_settings(
-        self, discovery_settings_id: str, discovery_settings: M.DiscoverySettings
+    def _set_discovery_settings(
+        self,
+        discovery_settings_id: str,
+        discovery_settings: M.DiscoverySettings,
+        session: SA.orm.Session,
     ):
         record = (
-            self._session.query(SM.DiscoverySettingsStorageRecord)
+            session.query(SM.DiscoverySettingsStorageRecord)
             .filter(
                 SM.DiscoverySettingsStorageRecord.discovery_settings_id
                 == discovery_settings_id
             )
             .first()
         )
         if record is None:
-            self._session.add(
+            session.add(
                 SM.DiscoverySettingsStorageRecord.from_model_instance(
                     discovery_settings
                 )
             )
-            self._session.commit()
+            session.commit()
             return
 
         record.update(discovery_settings)
 
-        self._session.commit()
-
-    def get_discovery_settings(self, discovery_settings_id: str) -> M.DiscoverySettings:
+    def _get_discovery_settings(
+        self, discovery_settings_id: str, session: SA.orm.Session
+    ) -> M.DiscoverySettings:
         record = (
-            self._session.query(SM.DiscoverySettingsStorageRecord)
+            session.query(SM.DiscoverySettingsStorageRecord)
             .filter(
                 SM.DiscoverySettingsStorageRecord.discovery_settings_id
                 == discovery_settings_id
             )
             .first()
         )
 
         if record is None:
             raise ValueError(
                 f"Discovery settings not found with project_id={discovery_settings_id}"
             )
 
         return record.as_model_instance()
 
-    def set_webapp_settings(
-        self, webapp_settings_id: str, webapp_settings: M.WebappSettings
+    def _set_webapp_settings(
+        self,
+        webapp_settings_id: str,
+        webapp_settings: M.WebappSettings,
+        session: SA.orm.Session,
     ):
         record = (
-            self._session.query(SM.WebappSettingsStorageRecord)
+            session.query(SM.WebappSettingsStorageRecord)
             .filter(
                 SM.WebappSettingsStorageRecord.webapp_settings_id == webapp_settings_id
             )
             .first()
         )
         if record is None:
-            self._session.add(
+            session.add(
                 SM.WebappSettingsStorageRecord.from_model_instance(webapp_settings)
             )
             return
 
         record.update(webapp_settings)
 
-        self._session.commit()
-
-    def get_webapp_settings(self, webapp_settings_id: str) -> M.WebappSettings:
+    def _get_webapp_settings(
+        self, webapp_settings_id: str, session: SA.orm.Session
+    ) -> M.WebappSettings:
         record = (
-            self._session.query(SM.WebappSettingsStorageRecord)
+            session.query(SM.WebappSettingsStorageRecord)
             .filter(
                 SM.WebappSettingsStorageRecord.webapp_settings_id == webapp_settings_id
             )
             .first()
         )
 
         if record is None:
@@ -355,264 +360,308 @@
                 f"Webapp settings not found with project_id={webapp_settings_id}"
             )
 
         return record.as_model_instance()
 
     def list_projects(self) -> List[str]:
         result = []
-        for record in self._session.query(SM.ProjectStorageRecord):
-            result.append(record.project_id)
-        return result
+        with self._new_db_session() as session:
+            for record in session.query(SM.ProjectStorageRecord):
+                result.append(record.project_id)
+            return result
 
     def set_connection(self, connection_id: str, connection: M.Connection):
-        session = self._session
+        with self._new_db_session() as session:
+            self._set_connection(connection_id, connection, session)
+            session.commit()
+
+    def _set_connection(
+        self, connection_id: str, connection: M.Connection, session: SA.orm.Session
+    ):
         record = (
             session.query(SM.ConnectionStorageRecord)
             .filter(SM.ConnectionStorageRecord.connection_id == connection_id)
             .first()
         )
         if record is None:
             session.add(SM.ConnectionStorageRecord.from_model_instance(connection))
         else:
             record.update(connection)
 
-        session.commit()
-
     def get_connection(self, connection_id: str) -> M.Connection:
+        with self._new_db_session() as session:
+            return self._get_connection(connection_id, session)
+
+    def _get_connection(
+        self, connection_id: str, session: SA.orm.Session
+    ) -> M.Connection:
         record = (
-            self._session.query(SM.ConnectionStorageRecord)
+            session.query(SM.ConnectionStorageRecord)
             .filter(SM.ConnectionStorageRecord.connection_id == connection_id)
             .first()
         )
 
         if record is None:
             raise ValueError(f"Connection not found with project_id={connection_id}")
 
         return record.as_model_instance()
 
     def delete_connection(self, connection_id: str):
-        session = self._session
-        record = (
-            session.query(SM.ConnectionStorageRecord)
-            .filter(SM.ConnectionStorageRecord.connection_id == connection_id)
-            .first()
-        )
-        if record is not None:
-            session.delete(record)
-            session.commit()
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.ConnectionStorageRecord)
+                .filter(SM.ConnectionStorageRecord.connection_id == connection_id)
+                .first()
+            )
+            if record is not None:
+                session.delete(record)
+                session.commit()
 
     def list_connections(
         self,
     ) -> List[str]:
-        result = []
-        for record in self._session.query(SM.ConnectionStorageRecord):
-            result.append(record.connection_id)
-        return result
+        with self._new_db_session() as session:
+            result = []
+            for record in session.query(SM.ConnectionStorageRecord):
+                result.append(record.connection_id)
+            return result
 
     def set_event_data_table_definition(
         self,
         event_data_table: M.EventDataTable,
         definitions: Dict[str, M.Reference[M.EventDef]],
     ):
+        with self._new_db_session() as session:
+            self._set_event_data_table_definition(
+                event_data_table, definitions, session
+            )
+            session.commit()
+
+    def _set_event_data_table_definition(
+        self,
+        event_data_table: M.EventDataTable,
+        definitions: Dict[str, M.Reference[M.EventDef]],
+        session: SA.orm.Session,
+    ):
         edt_id = event_data_table.id
         for event_name, event_def in definitions.items():
             rec = (
-                self._session.query(SM.EventDefStorageRecord)
+                session.query(SM.EventDefStorageRecord)
                 .filter(
                     (SM.EventDefStorageRecord.event_data_table_id == edt_id)
                     & (SM.EventDefStorageRecord.event_name == event_name)
                 )
                 .first()
             )
             if rec is not None:
-                self._session.delete(rec)
+                session.delete(rec)
 
             rec = SM.EventDefStorageRecord.from_model_instance(
                 edt_id, event_def.get_value_if_exists()
             )
-            self._session.add(rec)
-
-        self._session.commit()
+            session.add(rec)
 
     def populate_discovered_project(self, discovered_project: M.DiscoveredProject):
+        with self._new_db_session() as session:
+            self._populate_discovered_project(discovered_project, session)
+
+    def _populate_discovered_project(
+        self, discovered_project: M.DiscoveredProject, session: SA.orm.Session
+    ):
         defs = discovered_project.definitions
 
         for edt in defs.keys():
             records: List[SM.EventDefStorageRecord] = (
-                self._session.query(SM.EventDefStorageRecord)
+                session.query(SM.EventDefStorageRecord)
                 .filter(SM.EventDefStorageRecord.event_data_table_id == edt.id)
                 .all()
             )
 
             for rec in records:
                 defs[edt][rec.event_name].restore_value(rec.as_model_instance(edt))
 
     def get_event_definition(
         self, event_data_table: M.EventDataTable, event_definition_id: str
     ) -> M.EventDef:
-        record: SM.EventDefStorageRecord = (
-            self._session.query(SM.EventDefStorageRecord)
-            .filter(SM.EventDefStorageRecord.id == event_definition_id)
-            .first()
-        )
-        return record.as_model_instance(edt=event_data_table)
+        with self._new_db_session() as session:
+            record: SM.EventDefStorageRecord = (
+                session.query(SM.EventDefStorageRecord)
+                .filter(SM.EventDefStorageRecord.id == event_definition_id)
+                .first()
+            )
+            return record.as_model_instance(edt=event_data_table)
 
     def set_saved_metric(self, metric_id: str, saved_metric: WM.SavedMetric):
-        record = (
-            self._session.query(SM.SavedMetricStorageRecord)
-            .filter(SM.SavedMetricStorageRecord.saved_metric_id == metric_id)
-            .first()
-        )
-        if record is None:
-            self._session.add(
-                SM.SavedMetricStorageRecord.from_model_instance(saved_metric)
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.SavedMetricStorageRecord)
+                .filter(SM.SavedMetricStorageRecord.saved_metric_id == metric_id)
+                .first()
             )
-            self._session.commit()
-            return
+            if record is None:
+                session.add(
+                    SM.SavedMetricStorageRecord.from_model_instance(saved_metric)
+                )
+                session.commit()
+                return
 
-        record.update(saved_metric)
+            record.update(saved_metric)
 
-        self._session.commit()
+            session.commit()
 
     def get_saved_metric(self, metric_id: str) -> WM.SavedMetric:
-        record = (
-            self._session.query(SM.SavedMetricStorageRecord)
-            .filter(SM.SavedMetricStorageRecord.saved_metric_id == metric_id)
-            .first()
-        )
-        if record is None:
-            raise ValueError(f"Saved metric is not found with id {metric_id}")
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.SavedMetricStorageRecord)
+                .filter(SM.SavedMetricStorageRecord.saved_metric_id == metric_id)
+                .first()
+            )
+            if record is None:
+                raise ValueError(f"Saved metric is not found with id {metric_id}")
 
         project = self.get_project(record.project_id)
         return record.as_model_instance(project)
 
     def clear_saved_metric(self, metric_id: str):
-        record = (
-            self._session.query(SM.SavedMetricStorageRecord)
-            .filter(SM.SavedMetricStorageRecord.saved_metric_id == metric_id)
-            .first()
-        )
-        if record is not None:
-            self._session.delete(record)
-            self._session.commit()
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.SavedMetricStorageRecord)
+                .filter(SM.SavedMetricStorageRecord.saved_metric_id == metric_id)
+                .first()
+            )
+            if record is not None:
+                session.delete(record)
+                session.commit()
 
     def list_saved_metrics(self) -> List[str]:
-        result = []
-        for record in self._session.query(SM.SavedMetricStorageRecord):
-            result.append(record.saved_metric_id)
-        return result
+        with self._new_db_session() as session:
+            result = []
+            for record in session.query(SM.SavedMetricStorageRecord):
+                result.append(record.saved_metric_id)
+            return result
 
     def list_dashboards(self) -> List[str]:
         result = []
-        for record in self._session.query(SM.DashboardStorageRecord):
-            result.append(record.dashboard_id)
-        return result
+        with self._new_db_session() as session:
+            for record in session.query(SM.DashboardStorageRecord):
+                result.append(record.dashboard_id)
+            return result
 
     def get_dashboard(self, dashboard_id: str) -> WM.Dashboard:
-        record = (
-            self._session.query(SM.DashboardStorageRecord)
-            .filter(SM.DashboardStorageRecord.dashboard_id == dashboard_id)
-            .first()
-        )
-        if record is None:
-            raise ValueError(f"Dashboard is not found with id {dashboard_id}")
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.DashboardStorageRecord)
+                .filter(SM.DashboardStorageRecord.dashboard_id == dashboard_id)
+                .first()
+            )
+            if record is None:
+                raise ValueError(f"Dashboard is not found with id {dashboard_id}")
 
-        dashboard_metric_records = (
-            self._session.query(SM.DashboardMetricStorageRecord)
-            .filter(SM.DashboardMetricStorageRecord.dashboard_id == dashboard_id)
-            .all()
-        )
-        dashboard_metrics = []
-        for dm in dashboard_metric_records:
-            sm = self.get_saved_metric(dm.saved_metric_id)
-            dashboard_metrics.append(dm.as_model_instance(sm))
+            dashboard_metric_records = (
+                session.query(SM.DashboardMetricStorageRecord)
+                .filter(SM.DashboardMetricStorageRecord.dashboard_id == dashboard_id)
+                .all()
+            )
+            dashboard_metrics = []
+            for dm in dashboard_metric_records:
+                sm = self.get_saved_metric(dm.saved_metric_id)
+                dashboard_metrics.append(dm.as_model_instance(sm))
 
-        return record.as_model_instance(dashboard_metrics)
+            return record.as_model_instance(dashboard_metrics)
 
     def set_dashboard(self, dashboard_id: str, dashboard: WM.Dashboard):
-        record = (
-            self._session.query(SM.DashboardStorageRecord)
-            .filter(SM.DashboardStorageRecord.dashboard_id == dashboard_id)
-            .first()
-        )
-        if record is None:
-            self._session.add(SM.DashboardStorageRecord.from_model_instance(dashboard))
-        else:
-            record.update(dashboard)
-
-        dashboard_metrics = (
-            self._session.query(SM.DashboardMetricStorageRecord)
-            .filter(SM.DashboardMetricStorageRecord.dashboard_id == dashboard.id)
-            .all()
-        )
-        for dm in dashboard_metrics:
-            self._session.delete(dm)
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.DashboardStorageRecord)
+                .filter(SM.DashboardStorageRecord.dashboard_id == dashboard_id)
+                .first()
+            )
+            if record is None:
+                session.add(SM.DashboardStorageRecord.from_model_instance(dashboard))
+            else:
+                record.update(dashboard)
+
+            dashboard_metrics = (
+                session.query(SM.DashboardMetricStorageRecord)
+                .filter(SM.DashboardMetricStorageRecord.dashboard_id == dashboard.id)
+                .all()
+            )
+            for dm in dashboard_metrics:
+                session.delete(dm)
 
-        self._set_dashboard_metrics(dashboard.id, dashboard.dashboard_metrics)
-        self._session.commit()
+            self._set_dashboard_metrics(
+                dashboard.id, dashboard.dashboard_metrics, session
+            )
+            session.commit()
 
     def _set_dashboard_metrics(
-        self, dashboard_id: str, metrics: List[WM.DashboardMetric]
+        self,
+        dashboard_id: str,
+        metrics: List[WM.DashboardMetric],
+        session: SA.orm.Session,
     ):
         for dashboard_metric in metrics:
-            self._session.add(
+            session.add(
                 SM.DashboardMetricStorageRecord.from_model_instance(
                     dashboard_id, dashboard_metric
                 )
             )
 
     def clear_dashboard(self, dashboard_id: str):
-        record = (
-            self._session.query(SM.DashboardStorageRecord)
-            .filter(SM.DashboardStorageRecord.dashboard_id == dashboard_id)
-            .first()
-        )
-        if record is not None:
-            self._session.delete(record)
-            self._session.commit()
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.DashboardStorageRecord)
+                .filter(SM.DashboardStorageRecord.dashboard_id == dashboard_id)
+                .first()
+            )
+            if record is not None:
+                session.delete(record)
+                session.commit()
 
     def set_user(self, user: WM.User):
-        session = self._session
-        record = (
-            session.query(SM.UserStorageRecord)
-            .filter(SM.UserStorageRecord.user_id == user.id)
-            .first()
-        )
-        if record is None:
-            session.add(SM.UserStorageRecord.from_model_instance(user))
-            session.commit()
-            return
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.UserStorageRecord)
+                .filter(SM.UserStorageRecord.user_id == user.id)
+                .first()
+            )
+            if record is None:
+                session.add(SM.UserStorageRecord.from_model_instance(user))
+                session.commit()
+                return
 
-        record.update(user)
-        session.commit()
+            record.update(user)
+            session.commit()
 
     def get_user_by_id(self, user_id: str) -> Optional[WM.User]:
-        record = (
-            self._session.query(SM.UserStorageRecord)
-            .filter(SM.UserStorageRecord.user_id == user_id)
-            .first()
-        )
-        if record is None:
-            return None
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.UserStorageRecord)
+                .filter(SM.UserStorageRecord.user_id == user_id)
+                .first()
+            )
+            if record is None:
+                return None
 
-        return record.as_model_instance()
+            return record.as_model_instance()
 
     def list_users(self) -> List[WM.User]:
         result = []
-        for record in self._session.query(SM.UserStorageRecord):
-            result.append(record.as_model_instance())
-        return result
+        with self._new_db_session() as session:
+            for record in session.query(SM.UserStorageRecord):
+                result.append(record.as_model_instance())
+            return result
 
     def clear_user(self, user_id: str):
-        session = self._session
-        record = (
-            session.query(SM.UserStorageRecord)
-            .filter(SM.UserStorageRecord.user_id == user_id)
-            .first()
-        )
-        if record is not None:
-            session.delete(record)
-            session.commit()
+        with self._new_db_session() as session:
+            record = (
+                session.query(SM.UserStorageRecord)
+                .filter(SM.UserStorageRecord.user_id == user_id)
+                .first()
+            )
+            if record is not None:
+                session.delete(record)
+                session.commit()
 
     def health_check(self):
-        session = self._session
-        session.execute("select 1")
+        with self._new_db_session() as session:
+            session.execute("select 1")
```

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/storage_model.py` & `mitzu-0.6.0rc9/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc8/mitzu/webapp/webapp.py` & `mitzu-0.6.0rc9/mitzu/webapp/webapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,19 +53,15 @@
 
     @server.before_request
     def before_request():
         request = flask.request
         deps: DEPS.Dependencies = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
         )
-        resp = deps.authorizer.authorize_request(request)
-
-        # make sure there are no sessions left in the memory before dash forks a new worker
-        deps.storage._session.close_all()
-        return resp
+        return deps.authorizer.authorize_request(request)
 
     @server.after_request
     def after_request(response: flask.Response):
         request = flask.request
         deps: DEPS.Dependencies = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
         )
```

### Comparing `mitzu-0.6.0rc8/pyproject.toml` & `mitzu-0.6.0rc9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.0-rc.8"
+version = "0.6.0-rc.9"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.0rc8/PKG-INFO` & `mitzu-0.6.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.0rc8
+Version: 0.6.0rc9
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

