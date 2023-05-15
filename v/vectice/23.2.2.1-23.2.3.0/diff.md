# Comparing `tmp/vectice-23.2.2.1.tar.gz` & `tmp/vectice-23.2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.2.2.1.tar", last modified: Thu May  4 08:06:32 2023, max compression
+gzip compressed data, was "vectice-23.2.3.0.tar", last modified: Mon May 15 08:05:50 2023, max compression
```

## Comparing `vectice-23.2.2.1.tar` & `vectice-23.2.3.0.tar`

### file list

```diff
@@ -1,113 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 08:06:24.000000 vectice-23.2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-04 08:06:32.946823 vectice-23.2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 08:06:24.000000 vectice-23.2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 08:06:24.000000 vectice-23.2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 08:06:32.946823 vectice-23.2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-04 08:06:24.000000 vectice-23.2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.930823 vectice-23.2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.930823 vectice-23.2.2.1/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.934823 vectice-23.2.2.1/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.938823 vectice-23.2.2.1/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/dataframe_column_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    22703 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.930823 vectice-23.2.2.1/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.897836 vectice-23.2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 08:05:42.000000 vectice-23.2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-15 08:05:50.897836 vectice-23.2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-15 08:05:42.000000 vectice-23.2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 08:05:42.000000 vectice-23.2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 08:05:50.897836 vectice-23.2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-15 08:05:42.000000 vectice-23.2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.869836 vectice-23.2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.877836 vectice-23.2.3.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.885836 vectice-23.2.3.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.889836 vectice-23.2.3.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.893836 vectice-23.2.3.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.893836 vectice-23.2.3.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.893836 vectice-23.2.3.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.897836 vectice-23.2.3.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/metadata/dataframe_column_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30039 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.897836 vectice-23.2.3.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-15 08:05:42.000000 vectice-23.2.3.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:05:50.877836 vectice-23.2.3.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-15 08:05:50.000000 vectice-23.2.3.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-15 08:05:50.000000 vectice-23.2.3.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:05:50.000000 vectice-23.2.3.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-15 08:05:50.000000 vectice-23.2.3.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 08:05:50.000000 vectice-23.2.3.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.2.2.1/LICENSE` & `vectice-23.2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/PKG-INFO` & `vectice-23.2.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.2.1
+Version: 23.2.3.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.2.1/setup.py` & `vectice-23.2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/__init__.py` & `vectice-23.2.3.0/src/vectice/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,13 +82,13 @@
     "DatasetSourceOrigin",
     "DBMetadata",
     "FilesMetadata",
     "File",
     "MetadataDB",
     "DatasetType",
     "silent",
-    "Model",
     "Metric",
+    "Model",
     "Property",
     "CodeSource",
     "Dataset",
 ]
```

### Comparing `vectice-23.2.2.1/src/vectice/api/__init__.py` & `vectice-23.2.3.0/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/_auth.py` & `vectice-23.2.3.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/_utils.py` & `vectice-23.2.3.0/src/vectice/api/_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/attachment.py` & `vectice-23.2.3.0/src/vectice/api/attachment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Any, BinaryIO, NoReturn
 
-from vectice.api.http_error_handlers import InvalidReferenceError
+from vectice.api.http_error_handlers import InvalidReferenceError, VecticeException
 from vectice.api.json import AttachmentOutput, ModelVersionOutput, PagedResponse
 from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.rest_api import HttpError, RestApi
+from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
+from vectice.models.representation.model_version_representation import ModelVersionRepresentation
 
 if TYPE_CHECKING:
     from io import BytesIO
 
     from requests import Response
 
 
@@ -47,59 +49,67 @@
     ) -> tuple[str, str | None]:
         if isinstance(version, ModelVersionOutput):
             return self._generate_model_url_and_id(version)
 
         return self._generate_dataset_url_and_id(version)
 
     @staticmethod
-    def _build_url(project_id: int, version: int, type: str) -> str:
+    def _build_url(project_id: str | int, version: str, type: str) -> str:
         return f"/metadata/project/{project_id}/entityfiles/{type}/{version}"
 
     def post_attachment(
         self, files: list[tuple[str, tuple[str, BinaryIO]]], version: ModelVersionOutput | DatasetVersionOutput
     ) -> list[dict]:
         entity_files = []
-        try:
-            url, repr = self._generate_version_url_and_id(version)
-            if len(files) == 1:
+        url, repr = self._generate_version_url_and_id(version)
+        if len(files) == 1:
+            filename = files[0][1][0]
+            try:
                 response = self._post_attachments(url, files)
                 if response:
                     entity_files.append(response.json())
-                _logger.debug(f"Attachment with name: {files[0][1][0]} successfully attached to {repr}.")
-            elif len(files) > 1:
-                for file in files:
+                _logger.debug(f"Attachment with name: {filename} successfully attached to {repr}.")
+            except HttpError as e:
+                self._handle_http_error(e, version, filename)
+        elif len(files) > 1:
+            for file in files:
+                try:
                     response = self._post_attachments(url, [file])
                     if response:
                         entity_files.append(response.json())
-                _logger.debug(f"Attachments with names: {[f[1][0] for f in files]} successfully attached to {repr}.")
-            return entity_files
-        except HttpError as e:
-            self._handle_http_error(e, version)
+                except HttpError as e:
+                    self._handle_http_error(e, version, file[1][0])
+
+                filenames = ", ".join([f[1][0] for f in files])
+                _logger.debug(f"Attachments with names: {filenames} successfully attached to {repr}.")
+        return entity_files
 
     def post_model_predictor(self, model_type: str, model_content: BytesIO, model_version: ModelVersionOutput) -> None:
         url, model_repr = self._generate_model_url_and_id(model_version)
         url += f"?modelFramework={model_type}"
         attachment = ("file", ("model_pickle", model_content))
         self._post_attachments(url, [attachment])
         _logger.info(f"Model {model_type} successfully attached to {model_repr}.")
 
-    def _identify_object(self, code_version_id: int | None = None, phase_id: int | None = None) -> tuple:
+    def _identify_object(
+        self, code_version_id: int | None = None, phase_id: str | None = None
+    ) -> tuple[str, str | int]:
         if phase_id:
             return "phase", phase_id
         elif code_version_id:
             return "codeversion", code_version_id
         else:
             raise ValueError("No ID was provided for create attachment.")
 
     def create_attachments(
         self,
         files: list[tuple[str, tuple[str, Any]]],
-        project_id: int,
+        project_id: str,
         code_version_id: int | None = None,
-        phase_id: int | None = None,
+        phase_id: str | None = None,
     ) -> list[dict]:
         parent_object, object_id = self._identify_object(code_version_id, phase_id)
         entity_files = []
         try:
             for file in files:
                 response = self._post_attachments(
                     f"/metadata/project/{project_id}/entityfiles/{parent_object}/{object_id}", [file]
@@ -107,17 +117,17 @@
                 if response:
                     entity_files.append(response.json())
             _logger.debug(
                 f"Attachments with names: {[f[1][0] for f in files]} successfully attached to {parent_object} {object_id}."
             )
             return entity_files
         except HttpError as e:
-            self._handle_code_version_error(e, object_id)
+            self._httpErrorHandler.handle_get_http_error(e, parent_object, object_id)
 
-    def get_code_version_attachment(self, code_version_id: int, project_id: int, file_id: int) -> Response:
+    def get_code_version_attachment(self, code_version_id: int, project_id: str, file_id: int) -> Response:
         try:
             return self._get_attachment(
                 f"/metadata/project/{project_id}/entityfiles/codeversion/{code_version_id}/{file_id}"
             )
         except HttpError as e:
             self._handle_code_version_error(e, code_version_id)
 
@@ -132,42 +142,58 @@
         return PagedResponse(
             item_cls=AttachmentOutput,
             total=len(attachments),
             page={},
             items=attachments,
         )
 
-    def list_object_attachments(
-        self, project_id: int, code_version_id: int | None = None, phase_id: int | None = None
+    def list_version_representation_attachments(
+        self, project_id: str, version: ModelVersionRepresentation | DatasetVersionRepresentation
     ) -> PagedResponse[AttachmentOutput]:
-        parent_object, object_id = self._identify_object(code_version_id, phase_id)
         try:
-            attachments = self._list_attachments(
-                f"/metadata/project/{project_id}/entityfiles/{parent_object}/{object_id}"
-            )
+            url_type = "modelversion" if isinstance(version, ModelVersionRepresentation) else "datasetversion"
+            url = self._build_url(project_id, version.id, url_type)
+            attachments = self._list_attachments(url)
         except HttpError as e:
-            self._handle_code_version_error(e, object_id)
+            self._handle_http_error(e, version)
+
         return PagedResponse(
             item_cls=AttachmentOutput,
             total=len(attachments),
             page={},
             items=attachments,
         )
 
-    def list_phase_attachments(self, phase_id: int, project_id: int) -> PagedResponse[AttachmentOutput]:
+    def list_object_attachments(
+        self, project_id: str, code_version_id: int | None = None, phase_id: str | None = None
+    ) -> PagedResponse[AttachmentOutput]:
+        parent_object, object_id = self._identify_object(code_version_id, phase_id)
         try:
-            attachments = self._list_attachments(f"/metadata/project/{project_id}/entityfiles/phase/{phase_id}")
+            attachments = self._list_attachments(
+                f"/metadata/project/{project_id}/entityfiles/{parent_object}/{object_id}"
+            )
         except HttpError as e:
-            self._handle_code_version_error(e, phase_id)
+            self._httpErrorHandler.handle_get_http_error(e, parent_object, object_id)
         return PagedResponse(
             item_cls=AttachmentOutput,
             total=len(attachments),
             page={},
             items=attachments,
         )
 
-    def _handle_http_error(self, error: HttpError, version: ModelVersionOutput | DatasetVersionOutput) -> NoReturn:
-        ref_type = MODEL_VERSION if isinstance(version, ModelVersionOutput) else DATASET_VERSION
+    def _handle_http_error(
+        self,
+        error: HttpError,
+        version: ModelVersionOutput | DatasetVersionOutput | ModelVersionRepresentation | DatasetVersionRepresentation,
+        file: str | None = None,
+    ) -> NoReturn:
+        ref_type = (
+            MODEL_VERSION
+            if isinstance(version, ModelVersionOutput) or isinstance(version, ModelVersionRepresentation)
+            else DATASET_VERSION
+        )
+        if error.code == 413 and file is not None:
+            raise VecticeException(f"{ref_type}: {file} exceeds the maximum size of 100MB.")
         self._httpErrorHandler.handle_get_http_error(error, ref_type, version.id)
 
     def _handle_code_version_error(self, error: HttpError, code_version_id: int) -> NoReturn:
         self._httpErrorHandler.handle_get_http_error(error, "code version", code_version_id)
```

### Comparing `vectice-23.2.2.1/src/vectice/api/client.py` & `vectice-23.2.3.0/src/vectice/api/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+import re
 from datetime import datetime
 from typing import TYPE_CHECKING, BinaryIO
 
 from gql import Client as GQLClient
 from gql.transport.requests import RequestsHTTPTransport
 
 from vectice.__version__ import __version__
@@ -13,54 +14,58 @@
 from vectice.api.compatibility import CompatibilityApi
 from vectice.api.gql_code import GqlCodeApi
 from vectice.api.gql_code_version import GqlCodeVersionApi
 from vectice.api.gql_dataset import GqlDatasetApi
 from vectice.api.gql_feature_flag import GqlFeatureFlagApi
 from vectice.api.gql_model import GqlModelApi
 from vectice.api.gql_user_workspace_api import UserAndDefaultWorkspaceApi
-from vectice.api.http_error_handlers import MissingReferenceError, StepIdError, StepNameError, VecticeException
+from vectice.api.http_error_handlers import MissingReferenceError, VecticeException
 from vectice.api.iteration import IterationApi
 from vectice.api.json import (
     ArtifactName,
     CodeInput,
     CodeVersionCreateBody,
     ModelRegisterInput,
     ModelRegisterOutput,
     ModelType,
     ModelVersionOutput,
     ModelVersionStatus,
     Page,
     PagedResponse,
-    ProjectInput,
     PropertyInput,
     StepOutput,
 )
 from vectice.api.json.dataset_register import DatasetRegisterInput, DatasetRegisterOutput
+from vectice.api.json.dataset_representation import DatasetRepresentationOutput
 from vectice.api.json.dataset_version import DatasetVersionOutput
+from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
 from vectice.api.json.metric import MetricInput
-from vectice.api.json.step import StepUpdateInput
+from vectice.api.json.model_representation import ModelRepresentationOutput
+from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput
 from vectice.api.last_assets import LastAssetApi
 from vectice.api.phase import PhaseApi
 from vectice.api.project import ProjectApi
 from vectice.api.step import StepApi
 from vectice.api.version import VersionApi
 from vectice.api.workspace import WorkspaceApi
 from vectice.models.dataset import Dataset
+from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
+from vectice.models.representation.model_version_representation import ModelVersionRepresentation
+from vectice.utils.vectice_ids_regex import WORKSPACE_VID_REG
 
 if TYPE_CHECKING:
     from io import BytesIO, IOBase
 
     from requests import Response
 
     from vectice.api.json import AttachmentOutput, ProjectOutput, WorkspaceOutput
     from vectice.api.json.compatibility import CompatibilityOutput
     from vectice.api.json.iteration import IterationInput, IterationOutput, IterationStepArtifactInput
     from vectice.api.json.phase import PhaseOutput
     from vectice.api.json.step import StepType
-    from vectice.api.json.workspace import WorkspaceInput
     from vectice.models.model import Model
 
 _logger = logging.getLogger(__name__)
 
 
 DISABLED_FEATURE_FLAG_MESSAGE = (
     "This '{}' feature is not enabled. Please contact your Account Manager for Beta program access."
@@ -74,16 +79,16 @@
 
 
 class Client:
     """Low level Vectice API client."""
 
     def __init__(
         self,
-        workspace: str | int | None = None,
-        project: str | int | None = None,
+        workspace: str | None = None,
+        project: str | None = None,
         token: str | None = None,
         api_endpoint: str | None = None,
         auto_connect=True,
         allow_self_certificate=True,
     ):
         self.auth = Auth(
             api_endpoint=api_endpoint,
@@ -98,19 +103,17 @@
         self._workspace: WorkspaceOutput | None = None
         self._project: ProjectOutput | None = None
 
         if auto_connect:
             if workspace and project:
                 self._project = self.get_project(project, workspace)
                 self._workspace = self._project.workspace
-                if (
-                    isinstance(workspace, str)
-                    and workspace != self._workspace.name
-                    or isinstance(workspace, int)
-                    and workspace != self._workspace.id
+                is_vectice_id = re.search(WORKSPACE_VID_REG, workspace)
+                if (not is_vectice_id and workspace != self._workspace.name) or (
+                    is_vectice_id and workspace != self._workspace.id
                 ):
                     raise ValueError(
                         f"Inconsistency in configuration: Project {project} does not belong to Workspace {workspace}"
                     )
             elif workspace:
                 self._workspace = self.get_workspace(workspace)
             elif project:
@@ -149,133 +152,77 @@
             if version.artifact_name == ArtifactName.BACKEND:
                 return version.version
         raise ValueError("No version found for backend.")
 
     def check_compatibility(self) -> CompatibilityOutput:
         return CompatibilityApi(self.auth).check_version()
 
-    def create_project(self, data: ProjectInput, workspace: str | int) -> ProjectOutput:
-        """Create a project.
-
-        Parameters:
-            data: The ProjectInput JSON structure.
-            workspace: The workspace name or id.
-
-        Returns:
-            The project JSON structure.
-        """
-        result = ProjectApi(self.auth).create_project(data, workspace)
-        _logger.info(f"Project with id: {result.id} successfully created.")
-        return result
-
-    def delete_project(self, project: str | int, workspace: str | int | None = None):
-        """Delete a project.
-
-        Parameters:
-            project: The project name or id.
-            workspace: The workspace name or id.
-        """
-        ProjectApi(self.auth).delete_project(project, workspace)
-
-    def update_project(self, data: ProjectInput, project: str | int, workspace: str | int) -> ProjectOutput:
-        """Update a project.
-
-        Parameters:
-            data: The ProjectInput JSON structure.
-            project: The project name or id.
-            workspace: The workspace name or id.
-
-        Returns:
-            The project JSON structure.
-        """
-        return ProjectApi(self.auth).update_project(data, project, workspace)
-
     def list_projects(
         self,
-        workspace: str | int,
+        workspace: str,
         search: str | None = None,
         page_index: int | None = Page.index,
         page_size: int | None = Page.size,
-    ) -> PagedResponse[ProjectOutput]:
+    ) -> list[ProjectOutput]:
         """List the projects in a workspace.
 
         Parameters:
             workspace: The workspace name or id.
             search: A text to search for.
             page_index: The index of the page.
             page_size: The size of the page.
 
         Returns:
             The workspace's projects.
         """
-        return ProjectApi(self.auth).list_projects(workspace, search, page_index, page_size)
+        if not re.search(WORKSPACE_VID_REG, workspace):
+            workspace = WorkspaceApi(self._gql_client, self.auth).get_workspace(workspace).id
+        return ProjectApi(self._gql_client, self.auth).list_projects(workspace, search, page_index, page_size)
 
-    def get_project(self, project: str | int, workspace: str | int | None = None) -> ProjectOutput:
+    def get_project(self, project: str, workspace: str | None = None) -> ProjectOutput:
         """Get a project.
 
         Parameters:
-            project: The project name or id.
+            project: The project name or vectice id.
             workspace: The workspace name or id.
 
         Returns:
             The project JSON structure.
         """
-        return ProjectApi(self.auth).get_project(project, workspace)
+        if workspace is not None and not re.search(WORKSPACE_VID_REG, workspace):
+            workspace = WorkspaceApi(self._gql_client, self.auth).get_workspace(workspace).id
+        return ProjectApi(self._gql_client, self.auth).get_project(project, workspace)
 
-    def get_workspace(self, workspace: str | int) -> WorkspaceOutput:
+    def get_workspace(self, workspace: str) -> WorkspaceOutput:
         """Get a workspace.
 
         Parameters:
             workspace: The workspace name or id.
 
         Returns:
             The workspace JSON structure.
         """
-        return WorkspaceApi(self.auth).get_workspace(workspace)
-
-    def create_workspace(self, data: WorkspaceInput) -> WorkspaceOutput:
-        """Create a workspace.
-
-        Parameters:
-            data: The WorkspaceInput JSON structure.
-
-        Returns:
-            The workspace JSON structure.
-        """
-        result = WorkspaceApi(self.auth).create_workspace(data)
-        return result
-
-    def update_workspace(self, data: WorkspaceInput, workspace: str | int) -> WorkspaceOutput:
-        """Update a workspace.
-
-        Parameters:
-            data: The WorkspaceInput JSON structure.
-            workspace: The workspace name or id.
-
-        Returns:
-            The workspace JSON structure.
-        """
-        return WorkspaceApi(self.auth).update_workspace(data, workspace)
+        return WorkspaceApi(self._gql_client, self.auth).get_workspace(workspace)
 
     def list_workspaces(
         self, search: str | None = None, page_index: int = 1, page_size: int = 100
-    ) -> PagedResponse[WorkspaceOutput]:
+    ) -> list[WorkspaceOutput]:
         """List the workspaces.
 
         Parameters:
             search: A text to search for.
             page_index: The index of the page.
             page_size: The size of the page.
 
         Returns:
             The workspaces.
         """
-        return WorkspaceApi(self.auth).list_workspaces(search, page_index, page_size)
+        return WorkspaceApi(self._gql_client, self.auth).list_workspaces(search, page_index, page_size)
 
-    def create_code_attachments(self, files: list[tuple[str, tuple[str, str]]], code_version_id: int, project_id: int):
+    def create_code_attachments(self, files: list[tuple[str, tuple[str, str]]], code_version_id: int, project_id: str):
         """Create an attachment.
 
         Parameters:
             files: The paths to the files to attach.
             code_version_id: The code version id to attach files to.
             project_id: The project id associated to the code version id.
 
@@ -295,15 +242,15 @@
 
         Returns:
             The JSON structure.
         """
         return AttachmentApi(self.auth).post_attachment(files, version)
 
     def create_phase_attachments(
-        self, files: list[tuple[str, tuple[str, BytesIO | IOBase]]], phase_id: int, project_id: int
+        self, files: list[tuple[str, tuple[str, BytesIO | IOBase]]], phase_id: str, project_id: str
     ) -> list[dict]:
         """Create an attachment.
 
         Parameters:
             files: The paths to the files to attach.
             phase_id: The phase id to attach files to.
             project_id: The project id to attach files to.
@@ -322,153 +269,142 @@
             model_version: The model version to attach files to.
 
         Returns:
             The JSON structure.
         """
         return AttachmentApi(self.auth).post_model_predictor(model_type, model_content, model_version)
 
+    def list_version_representation_attachments(
+        self, project_id: str, version: ModelVersionRepresentation | DatasetVersionRepresentation
+    ) -> PagedResponse[AttachmentOutput]:
+        """List the attachments of an artifact.
+
+        Parameters:
+            version: The version to list attachments from.
+
+        Returns:
+            The attachments of an artifact.
+        """
+        return AttachmentApi(self.auth).list_version_representation_attachments(project_id, version)
+
     def list_attachments(self, version: ModelVersionOutput | DatasetVersionOutput) -> PagedResponse[AttachmentOutput]:
         """List the attachments of an artifact.
 
         Parameters:
             version: The version to list attachments from.
 
         Returns:
             The attachments of an artifact.
         """
         return AttachmentApi(self.auth).list_attachments(version)
 
-    def list_code_attachments(self, code_version_id: int, project_id: int) -> PagedResponse[AttachmentOutput]:
+    def list_code_attachments(self, code_version_id: int, project_id: str) -> PagedResponse[AttachmentOutput]:
         """List the attachments of a code version.
 
         Parameters:
             code_version_id: The id of the code version to list attachments from.
             project_id: The id of the project the code version belongs to.
 
         Returns:
             A list of attachments that belong to the code version.
         """
         return AttachmentApi(self.auth).list_object_attachments(project_id, code_version_id=code_version_id)
 
-    def list_phase_attachments(self, phase_id: int, project_id: int) -> PagedResponse[AttachmentOutput]:
+    def list_phase_attachments(self, phase_id: str, project_id: str) -> PagedResponse[AttachmentOutput]:
         """List the attachments of a phase.
 
         Parameters:
             phase_id: The id of the phase the attachments belongs to.
             project_id: The id of the project the attachments belongs to.
 
         Returns:
             An attachment.
         """
         return AttachmentApi(self.auth).list_object_attachments(project_id, phase_id=phase_id)
 
-    def get_code_version_attachment(self, code_version_id: int, project_id: int, file_id: int) -> Response:
+    def get_code_version_attachment(self, code_version_id: int, project_id: str, file_id: int) -> Response:
         """Get the attachment of a code version.
 
         Parameters:
             code_version_id: The code version id to list attachments from.
             project_id: The project id the code version belongs to.
             file_id: The file id attached to the code version.
 
         Returns:
             The file attached to the code version.
         """
         return AttachmentApi(self.auth).get_code_version_attachment(code_version_id, project_id, file_id)
 
     def list_phases(
         self,
-        search: str | None = None,
-        project: str | int | None = None,
-        workspace: str | int | None = None,
-    ) -> list[PhaseOutput]:
-        project, workspace = self.get_project_and_workspace_references_or_raise_error(project, workspace)
-        project_object = self.get_project(project, workspace)
-        return PhaseApi(self._gql_client, self.auth).list_phases(project_object.id, search)
+        project: str,
+    ) -> PagedResponse[PhaseOutput]:
+        return PhaseApi(self._gql_client, self.auth).list_phases(project)
 
-    def get_phase(self, phase: str | int, project_id: int | None = None) -> PhaseOutput:
+    def get_phase(self, phase: str, project_id: str | None = None) -> PhaseOutput:
         if project_id is None:
             raise MissingReferenceError("project")
         return PhaseApi(self._gql_client, self.auth).get_phase(phase, project_id)
 
-    def get_step(self, step_reference: str | int, phase_id: int, iteration_id: int) -> StepOutput:
-        if phase_id is None:
-            raise MissingReferenceError("iteration")
-        steps = self.list_steps(phase_id, iteration_id)
-        if isinstance(step_reference, int):
-            for step in steps:
-                if step.id == step_reference:
-                    return step
-            raise StepIdError(step_reference)
-        elif isinstance(step_reference, str):
-            for step in steps:
-                if step.name == step_reference:
-                    return step
-            raise StepNameError(step_reference)
-        raise ValueError(f"Step reference '{step_reference}' does not exists in the phase '{phase_id}'")
+    def get_full_phase(self, phase: str) -> PhaseOutput:
+        return PhaseApi(self._gql_client, self.auth).get_phase(phase=phase, full=True)
 
-    def get_step_by_name(self, step_reference: str, iteration_id: int) -> StepOutput:
+    def get_step_by_name(self, step_reference: str, iteration_id: str) -> StepOutput:
         return StepApi(self._gql_client, self.auth).get_step(step_reference, iteration_id)
 
     def list_steps(
         self,
-        phase_id: int,
-        iteration_index: int | None = None,
-        phase_name: str | None = None,
+        iteration_id: str,
     ) -> list[StepOutput]:
-        if iteration_index is not None:
-            return StepApi(self._gql_client, self.auth).list_steps_for_iteration(phase_id, iteration_index, phase_name)
-
-        return StepApi(self._gql_client, self.auth).list_steps(phase_id, phase_name)
-
-    def close_step(self, step_id: int, message: str | None = None) -> StepOutput:
-        step_update = StepUpdateInput(text=message)
-        return StepApi(self._gql_client, self.auth).close_step(step_id, step_update)
+        return StepApi(self._gql_client, self.auth).list_steps(iteration_id)
 
     def add_iteration_step_artifact(self, step_id: int, step_artifacts: IterationStepArtifactInput) -> StepOutput:
         return StepApi(self._gql_client, self.auth).add_iteration_step_artifact(step_artifacts, step_id)
 
     def update_iteration_step_artifact(
         self,
         step_id: int,
         step_type: StepType,
-        text: str | None = None,
         artifacts: list[IterationStepArtifactInput] | None = None,
     ) -> StepOutput:
-        return StepApi(self._gql_client, self.auth).update_iteration_step_artifact(step_id, step_type, text, artifacts)
+        return StepApi(self._gql_client, self.auth).update_iteration_step_artifact(step_id, step_type, artifacts)
 
-    def list_iterations(self, phase: int) -> list[IterationOutput]:
-        return IterationApi(self._gql_client, self.auth).list_iterations(phase)
+    def list_iterations(self, phase: str, only_mine: bool = False) -> PagedResponse[IterationOutput]:
+        return IterationApi(self._gql_client, self.auth).list_iterations(phase, only_mine)
 
-    def list_step_definitions(self, phase: int) -> list[StepOutput]:
+    def list_step_definitions(self, phase: str) -> list[StepOutput]:
         return PhaseApi(self._gql_client, self.auth).list_step_definitions(phase)
 
-    def get_iteration(self, iteration_id: int) -> IterationOutput:
+    def get_full_iteration(self, iteration_id: str) -> IterationOutput:
+        return IterationApi(self._gql_client, self.auth).get_iteration(iteration_id, full=True)
+
+    def get_iteration(self, iteration_id: str) -> IterationOutput:
         return IterationApi(self._gql_client, self.auth).get_iteration(iteration_id)
 
-    def get_iteration_by_index(self, phase_id: int, index: int) -> IterationOutput:
+    def get_iteration_by_index(self, phase_id: str, index: int) -> IterationOutput:
         return IterationApi(self._gql_client, self.auth).get_iteration_by_index(phase_id, index)
 
     def get_iteration_last_assets(self, iteration_id: int) -> IterationOutput:
         return IterationApi(self._gql_client, self.auth).get_iteration_last_assets(iteration_id)
 
-    def create_iteration(self, phase_id: int) -> IterationOutput:
+    def create_iteration(self, phase_id: str) -> IterationOutput:
         return IterationApi(self._gql_client, self.auth).create_iteration(phase_id)
 
-    def update_iteration(self, iteration_id: int, iteration: IterationInput) -> IterationOutput:
+    def update_iteration(self, iteration_id: str, iteration: IterationInput) -> IterationOutput:
         return IterationApi(self._gql_client, self.auth).update_iteration(iteration, iteration_id)
 
-    def delete_iteration(self, iteration_id: int) -> None:
+    def delete_iteration(self, iteration_id: str) -> None:
         IterationApi(self._gql_client, self.auth).delete_iteration(iteration_id)
 
     def register_dataset_from_source(
         self,
         dataset: Dataset,
-        project_id: int | None = None,
-        phase_id: int | None = None,
-        iteration_id: int | None = None,
+        project_id: str | None = None,
+        phase_id: str | None = None,
+        iteration_id: str | None = None,
         code_version_id: int | None = None,
     ) -> DatasetRegisterOutput:
         if dataset._has_bigquery_resource and self.is_feature_flag_enabled("bigquery-dataset-source") is False:
             raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format("bigquery-dataset-source"))
 
         if dataset._has_dataframe is True and self.is_feature_flag_enabled("dataset-dataframe") is False:
             raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format("dataset-dataframe"))
@@ -490,89 +426,81 @@
             type=dataset.type.value,
             datasetSources=metadata_asdict,
             inputs=derived_from,
             codeVersionId=code_version_id,
             properties=properties,
         )
         dataset_register_output = self.register_dataset(dataset_register_input, project_id, phase_id, iteration_id)
-        dataset.latest_version_id = dataset_register_output["datasetVersion"]["id"]
+        dataset.latest_version_id = dataset_register_output["datasetVersion"]["vecticeId"]
         return dataset_register_output
 
+    def get_dataset(self, id: str) -> DatasetRepresentationOutput:
+        return GqlDatasetApi(self._gql_client, self.auth).get_dataset(id)
+
+    def get_dataset_version(self, id: str) -> DatasetVersionRepresentationOutput:
+        return GqlDatasetApi(self._gql_client, self.auth).get_dataset_version(id)
+
+    def get_model(self, id: str) -> ModelRepresentationOutput:
+        return GqlModelApi(self._gql_client, self.auth).get_model(id)
+
+    def get_model_version(self, id: str) -> ModelVersionRepresentationOutput:
+        return GqlModelApi(self._gql_client, self.auth).get_model_version(id)
+
     @staticmethod
     def get_dataset_name(dataset: Dataset) -> str:
         return f"dataset {datetime.time}" if dataset.name is None else dataset.name
 
     @staticmethod
-    def get_derived_from(obj: Dataset | Model) -> list[int]:
+    def get_derived_from(obj: Dataset | Model) -> list[str]:
         return [] if obj.derived_from is None else obj.derived_from
 
     def register_dataset(
         self,
         dataset_register_input: DatasetRegisterInput,
-        project_id: int | None = None,
-        phase_id: int | None = None,
-        iteration_id: int | None = None,
+        project_id: str | None = None,
+        phase_id: str | None = None,
+        iteration_id: str | None = None,
     ) -> DatasetRegisterOutput:
         data: DatasetRegisterOutput = GqlDatasetApi(self._gql_client, self.auth).register_dataset(
             dataset_register_input, project_id, phase_id, iteration_id
         )
         _logger.debug(
             f"Successfully registered Dataset("
             f"name='{dataset_register_input.name}', "
-            f"id={data['datasetVersion']['id']}, "
+            f"id={data['datasetVersion']['vecticeId']}, "
             f"version='{data['datasetVersion']['name']}', "
             f"type={dataset_register_input.type})."
         )
         return data
 
-    def get_project_and_workspace_references(
-        self, project: str | int | None = None, workspace: str | int | None = None
-    ):
+    def get_project_and_workspace_references(self, project: str | None = None, workspace: str | None = None):
         if project is None and self.project is not None:
             project = self.project.id
         if workspace is None and self.workspace is not None:
             workspace = self.workspace.id
         return project, workspace
 
-    def get_project_and_workspace_refs_if_project_ref_is_str(
-        self, project: str | int | None = None, workspace: str | int | None = None
-    ):
-        if project is None and self.project is not None:
-            project = self.project.id
-        elif isinstance(project, str):
-            if workspace is None and self.workspace is not None:
-                workspace = self.workspace.id
-        return project, workspace
-
-    def get_project_and_workspace_refs_if_project_ref_is_str_or_raise_error(
-        self, project: str | int | None = None, workspace: str | int | None = None
-    ) -> tuple[str | int, str | int | None]:
-        project, workspace = self.get_project_and_workspace_refs_if_project_ref_is_str(project, workspace)
-        if project is None:
-            raise MissingReferenceError("project")
-        return project, workspace
-
     def get_project_and_workspace_references_or_raise_error(
-        self, project: str | int | None = None, workspace: str | int | None = None
-    ) -> tuple[str | int, str | int | None]:
+        self, project: str | None = None, workspace: str | None = None
+    ) -> tuple[str, str | None]:
         project, workspace = self.get_project_and_workspace_references(project, workspace)
         if project is None:
             raise MissingReferenceError("project")
         return project, workspace
 
     @staticmethod
     def _get_model_name(library: str, technique: str, name: str | None = None) -> str:
         return name if name else f"{library} {technique} model"
 
     def register_model(
         self,
         model: Model,
-        project_id: int,
-        phase_id: int | None = None,
-        iteration_id: int | None = None,
+        project_id: str,
+        phase_id: str | None = None,
+        iteration_id: str | None = None,
         code_version_id: int | None = None,
     ) -> ModelRegisterOutput:
         """Register a model.
 
         Parameters:
             model: The model to register
             project_id: The project ID
@@ -605,21 +533,21 @@
 
     def get_last_assets(self, target_types: list[str], page):
         return LastAssetApi(self._gql_client, self.auth).get_last_assets(target_types, page)
 
     def get_user_and_default_workspace(self):
         return UserAndDefaultWorkspaceApi(self._gql_client, self.auth).get_user_and_default_workspace()
 
-    def create_code_gql(self, project_id: int, code: CodeInput):
+    def create_code_gql(self, project_id: str, code: CodeInput):
         return GqlCodeApi(self._gql_client, self.auth).create_code(project_id, code)
 
     def create_code_version_gql(self, code_id: int, code_version: CodeVersionCreateBody):
         return GqlCodeVersionApi(self._gql_client, self.auth).create_code_version(code_id, code_version)
 
-    def get_code(self, code: str | int, project_id: int | None = None):
+    def get_code(self, code: str | int, project_id: str | None = None):
         if project_id is None:
             raise MissingReferenceError("project")
         return GqlCodeApi(self._gql_client, self.auth).get_code(code, project_id)
 
     def get_code_version(self, code_version: str | int, code_id: int | None = None):
         if code_id is None:
             raise MissingReferenceError("code")
```

### Comparing `vectice-23.2.2.1/src/vectice/api/gql_api.py` & `vectice-23.2.3.0/src/vectice/api/gql_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     ProjectOutput,
     PublicConfigOutput,
     StepOutput,
     UserActivity,
     UserAndDefaultWorkspaceOutput,
     WorkspaceOutput,
 )
+from vectice.api.json.dataset_representation import DatasetRepresentationOutput
+from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
+from vectice.api.json.model_representation import ModelRepresentationOutput
+from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput
 
 if TYPE_CHECKING:
     from gql import Client
 
     from vectice.api._auth import Auth
 
 ResultType = TypeVar("ResultType")
@@ -64,14 +68,18 @@
             "Workspace": WorkspaceOutput,
             "Project": ProjectOutput,
             "Phase": PhaseOutput,
             "IterationStep": StepOutput,
             "Iteration": IterationOutput,
             "DatasetRegisterResultOutput": DatasetRegisterOutput,
             "ModelRegisterResultOutput": ModelRegisterOutput,
+            "DataSet": DatasetRepresentationOutput,
+            "DataSetVersion": DatasetVersionRepresentationOutput,
+            "Model": ModelRepresentationOutput,
+            "ModelVersion": ModelVersionRepresentationOutput,
             "UserActivity": UserActivity,
             "Code": CodeOutput,
             "CodeVersion": CodeVersionOutput,
             "PublicConfigOutput": PublicConfigOutput,
             "UserAndDefaultWorkspaceOutput": UserAndDefaultWorkspaceOutput,
             "StepDefinition": StepOutput,
         }
```

### Comparing `vectice-23.2.2.1/src/vectice/api/gql_code.py` & `vectice-23.2.3.0/src/vectice/api/gql_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             authorId
             lastUpdatedById
             __typename
             """
 
 
 class GqlCodeApi(GqlApi):
-    def create_code(self, project_id: int, code: CodeInput) -> CodeOutput:
+    def create_code(self, project_id: str, code: CodeInput) -> CodeOutput:
         variable_types = "$projectId:VecticeId!,$code:CodeCreateInput!"
         kw = "projectId:$projectId,code:$code"
         variables = {"projectId": project_id, "code": code}
 
         query = GqlApi.build_query(
             gql_query="createCode",
             variable_types=variable_types,
@@ -48,15 +48,15 @@
         try:
             response = self.execute(query_built, variables)
             dataset_output: CodeOutput = Parser().parse_item(response["createCode"])
             return dataset_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "code", "createCode")
 
-    def get_code(self, code: str | int, project_id: int | None = None) -> CodeOutput:
+    def get_code(self, code: str | int, project_id: str | None = None) -> CodeOutput:
         if isinstance(code, int):
             gql_query = "getCode"
             variable_types = "$codeId:Float!"
             variables = {"codeId": code}
             kw = "codeId:$codeId"
         elif isinstance(code, str) and project_id:
             gql_query = "getCodeByName"
```

### Comparing `vectice-23.2.2.1/src/vectice/api/gql_code_version.py` & `vectice-23.2.3.0/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/gql_feature_flag.py` & `vectice-23.2.3.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/gql_model.py` & `vectice-23.2.3.0/src/vectice/api/last_assets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,54 @@
 from __future__ import annotations
 
+import logging
 from typing import TYPE_CHECKING
 
 from gql import gql
 from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
 
 if TYPE_CHECKING:
-    from vectice.api.json.model_register import ModelRegisterInput, ModelRegisterOutput
+    from vectice.api.json import PagedResponse
 
+_logger = logging.getLogger(__name__)
+
+# TODO JobRun for lineages
 _RETURNS = """
-            modelVersion{
-                          id
-                          name
-                          version
-                          description
-                          algorithmName
-                          framework
-                          modelId
-                          model {
-                            name
-                            projectId
-                          }
-            }
-            useExistingModel
+            items {
+                    id
+                    date
+                    targetType
+                    targetId
+                    targetName
+                    __typename
+                    }
+            total
+            page {
+                afterCursor
+                hasNextPage
+                }
             __typename
             """
 
 
-class GqlModelApi(GqlApi):
-    def register_model(
-        self,
-        data: ModelRegisterInput,
-        project_id: int,
-        phase_id: int | None = None,
-        iteration_id: int | None = None,
-    ) -> ModelRegisterOutput:
-        variables = {"projectId": project_id, "data": data}
-        kw = "projectId:$projectId,data:$data"
-        variable_types = "$projectId:VecticeId!,$data:ModelRegisterInput!"
-        if phase_id:
-            variable_types += ",$phaseId:VecticeId!"
-            kw += ",phaseId:$phaseId"
-            variables["phaseId"] = phase_id
-        if iteration_id:
-            variable_types += ",$iterationId:VecticeId!"
-            kw += ",iterationId:$iterationId"
-            variables["iterationId"] = iteration_id
-        query_name = "registerModel"
+class LastAssetApi(GqlApi):
+    def get_last_assets(self, target_types: list[str], page):
+        variable_types = "$targetTypes:[ActivityTargetType!],$page:PageIndexInput"
+        kw = "targetTypes:$targetTypes,page:$page"
+        variables = {"targetTypes": target_types, "page": page}
+
         query = GqlApi.build_query(
-            gql_query=query_name,
+            gql_query="getLastAssets",
             variable_types=variable_types,
             returns=_RETURNS,
             keyword_arguments=kw,
-            query=False,
+            query=True,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
-            model_output: ModelRegisterOutput = Parser().parse_item(response[query_name])
-            return model_output
+            assets_output: PagedResponse = Parser().parse_paged_response(response["getLastAssets"])
+            return assets_output
         except TransportQueryError as e:
-            self._error_handler.handle_post_gql_error(e, "model", "register model")
+            self._error_handler.handle_post_gql_error(e, "asset", "getLastAssets")
```

### Comparing `vectice-23.2.2.1/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.2.3.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 _logger = logging.getLogger(__name__)
 
 _RETURNS = """
                 user{
                     name
                 }
                 defaultWorkspace{
-                                id
+                                vecticeId
                 }
                 __typename
 """
 
 
 class UserAndDefaultWorkspaceApi(GqlApi):
     def get_user_and_default_workspace(self):
```

### Comparing `vectice-23.2.2.1/src/vectice/api/http_error.py` & `vectice-23.2.3.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/http_error_handlers.py` & `vectice-23.2.3.0/src/vectice/api/http_error_handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,62 @@
 from __future__ import annotations
 
+import re
 from typing import TYPE_CHECKING, Any, NoReturn
 
+from vectice.utils.vectice_ids_regex import ITERATION_VID_REG, PHASE_VID_REG, PROJECT_VID_REG, WORKSPACE_VID_REG
+
 if TYPE_CHECKING:
     from gql.transport.exceptions import TransportQueryError
 
     from vectice.api.http_error import HttpError
 
 BAD_OR_MISSING_CREDENTIALS_ERROR_MESSAGE = "Bad or missing credentials"
 
 
+class InvalidIdError(ValueError):
+    """When an incorrect value type is passed at the client level."""
+
+    def __init__(self, reference_type: str, value: Any) -> None:
+        valid_id = "a valid id"
+        wsp = "WSP-[int]"
+        prj = "PRJ-[int]"
+        pha = "PHA-[int]"
+        itr = "ITR-[int]"
+        dts = "DTS-[int]"
+        dsv = "DTV-[int]"
+        mod = "MDL-[int]"
+        mdv = "MDV-[int]"
+        if reference_type == "workspace":
+            valid_id = wsp
+        elif reference_type == "project":
+            valid_id = prj
+        elif reference_type == "phase":
+            valid_id = pha
+        elif reference_type == "iteration":
+            valid_id = itr
+        elif reference_type == "dataset":
+            valid_id = dts
+        elif reference_type == "dataset_version":
+            valid_id = dsv
+        elif reference_type == "model":
+            valid_id = mod
+        elif reference_type == "model_version":
+            valid_id = mdv
+        elif reference_type == "asset":
+            refs = {", ".join([wsp, prj, pha, itr, dts, dsv, mod, mdv])}
+            valid_id = f"one of ({refs})"
+
+        super().__init__(
+            f"The {reference_type} reference is invalid. Please check the provided value. "
+            + f"It should be {valid_id} "
+            + f"Provided value is {value}"
+        )
+
+
 class InvalidReferenceError(ValueError):
     """When an incorrect value type is passed at the client level."""
 
     def __init__(self, reference_type: str, value: Any) -> None:
         super().__init__(
             f"The {reference_type} reference is invalid."
             + "Please check the provided value as it should be a string or a number."
@@ -99,44 +142,48 @@
         Parameters:
             reference_type: The reference type.
             value: A value.
 
         Returns:
             An exception instance.
         """
-        if reference_type == "workspace":
-            if isinstance(value, str):
+        if isinstance(value, str) and reference_type == "workspace":
+            if not re.search(WORKSPACE_VID_REG, value):
                 return WorkspaceNameError(value)
-            elif isinstance(value, int):
-                return WorkspaceIdError(value)
-        elif reference_type == "project":
-            if isinstance(value, str):
+            return WorkspaceIdError(value)
+        elif isinstance(value, str) and reference_type == "project":
+            if not re.search(PROJECT_VID_REG, value):
                 return ProjectNameError(value)
-            elif isinstance(value, int):
-                return ProjectIdError(value)
-        elif reference_type == "phase":
-            if isinstance(value, str):
+            return ProjectIdError(value)
+        elif isinstance(value, str) and reference_type == "phase":
+            if not re.search(PHASE_VID_REG, value):
                 return PhaseNameError(value)
-            elif isinstance(value, int):
-                return PhaseIdError(value)
+            return PhaseIdError(value)
         elif reference_type == "step":
             if isinstance(value, str):
                 return StepNameError(value)
             elif isinstance(value, int):
                 return StepIdError(value)
-        elif reference_type == "iteration":
-            if isinstance(value, int):
+        elif isinstance(value, str) and reference_type == "iteration":
+            if re.search(ITERATION_VID_REG, value):
                 return IterationIdError(value)
-            elif isinstance(value, str):
-                return IterationNameError(value)
+            return IterationNameError(value)
         elif reference_type == "iteration_index":
             if isinstance(value, int):
                 return IterationIndexError(value)
-        elif reference_type == "steps":
+        elif isinstance(value, str) and reference_type == "steps":
             return NoStepsInPhaseError(value)
+        elif isinstance(value, str) and reference_type == "dataset":
+            return DatasetIdError(value)
+        elif isinstance(value, str) and reference_type == "dataset_version":
+            return DatasetVersionIdError(value)
+        elif isinstance(value, str) and reference_type == "model":
+            return ModelIdError(value)
+        elif isinstance(value, str) and reference_type == "model_version":
+            return ModelVersionIdError(value)
         return RuntimeError(f"The value {value} of type {reference_type} is not valid!")
 
 
 class VecticeException(Exception):  # noqa: N818
     def __init__(self, value):
         super().__init__(value)
         self.__suppress_context__ = True
@@ -156,35 +203,35 @@
 
 class WorkspaceNameError(VecticeBaseNameError):
     def __init__(self, value: str):
         super().__init__(f"The workspace with name '{value}' is unknown.")
 
 
 class WorkspaceIdError(VecticeBaseNameError):
-    def __init__(self, value: int):
+    def __init__(self, value: str):
         super().__init__(f"The workspace with id '{value}' is unknown.")
 
 
 class ProjectNameError(VecticeBaseNameError):
     def __init__(self, value: str):
         super().__init__(f"The project with name '{value}' is unknown.")
 
 
 class ProjectIdError(VecticeBaseNameError):
-    def __init__(self, value: int):
+    def __init__(self, value: str):
         super().__init__(f"The project with id '{value}' is unknown.")
 
 
 class PhaseNameError(VecticeBaseNameError):
     def __init__(self, value: str):
         super().__init__(f"The phase with name '{value}' is unknown.")
 
 
 class PhaseIdError(VecticeBaseNameError):
-    def __init__(self, value: int):
+    def __init__(self, value: str):
         super().__init__(f"The phase with id '{value}' is unknown.")
 
 
 class StepNameError(VecticeBaseNameError):
     def __init__(self, value: str):
         super().__init__(
             f"The step with name '{value}' is unknown. Use <your iteration>.list_steps() method to find step names."
@@ -195,25 +242,45 @@
     def __init__(self, value: int):
         super().__init__(
             f"The step with id '{value}' is unknown. Use <your iteration>.list_steps() method to find step ids."
         )
 
 
 class IterationIdError(VecticeBaseNameError):
-    def __init__(self, value: int):
+    def __init__(self, value: str):
         super().__init__(f"The iteration with id '{value}' is unknown.")
 
 
 class IterationIndexError(VecticeBaseNameError):
     def __init__(self, value: int):
         super().__init__(f"The iteration with index '{value}' is unknown.")
 
 
 class IterationNameError(VecticeBaseNameError):
     def __init__(self, value: str):
         super().__init__(f"The iteration with name '{value}' is unknown.")
 
 
 class NoStepsInPhaseError(VecticeBaseNameError):
-    def __init__(self, value: str | int):
-        ref = f"with id '{value}'" if isinstance(value, int) else f"'{value}'"
+    def __init__(self, value: str):
+        ref = f"with id '{value}'" if re.search(PHASE_VID_REG, value) else f"'{value}'"
         super().__init__(f"There are no steps in the phase {ref}. Must create steps for this phase in the UI.")
+
+
+class DatasetIdError(VecticeBaseNameError):
+    def __init__(self, value: str):
+        super().__init__(f"The dataset with id '{value}' is unknown.")
+
+
+class DatasetVersionIdError(VecticeBaseNameError):
+    def __init__(self, value: str):
+        super().__init__(f"The dataset version with id '{value}' is unknown.")
+
+
+class ModelIdError(VecticeBaseNameError):
+    def __init__(self, value: str):
+        super().__init__(f"The model with id '{value}' is unknown.")
+
+
+class ModelVersionIdError(VecticeBaseNameError):
+    def __init__(self, value: str):
+        super().__init__(f"The model version with id '{value}' is unknown.")
```

### Comparing `vectice-23.2.2.1/src/vectice/api/iteration.py` & `vectice-23.2.3.0/src/vectice/api/iteration.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,56 +3,119 @@
 import logging
 from typing import TYPE_CHECKING
 
 from gql import gql
 from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
+from vectice.api.json.paged_response import PagedResponse
+from vectice.utils.api_utils import INDEX_ORDERED_DESC, PAGINATE_OUTPUT, get_phase_input
 
 if TYPE_CHECKING:
     from vectice.api.json.iteration import IterationInput, IterationOutput
 
 _logger = logging.getLogger(__name__)
 
-_RETURNS = """id
+_RETURNS_LIST = """vecticeId
             index
             status
-            phase {
+            owner {
+                id
+                name
+            }
+            starred
+            __typename
+            """
+
+_RETURNS_PAGE = PAGINATE_OUTPUT.format(_RETURNS_LIST)
+
+_BASE_RETURNS = """vecticeId
+            index
+            status
+            owner {
                     id
                     name
-                    status
-                    __typename
-              }
+                    }
+            starred
             steps {
                     slug
                     id
                     name
                     stepType
                     artifacts {
-                    type
-                    datasetVersionId
+                        type
+                        datasetVersion {
+                            vecticeId
+                        }
+                        modelVersion {
+                            vecticeId
+                        }
+                        entityFileId
+                        text
+                        type
                     }
             }
             __typename
             """
+_BASE_PARENT = """
+            phase {
+                    vecticeId
+                    name
+                    status
+                    index
+                    __typename
+              }
+"""
 
-_RETURNS_LAST_ASSETS = """id
+_RETURNS = f"""
+    {_BASE_RETURNS}
+    {_BASE_PARENT}
+"""
+
+_PARENT_FULL = """
+            phase {
+                    vecticeId
+                    name
+                    status
+                    index
+                    __typename
+                    parent {
+                        vecticeId
+                        name
+                        description
+                        workspace {
+                            vecticeId
+                            name
+                            description
+                            __typename
+                        }
+                        __typename
+                    }
+              }
+"""
+
+_RETURNS_FULL = f"""
+    {_BASE_RETURNS}
+    {_PARENT_FULL}
+"""
+
+_RETURNS_LAST_ASSETS = """vecticeId
             index
             status
             phase {
-                    id
+                    vecticeId
                     name
                     status
                     __typename
                     parent {
-                            id
+                            vecticeId
                             name
                             __typename
                             workspace{
-                                    id
+                                    vecticeId
                                     name
                                     __typename
                             }
                     }
               }
               steps{
                     slug
@@ -64,38 +127,39 @@
                     __typename
               }
             __typename
             """
 
 
 class IterationApi(GqlApi):
-    def list_iterations(self, parent_id: int) -> list[IterationOutput]:
-        alias_filter = {"phaseId": parent_id, "search": ""}
-        returns = f"""items{{
-                                    {_RETURNS}
-                        }}"""
-        variable_types = "$filters:IterationFiltersInput!"
-        kw = "filters:$filters"
-        variables = {"filters": alias_filter}
+    def list_iterations(self, parent_id: str, only_mine: bool = False) -> PagedResponse[IterationOutput]:
+        gql_query = "getIterationList"
+        alias_filter = {"phaseId": parent_id, "onlyMine": only_mine}
+        variable_types = "$filters:IterationFiltersInput!,$order:ListOrderInput,$page:PageInput"
+        kw = "filters:$filters,order:$order,page:$page"
+        variables = {
+            "filters": alias_filter,
+            "order": INDEX_ORDERED_DESC,
+            "page": get_phase_input(),
+        }
         query = GqlApi.build_query(
-            gql_query="getIterationList",
+            gql_query=gql_query,
             variable_types=variable_types,
-            returns=returns,
+            returns=_RETURNS_PAGE,
             keyword_arguments=kw,
-            query=True,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
-            iterations_output: list[IterationOutput] = Parser().parse_list(response["getIterationList"]["items"])
+            iterations_output: PagedResponse[IterationOutput] = Parser().parse_paged_response(response[gql_query])
             return iterations_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "iteration", "list")
 
-    def create_iteration(self, phase_id: int) -> IterationOutput:
+    def create_iteration(self, phase_id: str) -> IterationOutput:
         gql_query = "createIteration"
         variable_types = "$phaseId:VecticeId!"
         variables = {"phaseId": phase_id}
         kw = "phaseId:$phaseId"
         query = GqlApi.build_query(
             gql_query=gql_query, variable_types=variable_types, returns=_RETURNS, keyword_arguments=kw, query=False
         )
@@ -103,21 +167,25 @@
         try:
             response = self.execute(query_built, variables)
             iteration_output: IterationOutput = Parser().parse_item(response[gql_query])
             return iteration_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "iteration", phase_id)
 
-    def get_iteration(self, iteration_id: int) -> IterationOutput:
+    def get_iteration(self, iteration_id: str, full: bool = False) -> IterationOutput:
         gql_query = "getIterationById"
         variable_types = "$id:VecticeId!"
         variables = {"id": iteration_id}
         kw = "id:$id"
         query = GqlApi.build_query(
-            gql_query=gql_query, variable_types=variable_types, returns=_RETURNS, keyword_arguments=kw, query=True
+            gql_query=gql_query,
+            variable_types=variable_types,
+            returns=_RETURNS_FULL if full else _RETURNS,
+            keyword_arguments=kw,
+            query=True,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             iteration_output: IterationOutput = Parser().parse_item(response[gql_query])
             return iteration_output
         except TransportQueryError as e:
@@ -139,15 +207,15 @@
         try:
             response = self.execute(query_built, variables)
             iteration_output: IterationOutput = Parser().parse_item(response[gql_query])
             return iteration_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "iteration", iteration_id)
 
-    def get_iteration_by_index(self, phase_id: int, index: int) -> IterationOutput:
+    def get_iteration_by_index(self, phase_id: str, index: int) -> IterationOutput:
         gql_query = "getIterationByIndex"
         variable_types = "$index:Float!,$phaseId:VecticeId!"
         variables = {"index": index, "phaseId": phase_id}
         kw = "index:$index,phaseId:$phaseId"
         query = GqlApi.build_query(
             gql_query=gql_query, variable_types=variable_types, returns=_RETURNS, keyword_arguments=kw, query=True
         )
@@ -155,15 +223,15 @@
         try:
             response = self.execute(query_built, variables)
             iteration_output: IterationOutput = Parser().parse_item(response[gql_query])
             return iteration_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "iteration_index", index)
 
-    def update_iteration(self, iteration: IterationInput, iteration_id: int) -> IterationOutput:
+    def update_iteration(self, iteration: IterationInput, iteration_id: str) -> IterationOutput:
         variable_types = "$id:VecticeId!,$data:IterationUpdateInput!"
         kw = "id:$id,data:$data"
         variables = {"id": iteration_id, "data": iteration}
         query = GqlApi.build_query(
             gql_query="updateIteration",
             variable_types=variable_types,
             returns=_RETURNS,
@@ -174,15 +242,15 @@
         try:
             response = self.execute(query_built, variables)
             iteration_output: IterationOutput = Parser().parse_item(response["updateIteration"])
             return iteration_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "iteration", "put")
 
-    def delete_iteration(self, iteration_id: int) -> None:
+    def delete_iteration(self, iteration_id: str) -> None:
         variable_types = "$id:VecticeId!"
         kw = "id:$id"
         variables = {"id": iteration_id}
         query = GqlApi.build_query(
             gql_query="removeIteration",
             variable_types=variable_types,
             keyword_arguments=kw,
```

### Comparing `vectice-23.2.2.1/src/vectice/api/json/__init__.py` & `vectice-23.2.3.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/artifact_version.py` & `vectice-23.2.3.0/src/vectice/api/json/artifact_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class ArtifactVersion(dict):
     def __init__(
         self,
         version_number: int | None = None,
         version_name: str | None = None,
-        version_id: int | None = None,
+        version_id: str | None = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if version_number is not None:
             self["versionNumber"] = version_number
         if version_name is not None:
```

### Comparing `vectice-23.2.2.1/src/vectice/api/json/code.py` & `vectice-23.2.3.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/code_version.py` & `vectice-23.2.3.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/dataset_register.py` & `vectice-23.2.3.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/dataset_version.py` & `vectice-23.2.3.0/src/vectice/api/json/dataset_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         super().__init__(*args, **kwargs)
         if "dataSet" in self:
             self._dataset: DatasetOutput = DatasetOutput(**self["dataSet"])
         else:
             self._dataset = None
 
     @property
-    def id(self) -> int:
-        return int(self["id"])
+    def id(self) -> str:
+        return str(self["vecticeId"])
 
     @property
     def name(self) -> str:
         return str(self["name"])
 
     @property
     def dataset(self) -> DatasetOutput:
```

### Comparing `vectice-23.2.2.1/src/vectice/api/json/files_metadata.py` & `vectice-23.2.3.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/iteration.py` & `vectice-23.2.3.0/src/vectice/api/json/step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,133 +1,112 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import TYPE_CHECKING
 
-from vectice.api.json.step import PhaseOutput
+from vectice.api.json.phase import PhaseOutput
 
 if TYPE_CHECKING:
-    from vectice.api.json.step import StepInput, StepOutput
+    from vectice.api.json.iteration import IterationStepArtifact
 
 
-class IterationStatus(Enum):
+class DocumentationPageStatus(Enum):
+    """Enumeration of the different statuses for documentation pages."""
+
     NotStarted = "NotStarted"
-    InProgress = "InProgress"
-    InReview = "InReview"
-    Abandoned = "Abandoned"
+    InProgress = "Draft"
     Completed = "Completed"
 
 
-class IterationStepArtifactType(Enum):
-    ModelVersion = "ModelVersion"
-    DataSetVersion = "DataSetVersion"
-    EntityFile = "EntityFile"
-    JobRun = "JobRun"
+class StepType(Enum):
+    """Enumeration of the different types of steps."""
 
+    Step = "UNKNOWN"
+    StepDataset = "DATASET"
+    StepModel = "MODEL"
+    StepNumber = "NUMBER"
+    StepString = "STRING"
+    StepPlot = "PLOT"
+    StepImage = "IMAGE"
 
-class IterationStepArtifact(dict):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    @property
-    def dataset_version_id(self) -> int | None:
-        if self.get("datasetVersionId"):
-            return int(self["datasetVersionId"])
-        else:
-            return None
-
-    @property
-    def model_version_id(self) -> int | None:
-        if self.get("modelVersionId"):
-            return int(self["modelVersionId"])
-        else:
-            return None
-
-    @property
-    def entity_file_id(self) -> int | None:
-        if self.get("entityFileId"):
-            return int(self["entityFileId"])
-        else:
-            return None
-
-    @property
-    def type(self) -> IterationStepArtifactType:
-        return IterationStepArtifactType(self["type"])
-
-
-class IterationStepArtifactInput(dict):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
 
+class StepInput(dict):
     @property
     def id(self) -> int:
         return int(self["id"])
 
     @property
-    def type(self) -> str:
-        return str(self["type"])
+    def index(self) -> int:
+        return int(self["index"])
 
     @property
-    def dataset_version_id(self) -> int | None:
-        if self.get("datasetVersionId"):
-            return int(self["datasetVersionId"])
-        else:
-            return None
+    def name(self) -> str:
+        return str(self["name"])
 
     @property
-    def model_version_id(self) -> int | None:
-        if self.get("modelVersionId"):
-            return int(self["modelVersionId"])
-        else:
-            return None
+    def completed(self) -> bool:
+        return bool(self["completed"])
 
     @property
-    def entity_file_id(self) -> int | None:
-        if self.get("entityFileId"):
-            return int(self["entityFileId"])
-        else:
-            return None
-
+    def description(self) -> str | None:
+        return str(self["description"])
 
-class IterationInput(dict):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    @property
+    def artifacts(self) -> list[IterationStepArtifact]:
+        # TODO: refactor to break cyclic import
+        from vectice.api.json.iteration import IterationStepArtifact
 
-    from vectice.api.json.step import StepInput
+        return [IterationStepArtifact(artifact) for artifact in self["artifacts"]]
 
     @property
-    def steps(self) -> list[StepInput]:
-        steps_json = self["steps"]
-        return [StepInput(step) for step in steps_json]
+    def step_type(self) -> StepType:
+        return StepType(self["stepType"])
 
 
-class IterationOutput(dict):
+class StepOutput(dict):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        if "phase" in self:
+            self._phase: PhaseOutput = PhaseOutput(**self["phase"])
+        else:
+            self._phase = None
+        if "slug" in self:
+            self["slug"] = f"step_{self['slug']}"
 
     @property
     def id(self) -> int:
         return int(self["id"])
 
     @property
     def index(self) -> int:
         return int(self["index"])
 
     @property
-    def phase(self) -> PhaseOutput:
-        return PhaseOutput(**self["phase"])
+    def parent(self) -> PhaseOutput:
+        return self._phase
+
+    @property
+    def name(self) -> str:
+        return str(self["name"])
 
     @property
-    def steps(self) -> list[StepOutput]:
-        from vectice.api.json.step import StepOutput
+    def completed(self) -> bool:
+        return bool(self["completed"])
 
-        steps_json = self["steps"]
-        steps = [StepOutput(step) for step in steps_json]
-        return steps
+    @property
+    def description(self) -> str | None:
+        return str(self["description"])
+
+    @property
+    def slug(self) -> str:
+        return str(self["slug"])
 
     @property
-    def alias(self) -> str:
-        return str(self["alias"])
+    def artifacts(self) -> list[IterationStepArtifact]:
+        # TODO: refactor to break cyclic import
+        from vectice.api.json.iteration import IterationStepArtifact
+
+        return [IterationStepArtifact(artifact) for artifact in self["artifacts"]]
 
     @property
-    def status(self) -> IterationStatus:
-        return IterationStatus(self["status"])
+    def step_type(self) -> StepType:
+        return StepType(self["stepType"])
```

### Comparing `vectice-23.2.2.1/src/vectice/api/json/last_assets.py` & `vectice-23.2.3.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/metric.py` & `vectice-23.2.3.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/model.py` & `vectice-23.2.3.0/src/vectice/api/json/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         return read_nodejs_date(str(self["deletedDate"]))
 
     @property
     def version(self) -> int:
         return int(self["version"])
 
     @property
-    def id(self) -> int:
-        return int(self["id"])
+    def id(self) -> str:
+        return str(self["vecticeId"])
 
     @property
     def name(self) -> str:
         return str(self["name"])
 
     @property
     def project(self) -> ProjectOutput:
```

### Comparing `vectice-23.2.2.1/src/vectice/api/json/model_register.py` & `vectice-23.2.3.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/model_version.py` & `vectice-23.2.3.0/src/vectice/api/json/model_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,16 +107,16 @@
         return ArtifactVersion(version_number=self.version_number, version_name=self.name, version_id=self.id)
 
     @property
     def version_number(self) -> int:
         return int(self["versionNumber"])
 
     @property
-    def id(self) -> int:
-        return int(self["id"])
+    def id(self) -> str:
+        return str(self["vecticeId"])
 
     @property
     def author_id(self) -> int:
         return int(self["authorId"])
 
     @property
     def deleted_date(self) -> datetime | None:
```

### Comparing `vectice-23.2.2.1/src/vectice/api/json/paged_response.py` & `vectice-23.2.3.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/project.py` & `vectice-23.2.3.0/src/vectice/api/json/dataset_representation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,50 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from vectice.api._utils import read_nodejs_date
-from vectice.api.json.workspace import WorkspaceOutput
+from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
+from vectice.models.resource.metadata.base import DatasetSourceOrigin, DatasetType
 
 if TYPE_CHECKING:
     from datetime import datetime
 
 
-class ProjectInput(dict):
+class DatasetRepresentationOutput(dict):
     @property
-    def name(self) -> str:
-        return str(self["name"])
-
-    @property
-    def description(self) -> str:
-        return str(self["description"])
-
-
-class ProjectOutput(dict):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        if "workspace" in self:
-            self._workspace: WorkspaceOutput = WorkspaceOutput(**self["workspace"])
-
-    def items(self):
-        result = []
-        for key in self:
-            if self[key] is not None:
-                result.append((key, self[key]))
-        return result
+    def created_date(self) -> datetime | None:
+        return read_nodejs_date(str(self["createdDate"]))
 
     @property
-    def workspace_id(self) -> int:
-        return int(self["workspaceId"])
+    def updated_date(self) -> datetime | None:
+        return read_nodejs_date(str(self["updatedDate"]))
 
     @property
-    def id(self) -> int:
-        return int(self["id"])
+    def id(self) -> str:
+        return str(self["vecticeId"])
 
     @property
     def name(self) -> str:
         return str(self["name"])
 
     @property
-    def description(self) -> str | None:
-        if "description" in self and self["description"] is not None:
-            return str(self["description"])
-        else:
-            return None
+    def type(self) -> DatasetType:
+        return DatasetType[self["type"]]
 
     @property
-    def created_date(self) -> datetime | None:
-        return read_nodejs_date(str(self["createdDate"]))
+    def origin(self) -> DatasetSourceOrigin:
+        return DatasetSourceOrigin[self["sourceOrigin"]]
 
     @property
-    def updated_date(self) -> datetime | None:
-        return read_nodejs_date(str(self["updatedDate"]))
-
-    @property
-    def deleted_date(self) -> datetime | None:
-        return read_nodejs_date(str(self["deletedDate"]))
+    def description(self) -> str | None:
+        return str(self["description"]) if self["description"] else None
 
     @property
-    def version(self) -> int:
-        return int(self["version"])
+    def version(self) -> DatasetVersionRepresentationOutput:
+        return DatasetVersionRepresentationOutput(**self["lastVersion"])
 
     @property
-    def workspace(self) -> WorkspaceOutput:
-        return self._workspace
+    def project_id(self) -> str | None:
+        if "project" in self:
+            return str(self["project"]["vecticeId"])
+        return None
```

### Comparing `vectice-23.2.2.1/src/vectice/api/json/property.py` & `vectice-23.2.3.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/public_config.py` & `vectice-23.2.3.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/json/workspace.py` & `vectice-23.2.3.0/src/vectice/api/json/model_version_representation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,49 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 from vectice.api._utils import read_nodejs_date
+from vectice.api.json.model_version import ModelVersionStatus
 
 if TYPE_CHECKING:
     from datetime import datetime
 
 
-@dataclass
-class WorkspaceInput:
-    name: str | None
-    description: str | None
-
-
-class WorkspaceOutput(dict):
-    def items(self):
-        result = []
-        for key in self:
-            if self[key] is not None:
-                result.append((key, self[key]))
-        return result
+class ModelVersionRepresentationOutput(dict):
+    @property
+    def created_date(self) -> datetime | None:
+        return read_nodejs_date(str(self["createdDate"]))
 
     @property
-    def organization_id(self) -> int:
-        return int(self["organizationId"])
+    def updated_date(self) -> datetime | None:
+        return read_nodejs_date(str(self["updatedDate"]))
 
     @property
-    def id(self) -> int:
-        return int(self["id"])
+    def id(self) -> str:
+        return str(self["vecticeId"])
 
     @property
     def name(self) -> str:
         return str(self["name"])
 
     @property
-    def description(self) -> str | None:
-        if "description" in self and self["description"] is not None:
-            return str(self["description"])
-        else:
-            return None
+    def status(self) -> ModelVersionStatus:
+        return ModelVersionStatus[self["status"]]
 
     @property
-    def created_date(self) -> datetime | None:
-        return read_nodejs_date(str(self["createdDate"]))
+    def description(self) -> str | None:
+        return str(self["description"]) if self["description"] else None
 
     @property
-    def updated_date(self) -> datetime | None:
-        return read_nodejs_date(str(self["updatedDate"]))
+    def technique(self) -> str | None:
+        return str(self["algorithmName"]) if self["algorithmName"] else None
 
     @property
-    def deleted_date(self) -> datetime | None:
-        return read_nodejs_date(str(self["deletedDate"]))
+    def library(self) -> str | None:
+        return str(self["framework"]) if self["framework"] else None
 
     @property
-    def version(self) -> int:
-        return int(self["version"])
+    def project_id(self) -> str | None:
+        if "model" in self:
+            return str(self["model"]["project"]["vecticeId"])
+        return None
```

### Comparing `vectice-23.2.2.1/src/vectice/api/phase.py` & `vectice-23.2.3.0/src/vectice/api/phase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,141 @@
 from __future__ import annotations
 
 import logging
+import re
 from typing import TYPE_CHECKING
 
 from gql import gql
 from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
+from vectice.utils.api_utils import INDEX_ORDERED, PAGINATE_OUTPUT, get_phase_input
+from vectice.utils.vectice_ids_regex import PHASE_VID_REG
 
 if TYPE_CHECKING:
+    from vectice.api.json.paged_response import PagedResponse
     from vectice.api.json.phase import PhaseOutput
     from vectice.api.json.step import StepOutput
 
 
-_RETURNS = """id
+_RETURNS = """vecticeId
               name
               status
               index
               owner {
-                    name
+                name
               }
               __typename
             """
 
+_RETURNS_LIST = f"""
+    {_RETURNS}
+    iterationsCount {{
+        notStarted
+        inProgress
+        inReview
+        total
+    }}
+    stepsCount
+"""
+
+_RETURNS_PAGE = PAGINATE_OUTPUT.format(_RETURNS_LIST)
+
+_PARENT_FULL = """
+                parent {
+                    vecticeId
+                    name
+                    description
+                    workspace {
+                        vecticeId
+                        name
+                        description
+                        __typename
+                    }
+                    __typename
+                }
+"""
+
+_RETURNS_FULL = f"""
+    {_RETURNS}
+    {_PARENT_FULL}
+"""
+
 _STEP_DEFINITION_RETURNS = """id
               name
               index
               slug
               description
               __typename
             """
 
 
 _logger = logging.getLogger(__name__)
 
 
 class PhaseApi(GqlApi):
-    def list_phases(self, parent_id: int, search_alias: str | None = None) -> list[PhaseOutput]:
-        alias_filter = {
-            "parentId": parent_id,
-            "searchFilter": {"search": search_alias if search_alias is not None else "", "fields": "name"},
-        }
+    def list_phases(self, parent_id: str) -> PagedResponse[PhaseOutput]:
+        gql_query = "getPhaseList"
 
-        variable_types = "$filters:PhaseFiltersInput!"
-        kw = "filters:$filters"
-        variables = {"filters": alias_filter}
-        returns = f"""items{{
-                    {_RETURNS}
-        }}"""
+        variable_types = "$filters:PhaseFiltersInput!,$order:ListOrderInput,$page:PageInput"
+        kw = "filters:$filters,order:$order,page:$page"
+        variables = {
+            "filters": {
+                "parentId": parent_id,
+            },
+            "order": INDEX_ORDERED,
+            "page": get_phase_input(),
+        }
         query = GqlApi.build_query(
-            gql_query="getPhaseList", variable_types=variable_types, returns=returns, keyword_arguments=kw, query=True
+            gql_query=gql_query, variable_types=variable_types, returns=_RETURNS_PAGE, keyword_arguments=kw
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
-            phase_output: list[PhaseOutput] = Parser().parse(response["getPhaseList"]["items"])  # type: ignore[assignment]
+            phase_output: PagedResponse[PhaseOutput] = Parser().parse_paged_response(response[gql_query])
             return phase_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "phase", "list")
 
-    def get_phase(self, phase: str | int, parent_id: int | None = None) -> PhaseOutput:
-        if isinstance(phase, int):
+    def get_phase(self, phase: str, parent_id: str | None = None, full: bool = False) -> PhaseOutput:
+        if re.search(PHASE_VID_REG, phase):
             gql_query = "getPhaseById"
             variable_types = "$id:VecticeId!"
             variables = {"id": phase}
             kw = "id:$id"
-        elif isinstance(phase, str) and parent_id:
+        elif parent_id:
             gql_query = "getPhaseByName"
             variable_types = "$name:String!,$parentId:VecticeId!"
-            variables = {"name": phase, "parentId": parent_id}  # type: ignore[dict-item]
+            variables = {"name": phase, "parentId": parent_id}
             kw = "name:$name,parentId:$parentId"
         else:
             raise ValueError("Missing parameters: string and parent id required.")
         query = GqlApi.build_query(
-            gql_query=gql_query, variable_types=variable_types, returns=_RETURNS, keyword_arguments=kw, query=True
+            gql_query=gql_query,
+            variable_types=variable_types,
+            returns=_RETURNS_FULL if full else _RETURNS,
+            keyword_arguments=kw,
+            query=True,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             phase_output: PhaseOutput = Parser().parse_item(response[gql_query])
             return phase_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "phase", phase)
 
-    def list_step_definitions(self, parent_id: int) -> list[StepOutput]:
+    def list_step_definitions(self, parent_id: str) -> list[StepOutput]:
         alias_filter = {"parentId": parent_id, "search": ""}
         returns = f"""items{{
                                     {_STEP_DEFINITION_RETURNS}
                         }}"""
-        variable_types = "$filters:BaseDocumentationListFiltersInput!"
-        kw = "filters:$filters"
-        variables = {"filters": alias_filter}
+        variable_types = "$filters:BaseDocumentationListFiltersInput!,$order:ListOrderInput"
+        kw = "filters:$filters,order:$order"
+        variables = {"filters": alias_filter, "order": INDEX_ORDERED}
         query = GqlApi.build_query(
             gql_query="getStepDefinitionList",
             variable_types=variable_types,
             returns=returns,
             keyword_arguments=kw,
             query=True,
         )
```

### Comparing `vectice-23.2.2.1/src/vectice/api/rest_api.py` & `vectice-23.2.3.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/api/step.py` & `vectice-23.2.3.0/src/vectice/api/step.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,93 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 from gql import gql
 
+from vectice.utils.api_utils import INDEX_ORDERED
+
 if TYPE_CHECKING:
-    from vectice.api.json import IterationOutput, IterationStepArtifactInput, StepOutput
-    from vectice.api.json.step import StepUpdateInput
+    from vectice.api.json import IterationStepArtifactInput, StepOutput
 
 from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
 from vectice.api.json.step import StepType
 
 _logger = logging.getLogger(__name__)
 
 _RETURNS_WITH_STEPS = """
-                steps {
+                items {
                     id
                     index
                     name
                     completed
                     description
                     stepType
-                    text
                     slug
                     artifacts {
                                 entityFileId
-                                modelVersionId
-                                datasetVersionId
+                                modelVersion {
+                                    vecticeId
+                                }
+                                datasetVersion {
+                                    vecticeId
+                                }
+                                text
                                 type
                     }
                     __typename
                 }
-                phase {
-                    name
-                }
-              __typename
             """
 
 _RETURNS = """
                 id
                 index
                 name
                 completed
                 description
                 stepType
-                text
                 slug
                 artifacts {
                                 entityFileId
-                                modelVersionId
-                                datasetVersionId
+                                modelVersion {
+                                    vecticeId
+                                }
+                                datasetVersion {
+                                    vecticeId
+                                }
+                                text
                                 type
                     }
                 __typename
             """
 
 
 class StepApi(GqlApi):
-    def list_steps(self, phase_id: int, phase_name: str | None) -> list[StepOutput]:
-        gql_query = "getActiveIterationOrCreateOne"
-        variable_types = "$phaseId:VecticeId!"
-        variables = {"phaseId": phase_id}
-        kw = "phaseId:$phaseId"
-        query = GqlApi.build_query(
-            gql_query=gql_query,
-            variable_types=variable_types,
-            returns=_RETURNS_WITH_STEPS,
-            keyword_arguments=kw,
-            query=True,
-        )
-        query_built = gql(query)
-        try:
-            response = self.execute(query_built, variables)
-            iteration_output: IterationOutput = Parser().parse_item(response[gql_query])
-            step_output: list[StepOutput] = iteration_output.steps
-            return step_output
-        except TransportQueryError as e:
-            phase_ref: int | str = phase_name if phase_name else phase_id
-            self._error_handler.handle_post_gql_error(e, "steps", phase_ref)
-
-    def list_steps_for_iteration(
-        self, phase_id: int, iteration_index: int, phase_name: str | None = None
-    ) -> list[StepOutput]:
-        gql_query = "getIterationByIndex"
-        variable_types = "$index:Float!,$phaseId:VecticeId!"
-        variables = {"index": iteration_index, "phaseId": phase_id}
-        kw = "index:$index,phaseId:$phaseId"
+    def list_steps(self, iteration_id: str) -> list[StepOutput]:
+        gql_query = "getIterationStepList"
+        variable_types = "$parentId:VecticeId!,$order:ListOrderInput"
+        variables = {"parentId": iteration_id, "order": INDEX_ORDERED}
+        kw = "parentId:$parentId,order:$order"
         query = GqlApi.build_query(
             gql_query=gql_query,
             variable_types=variable_types,
             returns=_RETURNS_WITH_STEPS,
             keyword_arguments=kw,
             query=True,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
-            iteration_output: IterationOutput = Parser().parse_item(response[gql_query])
-            step_output: list[StepOutput] = iteration_output.steps
+            step_output: list[StepOutput] = Parser().parse_list(response[gql_query]["items"])
             return step_output
         except TransportQueryError as e:
-            phase_ref: int | str = phase_name if phase_name else phase_id
-            self._error_handler.handle_post_gql_error(e, "steps", phase_ref)
-
-    def close_step(self, step_id: int, step_update: StepUpdateInput) -> StepOutput:
-        gql_query = "completeIterationStep"
-        variable_types = "$id:Float!,$data:IterationStepUpdateInput"
-        variables = {"id": step_id, "data": step_update}
-        kw = "id:$id, data:$data"
-        query = GqlApi.build_query(
-            gql_query=gql_query,
-            variable_types=variable_types,
-            returns=_RETURNS,
-            keyword_arguments=kw,
-            query=False,
-        )
-        query_built = gql(query)
-        try:
-            response = self.execute(query_built, variables)
-            step_output: StepOutput = Parser().parse_item(response[gql_query])
-            return step_output
-        except TransportQueryError as e:
-            self._error_handler.handle_post_gql_error(e, "step", step_id)
+            self._error_handler.handle_post_gql_error(e, "iteration", iteration_id)
 
     def add_iteration_step_artifact(self, data: IterationStepArtifactInput, step_id: int) -> StepOutput:
         gql_query = "addIterationStepArtifact"
         variable_types = "$id:Float!,$data:IterationStepArtifactInput!"
         variables = {"id": step_id, "data": data}
         kw = "id:$id, data:$data"
         query = GqlApi.build_query(
@@ -146,24 +105,22 @@
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "step", step_id)
 
     def update_iteration_step_artifact(
         self,
         step_id: int,
         step_type: StepType,
-        text: str | None = None,
         artifacts: list[IterationStepArtifactInput] | None = None,
     ) -> StepOutput:
         gql_query = "updateIterationStepContent"
         variable_types = "$id:Float!,$data:IterationStepUpdateInput!"
         variables: dict = {
             "id": step_id,
             "data": {
                 "stepType": step_type.value,
-                "text": str(text) if text else None,
             },
         }
         if artifacts:
             variables["data"]["artifacts"] = artifacts
         kw = "id:$id, data:$data"
         query = GqlApi.build_query(
             gql_query=gql_query,
@@ -174,17 +131,18 @@
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             step_output: StepOutput = Parser().parse_item(response[gql_query])
             return step_output
         except TransportQueryError as e:
+            print(e)
             self._error_handler.handle_post_gql_error(e, "step", step_id)
 
-    def get_step(self, step: str, iteration_id: int) -> StepOutput:
+    def get_step(self, step: str, iteration_id: str) -> StepOutput:
         if isinstance(step, str) and iteration_id:
             gql_query = "getStepByName"
             variable_types = "$name:String!,$parentId:VecticeId!"
             variables = {"name": step, "parentId": iteration_id}
             kw = "name:$name,parentId:$parentId"
         else:
             raise ValueError("Missing parameters: string and parent id required.")
```

### Comparing `vectice-23.2.2.1/src/vectice/api/version.py` & `vectice-23.2.3.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/__init__.py` & `vectice-23.2.3.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/attachment_container.py` & `vectice-23.2.3.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/dataset.py` & `vectice-23.2.3.0/src/vectice/models/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
+from typing import Union
 
 from vectice.models.property import Property
+from vectice.models.representation.dataset_representation import DatasetRepresentation
+from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.resource.base import Resource
 from vectice.models.resource.bigquery_resource import BigQueryResource
 from vectice.models.resource.metadata.base import DatasetSourceUsage, DatasetType
 
 _logger = logging.getLogger(__name__)
 
 
+TBaseDerivedFrom = Union[str, DatasetRepresentation, DatasetVersionRepresentation]
+
+
 class Dataset:
     def __init__(
         self,
         type: DatasetType,
         name: str | None = None,
         resource: Resource | None = None,
         training_resource: Resource | None = None,
         testing_resource: Resource | None = None,
         validation_resource: Resource | None = None,
-        derived_from: list[int | Dataset] | None = None,
+        derived_from: list[TBaseDerivedFrom | Dataset] | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
         attachments: str | list[str] | None = None,
     ):
         """Initialize a dataset.
 
         Users should not instantiate a dataset directly but rather use the provided static methods
         [`origin()`][vectice.models.dataset.Dataset.origin],
@@ -37,33 +43,22 @@
             resource: A single resource (for origin and clean datasets).
             training_resource: The resource for the training set (for modeling datasets).
             testing_resource: The resource for the testing set (for modeling datasets).
             validation_resource: The resource for the validation set (optional, for modeling datasets).
             derived_from: A list of datasets (or ids) from which this dataset is derived.
             attachments: Path of a file that will be attached to the step along with the dataset.
         """
-        derived_from_ids = []
-        for df in derived_from or []:
-            if isinstance(df, Dataset):
-                if df.latest_version_id is None:
-                    raise ValueError(
-                        f"Dataset '{df.name}' does not have a version id. "
-                        "Was it registered in Vectice (assigned to a step)?"
-                    )
-                derived_from_ids.append(df.latest_version_id)
-            else:
-                derived_from_ids.append(df)
         self._type = type
         self._name = name or f"dataset {datetime.time}"
         self._resource = resource
         self._training_resource = training_resource
         self._testing_resource = testing_resource
         self._validation_resource = validation_resource
-        self._derived_from = derived_from_ids
-        self._latest_version_id: int | None = None
+        self._derived_from = _get_derived_from(derived_from)
+        self._latest_version_id: str | None = None
         self._properties = self._format_properties(properties) if properties else None
         self._attachments = self._format_attachments(attachments) if attachments else None
 
         if self._type is DatasetType.MODELING:
             if self._training_resource is None or self._testing_resource is None:
                 raise ValueError("You cannot create a modeling dataset without both training and testing sets")
 
@@ -118,15 +113,15 @@
             attachments=attachments,
         )
 
     @staticmethod
     def clean(
         resource: Resource,
         name: str | None = None,
-        derived_from: list[int | Dataset] | None = None,
+        derived_from: list[str | Dataset | DatasetRepresentation | DatasetVersionRepresentation] | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
         attachments: str | list[str] | None = None,
     ) -> Dataset:
         """Create a clean dataset.
 
         Examples:
             ```python
@@ -233,33 +228,33 @@
 
         Parameters:
             name: The name of the dataset.
         """
         self._name = name
 
     @property
-    def derived_from(self) -> list[int]:
+    def derived_from(self) -> list[str]:
         """The datasets from which this dataset is derived.
 
         Returns:
             The datasets from which this dataset is derived.
         """
         return self._derived_from
 
     @property
-    def latest_version_id(self) -> int | None:
+    def latest_version_id(self) -> str | None:
         """The id of the latest version of this dataset.
 
         Returns:
             The id of the latest version of this dataset.
         """
         return self._latest_version_id
 
     @latest_version_id.setter
-    def latest_version_id(self, value: int) -> None:
+    def latest_version_id(self, value: str) -> None:
         """Set the id of the latest version of this dataset.
 
         Parameters:
             value: The id of the latest version of this dataset.
         """
         self._latest_version_id = value
 
@@ -326,7 +321,31 @@
     @staticmethod
     def _remove_incorrect_properties(properties: list[Property]) -> list[Property]:
         for prop in properties:
             if not isinstance(prop, Property):
                 _logger.warning(f"Incorrect property '{prop}'. Please check property type.")
                 properties.remove(prop)
         return properties
+
+
+TDerivedFrom = Union[TBaseDerivedFrom, Dataset]
+
+
+def _get_derived_from(
+    derived_from: list[TDerivedFrom] | None,
+) -> list[str]:
+    derived_from_ids: list[str] = []
+    for df in derived_from or []:
+        if isinstance(df, Dataset):
+            if df.latest_version_id is None:
+                raise ValueError(
+                    f"Dataset {df.name!r} does not have a version id. "
+                    "Was it registered in Vectice (assigned to a step)?"
+                )
+            derived_from_ids.append(df.latest_version_id)
+        elif isinstance(df, DatasetRepresentation):
+            derived_from_ids.append(df.version.id)
+        elif isinstance(df, DatasetVersionRepresentation):
+            derived_from_ids.append(df.id)
+        else:
+            derived_from_ids.append(df)
+    return derived_from_ids
```

### Comparing `vectice-23.2.2.1/src/vectice/models/git_version.py` & `vectice-23.2.3.0/src/vectice/models/git_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return self._user_declared_version
 
     @property
     def git_version(self) -> GitVersion | None:
         return self._git_version
 
 
-def _check_code_source(client: Client, project_id: int, _logger: Logger) -> int | None:
+def _check_code_source(client: Client, project_id: str, _logger: Logger) -> int | None:
     """Capture source code.
 
     Naive implementation that uses the commit hash to name the code.
 
     Only one version of the code is stored in backend.
     This allows to easily reuse versions based on their commits hash.
 
@@ -84,15 +84,15 @@
     code_version_output = client.create_code_version_gql(code_output.id, code_version_body)
     _logger.debug("Code captured and will be linked to asset.")
     code_version_id = int(code_version_output.id)
     _capture_local_changed_files(repository, client, project_id, code_version_id)
     return code_version_id
 
 
-def _capture_local_changed_files(repository: Repo, client: Client, project_id: int, code_version_id: int) -> None:
+def _capture_local_changed_files(repository: Repo, client: Client, project_id: str, code_version_id: int) -> None:
     diff_outputs = []
     file_names = []
     try:
         changed_files: list[Diff] = repository.index.diff(None)
     except Exception as error:
         changed_files = []
         _logger.warning(
@@ -128,15 +128,15 @@
             f"Code capture failed: {error.__class__.__name__}: {error_message}. "
             "Make sure the current directory is a valid Git repository (non-bare, non worktree) "
             "and its permissions allow the current user to access it."
         )
         return None
 
 
-def _check_for_code(client: Client, project_id: int, _logger: Logger) -> int | None:
+def _check_for_code(client: Client, project_id: str, _logger: Logger) -> int | None:
     code_version_id = None
 
     if vectice.code_capture:
         code_version_id = _check_code_source(client, project_id, _logger)
     return code_version_id
```

### Comparing `vectice-23.2.2.1/src/vectice/models/iteration.py` & `vectice-23.2.3.0/src/vectice/models/iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         "_current_step",
         "_steps",
         "__dict__",
     ]
 
     def __init__(
         self,
-        id: int,
+        id: str,
         index: int,
         phase: Phase,
         status: IterationStatus = IterationStatus.NotStarted,
     ):
         """Initialize an iteration.
 
         Vectice users shouldn't need to instantiate Iterations manually,
@@ -133,15 +133,14 @@
                 name=step.name,
                 index=step.index,
                 slug=step.slug,
                 description=step.description,
                 completed=step.completed,
                 artifacts=step.artifacts,
                 step_type=step.step_type,
-                text=step.text,
             )
             return step_object
         raise AttributeError(f"The attribute '{item}' does not exist.")
 
     def __setattr__(self, attr_name, attr_value):
         if hasattr(self, "_steps") and attr_name in super().__getattribute__("_steps"):
             if self._status in {IterationStatus.Abandoned, IterationStatus.Completed}:
@@ -149,24 +148,24 @@
             self._steps[attr_name] = self._steps[attr_name]._step_factory_and_update(value=attr_value)
         elif hasattr(self, "__dict__") and attr_name not in self.__slots__:
             raise AttributeError(f"The attribute '{attr_name}' does not exist.")
         else:
             super().__setattr__(attr_name, attr_value)
 
     @property
-    def id(self) -> int:
+    def id(self) -> str:
         """The iteration's identifier.
 
         Returns:
             The iteration's identifier.
         """
         return self._id
 
     @id.setter
-    def id(self, iteration_id: int):
+    def id(self, iteration_id: str):
         """Set the iteration's identifier.
 
         Parameters:
             iteration_id: The identifier.
         """
         _check_read_only(self)
         self._id = iteration_id
@@ -210,63 +209,61 @@
     @property
     def steps(self) -> list[Step]:
         """The steps required in this iteration.
 
         Returns:
             The steps required in this iteration.
         """
-        steps_output = self._client.list_steps(self._phase.id, self.index, self._phase.name)
+        steps_output = self._client.list_steps(self.id)
         return [
             _get_step_type(
                 id=item.id,
                 iteration=self,
                 name=item.name,
                 index=item.index,
                 slug=item.slug,
                 description=item.description,
                 completed=item.completed or None,
                 artifacts=item.artifacts,
                 step_type=item.step_type,
             )
-            for item in sorted(steps_output, key=lambda x: x.index)
+            for item in steps_output
         ]
 
     def list_steps(self) -> None:
         """Prints a list of steps belonging to the iteration in a tabular format, limited to the first 10 items. A link is provided to view the remaining steps.
 
         Returns:
             None
         """
-        steps_output = sorted(self._client.list_steps(self.phase.id, self.index), key=lambda x: x.index)
+        steps_output = self._client.list_steps(self.id)
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
         rich_table = Table(expand=True, show_edge=False)
 
         rich_table.add_column("index", justify="left", no_wrap=True, min_width=5, max_width=5)
         rich_table.add_column("shortcut", justify="left", no_wrap=True, min_width=5, max_width=20)
         rich_table.add_column("artifacts", justify="left", no_wrap=True, min_width=5, max_width=15)
-        rich_table.add_column("comment", justify="left", no_wrap=True, min_width=5, max_width=20)
 
         for count, step in enumerate(steps_output, 1):
             if count > 10:
                 break
-            step_text = 1 if step.text != "None" else 0
-            number_of_artifacts = len(step.artifacts) + step_text
-            rich_table.add_row(str(count), step.slug, str(number_of_artifacts), "True" if step_text == 1 else "False")
+            number_of_artifacts = len(step.artifacts)
+            rich_table.add_row(str(count), step.slug, str(number_of_artifacts))
 
         description = f"""There are {len(steps_output)} steps in Iteration '{self.index!r}' and a maximum of 10 steps are displayed in the table below:"""
         tips = dedent(
             """
         To access a specific step, use the step shortcut \033[1iiteration\033[0m.step_my_step_name
         The step reference is referred to as shortcut"""
         ).lstrip()
         link = dedent(
             f"""
         For quick access to the list of steps in the Vectice web app, visit:
-        {self._client.auth._API_BASE_URL}/project/phase/iteration?w={self.workspace.id}&iterationId={self.id}"""
+        {self._client.auth._API_BASE_URL}/browse/iteration/{self.id}"""
         ).lstrip()
 
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(tips)
         _temp_print(link)
 
@@ -285,15 +282,15 @@
         self._client.update_iteration(self.id, iteration_input)
         self._status = IterationStatus.Completed
         logging_output = dedent(
             f"""
                         Iteration with index {self.index} completed.
 
                         For quick access to the Iteration in the Vectice web app, visit:
-                        {self._client.auth._API_BASE_URL}/project/phase/iteration?w={self.workspace.id}&iterationId={self.id}"""
+                        {self._client.auth._API_BASE_URL}/browse/iteration/{self.id}"""
         ).lstrip()
         _logger.info(logging_output)
 
     def delete(self) -> None:
         self._client.delete_iteration(self.id)
         _logger.info(f"Iteration with index {self.index} was deleted.")
```

### Comparing `vectice-23.2.2.1/src/vectice/models/metric.py` & `vectice-23.2.3.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/model.py` & `vectice-23.2.3.0/src/vectice/models/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 import pickle  # nosec
 from typing import Any
 
 from vectice.models import Metric, Property
+from vectice.models.dataset import TDerivedFrom, _get_derived_from
 
 _logger = logging.getLogger(__name__)
 
 
 class Model:
     """Represent a wrapped model.
 
@@ -23,39 +24,39 @@
         library: str,
         technique: str,
         metrics: dict[str, int] | list[Metric] | Metric | None = None,
         properties: dict[str, str] | dict[str, int] | list[Property] | Property | None = None,
         name: str | None = None,
         attachments: str | list[str] | None = None,
         predictor: Any = None,
-        derived_from: list[int] | None = None,
+        derived_from: list[TDerivedFrom] | None = None,
     ):
         """Wrap a model (predictor).
 
         A Vectice Model is a wrapped predictor suitable for assignment
         to a Vectice Step.
 
         Parameters:
             library: The library used to generate the model.
             technique: The modeling technique used.
             metrics: A dict for example `{"MSE": 1}`.
             properties: A dict, for example `{"folds": 32}`.
             name: The model name. If None, will be auto-generated based on the library and technique.
             attachments: Path of a file that will be attached to the step along with the predictor.
             predictor: The predictor.
-            derived_from: List of dataset version ids to link as lineage.
+            derived_from: List of dataset (or version ids) to link as lineage.
         """
         self._library = library
         self._technique = technique
         self._name = name if name else self._generate_name()
         self._metrics = self._format_metrics(metrics) if metrics else None
         self._properties = self._format_properties(properties) if properties else None
         self._attachments = self._format_attachments(attachments) if attachments else None
         self._predictor = pickle.dumps(predictor)  # nosec
-        self._derived_from = derived_from
+        self._derived_from = _get_derived_from(derived_from)
 
     def __repr__(self):
         return (
             f"Model(name='{self.name}', library='{self.library}', technique='{self.technique}', "
             f"metrics={self.metrics}, properties={self.properties}, attachments={self.attachments})"
         )
 
@@ -187,15 +188,15 @@
 
         Parameters:
             attachments: The filename or filenames of the file or set of files to attach to the model.
         """
         self._attachments = self._format_attachments(attachments)
 
     @property
-    def derived_from(self) -> Any:
+    def derived_from(self) -> list[str]:
         """The datasets from which this model is derived.
 
         Returns:
             The datasets from which this model is derived.
         """
         return self._derived_from
```

### Comparing `vectice-23.2.2.1/src/vectice/models/phase.py` & `vectice-23.2.3.0/src/vectice/models/phase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import logging
+import re
 from textwrap import dedent
 from typing import TYPE_CHECKING
 
 from rich.table import Table
 
+from vectice.api.http_error_handlers import InvalidReferenceError
 from vectice.api.json.phase import PhaseStatus
 from vectice.models.iteration import Iteration
 from vectice.utils.common_utils import _temp_print
 from vectice.utils.last_assets import _get_last_user_and_default_workspace
-from vectice.utils.logging_utils import format_description
+from vectice.utils.logging_utils import format_description, get_iteration_status
+from vectice.utils.vectice_ids_regex import ITERATION_VID_REG
 
 if TYPE_CHECKING:
     from vectice import Connection
     from vectice.api import Client
     from vectice.models import Project, Workspace
 
 
@@ -74,15 +77,15 @@
         "_client",
         "_current_iteration",
         "_pointers",
     ]
 
     def __init__(
         self,
-        id: int,
+        id: str,
         project: Project,
         name: str,
         index: int,
         status: PhaseStatus = PhaseStatus.NotStarted,
     ):
         """Initialize a phase.
 
@@ -109,24 +112,24 @@
 
     def __eq__(self, other: object):
         if not isinstance(other, Phase):
             return NotImplemented
         return self.id == other.id
 
     @property
-    def id(self) -> int:
+    def id(self) -> str:
         """The phase's id.
 
         Returns:
             The phase's id.
         """
         return self._id
 
     @id.setter
-    def id(self, phase_id: int):
+    def id(self, phase_id: str):
         """Set the phase's id.
 
         Parameters:
             phase_id: The phase id to set.
         """
         self._id = phase_id
 
@@ -170,25 +173,57 @@
     def iterations(self) -> list[Iteration]:
         """The phase's iterations.
 
         Returns:
             The phase's iterations.
         """
         iteration_outputs = self._client.list_iterations(self.id)
-        return sorted(
-            [Iteration(item.id, item.index, self, item.status) for item in iteration_outputs], key=lambda x: x.index
-        )
+        return [Iteration(item.id, item.index, self, item.status) for item in iteration_outputs.list]
+
+    def list_iterations(self, only_mine: bool = False) -> None:
+        """Prints a list of iterations belonging to the phase in a tabular format, limited to the last 10 items.
+
+        Parameters:
+            only_mine (boolean, default 'False'): Display only the iterations where the user is the owner
+        Returns:
+            None
+
+        """
+        iteration_outputs = self._client.list_iterations(self.id, only_mine)
+        rich_table = Table(expand=True, show_edge=False)
+
+        rich_table.add_column("Id", justify="left", no_wrap=True, min_width=3, max_width=20)
+        rich_table.add_column("Index", justify="left", no_wrap=True, min_width=5, max_width=10)
+        rich_table.add_column("Status", justify="left", no_wrap=True, min_width=3, max_width=15)
+        rich_table.add_column("Owner", justify="left", no_wrap=True, min_width=5, max_width=15)
+
+        for iteration in iteration_outputs.list:
+            rich_table.add_row(
+                str(iteration.id),
+                str(iteration.index),
+                get_iteration_status(iteration.status, iteration.starred),
+                iteration.ownername,
+            )
+        description = f"""There are {iteration_outputs.total} iterations in the phase {self.name!r} and a maximum of 10 iterations are displayed in the table below:"""
+        link = dedent(
+            f"""
+        # For quick access to the list of iterations in the Vectice web app, visit:
+        # {self._client.auth._API_BASE_URL}/phase/{self.id}/iterations?w={self.workspace.id}"""
+        ).lstrip()
+        _temp_print(description)
+        _temp_print(table=rich_table)
+        _temp_print(link)
 
     def list_steps(self) -> None:
-        """Prints a list of step definitionss belonging to the phase in a tabular format, limited to the first 10 items. A link is provided to view the remaining step definitionss.
+        """Prints a list of step definitions belonging to the phase in a tabular format, limited to the first 10 items. A link is provided to view the remaining step definitions.
 
         Returns:
             None
         """
-        steps_output = sorted(self._client.list_step_definitions(self.id), key=lambda x: x.index)
+        steps_output = self._client.list_step_definitions(self.id)
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
         rich_table = Table(expand=True, show_edge=False)
 
         rich_table.add_column("shortcut", justify="left", no_wrap=True, min_width=3, max_width=20)
         rich_table.add_column("name", justify="left", no_wrap=True, min_width=5, max_width=10)
         rich_table.add_column("description", justify="left", no_wrap=True, min_width=3, max_width=15)
@@ -197,45 +232,51 @@
             if count > 10:
                 break
             rich_table.add_row(step.slug, step.name, format_description(step.description))
         description = f"""There are {len(steps_output)} steps required in the phase {self.name!r} and a maximum of 10 steps are displayed in the table below:"""
         link = dedent(
             f"""
         For quick access to the list of step definitions in the Vectice web app, visit:
-        {self._client.auth._API_BASE_URL}/project/phase/steps?w={self.workspace.id}&pageId={self.id}"""
+        {self._client.auth._API_BASE_URL}/phase/{self.id}/steps?w={self.workspace.id}"""
         ).lstrip()
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(link)
 
-    def iteration(self, index: int) -> Iteration:
+    def iteration(self, index: int | str) -> Iteration:
         """Get an iteration.
 
         Fetch and return an iteration by index.
 
         Parameters:
             index: The id of an existing iteration.
 
         Returns:
             An iteration.
         """
-        iteration_output = self._client.get_iteration_by_index(self.id, index)
+        if isinstance(index, str):
+            if re.search(ITERATION_VID_REG, index):
+                iteration_output = self._client.get_iteration(index)
+            else:
+                raise InvalidReferenceError("iteration", index)
+        else:
+            iteration_output = self._client.get_iteration_by_index(self.id, index)
 
         iteration_object = Iteration(
             id=iteration_output.id,
             index=iteration_output.index,
             phase=self,
             status=iteration_output.status,
         )
         logging_output = dedent(
             f"""
                 Iteration number '{iteration_output.index!r}' successfully retrieved."
 
                 For quick access to the Iteration in the Vectice web app, visit:
-                {self._client.auth._API_BASE_URL}/project/phase/iteration?w={self.workspace.id}&iterationId={iteration_object.id}"""
+                {self._client.auth._API_BASE_URL}/browse/iteration/{iteration_object.id}"""
         ).lstrip()
         _logger.info(logging_output)
         self._current_iteration = iteration_object
         return iteration_object
 
     def create_iteration(self) -> Iteration:
         """Create a new iteration.
@@ -247,15 +288,15 @@
         """
         iteration_output = self._client.create_iteration(self.id)
         logging_output = dedent(
             f"""
         New Iteration number '{iteration_output.index!r}' created.
 
         For quick access to the Iteration in the Vectice web app, visit:
-        {self._client.auth._API_BASE_URL}/project/phase/iteration?w={self.workspace.id}&iterationId={iteration_output.id}"""
+        {self._client.auth._API_BASE_URL}/browse/iteration/{iteration_output.id}"""
         ).lstrip()
         _logger.info(logging_output)
 
         iteration_object = Iteration(
             id=iteration_output.id,
             index=iteration_output.index,
             phase=self,
```

### Comparing `vectice-23.2.2.1/src/vectice/models/project.py` & `vectice-23.2.3.0/src/vectice/models/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 
 import logging
 from textwrap import dedent
 from typing import TYPE_CHECKING
 
 from rich.table import Table
 
-from vectice.api.json.iteration import IterationStatus
 from vectice.models.phase import Phase
 from vectice.utils.common_utils import _temp_print
-from vectice.utils.last_assets import _get_last_user_and_default_workspace
 from vectice.utils.logging_utils import get_phase_status
 
 if TYPE_CHECKING:
     from vectice import Connection
     from vectice.models import Workspace
 
 
@@ -50,15 +48,15 @@
     how to connect to Vectice.
     """
 
     __slots__ = ["_id", "_workspace", "_name", "_description", "_phase", "_client", "_pointers"]
 
     def __init__(
         self,
-        id: int,
+        id: str,
         workspace: Workspace,
         name: str,
         description: str | None = None,
     ):
         """Initialize a project.
 
         Vectice users shouldn't need to instantiate Projects manually,
@@ -83,15 +81,15 @@
 
     def __eq__(self, other: object):
         if not isinstance(other, Project):
             return NotImplemented
         return self.id == other.id
 
     @property
-    def id(self) -> int:
+    def id(self) -> str:
         """The project's id.
 
         Returns:
             The project's id.
         """
         return self._id
 
@@ -136,15 +134,15 @@
         """The project's identifiers.
 
         Returns:
             A dictionary containing the `name`, `id` and `workspace` items.
         """
         return {"name": self.name, "id": self.id, "workspace": self.workspace.id}
 
-    def phase(self, phase: str | int) -> Phase:
+    def phase(self, phase: str) -> Phase:
         """Get a phase.
 
         Parameters:
             phase: The name or id of the phase to get.
 
         Returns:
             The specified phase.
@@ -152,86 +150,66 @@
         item = self._client.get_phase(phase, project_id=self._id)
         phase_object = Phase(item.id, self, item.name, item.index, item.status)
         logging_output = dedent(
             f"""
                         Phase {item.name!r} successfully retrieved."
 
                         For quick access to the Phase in the Vectice web app, visit:
-                        {self._client.auth._API_BASE_URL}/project/phase?w={self.workspace.id}&pageId={phase_object.id}"""
+                        {self._client.auth._API_BASE_URL}/browse/phase/{phase_object.id}"""
         ).lstrip()
         _logger.info(logging_output)
 
         self._phase = phase_object
         return phase_object
 
     def list_phases(self) -> None:
         """Prints a list of phases belonging to the project in a tabular format, limited to the first 10 items. A link is provided to view the remaining phases.
 
         Returns:
             None
         """
-        phase_outputs = sorted(self._client.list_phases(project=self.id), key=lambda x: x.index)
-        user_name, _ = _get_last_user_and_default_workspace(self._client)
-
+        phase_outputs = self._client.list_phases(project=self.id)
         rich_table = Table(expand=True, show_edge=False)
 
         rich_table.add_column("phase id", justify="left", no_wrap=True, min_width=3, max_width=5)
         rich_table.add_column("name", justify="left", no_wrap=True, min_width=5, max_width=10)
         rich_table.add_column("owner", justify="left", no_wrap=True, min_width=4, max_width=4)
         rich_table.add_column("status", justify="left", no_wrap=True, min_width=4, max_width=4)
         rich_table.add_column("iterations", justify="left", no_wrap=True, min_width=4, max_width=4)
         rich_table.add_column("steps", justify="left", no_wrap=True, max_width=10)
 
-        for count, phase in enumerate(phase_outputs, 1):
-            if count > 10:
-                break
-            phase_iterations = self._client.list_iterations(phase.id)
-            iterations_total = len(phase_iterations)
-            active_iterations = len(
-                [
-                    iteration
-                    for iteration in phase_iterations
-                    if iteration.status is not (IterationStatus.Completed or IterationStatus.Abandoned)
-                ]
-            )
+        for phase in phase_outputs.list:
             phase_owner = phase["owner"]["name"] if phase.get("owner") else "Unassigned"
             phase_status = get_phase_status(phase.status)
-            phase_steps = self._client.list_step_definitions(phase.id)
-            total_phase_steps = len(phase_steps)
             rich_table.add_row(
-                str(phase.id),
+                phase.id,
                 phase.name,
                 phase_owner,
                 phase_status,
-                f"{active_iterations}/{iterations_total}",
-                str(total_phase_steps),
+                f"{phase.active_iterations_count}/{phase.iterations_count}",
+                str(phase.steps_count),
             )
-        description = f"""There are {len(phase_outputs)} phases in the project {self.name!r} and a maximum of 10 phases are displayed in the table below:"""
+        description = f"""There are {phase_outputs.total} phases in the project {self.name!r} and a maximum of 10 phases are displayed in the table below:"""
         tips = dedent(
             """
         To access a specific phase, use \033[1mproject\033[0m.phase(Phase ID)"""
         ).lstrip()
         link = dedent(
             f"""
         For quick access to the list of phases for this project, visit:
-        {self._client.auth._API_BASE_URL}/project?w={self.workspace.id}&resourceId={self.id}"""
+        {self._client.auth._API_BASE_URL}/browse/project/{self.id}"""
         ).lstrip()
-        legend = """**Legend**     [C]  Completed     [IP] In Progress
-               [IR] In Review     [NS] Not Started"""
 
         _temp_print(description)
-        _temp_print(legend)
         _temp_print(table=rich_table)
         _temp_print(tips)
         _temp_print(link)
 
     @property
     def phases(self) -> list[Phase]:
         """The project's phases.
 
         Returns:
             The phases associated with this project.
         """
         outputs = self._client.list_phases(project=self._id)
-        return sorted(
-            [Phase(item.id, self, item.name, item.index, item.status) for item in outputs], key=lambda x: x.index
-        )
+        return [Phase(item.id, self, item.name, item.index, item.status) for item in outputs.list]
```

### Comparing `vectice-23.2.2.1/src/vectice/models/property.py` & `vectice-23.2.3.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/__init__.py` & `vectice-23.2.3.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/base.py` & `vectice-23.2.3.0/src/vectice/models/resource/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,23 @@
 
         ```python
         from vectice import Resource, DatasetSourceOrigin, FilesMetadata
 
         class MyResource(Resource):
             _origin = "Data source name"
 
+            def __init__(
+                self,
+                paths: str | list[str],
+            ):
+                super().__init__(paths=paths)
+
             def _build_metadata(self) -> FilesMetadata:  # (1)
                 files = ...  # fetch file list from your custom storage
-                total_size = ...  # compute total file size
+                total_size = ...  # compute total file size, retrieve them from self._paths
                 return FilesMetadata(
                     size=total_size,
                     origin=self._origin,
                     files=files,
                     usage=self.usage,
                 )
```

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.2.3.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,62 +14,41 @@
     from google.cloud.bigquery import Client as BQClient
     from google.cloud.bigquery import Table
 
 _logger = logging.getLogger(__name__)
 
 
 class BigQueryResource(Resource):
-    """Wrap columnar data and its metadata in BigQuery.
+    """BigQuery resource reference wrapper.
 
-    Vectice stores metadata -- data about your dataset -- communicated
-    with a resource.  Your actual dataset is not stored by Vectice.
-
-    This resource wraps data that you have stored in BigQuery. You assign it to a step.
+    This resource wraps BigQuery paths that you have stored in BigQuery with optional metadata and versioning. You assign it to a step.
 
     ```python
     from vectice import BigQueryResource
-    from google.cloud.bigquery import Client
 
-    my_service_account_file = "MY_SERVICE_ACCOUNT_JSON_PATH"  # (1)
-    bq_client = Client.from_service_account_json(json_credentials_path=my_service_account_file)  # (2)
     bq_resource = BigQueryResource(
-        bq_client=bq_client,
         paths="bigquery-public-data.stackoverflow.posts_questions",
     )
     ```
-
-    1. See [Service account credentials](https://developers.google.com/workspace/guides/create-credentials#service-account).
-    1. See [GCS docs](https://cloud.google.com/python/docs/reference/storage/latest/modules).
-
-    Note that these three concepts are distinct, even if easily conflated:
-
-    * Where the data is stored
-    * The format at rest (in storage)
-    * The format when loaded in a running Python program
-
-    Notably, the statistics collectors provided by Vectice operate
-    only on this last and only in the event that the data is loaded as
-    a pandas dataframe.
     """
 
     _origin = DatasetSourceOrigin.BIGQUERY.value
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: DataFrame | list[DataFrame] | None = None,
         bq_client: BQClient | None = None,
     ):
         """Initialize a BigQuery resource.
 
         Parameters:
             paths: The paths to retrieve the datasets or the tables.
-            dataframes: The pandas dataframes allowing vectice to compute more metadata about this resource.
-            bq_client: The `google.cloud.bigquery.Client` used
-                to interact with BigQuery.
+            dataframes (Optional): The pandas dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats.
+            bq_client (Optional): The `google.cloud.bigquery.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning).
         """
         super().__init__(paths=paths, dataframes=dataframes)
         self.bq_client = bq_client
 
     def _fetch_data(self) -> dict[str, tuple[Table | None, DataFrame | None]]:
         tables: dict[str, tuple[Table | None, DataFrame | None]] = {}
         df_index = 0
```

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/description.py` & `vectice-23.2.3.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/file_resource.py` & `vectice-23.2.3.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/gcs_resource.py` & `vectice-23.2.3.0/src/vectice/models/resource/gcs_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,63 +12,42 @@
 if TYPE_CHECKING:
     from google.cloud.storage import Blob, Bucket, Client
 
 GS_URI_REG = r"(gs:\/\/)([^\/]+)\/(.+)"
 
 
 class GCSResource(Resource):
-    """Wrap columnar data and its metadata in GCS.
+    """GCS resource reference wrapper.
 
-    Vectice stores metadata -- data about your dataset -- communicated
-    with a resource.  Your actual dataset is not stored by Vectice.
-
-    This resource wraps data that you have stored in Google Cloud
-    Storage.  You assign it to a step.
+    This resource wraps GCS uris references such as file folders that you have stored in Google Cloud
+    Storage with optional metadata and versioning. You assign it to a step.
 
     ```python
     from vectice import GCSResource
-    from google.cloud.storage import Client
 
-    my_service_account_file = "MY_SERVICE_ACCOUNT_JSON_PATH"  # (1)
-    gcs_client = Client.from_service_account_json(json_credentials_path=my_service_account_file)  # (2)
     gcs_resource = GCSResource(
-        gcs_client=gcs_client,
         uris="gs://<bucket_name>/<file_path_inside_bucket>",
     )
     ```
-
-    1. See [Service account credentials](https://developers.google.com/workspace/guides/create-credentials#service-account).
-    1. See [GCS docs](https://cloud.google.com/python/docs/reference/storage/latest/modules).
-
-    Note that these three concepts are distinct, even if easily conflated:
-
-    * Where the data is stored
-    * The format at rest (in storage)
-    * The format when loaded in a running Python program
-
-    Notably, the statistics collectors provided by Vectice operate
-    only on this last and only in the event that the data is loaded as
-    a pandas dataframe.
     """
 
     _origin = DatasetSourceOrigin.GCS.value
 
     def __init__(
         self,
         uris: str | list[str],
         dataframes: DataFrame | list[DataFrame] | None = None,
         gcs_client: Client | None = None,
     ):
         """Initialize a GCS resource.
 
         Parameters:
-            uris: The uris of the resources to get. Should follow the pattern 'gs://<bucket_name>/<file_path_inside_bucket>'
-            dataframes: The pandas dataframes allowing vectice to compute more metadata about this resource.
-            gcs_client: The `google.cloud.storage.Client` used
-                to interact with Google Cloud Storage.
+            uris: The uris of the referenced resources. Should follow the pattern 'gs://<bucket_name>/<file_path_inside_bucket>'
+            dataframes (Optional): The pandas dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats.
+            gcs_client (Optional): The `google.cloud.storage.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning).
         """
         super().__init__(paths=uris, dataframes=dataframes)
         self.gcs_client = gcs_client
 
         for uri in self._paths:
             if not re.search(GS_URI_REG, uri):
                 raise ValueError(
```

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.2.3.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/metadata/base.py` & `vectice-23.2.3.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-23.2.3.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from enum import Enum
 
 import numpy as np
 
 
+class ColumnCategoryType(Enum):
+    """Enumeration of the column category types."""
+
+    BOOLEAN = "BOOLEAN"
+    NUMERICAL = "NUMERICAL"
+    DATE = "DATE"
+    TEXT = "TEXT"
+    CATEGORICAL = "CATEGORICAL"
+
+
 @dataclass
 class StatValue:
     """Model a key-value pair of a column statistic.
 
     Parameters:
         key: The key to identify the statistic.
         value: The value of the statistic.
@@ -33,32 +44,39 @@
     """Model a column of a dataset."""
 
     def __init__(
         self,
         name: str,
         data_type: str,
         stats: list[StatValue] | None = None,
+        category_type: ColumnCategoryType | None = None,
     ):
         """Initialize a column.
 
         Parameters:
             name: The name of the column.
             data_type: The type of the data contained in the column.
             stats: Additional statistics about the column.
+            category_type: Column category type.
         """
         self.name = name
         self.data_type = data_type
         self.stats = stats
+        self.category_type = category_type
 
     def asdict(self) -> dict:
-        return {
+        obj = {
             "name": self.name,
             "dataType": self.data_type,
             "stats": [vars(stat) for stat in self.stats or []],
         }
+        if self.category_type:
+            obj["categoryType"] = self.category_type.value
+
+        return obj
 
 
 class DBColumn(Column):
     """Model a column of a dataset, like a database column."""
 
     def __init__(
         self,
```

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/metadata/dataframe_column_parser.py` & `vectice-23.2.3.0/src/vectice/models/resource/metadata/dataframe_column_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 
 import pandas as pd
 from pandas import DataFrame, Series, api
 
-from vectice.models.resource.metadata.column_metadata import Column, StatValue
+from vectice.models.resource.metadata.column_metadata import Column, ColumnCategoryType, StatValue
 
 # mypy: ignore-errors
 
 _logger = logging.getLogger(__name__)
 
 
 def capture_columns(init_columns: list[Column] | None, dataframe: DataFrame | None) -> dict:
@@ -19,35 +19,37 @@
 
     columns: list[Column] = []
     column_names_with_types = dataframe.dtypes.astype(str).to_dict()
     for idx, (name, d_type) in enumerate(column_names_with_types.items()):
         if idx >= 100:
             _logger.warning("Statistics are only captured for the first 100 columns of your dataframe.")
             break
+        category_type, stats = capture_column_stats(dataframe[name])
         columns.append(
             Column(
                 name=name,
                 data_type=d_type if d_type != "object" else "string",
-                stats=capture_column_stats(dataframe[name]),
+                stats=stats,
+                category_type=category_type,
             )
         )
 
     return [column.asdict() for column in columns]
 
 
-def capture_column_stats(series: Series) -> list[StatValue] | None:
+def capture_column_stats(series: Series) -> tuple[str | None, list[StatValue] | None]:
     if api.types.is_bool_dtype(series):
-        return compute_boolean_column_statistics(series)
+        return ColumnCategoryType.BOOLEAN, compute_boolean_column_statistics(series)
     elif api.types.is_numeric_dtype(series):
-        return compute_numeric_column_statistics(series)
+        return ColumnCategoryType.NUMERICAL, compute_numeric_column_statistics(series)
     elif api.types.is_datetime64_any_dtype(series) | (series.dtypes == "dbdate"):
-        return compute_date_column_statistics(series)
+        return ColumnCategoryType.DATE, compute_date_column_statistics(series)
     elif api.types.is_string_dtype(series):
-        return compute_string_column_statistics(series)
-    return None
+        return ColumnCategoryType.TEXT, compute_string_column_statistics(series)
+    return None, None
 
 
 def compute_boolean_column_statistics(series: Series) -> list[StatValue]:
     """Parse a dataframe series and return statistics about it.
 
     The computed statistics are:
     - the series count (size)
```

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.2.3.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.2.3.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/metadata/source.py` & `vectice-23.2.3.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/models/resource/s3_resource.py` & `vectice-23.2.3.0/src/vectice/models/resource/s3_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,67 +14,42 @@
     from mypy_boto3_s3.type_defs import ListObjectsV2OutputTypeDef, ObjectTypeDef
 
 
 S3_URI_REG = r"(s3:\/\/)([^\/]+)\/(.+)"
 
 
 class S3Resource(Resource):
-    """Wrap columnar data and its metadata in AWS S3.
+    """AWS S3resource reference wrapper.
 
-    Vectice stores metadata -- data about your dataset -- communicated
-    with a resource. Your actual dataset is not stored by Vectice.
-
-    This resource wraps data that you have stored in AWS S3.
-    You assign it to a step.
+    This resource wraps AWS S3 uris references such as file folders that you have stored in AWS S3
+    with optional metadata and versioning. You assign it to a step.
 
     ```python
     from vectice import S3Resource
-    from boto3.session import Session
-
-    s3_session = Session(  # (1)
-        aws_access_key_id="...",
-        aws_secret_access_key="...",
-        region_name="us-east-1",
-    )
-    s3_client = s3_session.client(service_name="s3")  # (2)
 
     s3_resource = S3Resource(
-        s3_client=s3_client,
         uris="s3://<bucket_name>/<file_path_inside_bucket>",
     )
     ```
-
-    1. See [boto3 sessions][boto3.session.Session].
-    1. See [boto3 session client][boto3.session.Session.client].
-
-    Note that these three concepts are distinct, even if easily conflated:
-
-    * Where the data is stored
-    * The format at rest (in storage)
-    * The format when loaded in a running Python program
-
-    Notably, the statistics collectors provided by Vectice operate
-    only on this last and only in the event that the data is loaded as
-    a pandas dataframe.
     """
 
     _origin = DatasetSourceOrigin.S3.value
 
     def __init__(
         self,
         uris: str | list[str],
         dataframes: DataFrame | list[DataFrame] | None = None,
         s3_client: Client | None = None,
     ):
         """Initialize an S3 resource.
 
         Parameters:
-            uris: The uris of the resources to get. Should follow the pattern 'gs://<bucket_name>/<file_path_inside_bucket>'
-            dataframes: The pandas dataframes allowing vectice to compute more metadata about this resource.
-            s3_client: The client used to interact with Amazon s3.
+            uris: The uris of the resources to get. Should follow the pattern 's3://<bucket_name>/<file_path_inside_bucket>'
+            dataframes (Optional): The pandas dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats.
+            s3_client (Optional): The Amazon s3 client to optionally retrieve file size, creation date and updated date (used for auto-versioning).
         """
         super().__init__(paths=uris, dataframes=dataframes)
         self.s3_client = s3_client
 
         for uri in self._paths:
             if not re.search(S3_URI_REG, uri):
                 raise ValueError(
```

### Comparing `vectice-23.2.2.1/src/vectice/models/step.py` & `vectice-23.2.3.0/src/vectice/models/step.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 import pickle  # nosec
 from io import IOBase
 from typing import TYPE_CHECKING, Any
 
 from PIL.Image import Image
 
 import vectice
-from vectice.api.json.dataset_register import DatasetRegisterOutput
+from vectice.api.http_error_handlers import VecticeException
 from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.json.iteration import (
     IterationStatus,
     IterationStepArtifact,
     IterationStepArtifactInput,
     IterationStepArtifactType,
 )
-from vectice.api.json.model_register import ModelRegisterOutput
 from vectice.api.json.model_version import ModelVersionOutput
 from vectice.api.json.step import StepType
 from vectice.models.attachment_container import AttachmentContainer
-from vectice.utils.common_utils import _check_image_path, _get_image_variables
+from vectice.utils.common_utils import _get_image_variables
+from vectice.utils.instance_helper import is_image
 from vectice.utils.last_assets import _comment_or_image_logging, _register_dataset_logging, _register_model_logging
 
 if TYPE_CHECKING:
     from vectice import Connection
     from vectice.models import Iteration, Phase, Project, Workspace
     from vectice.models.dataset import Dataset
     from vectice.models.model import Model
+    from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
+    from vectice.models.representation.model_version_representation import ModelVersionRepresentation
     from vectice.models.step_dataset import StepDataset
     from vectice.models.step_model import StepModel
     from vectice.models.step_number import StepNumber
     from vectice.models.step_string import StepString
 
 _logger = logging.getLogger(__name__)
 
@@ -91,15 +93,14 @@
         iteration: Iteration,
         name: str,
         index: int,
         slug: str,
         description: str | None = None,
         artifacts: list[IterationStepArtifact] | None = None,
         step_type: StepType = StepType.Step,
-        text: str | None = None,
     ):
         """Initialize a step.
 
         Vectice users shouldn't need to instantiate Steps manually,
         but here are the step parameters.
 
         Parameters:
@@ -107,26 +108,24 @@
             iteration: The iteration to which the step belongs.
             name: The name of the step.
             index: The index of the step.
             slug: The slug of the step.
             description: The description of the step.
             artifacts: The artifacts linked to the steps.
             step_type: The step type.
-            text: The step text.
         """
         self._id = id
         self._iteration: Iteration = iteration
         self._name = name
         self._index = index
         self._description = description
         self._client = self._iteration._client
         self._artifacts = artifacts or []
         self._slug = slug
         self._type: StepType = step_type
-        self._text = text
         self._model: Model | None = None
 
         self._iteration_read_only = self._iteration._status in {IterationStatus.Completed, IterationStatus.Abandoned}
         if self._iteration_read_only:
             _logger.debug(f"Step {self.name}, iteration is {self._iteration._status.name} and is read-only!")
 
     def __repr__(self):
@@ -137,292 +136,431 @@
             return NotImplemented
         return self.id == other.id
 
     def __iadd__(self, value):
         # TODO cyclic import
         from vectice.models.dataset import Dataset
         from vectice.models.model import Model
+        from vectice.models.representation.dataset_representation import DatasetRepresentation
+        from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
+        from vectice.models.representation.model_representation import ModelRepresentation
+        from vectice.models.representation.model_version_representation import ModelVersionRepresentation
         from vectice.models.step_dataset import StepDataset
+        from vectice.models.step_image import StepImage
         from vectice.models.step_model import StepModel
+        from vectice.models.step_number import StepNumber
+        from vectice.models.step_string import StepString
+
+        self._ensure_correct_project_id_from_representation_objs(value)
+
+        if is_image(value):
+            step_artifacts, filename = self._create_image_artifact(value)
+            artifacts = [
+                IterationStepArtifact(entityFileId=artifact.id, type="EntityFile") for artifact in step_artifacts
+            ]
+            self.artifacts.extend(artifacts)
+            step = StepImage(self, value)
+            self._keep_artifacts_and_update_step(step._type, value)
+            _comment_or_image_logging(self, _logger, filename)
+        elif isinstance(value, (int, float, str)):
+            artifact = IterationStepArtifact(text=value, type="Comment")
+            self.artifacts += [artifact]
+            step = StepString(self, value) if isinstance(value, str) else StepNumber(self, value)
+            self._keep_artifacts_and_update_step(step._type, value)
+            _comment_or_image_logging(self, _logger)
+        elif (
+            isinstance(value, Model)
+            or isinstance(value, ModelRepresentation)
+            or isinstance(value, ModelVersionRepresentation)
+        ):
+            if isinstance(value, Model):
+                code_version_id = self._get_code_version_id()
+                model_data = self._client.register_model(
+                    model=value,
+                    project_id=self.project.id,
+                    phase_id=self.phase.id,
+                    iteration_id=self.iteration.id,
+                    code_version_id=code_version_id,
+                )
+                attachments_output = self._set_model_attachments(value, model_data.model_version)
+                model_artifact = IterationStepArtifact(
+                    modelVersionId=model_data["modelVersion"]["vecticeId"], type="ModelVersion"
+                )
+            elif isinstance(value, ModelRepresentation):
+                model_data = {
+                    "useExistingModel": True,
+                    "modelVersion": {"vecticeId": value.version.id, "name": value.version.name},
+                }
+                model_artifact = IterationStepArtifact(
+                    modelVersionId=value.version.id,
+                    type=IterationStepArtifactType.ModelVersion.name,
+                )
+                attachments_output = self._get_version_attachments(value.version)
+
+            elif isinstance(value, ModelVersionRepresentation):
+                model_data = {
+                    "useExistingModel": True,
+                    "modelVersion": {"vecticeId": value.id, "name": value.name},
+                }
+                model_artifact = IterationStepArtifact(
+                    modelVersionId=value.id,
+                    type=IterationStepArtifactType.ModelVersion.name,
+                )
+                attachments_output = self._get_version_attachments(value)
 
-        if isinstance(value, Model):
-            if self._type not in {StepType.StepModel, StepType.Step}:
-                raise TypeError(f"A model can't be added to a step of type {self._type!r}.")
-            code_version_id = self._get_code_version_id()
-            model_data = self._client.register_model(
-                model=value,
-                project_id=self.project.id,
-                phase_id=self.phase.id,
-                iteration_id=self.iteration.id,
-                code_version_id=code_version_id,
-            )
-            attachments_output = self._set_model_attachments(value, model_data.model_version)
-            model_artifact = IterationStepArtifact(modelVersionId=model_data["modelVersion"]["id"], type="ModelVersion")
-            copy_artifacts = self.artifacts.copy()
-            self.artifacts += [model_artifact]
             attachments = (
                 [
                     IterationStepArtifact(entityFileId=attach["fileId"], type="EntityFile")
                     for attach in attachments_output
                 ]
                 if attachments_output
                 else []
             )
             self.artifacts += attachments
-
+            copy_artifacts = self.artifacts.copy()
+            self.artifacts += [model_artifact]
             self._keep_artifacts_and_update_step(StepType.StepModel, value)
             step = StepModel(self, model_artifact, value)
             _register_model_logging(self, model_data, value, self.name, attachments_output, _logger, copy_artifacts)
-            self._iteration._steps[self.name] = step
-        elif isinstance(value, Dataset):
-            if self._type not in {StepType.StepDataset, StepType.Step}:
-                raise TypeError(f"A dataset can't be added to a step of type {self._type!r}.")
-            code_version_id = self._get_code_version_id()
-            dataset_output = self._client.register_dataset_from_source(
-                dataset=value,
-                project_id=self.project.id,
-                phase_id=self.phase.id,
-                iteration_id=self.iteration.id,
-                code_version_id=code_version_id,
-            )
-            attachments_output = self._set_dataset_attachments(value, dataset_output.dataset_version)
-            dataset_artifact = IterationStepArtifact(
-                datasetVersionId=dataset_output["datasetVersion"]["id"],
-                type=IterationStepArtifactType.DataSetVersion.name,
-            )
+        elif (
+            isinstance(value, Dataset)
+            or isinstance(value, DatasetRepresentation)
+            or isinstance(value, DatasetVersionRepresentation)
+        ):
+            if isinstance(value, Dataset):
+                code_version_id = self._get_code_version_id()
+                dataset_output = self._client.register_dataset_from_source(
+                    dataset=value,
+                    project_id=self.project.id,
+                    phase_id=self.phase.id,
+                    iteration_id=self.iteration.id,
+                    code_version_id=code_version_id,
+                )
+                dataset_artifact = IterationStepArtifact(
+                    datasetVersionId=dataset_output["datasetVersion"]["vecticeId"],
+                    type=IterationStepArtifactType.DataSetVersion.name,
+                )
+                attachments_output = self._set_dataset_attachments(value, dataset_output.dataset_version)
+            elif isinstance(value, DatasetRepresentation):
+                dataset_output = {
+                    "useExistingDataset": True,
+                    "useExistingVersion": True,
+                    "datasetVersion": {"vecticeId": value.version.id, "name": value.version.name},
+                }
+                dataset_artifact = IterationStepArtifact(
+                    datasetVersionId=value.version.id,
+                    type=IterationStepArtifactType.DataSetVersion.name,
+                )
+                attachments_output = self._get_version_attachments(value.version)
+            elif isinstance(value, DatasetVersionRepresentation):
+                dataset_output = {
+                    "useExistingDataset": True,
+                    "useExistingVersion": True,
+                    "datasetVersion": {"vecticeId": value.id, "name": value.name},
+                }
+                dataset_artifact = IterationStepArtifact(
+                    datasetVersionId=value.id,
+                    type=IterationStepArtifactType.DataSetVersion.name,
+                )
+                attachments_output = self._get_version_attachments(value)
+
             copy_artifacts = self.artifacts.copy()
             self.artifacts.append(dataset_artifact)
             attachments = (
                 [
                     IterationStepArtifact(entityFileId=attach["fileId"], type="EntityFile")
                     for attach in attachments_output
                 ]
                 if attachments_output
                 else []
             )
             self.artifacts += attachments
             self._keep_artifacts_and_update_step(StepType.StepDataset, value)
             step = StepDataset(self, dataset_artifact)
             _register_dataset_logging(self, dataset_output, value, attachments_output, _logger, copy_artifacts)
-            self._iteration._steps[self.name] = step
         else:
-            raise TypeError(f"Expected Dataset or a Model, got {type(value)}")
+            raise TypeError(f"Expected Comment, Dataset or a Model, got {type(value)}")
+
+        self._iteration._steps[self.name] = step
 
     def _keep_artifacts_and_update_step(self, step_type: StepType, value) -> None:
-        artifacts = self._client.get_step_by_name(self.name, self._iteration.id).artifacts
+        artifacts = list(
+            filter(
+                self._filter_non_empty_artifact,
+                self._client.get_step_by_name(self.name, self._iteration.id).artifacts,
+            )
+        )
 
-        def _get_artifact_id(artifact: IterationStepArtifact) -> int:
+        def _get_artifact_id(artifact: IterationStepArtifact) -> int | str | None:
             if artifact.model_version_id:
                 return artifact.model_version_id
             if artifact.dataset_version_id:
                 return artifact.dataset_version_id
             if artifact.entity_file_id:
                 return artifact.entity_file_id
-            raise ValueError("No artifact ID.")
+
+            return None
 
         def _maintain_and_add_artifacts(session_artifacts, existing_artifacts):
             # Ensure we don't keep adding an instances artifacts to the step
             maintain_artifacts = existing_artifacts
-            for artifact in session_artifacts:
-                match = any(filter(lambda x: x.id == artifact.id, existing_artifacts))
-                if not match:
-                    maintain_artifacts += [artifact]
+            for ia, art in enumerate(session_artifacts):
+                if len(maintain_artifacts) >= ia + 1:
+                    existing_art = maintain_artifacts[ia]
+                    if (art.id is not None and existing_art.id == art.id) or (
+                        art.text is not None and existing_art.text == art.text
+                    ):
+                        continue
+                    maintain_artifacts += [art]
+                else:
+                    maintain_artifacts += [art]
             return maintain_artifacts
 
         # These are artifacts that exist in the current instance
+        filtered_artifacts = list(filter(self._filter_non_empty_artifact, self.artifacts))
         session_artifacts = [
-            IterationStepArtifactInput(id=_get_artifact_id(artifact), type=artifact.type.value)
-            for artifact in self.artifacts
+            IterationStepArtifactInput(
+                id=_get_artifact_id(artifact),
+                type=artifact.type.value,
+                text=str(artifact.text) if artifact.text is not None else None,
+            )
+            for artifact in filtered_artifacts
         ]
         # These are artifacts in Vectice
         existing_artifacts = [
-            IterationStepArtifactInput(id=_get_artifact_id(artifact), type=artifact.type.value)
+            IterationStepArtifactInput(
+                id=_get_artifact_id(artifact),
+                type=artifact.type.value,
+                text=str(artifact.text) if artifact.text is not None else None,
+            )
             for artifact in artifacts
         ]
         # Ensure no crossover or duplicates
         maintain_artifacts = _maintain_and_add_artifacts(session_artifacts, existing_artifacts)
         self._client.update_iteration_step_artifact(self.id, step_type, artifacts=maintain_artifacts)
         self._warn_step_change(value)
 
-    def _step_factory_and_update(
-        self, value: Dataset | Model | int | float | str | None = None
-    ) -> Step | StepString | StepNumber | StepDataset | StepModel:
+    def _step_factory_and_update(self, value) -> Step | StepString | StepNumber | StepDataset | StepModel:
         # TODO cyclic imports
         from vectice.models.dataset import Dataset
         from vectice.models.model import Model
+        from vectice.models.representation.dataset_representation import DatasetRepresentation
+        from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
+        from vectice.models.representation.model_representation import ModelRepresentation
+        from vectice.models.representation.model_version_representation import ModelVersionRepresentation
         from vectice.models.step_dataset import StepDataset
         from vectice.models.step_image import StepImage
         from vectice.models.step_model import StepModel
         from vectice.models.step_number import StepNumber
         from vectice.models.step_string import StepString
 
+        self._ensure_correct_project_id_from_representation_objs(value)
+
         if isinstance(value, (int, float)):
             self._update_iteration_step(StepType.StepNumber, value)
             _comment_or_image_logging(self, _logger)
             return StepNumber(step=self, number=value)
 
-        if (
-            isinstance(value, Image)
-            or isinstance(value, IOBase)
-            or (isinstance(value, str) and _check_image_path(value))
-        ):
-            step_artifacts, filename = self._create_image_artifact(value)
-            self._update_iteration_step(StepType.StepImage, value, step_artifacts)
+        img_value = is_image(value)
+        if img_value:
+            step_artifacts, filename = self._create_image_artifact(img_value)
+            self._update_iteration_step(StepType.StepImage, img_value, step_artifacts)
             _comment_or_image_logging(self, _logger, filename)
-            return StepImage(self, value)
+            return StepImage(self, img_value)
 
         if isinstance(value, str):
             self._update_iteration_step(StepType.StepString, value)
             _comment_or_image_logging(self, _logger)
             return StepString(self, string=value)
 
-        if isinstance(value, Model):
-            code_version_id = self._get_code_version_id()
-            data = self._client.register_model(
-                model=value,
-                project_id=self.project.id,
-                phase_id=self.phase.id,
-                iteration_id=self.iteration.id,
-                code_version_id=code_version_id,
-            )
-            attachments_output = self._set_model_attachments(value, data.model_version)
+        if (
+            isinstance(value, Model)
+            or isinstance(value, ModelRepresentation)
+            or isinstance(value, ModelVersionRepresentation)
+        ):
+            data: dict[str, Any] = {}
+            if isinstance(value, Model):
+                code_version_id = self._get_code_version_id()
+                data = self._client.register_model(
+                    model=value,
+                    project_id=self.project.id,
+                    phase_id=self.phase.id,
+                    iteration_id=self.iteration.id,
+                    code_version_id=code_version_id,
+                )
+                attachments_output = self._set_model_attachments(value, data.model_version)
+            elif isinstance(value, ModelRepresentation):
+                data = {
+                    "useExistingModel": True,
+                    "modelVersion": {"vecticeId": value.version.id, "name": value.version.name},
+                }
+                attachments_output = self._get_version_attachments(value.version)
+            elif isinstance(value, ModelVersionRepresentation):
+                data = {
+                    "useExistingModel": True,
+                    "modelVersion": {"vecticeId": value.id, "name": value.name},
+                }
+                attachments_output = self._get_version_attachments(value)
 
             artifacts = self._get_version_artifacts(data, attachments_output)
             self._client.update_iteration_step_artifact(
                 self.id,
                 StepType.StepModel,
-                None,
                 artifacts,
             )
             _register_model_logging(self, data, value, self.name, attachments_output, _logger)
-            self.artifacts = [IterationStepArtifact(modelVersionId=data["modelVersion"]["id"], type="ModelVersion")]
+            self.artifacts = [
+                IterationStepArtifact(modelVersionId=data["modelVersion"]["vecticeId"], type="ModelVersion")
+            ]
             self._warn_step_change(value)
             return StepModel(self, self.artifacts[0], value)
 
-        if isinstance(value, Dataset):
-            code_version_id = self._get_code_version_id()
-            dataset = self._client.register_dataset_from_source(
-                dataset=value,
-                project_id=self.project.id,
-                phase_id=self.phase.id,
-                iteration_id=self.iteration.id,
-                code_version_id=code_version_id,
-            )
-            attachments_output = self._set_dataset_attachments(value, dataset.dataset_version)
+        elif (
+            isinstance(value, Dataset)
+            or isinstance(value, DatasetRepresentation)
+            or isinstance(value, DatasetVersionRepresentation)
+        ):
+            dataset: dict[str, Any] = {}
+            if isinstance(value, Dataset):
+                code_version_id = self._get_code_version_id()
+                dataset = self._client.register_dataset_from_source(
+                    dataset=value,
+                    project_id=self.project.id,
+                    phase_id=self.phase.id,
+                    iteration_id=self.iteration.id,
+                    code_version_id=code_version_id,
+                )
+                attachments_output = self._set_dataset_attachments(value, dataset.dataset_version)
+            elif isinstance(value, DatasetRepresentation):
+                dataset = {
+                    "useExistingDataset": True,
+                    "useExistingVersion": True,
+                    "datasetVersion": {"vecticeId": value.version.id, "name": value.version.name},
+                }
+                attachments_output = self._get_version_attachments(value.version)
+            elif isinstance(value, DatasetVersionRepresentation):
+                dataset = {
+                    "useExistingDataset": True,
+                    "useExistingVersion": True,
+                    "datasetVersion": {"vecticeId": value.id, "name": value.name},
+                }
+                attachments_output = self._get_version_attachments(value)
+
             artifacts = self._get_version_artifacts(dataset, attachments_output)
             self._client.update_iteration_step_artifact(
                 self.id,
                 StepType.StepDataset,
-                None,
                 artifacts,
             )
             _register_dataset_logging(self, dataset, value, attachments_output, _logger)
             self.artifacts = [
-                IterationStepArtifact(datasetVersionId=dataset["datasetVersion"]["id"], type="DataSetVersion")
+                IterationStepArtifact(datasetVersionId=dataset["datasetVersion"]["vecticeId"], type="DataSetVersion")
             ]
             self._warn_step_change(value)
             return StepDataset(self, dataset_version=self.artifacts[0])
 
         return self
 
+    def _get_version_attachments(self, value: ModelVersionRepresentation | DatasetVersionRepresentation):
+        return [
+            vars(attach)
+            for attach in self.project._client.list_version_representation_attachments(self.project.id, value).list
+        ]
+
+    def _ensure_correct_project_id_from_representation_objs(self, value):
+        from vectice.models.representation.dataset_representation import DatasetRepresentation
+        from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
+        from vectice.models.representation.model_representation import ModelRepresentation
+        from vectice.models.representation.model_version_representation import ModelVersionRepresentation
+
+        if (
+            isinstance(value, DatasetRepresentation)
+            or isinstance(value, DatasetVersionRepresentation)
+            or isinstance(value, ModelRepresentation)
+            or isinstance(value, ModelVersionRepresentation)
+        ) and value.project_id != self.project.id:
+            raise VecticeException("Assigning an asset coming from another project is forbidden")
+
     def _get_version_artifacts(
-        self, data: ModelRegisterOutput | DatasetRegisterOutput, attachments_output: list[dict] | None = None
+        self, data, attachments_output: list[dict] | None = None
     ) -> list[IterationStepArtifactInput]:
         attachments = None
         if attachments_output:
             attachments = (
                 [IterationStepArtifactInput(id=attach["fileId"], type="EntityFile") for attach in attachments_output]
                 if attachments_output
                 else None
             )
-        if isinstance(data, ModelRegisterOutput):
+        if "modelVersion" in data:
             artifact = IterationStepArtifactInput(
-                id=data["modelVersion"]["id"],
+                id=data["modelVersion"]["vecticeId"],
                 type=IterationStepArtifactType.ModelVersion.name,
             )
         else:
             artifact = IterationStepArtifactInput(
-                id=data["datasetVersion"]["id"],
+                id=data["datasetVersion"]["vecticeId"],
                 type=IterationStepArtifactType.DataSetVersion.name,
             )
         artifacts = [artifact]
         artifacts += attachments if attachments else []
         return artifacts
 
     def _create_image_artifact(self, value: str | IOBase | Image) -> tuple[list[IterationStepArtifactInput], str]:
         image, filename = _get_image_variables(value)
         try:
             attachments_output = self._client.create_phase_attachments(
                 [("file", (filename, image))], self.phase.id, self.project.id
             )
             return [
-                IterationStepArtifactInput(id=artifact["fileId"], type="EntityFile") for artifact in attachments_output
+                IterationStepArtifactInput(id=artifact["fileId"], type=IterationStepArtifactType.EntityFile.name)
+                for artifact in attachments_output
             ], filename
         except Exception as error:
             raise ValueError("Check the provided image.") from error
 
-    def _keep_artifacts(self, artifacts: list[IterationStepArtifact]) -> list[IterationStepArtifactInput]:
-        def _get_artifact_id(artifact: IterationStepArtifact) -> int:
-            if artifact.model_version_id:
-                return artifact.model_version_id
-            if artifact.dataset_version_id:
-                return artifact.dataset_version_id
-            if artifact.entity_file_id:
-                return artifact.entity_file_id
-            raise ValueError("No artifact ID.")
-
-        return [
-            IterationStepArtifactInput(id=_get_artifact_id(artifact), type=artifact.type.value)
-            for artifact in artifacts
-        ]
-
     def _update_iteration_step(
         self, type: StepType, value, step_artifacts: list[IterationStepArtifactInput] | None = None
     ):
-        # TODO: cyclic import
-        from vectice.models.model import Model
-
         if type is StepType.StepImage:
             self._client.update_iteration_step_artifact(
                 self.id,
                 type,
-                None,
                 artifacts=step_artifacts or [],
             )
             self._warn_step_change(StepType.StepImage)
         elif isinstance(value, (str, int, float)):
-            maintain_artifacts = self._keep_artifacts(
-                self._client.get_step(self.id, self.phase.id, self.iteration.index).artifacts
-            )
             self._client.update_iteration_step_artifact(
                 self.id,
                 type,
-                str(value),
-                maintain_artifacts,
+                [IterationStepArtifactInput(type="Comment", text=str(value))],
             )
-
-            self._warn_step_change(value)
-        elif isinstance(value, Model) or type is StepType.StepModel:
-            self._client.update_iteration_step_artifact(self.id, StepType.StepModel, artifacts=step_artifacts)
-            self._warn_step_change(value)
-            self._model = value
-        elif type is StepType.StepDataset:
-            self._client.update_iteration_step_artifact(self.id, StepType.StepDataset, artifacts=step_artifacts)
             self._warn_step_change(value)
 
     def _warn_step_change(self, value):
         # TODO: cyclic import
         from vectice.models.dataset import Dataset
         from vectice.models.model import Model
+        from vectice.models.representation.dataset_representation import DatasetRepresentation
+        from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
+        from vectice.models.representation.model_representation import ModelRepresentation
+        from vectice.models.representation.model_version_representation import ModelVersionRepresentation
 
         if self._type is StepType.Step:
             return
-        elif self._type is not StepType.StepModel and isinstance(value, Model):
+        elif self._type is not StepType.StepModel and (
+            isinstance(value, Model)
+            or isinstance(value, ModelRepresentation)
+            or isinstance(value, ModelVersionRepresentation)
+        ):
             _logger.debug(f"Step type changed from {self._type.name} to StepModel")
-        elif self._type is not StepType.StepDataset and isinstance(value, Dataset):
+        elif self._type is not StepType.StepDataset and (
+            isinstance(value, Dataset)
+            or isinstance(value, DatasetRepresentation)
+            or isinstance(value, DatasetVersionRepresentation)
+        ):
             _logger.debug(f"Step type changed from {self._type.name} to StepDataset")
         elif self._type is not StepType.StepImage and StepType.StepImage is value:
             _logger.debug(f"Step type changed from {self._type.name} to StepImage")
         elif self._type is not StepType.StepNumber and isinstance(value, (int, float)):
             _logger.debug(f"Step type changed from {self._type.name} to StepNumber")
         elif self._type is not StepType.StepString and isinstance(value, str):
             _logger.debug(f"Step type changed from {self._type.name} to StepString")
@@ -486,25 +624,14 @@
         return self._artifacts
 
     @artifacts.setter
     def artifacts(self, artifacts: list[IterationStepArtifact]):
         self._artifacts = artifacts
 
     @property
-    def text(self) -> str | None:
-        """The step's text.
-
-        A string that is stored in the step.
-
-        Returns:
-            The step's text.
-        """
-        return self._text
-
-    @property
     def connection(self) -> Connection:
         """The connection to which this step belongs.
 
         Returns:
             The connection to which this step belongs.
         """
         return self._iteration.connection
@@ -581,10 +708,13 @@
         logging.getLogger("vectice.models.attachment_container").propagate = True
         attachments = None
         if dataset.attachments:
             container = AttachmentContainer(dataset_version, self._client)
             attachments = container.add_attachments(dataset.attachments)
         return attachments
 
+    def _filter_non_empty_artifact(self, artifact: IterationStepArtifact) -> str | int | float | None:
+        return artifact.model_version_id or artifact.dataset_version_id or artifact.entity_file_id or artifact.text
+
     @staticmethod
     def _serialize_model(model: Any) -> bytes:
         return pickle.dumps(model)
```

### Comparing `vectice-23.2.2.1/src/vectice/models/step_dataset.py` & `vectice-23.2.3.0/src/vectice/models/step_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             step.id,
             step._iteration,
             step.name,
             step.index,
             step.slug,
             step._description,
             step_type=StepType.StepDataset,
-            text=None,
             artifacts=step.artifacts,
         )
         self._dataset_version = dataset_version
 
     def __repr__(self):
         return f"StepDataset(name={self.name!r}, id={self.id!r}, description={self._description!r}, dataset_version_id={self.dataset_version!r})"
```

### Comparing `vectice-23.2.2.1/src/vectice/models/step_image.py` & `vectice-23.2.3.0/src/vectice/models/step_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,10 +88,9 @@
         )
         step_artifacts = [
             IterationStepArtifactInput(id=artifact["entityId"], type="EntityFile") for artifact in attachments_output
         ]
         self._client.update_iteration_step_artifact(
             self.id,
             StepType.StepImage,
-            self.text,
             step_artifacts,
         )
```

### Comparing `vectice-23.2.2.1/src/vectice/models/step_model.py` & `vectice-23.2.3.0/src/vectice/models/step_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
             step.id,
             step._iteration,
             step.name,
             step.index,
             step.slug,
             step._description,
             step_type=StepType.StepModel,
-            text=None,
             artifacts=step.artifacts,
         )
         self._model_version = model_version
         self._model = model
 
     def __repr__(self):
         return f"StepModel(name={self.name!r}, id={self.id!r}, description={self._description!r}, model_version_id={self.model_version!r})"
```

### Comparing `vectice-23.2.2.1/src/vectice/models/step_number.py` & `vectice-23.2.3.0/src/vectice/models/step_number.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
 
+from vectice.api.json.iteration import IterationStepArtifactInput
 from vectice.api.json.step import StepType
 from vectice.models.step import Step
 from vectice.utils.common_utils import _check_read_only
 
 _logger = logging.getLogger(__name__)
 
 
@@ -26,15 +27,14 @@
             id=step.id,
             iteration=step._iteration,
             name=step.name,
             index=step.index,
             slug=step.slug,
             description=step._description,
             step_type=StepType.StepNumber,
-            text=step.text if not number else str(number),
             artifacts=step.artifacts,
         )
         self._number = number
 
     def __repr__(self):
         return (
             f"StepNumber(name={self.name!r}, id={self.id!r}, description={self._description!r}, number={self.number!r})"
@@ -60,14 +60,14 @@
         ... my_iteration.step_scoring = 21
         ```
 
         Parameters:
             value: The number.
         """
         _check_read_only(self.iteration)
+        step_artifacts = [IterationStepArtifactInput(type="Comment", text=value)]
         self._client.update_iteration_step_artifact(
             self.id,
             StepType.StepNumber,
-            self.text,
-            [],
+            step_artifacts,
         )
         self._number = value
```

### Comparing `vectice-23.2.2.1/src/vectice/models/step_string.py` & `vectice-23.2.3.0/src/vectice/models/step_string.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
 
+from vectice.api.json.iteration import IterationStepArtifactInput
 from vectice.api.json.step import StepType
 from vectice.models.step import Step
 from vectice.utils.common_utils import _check_read_only
 
 _logger = logging.getLogger(__name__)
 
 
@@ -54,14 +55,10 @@
         ... my_iteration.step_exploration = "Step information"
         ```
 
         Parameters:
             value: The string to set.
         """
         _check_read_only(self.iteration)
-        self._client.update_iteration_step_artifact(
-            self.id,
-            StepType.StepString,
-            self.text,
-            [],
-        )
+        step_artifacts = [IterationStepArtifactInput(type="Comment", text=value)]
+        self._client.update_iteration_step_artifact(self.id, StepType.StepString, step_artifacts)
         self._string = value
```

### Comparing `vectice-23.2.2.1/src/vectice/models/workspace.py` & `vectice-23.2.3.0/src/vectice/models/workspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     my_workspace = vectice.connect(..., workspace="Iris workspace")
     ```
 
     See [`Connection.connect`][vectice.Connection.connect] to learn
     how to connect to Vectice.
     """
 
-    def __init__(self, id: int, name: str, description: str | None = None):
+    def __init__(self, id: str, name: str, description: str | None = None):
         """Initialize a workspace.
 
         Vectice users shouldn't need to instantiate Workspaces manually,
         but here are the workspace parameters.
 
         Parameters:
             id: The workspace identifier.
@@ -82,15 +82,15 @@
         return self.id == other.id
 
     def __repr__(self):
         description = self._description if self._description else "None"
         return f"Workspace(name={self.name!r}, id={self._id}, description={description!r})"
 
     @property
-    def id(self) -> int:
+    def id(self) -> str:
         """The workspace's id.
 
         Returns:
             The workspace's id.
         """
         return self._id
 
@@ -117,25 +117,32 @@
         """The workspace's name and id.
 
         Returns:
             A dictionary containing the `name` and `id` items.
         """
         return {"name": self.name, "id": self.id}
 
-    def project(self, project: str | int) -> Project:
+    def project(self, project: str) -> Project:
         """Get a project.
 
         Parameters:
             project: The project name or id.
 
         Returns:
             The project.
         """
-        item = self._client.get_project(project, self.id)
-        _logger.debug(f"Your current project: {item.id}")
+        item = self._client.get_project(project, self.name)
+        logging_output = dedent(
+            f"""
+                Project {item.name!r} successfully retrieved."
+
+                For quick access to the Project in the Vectice web app, visit:
+                {self._client.auth._API_BASE_URL}/browse/project/{item.id}"""
+        ).lstrip()
+        _logger.info(logging_output)
         project_object = Project(item.id, self, item.name, item.description)
         return project_object
 
     def list_projects(self) -> None:
         """Prints a list of projects belonging to the workspace in a tabular format, limited to the first 10 items. A link is provided to view the remaining projects.
 
         Returns:
@@ -149,29 +156,29 @@
         rich_table.add_column("project id", justify="left", no_wrap=True, min_width=4, max_width=10)
         rich_table.add_column("name", justify="left", no_wrap=True, max_width=15)
         rich_table.add_column("description", justify="left", no_wrap=True, max_width=50)
 
         for count, project in enumerate(project_outputs, 1):
             if count > 10:
                 break
-            rich_table.add_row(str(project.id), project.name, format_description(project.description))
+            rich_table.add_row(project.id, project.name, format_description(project.description))
 
         description = dedent(
             f"""
         There are {len(project_outputs)} projects in the workspace {self.name!r} and a maximum of 10 projects are displayed in the table below:
         """
         ).lstrip()
         tips = dedent(
             """
         To access a specific project, use \033[1mworkspace\033[0m.project(Project ID)"""
         ).lstrip()
         link = dedent(
             f"""
             For quick access to the list of projects in the Vectice web app, visit:
-            {self._client.auth._API_BASE_URL}/workspace/projects?w={self.id}"""
+            {self._client.auth._API_BASE_URL}/browse/workspace/{self.id}"""
         ).lstrip()
 
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(tips)
         _temp_print(link)
 
@@ -179,15 +186,15 @@
     def projects(self) -> list[Project]:
         """List projects.
 
         Returns:
             A list of projects in this workspace.
         """
         response = self._client.list_projects(self.id)
-        return [Project(item.id, self, item.name, item.description) for item in response.list]
+        return [Project(item.id, self, item.name, item.description) for item in response]
 
     @property
     def connection(self) -> Connection:
         """The Connection to which this workspace belongs.
 
         Returns:
             The Connection to which this workspace belongs.
```

### Comparing `vectice-23.2.2.1/src/vectice/utils/automatic_link_utils.py` & `vectice-23.2.3.0/src/vectice/utils/automatic_link_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/utils/common_utils.py` & `vectice-23.2.3.0/src/vectice/utils/common_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     name: str,
     index: int,
     slug: str,
     step_type: StepType,
     description: str | None = None,
     completed: bool | None = None,
     artifacts: list[IterationStepArtifact] | None = None,
-    text: str | None = None,
 ) -> Step | Any:
     # TODO: cyclic imports
     from vectice.models.step import Step
     from vectice.models.step_dataset import StepDataset
     from vectice.models.step_image import StepImage
     from vectice.models.step_model import StepModel
     from vectice.models.step_number import StepNumber
@@ -71,50 +70,49 @@
         iteration=iteration,
         name=name,
         index=index,
         slug=slug,
         description=description,
         artifacts=artifacts,
         step_type=step_type,
-        text=text,
     )
 
     def _get_number(text):
         try:
             number = float(text)
         except ValueError:
             number = int(text)
         return number
 
-    if step_type is StepType.StepNumber:
-        number = _get_number(text) if text else None
-        return StepNumber(step, number)
-    if step_type is StepType.StepString:
-        return StepString(step, text)
-    if step_type is StepType.StepImage:
-        image = _get_image_info(iteration, artifacts) if artifacts else None
-        return StepImage(step, image=image)
-    if step_type is StepType.StepDataset:
-        dataset_version = artifacts[0]  # type: ignore[index]
-        return StepDataset(step, dataset_version=dataset_version)
-    if step_type is StepType.StepModel:
-        model_version = artifacts[0]  # type: ignore[index]
-        return StepModel(step, model_version=model_version)
+    if artifacts is not None and len(artifacts) >= 1:
+        artifact = artifacts[len(artifacts) - 1]
+        if step_type is StepType.StepNumber:
+            number = _get_number(artifact.text) if artifact.text else None
+            return StepNumber(step, number)
+        if step_type is StepType.StepString:
+            return StepString(step, str(artifact.text))
+        if step_type is StepType.StepImage:
+            image = _get_image_info(iteration, artifacts) if artifacts else None
+            return StepImage(step, image=image)
+        if step_type is StepType.StepDataset:
+            dataset_version = artifact
+            return StepDataset(step, dataset_version=dataset_version)
+        if step_type is StepType.StepModel:
+            model_version = artifact
+            return StepModel(step, model_version=model_version)
     return step
 
 
 def _get_image_info(iteration: Iteration, artifacts: list[IterationStepArtifact]):
     artifacts = [image for image in artifacts if image.type.value == "EntityFile"]
-    artifact = artifacts[0] if artifacts else None
+    artifact = artifacts[len(artifacts) - 1] if len(artifacts) >= 1 else None
     attachments = iteration._client.list_phase_attachments(iteration.phase.id, iteration.project.id)
     if not artifact:
         return None
-    image = next(
-        img for img in attachments.list if img.contentType == "ImageFile" and img.fileId == artifact.entity_file_id
-    )
+    image = next(img for img in attachments.list if img.fileId == artifact.entity_file_id)
     return image.fileName
 
 
 def _check_image_path(path: str) -> bool:
     try:
         check_path = Path(path).exists()
     except OSError:
@@ -129,14 +127,15 @@
 
 
 def _validate_image(path: str) -> BytesIO:
     try:
         byte_io = BytesIO()
         image = Image.open(path)
         image.save(byte_io, image.format)
+        image.close()
         byte_io.seek(0)
     except UnidentifiedImageError:
         raise ValueError(f"The provided image {path!r} cannot be opened. Check its format and permissions.") from None
     return byte_io
 
 
 def _get_image_variables(value: str | IOBase | Image.Image) -> tuple[BytesIO | IOBase, str]:
```

### Comparing `vectice-23.2.2.1/src/vectice/utils/configuration.py` & `vectice-23.2.3.0/src/vectice/utils/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,12 @@
     def __init__(self, config_file_path: str):
         with open(config_file_path, "r") as config_file:
             try:
                 self.config_object = json.load(config_file)
             except JSONDecodeError as error:
                 raise SyntaxError("Can not read JSON config file. Check that the file structure is valid.") from error
 
-    def __getitem__(self, key) -> str | int:
-        information: str | int = self.config_object.get(key)
+    def __getitem__(self, key) -> str:
+        information: str = self.config_object.get(key)
         if not information:
             raise KeyError(f"Error while reading the configuration, {key} is empty.")
         return information
```

### Comparing `vectice-23.2.2.1/src/vectice/utils/deprecation.py` & `vectice-23.2.3.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.2.1/src/vectice/utils/last_assets.py` & `vectice-23.2.3.0/src/vectice/utils/last_assets.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,43 +19,43 @@
         last_asset = client.get_last_assets(target_types_array, {"index": 1, "size": 1}).list[0]
         return last_asset
     except IndexError as e:
         _logger.debug(f"There were no assets with activity found. Sanity check {e}")
         return
 
 
-def _get_last_user_and_default_workspace(client: Client) -> tuple[str, int | None]:
+def _get_last_user_and_default_workspace(client: Client) -> tuple[str, str | None]:
     asset = client.get_user_and_default_workspace()
-    workspace_id = int(asset["defaultWorkspace"]["id"]) if asset["defaultWorkspace"] else None
+    workspace_id = str(asset["defaultWorkspace"]["vecticeId"]) if asset["defaultWorkspace"] else None
     return asset["user"]["name"], workspace_id
 
 
-def _connection_logging(_logger: Logger, user_name: str, host: str, workspace_id: int | None):
+def _connection_logging(_logger: Logger, user_name: str, host: str, workspace_id: str | None):
     from vectice.utils.logging_utils import CONNECTION_LOGGING
 
     if workspace_id:
-        logging_output = f"For quick access to your default workspace in the Vectice web app, visit:\n{host}/workspace/dashboard?w={workspace_id}"
+        logging_output = f"For quick access to your default workspace in the Vectice web app, visit:\n{host}/browse/workspace/{workspace_id}"
         _logger.info(CONNECTION_LOGGING.format(user=user_name, logging_output=logging_output))
         return
     logging_output = f"For quick access to the list of workspaces in the Vectice web app, visit:\n{host}/workspaces"
     _logger.info(CONNECTION_LOGGING.format(user=user_name, logging_output=logging_output))
 
 
 def _register_dataset_logging(
     step: Step, data: dict, value: Any, attachments, _logger: Logger, step_artifacts: Any | None = None
 ):
     iteration_id = step._iteration.id
     url = step._client.auth.api_base_url
-    hyper_link = f"{url}/project/phase/iteration?w={step.workspace.id}&iterationId={iteration_id}"
+    hyper_link = f"{url}/browse/iteration/{iteration_id}"
 
     # check if exists
     existing_logging = existing_dataset_logger(data, value.name, _logger)
     # check if attached to step
     check_artifacts = step_artifacts if step_artifacts else step.artifacts
-    match = next(filter(lambda x: x.dataset_version_id == data["datasetVersion"]["id"], check_artifacts), None)
+    match = next(filter(lambda x: x.dataset_version_id == data["datasetVersion"]["vecticeId"], check_artifacts), None)
     attachments_output = None
     if attachments:
         attachments_output = ", ".join([attach["fileName"] for attach in attachments])
     logging_output = None
     if existing_logging and match:
         logging_output = dedent(
             f"""
@@ -85,15 +85,15 @@
     else:
         _logger.debug("Logging failed for register dataset at step, check _register_dataset_logging.")
 
 
 def _comment_or_image_logging(step: Step, _logger: Logger, filename: str | None = None):
     iteration_id = step._iteration.id
     url = step._client.auth.api_base_url
-    hyper_link = f"{url}/project/phase/iteration?w={step.workspace.id}&iterationId={iteration_id}"
+    hyper_link = f"{url}/browse/iteration/{iteration_id}"
     if filename:
         artifact_reference = f"Image: {filename!r}"
     else:
         artifact_reference = "Comment"
     logging_output = dedent(
         f"""
         Added {artifact_reference} to Step: {step.name}
@@ -106,21 +106,21 @@
 
 
 def _register_model_logging(
     step: Step, data: dict, value: Any, step_name: str, attachments, _logger: Logger, step_artifacts: Any | None = None
 ):
     iteration_id = step._iteration.id
     url = step._client.auth.api_base_url
-    hyper_link = f"{url}/project/phase/iteration?w={step.workspace.id}&iterationId={iteration_id}"
+    hyper_link = f"{url}/browse/iteration/{iteration_id}"
 
     # check if exists
     existing_logging = existing_model_logger(data, value.name, _logger)
     # check if attached to step already
     check_artifacts = step_artifacts if step_artifacts else step.artifacts
-    match = next(filter(lambda x: x.model_version_id == data["modelVersion"]["id"], check_artifacts), None)
+    match = next(filter(lambda x: x.model_version_id == data["modelVersion"]["vecticeId"], check_artifacts), None)
     attachments_output = None
     if attachments:
         attachments_output = ", ".join([attach["fileName"] for attach in attachments])
     logging_output = None
     if existing_logging and match:
         logging_output = dedent(
             f"""
```

### Comparing `vectice-23.2.2.1/src/vectice/utils/logging_utils.py` & `vectice-23.2.3.0/src/vectice/utils/logging_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import logging
 import logging.config
 import sys
+from collections import defaultdict
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
+    from vectice.api.json.iteration import IterationStatus
     from vectice.api.json.phase import PhaseStatus
 
 
 CONNECTION_LOGGING = """Welcome, {user}. You`re now successfully connected to Vectice.
 
 To access your personal workspace, use \033[1mconnection\033[0m.my_workspace
 To access a specific workspace, use \033[1mconnection\033[0m.workspace(Workspace ID)
@@ -25,23 +27,23 @@
 
 CONNECTION_WORKSPACE_LOGGING = """Welcome, {user!r}. You`re now successfully connected to the workspace {workspace_name!r} in Vectice.
 
 To access a specific project, use \033[1mworkspace\033[0m.project(Project ID)
 To get a list of projects you can access and their IDs, use \033[1mworkspace\033[0m.list_projects()
 
 For quick access to the list of projects in the Vectice web app, visit:
-{url}/workspace/projects?w={workspace_id}"""
+{url}/browse/workspace/{workspace_id}"""
 
 CONNECTION_PROJECT_LOGGING = """Welcome, {user!r}. You`re now successfully connected to the project {project_name!r} in Vectice.
 
 To access a specific phase, use \033[1mproject\033[0m.phase(Phase ID)
 To get a list of phases you can access and their IDs, use \033[1mproject\033[0m.list_phases()
 
 For quick access to the list of phases in the Vectice web app, visit:
-{url}/project?w={workspace_id}&resourceId={project_id}"""
+{url}/browse/project/{project_id}"""
 
 
 class VecticeLoggingStream:
     """A Python stream for use with event logging APIs throughout vectice (`logger.info()`, etc.).
 
     This stream wraps `sys.stderr`, forwarding `write()`
     and `flush()` calls to the stream referred to by `sys.stderr` at the time of the call.
@@ -130,19 +132,34 @@
 
 def format_description(description: str | None) -> str | None:
     if not description:
         return None
     return description
 
 
-def get_phase_status(status: PhaseStatus) -> str:
-    from vectice.api.json.phase import PhaseStatus
+def get_iteration_status(status: IterationStatus, starred: bool | None) -> str:
+    verbose_dict: dict[str, str | None] = defaultdict(lambda: None)
+    verbose_dict["NotStarted"] = "Not Started"
+    verbose_dict["InProgress"] = "In Progress"
+    verbose_dict["Abandoned"] = "Abandoned"
+    verbose_dict["Completed"] = "Completed"
+    verbose_dict["InReview"] = "In Review"
+
+    status_value = verbose_dict[status.value]
+    if status_value is None:
+        raise ValueError("Iteration status unknown")
+    if starred:
+        return status_value + " (*)"
+    return status_value
 
-    if status is PhaseStatus.Completed:
-        return "[C]"
-    if status is PhaseStatus.NotStarted:
-        return "[NS]"
-    if status is PhaseStatus.InProgress:
-        return "[IP]"
-    if status is PhaseStatus.InReview:
-        return "[IR]"
-    return "UK"
+
+def get_phase_status(status: PhaseStatus) -> str:
+    verbose_dict: dict[str, str | None] = defaultdict(lambda: None)
+    verbose_dict["NotStarted"] = "Not Started"
+    verbose_dict["Draft"] = "In Progress"
+    verbose_dict["InReview"] = "In Review"
+    verbose_dict["Completed"] = "Completed"
+
+    status_value = verbose_dict[status.value]
+    if status_value is None:
+        raise ValueError("Phase status unknown")
+    return status_value
```

### Comparing `vectice-23.2.2.1/src/vectice.egg-info/PKG-INFO` & `vectice-23.2.3.0/src/vectice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.2.1
+Version: 23.2.3.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.2.1/src/vectice.egg-info/requires.txt` & `vectice-23.2.3.0/src/vectice.egg-info/requires.txt`

 * *Files identical despite different names*

