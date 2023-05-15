# Comparing `tmp/dagworks-sdk-0.0.2.tar.gz` & `tmp/dagworks-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagworks-sdk-0.0.2.tar", last modified: Fri May 12 05:33:49 2023, max compression
+gzip compressed data, was "dagworks-sdk-0.0.3.tar", last modified: Mon May 15 06:50:14 2023, max compression
```

## Comparing `dagworks-sdk-0.0.2.tar` & `dagworks-sdk-0.0.3.tar`

### file list

```diff
@@ -1,176 +1,184 @@
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.670145 dagworks-sdk-0.0.2/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-05-06 22:02:15.000000 dagworks-sdk-0.0.2/LICENSE
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-05-12 05:33:49.669782 dagworks-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3655 2023-05-11 21:36:24.000000 dagworks-sdk-0.0.2/README.md
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-05-09 05:21:02.000000 dagworks-sdk-0.0.2/pyproject.toml
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        7 2023-05-06 23:25:38.000000 dagworks-sdk-0.0.2/requirements-test.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      159 2023-05-12 05:33:31.000000 dagworks-sdk-0.0.2/requirements.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2023-05-12 05:33:49.670212 dagworks-sdk-0.0.2/setup.cfg
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-05-06 22:26:36.000000 dagworks-sdk-0.0.2/setup.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.619007 dagworks-sdk-0.0.2/src/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.621050 dagworks-sdk-0.0.2/src/dagworks/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1092 2023-05-12 05:13:53.000000 dagworks-sdk-0.0.2/src/dagworks/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.621982 dagworks-sdk-0.0.2/src/dagworks/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/api/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.622910 dagworks-sdk-0.0.2/src/dagworks/api/api_client/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      152 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.623144 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       47 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.624794 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3357 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2884 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5093 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4089 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3467 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.627962 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5253 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4689 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5031 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4526 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4972 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7040 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5671 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5489 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5753 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5625 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.629413 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4399 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5065 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6036 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6264 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5345 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2673 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/client.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      282 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/errors.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.643862 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3578 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2443 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/api_key_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1982 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/dependency.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2766 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2480 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_function.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3778 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1692 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1175 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1616 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/organization_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_api_key_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2238 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_project_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_run_log_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1649 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/phone_home_result.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1977 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1179 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_in_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3483 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1165 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3909 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1243 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5076 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1203 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_version_info.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5585 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1244 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1282 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1422 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/python_type.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1791 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_data.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4299 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1171 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_run_log.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5431 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1163 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5908 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3710 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1198 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run_result_summary.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      226 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run_status.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2101 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2101 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1586 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/user_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4362 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/visibility_full.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2570 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/visibility_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2306 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/who_am_i_result.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      974 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/types.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9242 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/api/clients.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1168 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/api/constants.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/api/projecttypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.645138 dagworks-sdk-0.0.2/src/dagworks/cli/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/cli/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1995 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/cli/cli.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6512 2023-05-12 05:28:39.000000 dagworks-sdk-0.0.2/src/dagworks/cli/initialize.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.645454 dagworks-sdk-0.0.2/src/dagworks/cli/templates/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.647412 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/.env.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-05-08 21:41:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/README.md.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-05-08 21:39:25.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/run.py.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2023-05-12 05:13:34.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.647745 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.648939 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-05-06 23:33:53.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/common.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2023-05-12 05:09:58.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.649302 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/config/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.650672 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2023-05-12 05:13:41.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.651168 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.651992 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1551 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.652830 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.653229 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.656057 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-05-04 05:23:39.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2023-05-12 05:08:52.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2023-05-12 05:08:52.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-05-12 05:09:11.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.656615 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.659340 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.659788 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    13968 2023-05-11 21:36:24.000000 dagworks-sdk-0.0.2/src/dagworks/driver.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.662927 dagworks-sdk-0.0.2/src/dagworks/parsing/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/parsing/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2394 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/parsing/dagtypes.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7810 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/parsing/parse.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.663693 dagworks-sdk-0.0.2/src/dagworks/telemetry/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/telemetry/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/telemetry/telemetry.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.665477 dagworks-sdk-0.0.2/src/dagworks/tracking/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/tracking/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/tracking/example_tracking.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9709 2023-05-08 17:27:34.000000 dagworks-sdk-0.0.2/src/dagworks/tracking/runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2411 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/tracking/trackingtypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.667885 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8007 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/entry_points.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      177 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/requires.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.669395 dagworks-sdk-0.0.2/tests/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2970 2023-05-06 23:49:00.000000 dagworks-sdk-0.0.2/tests/test_driver.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5497 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/tests/test_runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-02-13 05:18:55.000000 dagworks-sdk-0.0.2/tests/test_telemetry.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5924 2023-05-06 23:33:52.000000 dagworks-sdk-0.0.2/tests/test_tracking.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.794219 dagworks-sdk-0.0.3/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-05-06 22:02:15.000000 dagworks-sdk-0.0.3/LICENSE
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-05-15 06:50:14.793932 dagworks-sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3655 2023-05-11 21:36:24.000000 dagworks-sdk-0.0.3/README.md
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-05-09 05:21:02.000000 dagworks-sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        7 2023-05-06 23:25:38.000000 dagworks-sdk-0.0.3/requirements-test.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      159 2023-05-12 05:33:31.000000 dagworks-sdk-0.0.3/requirements.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2023-05-15 06:50:14.794346 dagworks-sdk-0.0.3/setup.cfg
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-05-06 22:26:36.000000 dagworks-sdk-0.0.3/setup.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.728571 dagworks-sdk-0.0.3/src/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.731438 dagworks-sdk-0.0.3/src/dagworks/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1092 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.734625 dagworks-sdk-0.0.3/src/dagworks/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/api/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.738502 dagworks-sdk-0.0.3/src/dagworks/api/api_client/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      152 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.739193 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       47 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.741953 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3379 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2926 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5383 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4111 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4813 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.746467 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3035 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5855 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4711 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5053 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4516 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4994 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8029 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5693 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5511 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5779 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6327 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.748537 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4421 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5087 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6058 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6286 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5367 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2817 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/client.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      470 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/errors.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.767729 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4237 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2443 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/api_key_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1982 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/dependency.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2706 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1285 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3019 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1268 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2766 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2480 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_function.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3778 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1692 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1175 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/organization_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_api_key_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2238 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_project_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_run_log_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1649 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/phone_home_result.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1977 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1179 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_in_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4499 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1165 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3909 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1243 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5339 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1203 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_version_info.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5848 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1244 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1282 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1422 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/python_type.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1791 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_data.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5416 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1185 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1171 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_run_log.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6517 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1163 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7054 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3710 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1198 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run_result_summary.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      226 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run_status.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3189 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2916 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1586 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/user_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4362 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/visibility_full.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3802 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/visibility_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2306 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/who_am_i_result.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      993 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/types.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9750 2023-05-15 05:04:41.000000 dagworks-sdk-0.0.3/src/dagworks/api/clients.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1168 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/api/constants.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/api/projecttypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.768718 dagworks-sdk-0.0.3/src/dagworks/cli/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/cli/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2025 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/cli/cli.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6513 2023-05-12 05:36:10.000000 dagworks-sdk-0.0.3/src/dagworks/cli/initialize.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.769149 dagworks-sdk-0.0.3/src/dagworks/cli/templates/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.771162 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/.env.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-05-08 21:41:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-05-08 21:39:25.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2023-05-12 05:13:34.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.771717 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.773165 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-05-06 23:33:53.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2023-05-12 05:09:58.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.773587 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/config/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.774685 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2023-05-12 05:13:41.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.775068 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.775570 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2023-05-14 22:17:33.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.776330 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.776604 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.778683 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-05-04 05:23:39.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2023-05-12 05:08:52.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2023-05-12 05:08:52.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-05-12 05:09:11.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.779266 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.781436 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.781755 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    14062 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/driver.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.786514 dagworks-sdk-0.0.3/src/dagworks/parsing/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/parsing/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2394 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/parsing/dagtypes.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7810 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/parsing/parse.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.788478 dagworks-sdk-0.0.3/src/dagworks/telemetry/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/telemetry/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/telemetry/telemetry.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.790021 dagworks-sdk-0.0.3/src/dagworks/tracking/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/tracking/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/tracking/example_tracking.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    10840 2023-05-12 23:31:41.000000 dagworks-sdk-0.0.3/src/dagworks/tracking/runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2411 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/tracking/trackingtypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.791561 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8551 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      177 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/requires.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.793291 dagworks-sdk-0.0.3/tests/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2970 2023-05-06 23:49:00.000000 dagworks-sdk-0.0.3/tests/test_driver.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5497 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/tests/test_runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-02-13 05:18:55.000000 dagworks-sdk-0.0.3/tests/test_telemetry.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6081 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/tests/test_tracking.py
```

### Comparing `dagworks-sdk-0.0.2/LICENSE` & `dagworks-sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/PKG-INFO` & `dagworks-sdk-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.2/README.md` & `dagworks-sdk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/pyproject.toml` & `dagworks-sdk-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/__init__.py` & `dagworks-sdk-0.0.3/src/dagworks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = (0, 0, 2)
+__version__ = (0, 0, 3)
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/__init__.py` & `dagworks-sdk-0.0.3/src/dagworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[str]:
     if response.status_code == HTTPStatus.OK:
         response_200 = cast(str, response.json())
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[str]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -78,15 +79,15 @@
     """Create Api Key
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[str]
+        str
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
@@ -121,15 +122,15 @@
     """Create Api Key
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[str]
+        str
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
     if response.status_code == HTTPStatus.OK:
         return None
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -50,17 +51,17 @@
     *,
     client: AuthenticatedClient,
 ) -> Response[Any]:
     """Delete Api Key
 
      Deletes an API key
 
-    :param request: Django request
-    :param api_key_id: ID of the API key to delete
-    :return:
+    @param request: Django request
+    @param api_key_id: ID of the API key to delete
+    @return:
 
     Args:
         api_key_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -87,17 +88,17 @@
     *,
     client: AuthenticatedClient,
 ) -> Response[Any]:
     """Delete Api Key
 
      Deletes an API key
 
-    :param request: Django request
-    :param api_key_id: ID of the API key to delete
-    :return:
+    @param request: Django request
+    @param api_key_id: ID of the API key to delete
+    @return:
 
     Args:
         api_key_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PagedApiKeyOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = PagedApiKeyOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[PagedApiKeyOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -61,18 +62,19 @@
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Response[PagedApiKeyOut]:
     """Get Api Keys
 
-     Gets the API keys for the current user
+     Gets the API keys for the current user.
+    All users can get this. Note that these are not in plaintext.
 
-    :param request:
-    :return:
+    @param request:
+    @return:
 
     Args:
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -100,29 +102,30 @@
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Optional[PagedApiKeyOut]:
     """Get Api Keys
 
-     Gets the API keys for the current user
+     Gets the API keys for the current user.
+    All users can get this. Note that these are not in plaintext.
 
-    :param request:
-    :return:
+    @param request:
+    @return:
 
     Args:
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PagedApiKeyOut]
+        PagedApiKeyOut
     """
 
     return sync_detailed(
         client=client,
         limit=limit,
         offset=offset,
     ).parsed
@@ -132,18 +135,19 @@
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Response[PagedApiKeyOut]:
     """Get Api Keys
 
-     Gets the API keys for the current user
+     Gets the API keys for the current user.
+    All users can get this. Note that these are not in plaintext.
 
-    :param request:
-    :return:
+    @param request:
+    @return:
 
     Args:
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -169,29 +173,30 @@
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Optional[PagedApiKeyOut]:
     """Get Api Keys
 
-     Gets the API keys for the current user
+     Gets the API keys for the current user.
+    All users can get this. Note that these are not in plaintext.
 
-    :param request:
-    :return:
+    @param request:
+    @return:
 
     Args:
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PagedApiKeyOut]
+        PagedApiKeyOut
     """
 
     return (
         await asyncio_detailed(
             client=client,
             limit=limit,
             offset=offset,
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,24 +20,25 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PhoneHomeResult]:
     if response.status_code == HTTPStatus.OK:
         response_200 = PhoneHomeResult.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[PhoneHomeResult]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -51,17 +52,17 @@
     *,
     client: AuthenticatedClient,
 ) -> Response[PhoneHomeResult]:
     """Phone Home
 
      Quick authentication validator. Tells you if you username/auth setup are legit.
 
-    :param request:
-    :param username:
-    :return:
+    @param request:
+    @param username:
+    @return:
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PhoneHomeResult]
@@ -83,24 +84,24 @@
     *,
     client: AuthenticatedClient,
 ) -> Optional[PhoneHomeResult]:
     """Phone Home
 
      Quick authentication validator. Tells you if you username/auth setup are legit.
 
-    :param request:
-    :param username:
-    :return:
+    @param request:
+    @param username:
+    @return:
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PhoneHomeResult]
+        PhoneHomeResult
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
@@ -108,17 +109,17 @@
     *,
     client: AuthenticatedClient,
 ) -> Response[PhoneHomeResult]:
     """Phone Home
 
      Quick authentication validator. Tells you if you username/auth setup are legit.
 
-    :param request:
-    :param username:
-    :return:
+    @param request:
+    @param username:
+    @return:
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PhoneHomeResult]
@@ -138,24 +139,24 @@
     *,
     client: AuthenticatedClient,
 ) -> Optional[PhoneHomeResult]:
     """Phone Home
 
      Quick authentication validator. Tells you if you username/auth setup are legit.
 
-    :param request:
-    :param username:
-    :return:
+    @param request:
+    @param username:
+    @return:
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PhoneHomeResult]
+        PhoneHomeResult
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,183 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.who_am_i_result import WhoAmIResult
+from ...models.run_log_out_with_run import RunLogOutWithRun
 from ...types import Response
 
 
 def _get_kwargs(
+    run_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/api/v0/whoami".format(client.base_url)
+    url = "{}/api/v0/runs/{run_id}".format(client.base_url, run_id=run_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[WhoAmIResult]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[RunLogOutWithRun]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = WhoAmIResult.from_dict(response.json())
+        response_200 = RunLogOutWithRun.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[WhoAmIResult]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[RunLogOutWithRun]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    run_id: int,
     *,
     client: AuthenticatedClient,
-) -> Response[WhoAmIResult]:
-    """Whoami
+) -> Response[RunLogOutWithRun]:
+    """Get Run
+
+     Gets a DAG run by ID
+
+    @param request:
+    @param run_id: The DAG run ID to query
+    @return: The DAG run we get from the DB
+
+    Args:
+        run_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[WhoAmIResult]
+        Response[RunLogOutWithRun]
     """
 
     kwargs = _get_kwargs(
+        run_id=run_id,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    run_id: int,
     *,
     client: AuthenticatedClient,
-) -> Optional[WhoAmIResult]:
-    """Whoami
+) -> Optional[RunLogOutWithRun]:
+    """Get Run
+
+     Gets a DAG run by ID
+
+    @param request:
+    @param run_id: The DAG run ID to query
+    @return: The DAG run we get from the DB
+
+    Args:
+        run_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[WhoAmIResult]
+        RunLogOutWithRun
     """
 
     return sync_detailed(
+        run_id=run_id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    run_id: int,
     *,
     client: AuthenticatedClient,
-) -> Response[WhoAmIResult]:
-    """Whoami
+) -> Response[RunLogOutWithRun]:
+    """Get Run
+
+     Gets a DAG run by ID
+
+    @param request:
+    @param run_id: The DAG run ID to query
+    @return: The DAG run we get from the DB
+
+    Args:
+        run_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[WhoAmIResult]
+        Response[RunLogOutWithRun]
     """
 
     kwargs = _get_kwargs(
+        run_id=run_id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    run_id: int,
     *,
     client: AuthenticatedClient,
-) -> Optional[WhoAmIResult]:
-    """Whoami
+) -> Optional[RunLogOutWithRun]:
+    """Get Run
+
+     Gets a DAG run by ID
+
+    @param request:
+    @param run_id: The DAG run ID to query
+    @return: The DAG run we get from the DB
+
+    Args:
+        run_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[WhoAmIResult]
+        RunLogOutWithRun
     """
 
     return (
         await asyncio_detailed(
+            run_id=run_id,
             client=client,
         )
     ).parsed
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,25 +26,26 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ProjectOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ProjectOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[ProjectOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -59,18 +60,20 @@
     client: AuthenticatedClient,
     json_body: TrackingserverApiApiCreateProjectBodyParams,
 ) -> Response[ProjectOut]:
     """Create Project
 
      Creates a project. User specifies visibility -- it will always be user-visible.
 
-    :param request:
-    :param exists_ok: Whether or not its OK if the project already exists
-    :param project:
-    :return:
+    @param request: Request from django ninja
+    @param project: Project to create
+    @param documentation: Documentation asset -- will be attached to the project
+    @param exists_ok: Whether or not its OK if the project already exists
+    @param project:
+    @return:
 
     Args:
         json_body (TrackingserverApiApiCreateProjectBodyParams):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -97,28 +100,30 @@
     client: AuthenticatedClient,
     json_body: TrackingserverApiApiCreateProjectBodyParams,
 ) -> Optional[ProjectOut]:
     """Create Project
 
      Creates a project. User specifies visibility -- it will always be user-visible.
 
-    :param request:
-    :param exists_ok: Whether or not its OK if the project already exists
-    :param project:
-    :return:
+    @param request: Request from django ninja
+    @param project: Project to create
+    @param documentation: Documentation asset -- will be attached to the project
+    @param exists_ok: Whether or not its OK if the project already exists
+    @param project:
+    @return:
 
     Args:
         json_body (TrackingserverApiApiCreateProjectBodyParams):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectOut]
+        ProjectOut
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
     ).parsed
 
@@ -128,18 +133,20 @@
     client: AuthenticatedClient,
     json_body: TrackingserverApiApiCreateProjectBodyParams,
 ) -> Response[ProjectOut]:
     """Create Project
 
      Creates a project. User specifies visibility -- it will always be user-visible.
 
-    :param request:
-    :param exists_ok: Whether or not its OK if the project already exists
-    :param project:
-    :return:
+    @param request: Request from django ninja
+    @param project: Project to create
+    @param documentation: Documentation asset -- will be attached to the project
+    @param exists_ok: Whether or not its OK if the project already exists
+    @param project:
+    @return:
 
     Args:
         json_body (TrackingserverApiApiCreateProjectBodyParams):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -164,28 +171,30 @@
     client: AuthenticatedClient,
     json_body: TrackingserverApiApiCreateProjectBodyParams,
 ) -> Optional[ProjectOut]:
     """Create Project
 
      Creates a project. User specifies visibility -- it will always be user-visible.
 
-    :param request:
-    :param exists_ok: Whether or not its OK if the project already exists
-    :param project:
-    :return:
+    @param request: Request from django ninja
+    @param project: Project to create
+    @param documentation: Documentation asset -- will be attached to the project
+    @param exists_ok: Whether or not its OK if the project already exists
+    @param project:
+    @return:
 
     Args:
         json_body (TrackingserverApiApiCreateProjectBodyParams):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectOut]
+        ProjectOut
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
         )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,26 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ProjectVersionOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ProjectVersionOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[ProjectVersionOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -57,18 +58,18 @@
     client: AuthenticatedClient,
     json_body: ProjectVersionInGit,
 ) -> Response[ProjectVersionOut]:
     """Create Project Version
 
      Creates a project version
 
-    :param request:
-    :param project_id:
-    :param version:
-    :return:
+    @param request:
+    @param project_id:
+    @param version:
+    @return:
 
     Args:
         json_body (ProjectVersionInGit):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -95,28 +96,28 @@
     client: AuthenticatedClient,
     json_body: ProjectVersionInGit,
 ) -> Optional[ProjectVersionOut]:
     """Create Project Version
 
      Creates a project version
 
-    :param request:
-    :param project_id:
-    :param version:
-    :return:
+    @param request:
+    @param project_id:
+    @param version:
+    @return:
 
     Args:
         json_body (ProjectVersionInGit):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectVersionOut]
+        ProjectVersionOut
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
     ).parsed
 
@@ -126,18 +127,18 @@
     client: AuthenticatedClient,
     json_body: ProjectVersionInGit,
 ) -> Response[ProjectVersionOut]:
     """Create Project Version
 
      Creates a project version
 
-    :param request:
-    :param project_id:
-    :param version:
-    :return:
+    @param request:
+    @param project_id:
+    @param version:
+    @return:
 
     Args:
         json_body (ProjectVersionInGit):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -162,28 +163,28 @@
     client: AuthenticatedClient,
     json_body: ProjectVersionInGit,
 ) -> Optional[ProjectVersionOut]:
     """Create Project Version
 
      Creates a project version
 
-    :param request:
-    :param project_id:
-    :param version:
-    :return:
+    @param request:
+    @param project_id:
+    @param version:
+    @return:
 
     Args:
         json_body (ProjectVersionInGit):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectVersionOut]
+        ProjectVersionOut
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
         )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,26 +23,27 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[ProjectVersionOutWithDAG]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ProjectVersionOutWithDAG.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
 ) -> Response[ProjectVersionOutWithDAG]:
@@ -58,17 +59,17 @@
     project_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Response[ProjectVersionOutWithDAG]:
     """Get Latest Project Version
 
      Gets the latest project version for a project
-    :param request: The Django request object
-    :param project_id: The project ID to query
-    :return: The latest project version associated with that project ID
+    @param request: The Django request object
+    @param project_id: The project ID to query
+    @return: The latest project version associated with that project ID
 
     Args:
         project_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -94,27 +95,27 @@
     project_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Optional[ProjectVersionOutWithDAG]:
     """Get Latest Project Version
 
      Gets the latest project version for a project
-    :param request: The Django request object
-    :param project_id: The project ID to query
-    :return: The latest project version associated with that project ID
+    @param request: The Django request object
+    @param project_id: The project ID to query
+    @return: The latest project version associated with that project ID
 
     Args:
         project_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectVersionOutWithDAG]
+        ProjectVersionOutWithDAG
     """
 
     return sync_detailed(
         project_id=project_id,
         client=client,
     ).parsed
 
@@ -123,17 +124,17 @@
     project_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Response[ProjectVersionOutWithDAG]:
     """Get Latest Project Version
 
      Gets the latest project version for a project
-    :param request: The Django request object
-    :param project_id: The project ID to query
-    :return: The latest project version associated with that project ID
+    @param request: The Django request object
+    @param project_id: The project ID to query
+    @return: The latest project version associated with that project ID
 
     Args:
         project_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -157,27 +158,27 @@
     project_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Optional[ProjectVersionOutWithDAG]:
     """Get Latest Project Version
 
      Gets the latest project version for a project
-    :param request: The Django request object
-    :param project_id: The project ID to query
-    :return: The latest project version associated with that project ID
+    @param request: The Django request object
+    @param project_id: The project ID to query
+    @return: The latest project version associated with that project ID
 
     Args:
         project_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectVersionOutWithDAG]
+        ProjectVersionOutWithDAG
     """
 
     return (
         await asyncio_detailed(
             project_id=project_id,
             client=client,
         )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,24 +21,25 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ProjectOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ProjectOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[ProjectOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -51,19 +52,19 @@
 def sync_detailed(
     project_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Response[ProjectOut]:
     """Get Project By Id
 
-     Gets a project by ID or name
+     Gets a project by ID
 
-    :param request: Django request
-    :param project_id:
-    :return: Null if project does not exist, else the project
+    @param request: Django request
+    @param project_id:
+    @return: Null if project does not exist, else the project
 
     Args:
         project_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -88,29 +89,29 @@
 def sync(
     project_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Optional[ProjectOut]:
     """Get Project By Id
 
-     Gets a project by ID or name
+     Gets a project by ID
 
-    :param request: Django request
-    :param project_id:
-    :return: Null if project does not exist, else the project
+    @param request: Django request
+    @param project_id:
+    @return: Null if project does not exist, else the project
 
     Args:
         project_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectOut]
+        ProjectOut
     """
 
     return sync_detailed(
         project_id=project_id,
         client=client,
     ).parsed
 
@@ -118,19 +119,19 @@
 async def asyncio_detailed(
     project_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Response[ProjectOut]:
     """Get Project By Id
 
-     Gets a project by ID or name
+     Gets a project by ID
 
-    :param request: Django request
-    :param project_id:
-    :return: Null if project does not exist, else the project
+    @param request: Django request
+    @param project_id:
+    @return: Null if project does not exist, else the project
 
     Args:
         project_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -153,29 +154,29 @@
 async def asyncio(
     project_id: int,
     *,
     client: AuthenticatedClient,
 ) -> Optional[ProjectOut]:
     """Get Project By Id
 
-     Gets a project by ID or name
+     Gets a project by ID
 
-    :param request: Django request
-    :param project_id:
-    :return: Null if project does not exist, else the project
+    @param request: Django request
+    @param project_id:
+    @return: Null if project does not exist, else the project
 
     Args:
         project_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectOut]
+        ProjectOut
     """
 
     return (
         await asyncio_detailed(
             project_id=project_id,
             client=client,
         )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,26 +23,27 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[ProjectVersionOutWithDAG]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ProjectVersionOutWithDAG.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
 ) -> Response[ProjectVersionOutWithDAG]:
@@ -61,16 +62,16 @@
 ) -> Response[ProjectVersionOutWithDAG]:
     """Get Project Version
 
      Gets a project version by ID
 
     # TODO -- validate that this works
 
-    :param project_version_id: ID to query
-    :return: The project version we get from the DB
+    @param project_version_id: ID to query
+    @return: The project version we get from the DB
 
     Args:
         project_version_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -99,26 +100,26 @@
 ) -> Optional[ProjectVersionOutWithDAG]:
     """Get Project Version
 
      Gets a project version by ID
 
     # TODO -- validate that this works
 
-    :param project_version_id: ID to query
-    :return: The project version we get from the DB
+    @param project_version_id: ID to query
+    @return: The project version we get from the DB
 
     Args:
         project_version_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectVersionOutWithDAG]
+        ProjectVersionOutWithDAG
     """
 
     return sync_detailed(
         project_version_id=project_version_id,
         client=client,
     ).parsed
 
@@ -130,16 +131,16 @@
 ) -> Response[ProjectVersionOutWithDAG]:
     """Get Project Version
 
      Gets a project version by ID
 
     # TODO -- validate that this works
 
-    :param project_version_id: ID to query
-    :return: The project version we get from the DB
+    @param project_version_id: ID to query
+    @return: The project version we get from the DB
 
     Args:
         project_version_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -166,26 +167,26 @@
 ) -> Optional[ProjectVersionOutWithDAG]:
     """Get Project Version
 
      Gets a project version by ID
 
     # TODO -- validate that this works
 
-    :param project_version_id: ID to query
-    :return: The project version we get from the DB
+    @param project_version_id: ID to query
+    @return: The project version we get from the DB
 
     Args:
         project_version_id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectVersionOutWithDAG]
+        ProjectVersionOutWithDAG
     """
 
     return (
         await asyncio_detailed(
             project_version_id=project_version_id,
             client=client,
         )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,35 +12,39 @@
 def _get_kwargs(
     project_id: int,
     *,
     client: AuthenticatedClient,
     name: Union[Unset, None, str] = UNSET,
     git_hash: Union[Unset, None, str] = UNSET,
     git_repo: Union[Unset, None, str] = UNSET,
+    include_archived: Union[Unset, None, bool] = False,
 ) -> Dict[str, Any]:
     url = "{}/api/v0/project_versions/{project_id}".format(client.base_url, project_id=project_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["name"] = name
 
     params["git_hash"] = git_hash
 
     params["git_repo"] = git_repo
 
+    params["include_archived"] = include_archived
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[List["ProjectVersionOut"]]:
@@ -50,15 +54,15 @@
         for response_200_item_data in _response_200:
             response_200_item = ProjectVersionOut.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
 ) -> Response[List["ProjectVersionOut"]]:
@@ -73,30 +77,33 @@
 def sync_detailed(
     project_id: int,
     *,
     client: AuthenticatedClient,
     name: Union[Unset, None, str] = UNSET,
     git_hash: Union[Unset, None, str] = UNSET,
     git_repo: Union[Unset, None, str] = UNSET,
+    include_archived: Union[Unset, None, bool] = False,
 ) -> Response[List["ProjectVersionOut"]]:
     """Get Project Versions
 
-     Gets a list of project versions for a project
+     Gets a list of project versions for a project.
+    At some point soon we'll likely need to paginate this...
 
-    :param git_repo:
-    :param git_hash:
-    :param request:
-    :param project_id: The project ID to query
-    :return: A list of project versions associated with that project ID, paginated
+    @param git_repo:
+    @param git_hash:
+    @param request:
+    @param project_id: The project ID to query
+    @return: A list of project versions associated with that project ID, paginated
 
     Args:
         project_id (int):
         name (Union[Unset, None, str]):
         git_hash (Union[Unset, None, str]):
         git_repo (Union[Unset, None, str]):
+        include_archived (Union[Unset, None, bool]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ProjectVersionOut']]
@@ -104,14 +111,15 @@
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         name=name,
         git_hash=git_hash,
         git_repo=git_repo,
+        include_archived=include_archived,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
@@ -121,71 +129,78 @@
 def sync(
     project_id: int,
     *,
     client: AuthenticatedClient,
     name: Union[Unset, None, str] = UNSET,
     git_hash: Union[Unset, None, str] = UNSET,
     git_repo: Union[Unset, None, str] = UNSET,
+    include_archived: Union[Unset, None, bool] = False,
 ) -> Optional[List["ProjectVersionOut"]]:
     """Get Project Versions
 
-     Gets a list of project versions for a project
+     Gets a list of project versions for a project.
+    At some point soon we'll likely need to paginate this...
 
-    :param git_repo:
-    :param git_hash:
-    :param request:
-    :param project_id: The project ID to query
-    :return: A list of project versions associated with that project ID, paginated
+    @param git_repo:
+    @param git_hash:
+    @param request:
+    @param project_id: The project ID to query
+    @return: A list of project versions associated with that project ID, paginated
 
     Args:
         project_id (int):
         name (Union[Unset, None, str]):
         git_hash (Union[Unset, None, str]):
         git_repo (Union[Unset, None, str]):
+        include_archived (Union[Unset, None, bool]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ProjectVersionOut']]
+        List['ProjectVersionOut']
     """
 
     return sync_detailed(
         project_id=project_id,
         client=client,
         name=name,
         git_hash=git_hash,
         git_repo=git_repo,
+        include_archived=include_archived,
     ).parsed
 
 
 async def asyncio_detailed(
     project_id: int,
     *,
     client: AuthenticatedClient,
     name: Union[Unset, None, str] = UNSET,
     git_hash: Union[Unset, None, str] = UNSET,
     git_repo: Union[Unset, None, str] = UNSET,
+    include_archived: Union[Unset, None, bool] = False,
 ) -> Response[List["ProjectVersionOut"]]:
     """Get Project Versions
 
-     Gets a list of project versions for a project
+     Gets a list of project versions for a project.
+    At some point soon we'll likely need to paginate this...
 
-    :param git_repo:
-    :param git_hash:
-    :param request:
-    :param project_id: The project ID to query
-    :return: A list of project versions associated with that project ID, paginated
+    @param git_repo:
+    @param git_hash:
+    @param request:
+    @param project_id: The project ID to query
+    @return: A list of project versions associated with that project ID, paginated
 
     Args:
         project_id (int):
         name (Union[Unset, None, str]):
         git_hash (Union[Unset, None, str]):
         git_repo (Union[Unset, None, str]):
+        include_archived (Union[Unset, None, bool]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ProjectVersionOut']]
@@ -193,14 +208,15 @@
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         name=name,
         git_hash=git_hash,
         git_repo=git_repo,
+        include_archived=include_archived,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
@@ -208,41 +224,45 @@
 async def asyncio(
     project_id: int,
     *,
     client: AuthenticatedClient,
     name: Union[Unset, None, str] = UNSET,
     git_hash: Union[Unset, None, str] = UNSET,
     git_repo: Union[Unset, None, str] = UNSET,
+    include_archived: Union[Unset, None, bool] = False,
 ) -> Optional[List["ProjectVersionOut"]]:
     """Get Project Versions
 
-     Gets a list of project versions for a project
+     Gets a list of project versions for a project.
+    At some point soon we'll likely need to paginate this...
 
-    :param git_repo:
-    :param git_hash:
-    :param request:
-    :param project_id: The project ID to query
-    :return: A list of project versions associated with that project ID, paginated
+    @param git_repo:
+    @param git_hash:
+    @param request:
+    @param project_id: The project ID to query
+    @return: A list of project versions associated with that project ID, paginated
 
     Args:
         project_id (int):
         name (Union[Unset, None, str]):
         git_hash (Union[Unset, None, str]):
         git_repo (Union[Unset, None, str]):
+        include_archived (Union[Unset, None, bool]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ProjectVersionOut']]
+        List['ProjectVersionOut']
     """
 
     return (
         await asyncio_detailed(
             project_id=project_id,
             client=client,
             name=name,
             git_hash=git_hash,
             git_repo=git_repo,
+            include_archived=include_archived,
         )
     ).parsed
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[List["ProjectVersionOutWithDAG"]]:
     if response.status_code == HTTPStatus.OK:
@@ -39,15 +40,15 @@
         for response_200_item_data in _response_200:
             response_200_item = ProjectVersionOutWithDAG.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
 ) -> Response[List["ProjectVersionOutWithDAG"]]:
@@ -65,16 +66,16 @@
     client: AuthenticatedClient,
 ) -> Response[List["ProjectVersionOutWithDAG"]]:
     """Get Project Versions Bulk By Id
 
      Gets project versions by IDs, in bulk.l This will return the same number out as it got it,
     in the same order.
 
-    :param project_version_ids: Comma-separated list of project version IDs to query
-    :return: The project versions we get from the DB
+    @param project_version_ids: Comma-separated list of project version IDs to query
+    @return: The project versions we get from the DB
 
     Args:
         project_version_ids (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -102,26 +103,26 @@
     client: AuthenticatedClient,
 ) -> Optional[List["ProjectVersionOutWithDAG"]]:
     """Get Project Versions Bulk By Id
 
      Gets project versions by IDs, in bulk.l This will return the same number out as it got it,
     in the same order.
 
-    :param project_version_ids: Comma-separated list of project version IDs to query
-    :return: The project versions we get from the DB
+    @param project_version_ids: Comma-separated list of project version IDs to query
+    @return: The project versions we get from the DB
 
     Args:
         project_version_ids (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ProjectVersionOutWithDAG']]
+        List['ProjectVersionOutWithDAG']
     """
 
     return sync_detailed(
         project_version_ids=project_version_ids,
         client=client,
     ).parsed
 
@@ -132,16 +133,16 @@
     client: AuthenticatedClient,
 ) -> Response[List["ProjectVersionOutWithDAG"]]:
     """Get Project Versions Bulk By Id
 
      Gets project versions by IDs, in bulk.l This will return the same number out as it got it,
     in the same order.
 
-    :param project_version_ids: Comma-separated list of project version IDs to query
-    :return: The project versions we get from the DB
+    @param project_version_ids: Comma-separated list of project version IDs to query
+    @return: The project versions we get from the DB
 
     Args:
         project_version_ids (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -167,26 +168,26 @@
     client: AuthenticatedClient,
 ) -> Optional[List["ProjectVersionOutWithDAG"]]:
     """Get Project Versions Bulk By Id
 
      Gets project versions by IDs, in bulk.l This will return the same number out as it got it,
     in the same order.
 
-    :param project_version_ids: Comma-separated list of project version IDs to query
-    :return: The project versions we get from the DB
+    @param project_version_ids: Comma-separated list of project version IDs to query
+    @return: The project versions we get from the DB
 
     Args:
         project_version_ids (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ProjectVersionOutWithDAG']]
+        List['ProjectVersionOutWithDAG']
     """
 
     return (
         await asyncio_detailed(
             project_version_ids=project_version_ids,
             client=client,
         )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PagedProjectOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = PagedProjectOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[PagedProjectOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -64,16 +65,16 @@
     offset: Union[Unset, None, int] = 0,
 ) -> Response[PagedProjectOut]:
     """Get Projects
 
      Gets a list of projects visible by a user, auto-paginating.
     TODO -- fix to use actual pagination on the db side
 
-    :param request:
-    :return: A list of projects
+    @param request:
+    @return: A list of projects
 
     Args:
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -104,27 +105,27 @@
     offset: Union[Unset, None, int] = 0,
 ) -> Optional[PagedProjectOut]:
     """Get Projects
 
      Gets a list of projects visible by a user, auto-paginating.
     TODO -- fix to use actual pagination on the db side
 
-    :param request:
-    :return: A list of projects
+    @param request:
+    @return: A list of projects
 
     Args:
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PagedProjectOut]
+        PagedProjectOut
     """
 
     return sync_detailed(
         client=client,
         limit=limit,
         offset=offset,
     ).parsed
@@ -137,16 +138,16 @@
     offset: Union[Unset, None, int] = 0,
 ) -> Response[PagedProjectOut]:
     """Get Projects
 
      Gets a list of projects visible by a user, auto-paginating.
     TODO -- fix to use actual pagination on the db side
 
-    :param request:
-    :return: A list of projects
+    @param request:
+    @return: A list of projects
 
     Args:
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -175,27 +176,27 @@
     offset: Union[Unset, None, int] = 0,
 ) -> Optional[PagedProjectOut]:
     """Get Projects
 
      Gets a list of projects visible by a user, auto-paginating.
     TODO -- fix to use actual pagination on the db side
 
-    :param request:
-    :return: A list of projects
+    @param request:
+    @return: A list of projects
 
     Args:
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PagedProjectOut]
+        PagedProjectOut
     """
 
     return (
         await asyncio_detailed(
             client=client,
             limit=limit,
             offset=offset,
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,29 +23,30 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List["ProjectOut"]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
             response_200_item = ProjectOut.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[List["ProjectOut"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -56,23 +57,23 @@
 
 
 def sync_detailed(
     project_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[List["ProjectOut"]]:
-    """Get Projects By Name
+    r"""Get Projects By Name
 
      Gets a project by name. Note that this doesn't use the standard auth mechanism,
     as a user could see a \"subset\" of projects by name. So we do the auth check manually
     in the loop below. A little inefficient, but this will be fine for now.
 
-    :param request: Django request
-    :param project_name:
-    :return: Null if project does not exist, else the project
+    @param request: Django request
+    @param project_name:
+    @return: Null if project does not exist, else the project
 
     Args:
         project_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -95,55 +96,55 @@
 
 
 def sync(
     project_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Optional[List["ProjectOut"]]:
-    """Get Projects By Name
+    r"""Get Projects By Name
 
      Gets a project by name. Note that this doesn't use the standard auth mechanism,
     as a user could see a \"subset\" of projects by name. So we do the auth check manually
     in the loop below. A little inefficient, but this will be fine for now.
 
-    :param request: Django request
-    :param project_name:
-    :return: Null if project does not exist, else the project
+    @param request: Django request
+    @param project_name:
+    @return: Null if project does not exist, else the project
 
     Args:
         project_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ProjectOut']]
+        List['ProjectOut']
     """
 
     return sync_detailed(
         project_name=project_name,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[List["ProjectOut"]]:
-    """Get Projects By Name
+    r"""Get Projects By Name
 
      Gets a project by name. Note that this doesn't use the standard auth mechanism,
     as a user could see a \"subset\" of projects by name. So we do the auth check manually
     in the loop below. A little inefficient, but this will be fine for now.
 
-    :param request: Django request
-    :param project_name:
-    :return: Null if project does not exist, else the project
+    @param request: Django request
+    @param project_name:
+    @return: Null if project does not exist, else the project
 
     Args:
         project_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -164,33 +165,33 @@
 
 
 async def asyncio(
     project_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Optional[List["ProjectOut"]]:
-    """Get Projects By Name
+    r"""Get Projects By Name
 
      Gets a project by name. Note that this doesn't use the standard auth mechanism,
     as a user could see a \"subset\" of projects by name. So we do the auth check manually
     in the loop below. A little inefficient, but this will be fine for now.
 
-    :param request: Django request
-    :param project_name:
-    :return: Null if project does not exist, else the project
+    @param request: Django request
+    @param project_name:
+    @return: Null if project does not exist, else the project
 
     Args:
         project_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ProjectOut']]
+        List['ProjectOut']
     """
 
     return (
         await asyncio_detailed(
             project_name=project_name,
             client=client,
         )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,25 +27,26 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ProjectOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ProjectOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[ProjectOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -61,18 +62,20 @@
     client: AuthenticatedClient,
     json_body: TrackingserverApiApiUpdateProjectBodyParams,
 ) -> Response[ProjectOut]:
     """Update Project
 
      Creates a project. User specifies visibility -- it will always be user-visible.
 
-    :param request:
-    :param exists_ok: Whether or not its OK if the project already exists
-    :param project:
-    :return:
+    @param request: Request from django ninja
+    @param project_id: The project id
+    @param project: Project to create
+    @param visibility: Visibility object of the project
+    @param documentation: Documentation asset  list-- will be attached to the project
+    @return: The updated project
 
     Args:
         project_id (int):
         json_body (TrackingserverApiApiUpdateProjectBodyParams):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -102,29 +105,31 @@
     client: AuthenticatedClient,
     json_body: TrackingserverApiApiUpdateProjectBodyParams,
 ) -> Optional[ProjectOut]:
     """Update Project
 
      Creates a project. User specifies visibility -- it will always be user-visible.
 
-    :param request:
-    :param exists_ok: Whether or not its OK if the project already exists
-    :param project:
-    :return:
+    @param request: Request from django ninja
+    @param project_id: The project id
+    @param project: Project to create
+    @param visibility: Visibility object of the project
+    @param documentation: Documentation asset  list-- will be attached to the project
+    @return: The updated project
 
     Args:
         project_id (int):
         json_body (TrackingserverApiApiUpdateProjectBodyParams):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectOut]
+        ProjectOut
     """
 
     return sync_detailed(
         project_id=project_id,
         client=client,
         json_body=json_body,
     ).parsed
@@ -136,18 +141,20 @@
     client: AuthenticatedClient,
     json_body: TrackingserverApiApiUpdateProjectBodyParams,
 ) -> Response[ProjectOut]:
     """Update Project
 
      Creates a project. User specifies visibility -- it will always be user-visible.
 
-    :param request:
-    :param exists_ok: Whether or not its OK if the project already exists
-    :param project:
-    :return:
+    @param request: Request from django ninja
+    @param project_id: The project id
+    @param project: Project to create
+    @param visibility: Visibility object of the project
+    @param documentation: Documentation asset  list-- will be attached to the project
+    @return: The updated project
 
     Args:
         project_id (int):
         json_body (TrackingserverApiApiUpdateProjectBodyParams):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -175,29 +182,31 @@
     client: AuthenticatedClient,
     json_body: TrackingserverApiApiUpdateProjectBodyParams,
 ) -> Optional[ProjectOut]:
     """Update Project
 
      Creates a project. User specifies visibility -- it will always be user-visible.
 
-    :param request:
-    :param exists_ok: Whether or not its OK if the project already exists
-    :param project:
-    :return:
+    @param request: Request from django ninja
+    @param project_id: The project id
+    @param project: Project to create
+    @param visibility: Visibility object of the project
+    @param documentation: Documentation asset  list-- will be attached to the project
+    @return: The updated project
 
     Args:
         project_id (int):
         json_body (TrackingserverApiApiUpdateProjectBodyParams):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ProjectOut]
+        ProjectOut
     """
 
     return (
         await asyncio_detailed(
             project_id=project_id,
             client=client,
             json_body=json_body,
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,182 +1,192 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.run_log_out_with_run import RunLogOutWithRun
 from ...types import Response
 
 
 def _get_kwargs(
-    run_id: int,
+    run_ids: str,
     *,
     client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/api/v0/runs/{run_id}".format(client.base_url, run_id=run_id)
+    url = "{}/api/v0/runs/bulk/{run_ids}".format(client.base_url, run_ids=run_ids)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[RunLogOutWithRun]:
+def _parse_response(
+    *, client: Client, response: httpx.Response
+) -> Optional[List["RunLogOutWithRun"]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = RunLogOutWithRun.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = RunLogOutWithRun.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[RunLogOutWithRun]:
+def _build_response(
+    *, client: Client, response: httpx.Response
+) -> Response[List["RunLogOutWithRun"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    run_id: int,
+    run_ids: str,
     *,
     client: AuthenticatedClient,
-) -> Response[RunLogOutWithRun]:
-    """Get Run
+) -> Response[List["RunLogOutWithRun"]]:
+    """Get Runs
 
-     Gets a DAG run by ID
+     Bulk queries run IDs. This will return a list of runs, in the same order as the run IDs.
 
-    :param request:
-    :param run_id: The DAG run ID to query
-    :return: The DAG run we get from the DB
+    @param request:
+    @param run_ids: The DAG run ID to query -- comma separated
+    @return: The DAG run we get from the DB
 
     Args:
-        run_id (int):
+        run_ids (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[RunLogOutWithRun]
+        Response[List['RunLogOutWithRun']]
     """
 
     kwargs = _get_kwargs(
-        run_id=run_id,
+        run_ids=run_ids,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    run_id: int,
+    run_ids: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[RunLogOutWithRun]:
-    """Get Run
+) -> Optional[List["RunLogOutWithRun"]]:
+    """Get Runs
 
-     Gets a DAG run by ID
+     Bulk queries run IDs. This will return a list of runs, in the same order as the run IDs.
 
-    :param request:
-    :param run_id: The DAG run ID to query
-    :return: The DAG run we get from the DB
+    @param request:
+    @param run_ids: The DAG run ID to query -- comma separated
+    @return: The DAG run we get from the DB
 
     Args:
-        run_id (int):
+        run_ids (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[RunLogOutWithRun]
+        List['RunLogOutWithRun']
     """
 
     return sync_detailed(
-        run_id=run_id,
+        run_ids=run_ids,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    run_id: int,
+    run_ids: str,
     *,
     client: AuthenticatedClient,
-) -> Response[RunLogOutWithRun]:
-    """Get Run
+) -> Response[List["RunLogOutWithRun"]]:
+    """Get Runs
 
-     Gets a DAG run by ID
+     Bulk queries run IDs. This will return a list of runs, in the same order as the run IDs.
 
-    :param request:
-    :param run_id: The DAG run ID to query
-    :return: The DAG run we get from the DB
+    @param request:
+    @param run_ids: The DAG run ID to query -- comma separated
+    @return: The DAG run we get from the DB
 
     Args:
-        run_id (int):
+        run_ids (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[RunLogOutWithRun]
+        Response[List['RunLogOutWithRun']]
     """
 
     kwargs = _get_kwargs(
-        run_id=run_id,
+        run_ids=run_ids,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    run_id: int,
+    run_ids: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[RunLogOutWithRun]:
-    """Get Run
+) -> Optional[List["RunLogOutWithRun"]]:
+    """Get Runs
 
-     Gets a DAG run by ID
+     Bulk queries run IDs. This will return a list of runs, in the same order as the run IDs.
 
-    :param request:
-    :param run_id: The DAG run ID to query
-    :return: The DAG run we get from the DB
+    @param request:
+    @param run_ids: The DAG run ID to query -- comma separated
+    @return: The DAG run we get from the DB
 
     Args:
-        run_id (int):
+        run_ids (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[RunLogOutWithRun]
+        List['RunLogOutWithRun']
     """
 
     return (
         await asyncio_detailed(
-            run_id=run_id,
+            run_ids=run_ids,
             client=client,
         )
     ).parsed
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,191 +1,170 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.run_log_out_with_run import RunLogOutWithRun
+from ...models.who_am_i_result import WhoAmIResult
 from ...types import Response
 
 
 def _get_kwargs(
-    run_ids: str,
     *,
     client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/api/v0/runs/bulk/{run_ids}".format(client.base_url, run_ids=run_ids)
+    url = "{}/api/v0/whoami".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[List["RunLogOutWithRun"]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[WhoAmIResult]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = RunLogOutWithRun.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
+        response_200 = WhoAmIResult.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[List["RunLogOutWithRun"]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[WhoAmIResult]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    run_ids: str,
     *,
     client: AuthenticatedClient,
-) -> Response[List["RunLogOutWithRun"]]:
-    """Get Runs
-
-     Bulk queries run IDs. This will return a list of runs, in the same order as the run IDs.
+) -> Response[WhoAmIResult]:
+    """Whoami
 
-    :param request:
-    :param run_ids: The DAG run ID to query -- comma separated
-    :return: The DAG run we get from the DB
+     Gives information about who you are, for the UI.
+    This allows us to be the central source of auth information/connected teams.
+    We synchronize everything on requests from the API, so that we don't have to
+    worry about stale data.
 
-    Args:
-        run_ids (str):
+    @param request: Incoming request with auth information
+    @return: WhoAmIResult
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['RunLogOutWithRun']]
+        Response[WhoAmIResult]
     """
 
     kwargs = _get_kwargs(
-        run_ids=run_ids,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    run_ids: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[List["RunLogOutWithRun"]]:
-    """Get Runs
-
-     Bulk queries run IDs. This will return a list of runs, in the same order as the run IDs.
+) -> Optional[WhoAmIResult]:
+    """Whoami
 
-    :param request:
-    :param run_ids: The DAG run ID to query -- comma separated
-    :return: The DAG run we get from the DB
+     Gives information about who you are, for the UI.
+    This allows us to be the central source of auth information/connected teams.
+    We synchronize everything on requests from the API, so that we don't have to
+    worry about stale data.
 
-    Args:
-        run_ids (str):
+    @param request: Incoming request with auth information
+    @return: WhoAmIResult
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['RunLogOutWithRun']]
+        WhoAmIResult
     """
 
     return sync_detailed(
-        run_ids=run_ids,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    run_ids: str,
     *,
     client: AuthenticatedClient,
-) -> Response[List["RunLogOutWithRun"]]:
-    """Get Runs
+) -> Response[WhoAmIResult]:
+    """Whoami
 
-     Bulk queries run IDs. This will return a list of runs, in the same order as the run IDs.
+     Gives information about who you are, for the UI.
+    This allows us to be the central source of auth information/connected teams.
+    We synchronize everything on requests from the API, so that we don't have to
+    worry about stale data.
 
-    :param request:
-    :param run_ids: The DAG run ID to query -- comma separated
-    :return: The DAG run we get from the DB
-
-    Args:
-        run_ids (str):
+    @param request: Incoming request with auth information
+    @return: WhoAmIResult
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['RunLogOutWithRun']]
+        Response[WhoAmIResult]
     """
 
     kwargs = _get_kwargs(
-        run_ids=run_ids,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    run_ids: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[List["RunLogOutWithRun"]]:
-    """Get Runs
-
-     Bulk queries run IDs. This will return a list of runs, in the same order as the run IDs.
+) -> Optional[WhoAmIResult]:
+    """Whoami
 
-    :param request:
-    :param run_ids: The DAG run ID to query -- comma separated
-    :return: The DAG run we get from the DB
+     Gives information about who you are, for the UI.
+    This allows us to be the central source of auth information/connected teams.
+    We synchronize everything on requests from the API, so that we don't have to
+    worry about stale data.
 
-    Args:
-        run_ids (str):
+    @param request: Incoming request with auth information
+    @return: WhoAmIResult
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['RunLogOutWithRun']]
+        WhoAmIResult
     """
 
     return (
         await asyncio_detailed(
-            run_ids=run_ids,
             client=client,
         )
     ).parsed
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,25 +32,26 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PagedRunLogOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = PagedRunLogOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[PagedRunLogOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -67,17 +68,17 @@
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Response[PagedRunLogOut]:
     """Get Runs From Project
 
      Gets a list of DAG runs for a project version
 
-    :param request:
-    :param project_id: The ID of the project to query
-    :return: A list of DAG runs associated with that project version ID, paginated
+    @param request:
+    @param project_id: The ID of the project to query
+    @return: A list of DAG runs associated with that project version ID, paginated
 
     Args:
         project_id (int):
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
@@ -110,29 +111,29 @@
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Optional[PagedRunLogOut]:
     """Get Runs From Project
 
      Gets a list of DAG runs for a project version
 
-    :param request:
-    :param project_id: The ID of the project to query
-    :return: A list of DAG runs associated with that project version ID, paginated
+    @param request:
+    @param project_id: The ID of the project to query
+    @return: A list of DAG runs associated with that project version ID, paginated
 
     Args:
         project_id (int):
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PagedRunLogOut]
+        PagedRunLogOut
     """
 
     return sync_detailed(
         client=client,
         project_id=project_id,
         limit=limit,
         offset=offset,
@@ -146,17 +147,17 @@
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Response[PagedRunLogOut]:
     """Get Runs From Project
 
      Gets a list of DAG runs for a project version
 
-    :param request:
-    :param project_id: The ID of the project to query
-    :return: A list of DAG runs associated with that project version ID, paginated
+    @param request:
+    @param project_id: The ID of the project to query
+    @return: A list of DAG runs associated with that project version ID, paginated
 
     Args:
         project_id (int):
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
@@ -187,29 +188,29 @@
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Optional[PagedRunLogOut]:
     """Get Runs From Project
 
      Gets a list of DAG runs for a project version
 
-    :param request:
-    :param project_id: The ID of the project to query
-    :return: A list of DAG runs associated with that project version ID, paginated
+    @param request:
+    @param project_id: The ID of the project to query
+    @return: A list of DAG runs associated with that project version ID, paginated
 
     Args:
         project_id (int):
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PagedRunLogOut]
+        PagedRunLogOut
     """
 
     return (
         await asyncio_detailed(
             client=client,
             project_id=project_id,
             limit=limit,
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,26 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PagedRunLogOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = PagedRunLogOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[PagedRunLogOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -67,17 +68,17 @@
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Response[PagedRunLogOut]:
     """Get Runs From Project Version
 
      Gets a list of DAG runs for a project version
 
-    :param request:
-    :param project_version_id: The project version ID to query
-    :return: A list of DAG runs associated with that project version ID, paginated
+    @param request:
+    @param project_version_id: The project version ID to query
+    @return: A list of DAG runs associated with that project version ID, paginated
 
     Args:
         project_version_id (int):
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
@@ -110,29 +111,29 @@
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Optional[PagedRunLogOut]:
     """Get Runs From Project Version
 
      Gets a list of DAG runs for a project version
 
-    :param request:
-    :param project_version_id: The project version ID to query
-    :return: A list of DAG runs associated with that project version ID, paginated
+    @param request:
+    @param project_version_id: The project version ID to query
+    @return: A list of DAG runs associated with that project version ID, paginated
 
     Args:
         project_version_id (int):
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PagedRunLogOut]
+        PagedRunLogOut
     """
 
     return sync_detailed(
         client=client,
         project_version_id=project_version_id,
         limit=limit,
         offset=offset,
@@ -146,17 +147,17 @@
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Response[PagedRunLogOut]:
     """Get Runs From Project Version
 
      Gets a list of DAG runs for a project version
 
-    :param request:
-    :param project_version_id: The project version ID to query
-    :return: A list of DAG runs associated with that project version ID, paginated
+    @param request:
+    @param project_version_id: The project version ID to query
+    @return: A list of DAG runs associated with that project version ID, paginated
 
     Args:
         project_version_id (int):
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
@@ -187,29 +188,29 @@
     limit: Union[Unset, None, int] = 100,
     offset: Union[Unset, None, int] = 0,
 ) -> Optional[PagedRunLogOut]:
     """Get Runs From Project Version
 
      Gets a list of DAG runs for a project version
 
-    :param request:
-    :param project_version_id: The project version ID to query
-    :return: A list of DAG runs associated with that project version ID, paginated
+    @param request:
+    @param project_version_id: The project version ID to query
+    @return: A list of DAG runs associated with that project version ID, paginated
 
     Args:
         project_version_id (int):
         limit (Union[Unset, None, int]):  Default: 100.
         offset (Union[Unset, None, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PagedRunLogOut]
+        PagedRunLogOut
     """
 
     return (
         await asyncio_detailed(
             client=client,
             project_version_id=project_version_id,
             limit=limit,
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,26 +30,27 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
         "params": params,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[RunLogOut]:
     if response.status_code == HTTPStatus.OK:
         response_200 = RunLogOut.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
+        raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[RunLogOut]:
     return Response(
         status_code=HTTPStatus(response.status_code),
@@ -65,17 +66,17 @@
     json_body: RunLogIn,
     project_version_id: int,
 ) -> Response[RunLogOut]:
     """Log Run
 
      Logs a DAG run
 
-    :param project_version_id: The project version ID to log the run for
-    :param dag_run: The DAG run to log
-    :return: The DAG run we get from the DB
+    @param project_version_id: The project version ID to log the run for
+    @param dag_run: The DAG run to log
+    @return: The DAG run we get from the DB
 
     Args:
         project_version_id (int):
         json_body (RunLogIn):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -105,28 +106,28 @@
     json_body: RunLogIn,
     project_version_id: int,
 ) -> Optional[RunLogOut]:
     """Log Run
 
      Logs a DAG run
 
-    :param project_version_id: The project version ID to log the run for
-    :param dag_run: The DAG run to log
-    :return: The DAG run we get from the DB
+    @param project_version_id: The project version ID to log the run for
+    @param dag_run: The DAG run to log
+    @return: The DAG run we get from the DB
 
     Args:
         project_version_id (int):
         json_body (RunLogIn):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[RunLogOut]
+        RunLogOut
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         project_version_id=project_version_id,
     ).parsed
@@ -138,17 +139,17 @@
     json_body: RunLogIn,
     project_version_id: int,
 ) -> Response[RunLogOut]:
     """Log Run
 
      Logs a DAG run
 
-    :param project_version_id: The project version ID to log the run for
-    :param dag_run: The DAG run to log
-    :return: The DAG run we get from the DB
+    @param project_version_id: The project version ID to log the run for
+    @param dag_run: The DAG run to log
+    @return: The DAG run we get from the DB
 
     Args:
         project_version_id (int):
         json_body (RunLogIn):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -176,28 +177,28 @@
     json_body: RunLogIn,
     project_version_id: int,
 ) -> Optional[RunLogOut]:
     """Log Run
 
      Logs a DAG run
 
-    :param project_version_id: The project version ID to log the run for
-    :param dag_run: The DAG run to log
-    :return: The DAG run we get from the DB
+    @param project_version_id: The project version ID to log the run for
+    @param dag_run: The DAG run to log
+    @return: The DAG run we get from the DB
 
     Args:
         project_version_id (int):
         json_body (RunLogIn):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[RunLogOut]
+        RunLogOut
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
             project_version_id=project_version_id,
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/client.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,24 @@
         headers: A dictionary of headers to be sent with every request
         timeout: The maximum amount of a time in seconds a request can take. API functions will raise
             httpx.TimeoutException if this is exceeded.
         verify_ssl: Whether or not to verify the SSL certificate of the API server. This should be True in production,
             but can be set to False for testing purposes.
         raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
             status code that was not documented in the source OpenAPI document.
+        follow_redirects: Whether or not to follow redirects. Default value is False.
     """
 
     base_url: str
     cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
     headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
     timeout: float = attr.ib(5.0, kw_only=True)
     verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
     raise_on_unexpected_status: bool = attr.ib(False, kw_only=True)
+    follow_redirects: bool = attr.ib(False, kw_only=True)
 
     def get_headers(self) -> Dict[str, str]:
         """Get headers to be used in all endpoints"""
         return {**self.headers}
 
     def with_headers(self, headers: Dict[str, str]) -> "Client":
         """Get a new client matching this one with additional headers"""
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/__init__.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """ Contains all the data models used in inputs/outputs """
 
 from .api_key_out import ApiKeyOut
 from .dependency import Dependency
+from .documentation_asset_in import DocumentationAssetIn
+from .documentation_asset_in_documentation import DocumentationAssetInDocumentation
+from .documentation_asset_out import DocumentationAssetOut
+from .documentation_asset_out_documentation import DocumentationAssetOutDocumentation
 from .hamilton_dag import HamiltonDAG
 from .hamilton_function import HamiltonFunction
 from .hamilton_node import HamiltonNode
 from .hamilton_node_dependencies import HamiltonNodeDependencies
 from .hamilton_node_tags import HamiltonNodeTags
 from .organization_out import OrganizationOut
 from .paged_api_key_out import PagedApiKeyOut
@@ -25,21 +29,24 @@
 from .project_version_out_with_dag import ProjectVersionOutWithDAG
 from .project_version_out_with_dag_tags import ProjectVersionOutWithDAGTags
 from .project_version_out_with_dag_version_info import ProjectVersionOutWithDAGVersionInfo
 from .python_type import PythonType
 from .run_log_data import RunLogData
 from .run_log_in import RunLogIn
 from .run_log_in_config import RunLogInConfig
+from .run_log_in_inputs import RunLogInInputs
 from .run_log_in_run_log import RunLogInRunLog
 from .run_log_in_tags import RunLogInTags
 from .run_log_out import RunLogOut
 from .run_log_out_config import RunLogOutConfig
+from .run_log_out_inputs import RunLogOutInputs
 from .run_log_out_tags import RunLogOutTags
 from .run_log_out_with_run import RunLogOutWithRun
 from .run_log_out_with_run_config import RunLogOutWithRunConfig
+from .run_log_out_with_run_inputs import RunLogOutWithRunInputs
 from .run_log_out_with_run_tags import RunLogOutWithRunTags
 from .task_run import TaskRun
 from .task_run_result_summary import TaskRunResultSummary
 from .task_run_status import TaskRunStatus
 from .trackingserver_api_api_create_project_body_params import (
     TrackingserverApiApiCreateProjectBodyParams,
 )
@@ -50,14 +57,18 @@
 from .visibility_full import VisibilityFull
 from .visibility_in import VisibilityIn
 from .who_am_i_result import WhoAmIResult
 
 __all__ = (
     "ApiKeyOut",
     "Dependency",
+    "DocumentationAssetIn",
+    "DocumentationAssetInDocumentation",
+    "DocumentationAssetOut",
+    "DocumentationAssetOutDocumentation",
     "HamiltonDAG",
     "HamiltonFunction",
     "HamiltonNode",
     "HamiltonNodeDependencies",
     "HamiltonNodeTags",
     "OrganizationOut",
     "PagedApiKeyOut",
@@ -77,21 +88,24 @@
     "ProjectVersionOutWithDAG",
     "ProjectVersionOutWithDAGTags",
     "ProjectVersionOutWithDAGVersionInfo",
     "PythonType",
     "RunLogData",
     "RunLogIn",
     "RunLogInConfig",
+    "RunLogInInputs",
     "RunLogInRunLog",
     "RunLogInTags",
     "RunLogOut",
     "RunLogOutConfig",
+    "RunLogOutInputs",
     "RunLogOutTags",
     "RunLogOutWithRun",
     "RunLogOutWithRunConfig",
+    "RunLogOutWithRunInputs",
     "RunLogOutWithRunTags",
     "TaskRun",
     "TaskRunResultSummary",
     "TaskRunStatus",
     "TrackingserverApiApiCreateProjectBodyParams",
     "TrackingserverApiApiUpdateProjectBodyParams",
     "UserOut",
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/api_key_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/dependency.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/dependency.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_dag.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_function.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_function.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node_dependencies.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node_dependencies.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/organization_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_project_out.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,75 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OrganizationOut")
+if TYPE_CHECKING:
+    from ..models.project_out import ProjectOut
+
+
+T = TypeVar("T", bound="PagedProjectOut")
 
 
 @attr.s(auto_attribs=True)
-class OrganizationOut:
+class PagedProjectOut:
     """
     Attributes:
-        name (str):
-        id (Union[Unset, int]):
+        count (int):
+        items (Union[Unset, List['ProjectOut']]):
     """
 
-    name: str
-    id: Union[Unset, int] = UNSET
+    count: int
+    items: Union[Unset, List["ProjectOut"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        id = self.id
+        count = self.count
+        items: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.items, Unset):
+            items = []
+            for items_item_data in self.items:
+                items_item = items_item_data.to_dict()
+
+                items.append(items_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "name": name,
+                "count": count,
             }
         )
-        if id is not UNSET:
-            field_dict["id"] = id
+        if items is not UNSET:
+            field_dict["items"] = items
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        name = d.pop("name")
+        from ..models.project_out import ProjectOut
 
-        id = d.pop("id", UNSET)
+        d = src_dict.copy()
+        count = d.pop("count")
 
-        organization_out = cls(
-            name=name,
-            id=id,
+        items = []
+        _items = d.pop("items", UNSET)
+        for items_item_data in _items or []:
+            items_item = ProjectOut.from_dict(items_item_data)
+
+            items.append(items_item)
+
+        paged_project_out = cls(
+            count=count,
+            items=items,
         )
 
-        organization_out.additional_properties = d
-        return organization_out
+        paged_project_out.additional_properties = d
+        return paged_project_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_api_key_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_project_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_run_log_out.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.project_out import ProjectOut
+    from ..models.run_log_out import RunLogOut
 
 
-T = TypeVar("T", bound="PagedProjectOut")
+T = TypeVar("T", bound="PagedRunLogOut")
 
 
 @attr.s(auto_attribs=True)
-class PagedProjectOut:
+class PagedRunLogOut:
     """
     Attributes:
         count (int):
-        items (Union[Unset, List['ProjectOut']]):
+        items (Union[Unset, List['RunLogOut']]):
     """
 
     count: int
-    items: Union[Unset, List["ProjectOut"]] = UNSET
+    items: Union[Unset, List["RunLogOut"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
         items: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.items, Unset):
             items = []
@@ -43,33 +43,33 @@
         if items is not UNSET:
             field_dict["items"] = items
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_out import ProjectOut
+        from ..models.run_log_out import RunLogOut
 
         d = src_dict.copy()
         count = d.pop("count")
 
         items = []
         _items = d.pop("items", UNSET)
         for items_item_data in _items or []:
-            items_item = ProjectOut.from_dict(items_item_data)
+            items_item = RunLogOut.from_dict(items_item_data)
 
             items.append(items_item)
 
-        paged_project_out = cls(
+        paged_run_log_out = cls(
             count=count,
             items=items,
         )
 
-        paged_project_out.additional_properties = d
-        return paged_project_out
+        paged_run_log_out.additional_properties = d
+        return paged_run_log_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_run_log_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,63 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
 if TYPE_CHECKING:
-    from ..models.run_log_out import RunLogOut
+    from ..models.task_run import TaskRun
 
 
-T = TypeVar("T", bound="PagedRunLogOut")
+T = TypeVar("T", bound="RunLogData")
 
 
 @attr.s(auto_attribs=True)
-class PagedRunLogOut:
+class RunLogData:
     """
     Attributes:
-        count (int):
-        items (Union[Unset, List['RunLogOut']]):
+        tasks (List['TaskRun']):
     """
 
-    count: int
-    items: Union[Unset, List["RunLogOut"]] = UNSET
+    tasks: List["TaskRun"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        count = self.count
-        items: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.items, Unset):
-            items = []
-            for items_item_data in self.items:
-                items_item = items_item_data.to_dict()
+        tasks = []
+        for tasks_item_data in self.tasks:
+            tasks_item = tasks_item_data.to_dict()
 
-                items.append(items_item)
+            tasks.append(tasks_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "count": count,
+                "tasks": tasks,
             }
         )
-        if items is not UNSET:
-            field_dict["items"] = items
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.run_log_out import RunLogOut
+        from ..models.task_run import TaskRun
 
         d = src_dict.copy()
-        count = d.pop("count")
+        tasks = []
+        _tasks = d.pop("tasks")
+        for tasks_item_data in _tasks:
+            tasks_item = TaskRun.from_dict(tasks_item_data)
+
+            tasks.append(tasks_item)
 
-        items = []
-        _items = d.pop("items", UNSET)
-        for items_item_data in _items or []:
-            items_item = RunLogOut.from_dict(items_item_data)
-
-            items.append(items_item)
-
-        paged_run_log_out = cls(
-            count=count,
-            items=items,
+        run_log_data = cls(
+            tasks=tasks,
         )
 
-        paged_run_log_out.additional_properties = d
-        return paged_run_log_out
+        run_log_data.additional_properties = d
+        return run_log_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/phone_home_result.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/phone_home_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_in.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_in_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_out.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
+    from ..models.documentation_asset_out import DocumentationAssetOut
     from ..models.project_out_tags import ProjectOutTags
     from ..models.visibility_full import VisibilityFull
 
 
 T = TypeVar("T", bound="ProjectOut")
 
 
@@ -21,25 +22,29 @@
         name (str):
         description (str):
         tags (ProjectOutTags):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
         owner (str):
         permissions (VisibilityFull):
+        documentation (List['DocumentationAssetOut']):
+        can_write (bool):
         id (Union[Unset, int]):
         slug (Union[Unset, str]):
     """
 
     name: str
     description: str
     tags: "ProjectOutTags"
     created_at: datetime.datetime
     updated_at: datetime.datetime
     owner: str
     permissions: "VisibilityFull"
+    documentation: List["DocumentationAssetOut"]
+    can_write: bool
     id: Union[Unset, int] = UNSET
     slug: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         description = self.description
@@ -48,39 +53,49 @@
         created_at = self.created_at.isoformat()
 
         updated_at = self.updated_at.isoformat()
 
         owner = self.owner
         permissions = self.permissions.to_dict()
 
+        documentation = []
+        for documentation_item_data in self.documentation:
+            documentation_item = documentation_item_data.to_dict()
+
+            documentation.append(documentation_item)
+
+        can_write = self.can_write
         id = self.id
         slug = self.slug
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "name": name,
                 "description": description,
                 "tags": tags,
                 "created_at": created_at,
                 "updated_at": updated_at,
                 "owner": owner,
                 "permissions": permissions,
+                "documentation": documentation,
+                "can_write": can_write,
             }
         )
         if id is not UNSET:
             field_dict["id"] = id
         if slug is not UNSET:
             field_dict["slug"] = slug
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.documentation_asset_out import DocumentationAssetOut
         from ..models.project_out_tags import ProjectOutTags
         from ..models.visibility_full import VisibilityFull
 
         d = src_dict.copy()
         name = d.pop("name")
 
         description = d.pop("description")
@@ -91,26 +106,37 @@
 
         updated_at = isoparse(d.pop("updated_at"))
 
         owner = d.pop("owner")
 
         permissions = VisibilityFull.from_dict(d.pop("permissions"))
 
+        documentation = []
+        _documentation = d.pop("documentation")
+        for documentation_item_data in _documentation:
+            documentation_item = DocumentationAssetOut.from_dict(documentation_item_data)
+
+            documentation.append(documentation_item)
+
+        can_write = d.pop("can_write")
+
         id = d.pop("id", UNSET)
 
         slug = d.pop("slug", UNSET)
 
         project_out = cls(
             name=name,
             description=description,
             tags=tags,
             created_at=created_at,
             updated_at=updated_at,
             owner=owner,
             permissions=permissions,
+            documentation=documentation,
+            can_write=can_write,
             id=id,
             slug=slug,
         )
 
         project_out.additional_properties = d
         return project_out
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_out_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git_dag.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         dag_schema_version (int):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
         logged_by (int):
         id (Union[Unset, int]):
         slug (Union[Unset, str]):
         tags (Union[Unset, ProjectVersionOutTags]):
+        active (Union[Unset, bool]):  Default: True.
     """
 
     project: int
     name: str
     version_info: "ProjectVersionOutVersionInfo"
     version_info_type: str
     version_info_schema: int
@@ -42,14 +43,15 @@
     dag_schema_version: int
     created_at: datetime.datetime
     updated_at: datetime.datetime
     logged_by: int
     id: Union[Unset, int] = UNSET
     slug: Union[Unset, str] = UNSET
     tags: Union[Unset, "ProjectVersionOutTags"] = UNSET
+    active: Union[Unset, bool] = True
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project = self.project
         name = self.name
         version_info = self.version_info.to_dict()
 
@@ -64,14 +66,16 @@
         logged_by = self.logged_by
         id = self.id
         slug = self.slug
         tags: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.tags, Unset):
             tags = self.tags.to_dict()
 
+        active = self.active
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "project": project,
                 "name": name,
                 "version_info": version_info,
@@ -86,14 +90,16 @@
         )
         if id is not UNSET:
             field_dict["id"] = id
         if slug is not UNSET:
             field_dict["slug"] = slug
         if tags is not UNSET:
             field_dict["tags"] = tags
+        if active is not UNSET:
+            field_dict["active"] = active
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.project_version_out_tags import ProjectVersionOutTags
         from ..models.project_version_out_version_info import ProjectVersionOutVersionInfo
@@ -126,28 +132,31 @@
         _tags = d.pop("tags", UNSET)
         tags: Union[Unset, ProjectVersionOutTags]
         if isinstance(_tags, Unset):
             tags = UNSET
         else:
             tags = ProjectVersionOutTags.from_dict(_tags)
 
+        active = d.pop("active", UNSET)
+
         project_version_out = cls(
             project=project,
             name=name,
             version_info=version_info,
             version_info_type=version_info_type,
             version_info_schema=version_info_schema,
             dag_pointer=dag_pointer,
             dag_schema_version=dag_schema_version,
             created_at=created_at,
             updated_at=updated_at,
             logged_by=logged_by,
             id=id,
             slug=slug,
             tags=tags,
+            active=active,
         )
 
         project_version_out.additional_properties = d
         return project_version_out
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_version_info.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
         logged_by (int):
         dag (HamiltonDAG): Represents a logical DAG
         id (Union[Unset, int]):
         slug (Union[Unset, str]):
         tags (Union[Unset, ProjectVersionOutWithDAGTags]):
+        active (Union[Unset, bool]):  Default: True.
     """
 
     project: int
     name: str
     version_info: "ProjectVersionOutWithDAGVersionInfo"
     version_info_type: str
     version_info_schema: int
@@ -47,14 +48,15 @@
     created_at: datetime.datetime
     updated_at: datetime.datetime
     logged_by: int
     dag: "HamiltonDAG"
     id: Union[Unset, int] = UNSET
     slug: Union[Unset, str] = UNSET
     tags: Union[Unset, "ProjectVersionOutWithDAGTags"] = UNSET
+    active: Union[Unset, bool] = True
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project = self.project
         name = self.name
         version_info = self.version_info.to_dict()
 
@@ -71,14 +73,16 @@
 
         id = self.id
         slug = self.slug
         tags: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.tags, Unset):
             tags = self.tags.to_dict()
 
+        active = self.active
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "project": project,
                 "name": name,
                 "version_info": version_info,
@@ -94,14 +98,16 @@
         )
         if id is not UNSET:
             field_dict["id"] = id
         if slug is not UNSET:
             field_dict["slug"] = slug
         if tags is not UNSET:
             field_dict["tags"] = tags
+        if active is not UNSET:
+            field_dict["active"] = active
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.hamilton_dag import HamiltonDAG
         from ..models.project_version_out_with_dag_tags import ProjectVersionOutWithDAGTags
@@ -139,14 +145,16 @@
         _tags = d.pop("tags", UNSET)
         tags: Union[Unset, ProjectVersionOutWithDAGTags]
         if isinstance(_tags, Unset):
             tags = UNSET
         else:
             tags = ProjectVersionOutWithDAGTags.from_dict(_tags)
 
+        active = d.pop("active", UNSET)
+
         project_version_out_with_dag = cls(
             project=project,
             name=name,
             version_info=version_info,
             version_info_type=version_info_type,
             version_info_schema=version_info_schema,
             dag_pointer=dag_pointer,
@@ -154,14 +162,15 @@
             created_at=created_at,
             updated_at=updated_at,
             logged_by=logged_by,
             dag=dag,
             id=id,
             slug=slug,
             tags=tags,
+            active=active,
         )
 
         project_version_out_with_dag.additional_properties = d
         return project_version_out_with_dag
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/python_type.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/python_type.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_data.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/user_out.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,58 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.task_run import TaskRun
+from ..types import UNSET, Unset
 
-
-T = TypeVar("T", bound="RunLogData")
+T = TypeVar("T", bound="UserOut")
 
 
 @attr.s(auto_attribs=True)
-class RunLogData:
+class UserOut:
     """
     Attributes:
-        tasks (List['TaskRun']):
+        email (str):
+        id (Union[Unset, int]):
     """
 
-    tasks: List["TaskRun"]
+    email: str
+    id: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        tasks = []
-        for tasks_item_data in self.tasks:
-            tasks_item = tasks_item_data.to_dict()
-
-            tasks.append(tasks_item)
+        email = self.email
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "tasks": tasks,
+                "email": email,
             }
         )
+        if id is not UNSET:
+            field_dict["id"] = id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.task_run import TaskRun
-
         d = src_dict.copy()
-        tasks = []
-        _tasks = d.pop("tasks")
-        for tasks_item_data in _tasks:
-            tasks_item = TaskRun.from_dict(tasks_item_data)
+        email = d.pop("email")
 
-            tasks.append(tasks_item)
+        id = d.pop("id", UNSET)
 
-        run_log_data = cls(
-            tasks=tasks,
+        user_out = cls(
+            email=email,
+            id=id,
         )
 
-        run_log_data.additional_properties = d
-        return run_log_data
+        user_out.additional_properties = d
+        return user_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.run_log_in_config import RunLogInConfig
+    from ..models.run_log_in_inputs import RunLogInInputs
     from ..models.run_log_in_run_log import RunLogInRunLog
     from ..models.run_log_in_tags import RunLogInTags
 
 
 T = TypeVar("T", bound="RunLogIn")
 
 
@@ -24,25 +25,29 @@
         run_id (str): User-generated run ID
         start_time (datetime.datetime): The time the run started
         end_time (datetime.datetime): The time the run ended
         run_log_schema_version (int): The schema version of the run log
         run_log (RunLogInRunLog):
         status (str): The status of the run
         tags (Union[Unset, RunLogInTags]): Tags for the run
+        inputs (Union[Unset, RunLogInInputs]): Inputs for the run
+        outputs (Union[Unset, List[str]]): Outputs for the run
     """
 
     project_version_id: int
     config: "RunLogInConfig"
     run_id: str
     start_time: datetime.datetime
     end_time: datetime.datetime
     run_log_schema_version: int
     run_log: "RunLogInRunLog"
     status: str
     tags: Union[Unset, "RunLogInTags"] = UNSET
+    inputs: Union[Unset, "RunLogInInputs"] = UNSET
+    outputs: Union[Unset, List[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project_version_id = self.project_version_id
         config = self.config.to_dict()
 
         run_id = self.run_id
@@ -54,14 +59,22 @@
         run_log = self.run_log.to_dict()
 
         status = self.status
         tags: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.tags, Unset):
             tags = self.tags.to_dict()
 
+        inputs: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.inputs, Unset):
+            inputs = self.inputs.to_dict()
+
+        outputs: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.outputs, Unset):
+            outputs = self.outputs
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "project_version_id": project_version_id,
                 "config": config,
                 "run_id": run_id,
@@ -70,20 +83,25 @@
                 "run_log_schema_version": run_log_schema_version,
                 "run_log": run_log,
                 "status": status,
             }
         )
         if tags is not UNSET:
             field_dict["tags"] = tags
+        if inputs is not UNSET:
+            field_dict["inputs"] = inputs
+        if outputs is not UNSET:
+            field_dict["outputs"] = outputs
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.run_log_in_config import RunLogInConfig
+        from ..models.run_log_in_inputs import RunLogInInputs
         from ..models.run_log_in_run_log import RunLogInRunLog
         from ..models.run_log_in_tags import RunLogInTags
 
         d = src_dict.copy()
         project_version_id = d.pop("project_version_id")
 
         config = RunLogInConfig.from_dict(d.pop("config"))
@@ -103,24 +121,35 @@
         _tags = d.pop("tags", UNSET)
         tags: Union[Unset, RunLogInTags]
         if isinstance(_tags, Unset):
             tags = UNSET
         else:
             tags = RunLogInTags.from_dict(_tags)
 
+        _inputs = d.pop("inputs", UNSET)
+        inputs: Union[Unset, RunLogInInputs]
+        if isinstance(_inputs, Unset):
+            inputs = UNSET
+        else:
+            inputs = RunLogInInputs.from_dict(_inputs)
+
+        outputs = cast(List[str], d.pop("outputs", UNSET))
+
         run_log_in = cls(
             project_version_id=project_version_id,
             config=config,
             run_id=run_id,
             start_time=start_time,
             end_time=end_time,
             run_log_schema_version=run_log_schema_version,
             run_log=run_log,
             status=status,
             tags=tags,
+            inputs=inputs,
+            outputs=outputs,
         )
 
         run_log_in.additional_properties = d
         return run_log_in
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_config.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_run_log.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_run_log.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.run_log_out_config import RunLogOutConfig
+    from ..models.run_log_out_inputs import RunLogOutInputs
     from ..models.run_log_out_tags import RunLogOutTags
 
 
 T = TypeVar("T", bound="RunLogOut")
 
 
 @attr.s(auto_attribs=True)
@@ -26,14 +27,16 @@
         run_log_pointer (str):
         run_log_schema_version (int):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
         status (str):
         username_resolved (str):
         id (Union[Unset, int]):
+        inputs (Union[Unset, RunLogOutInputs]):
+        outputs (Union[Unset, List[Any]]):
         tags (Union[Unset, RunLogOutTags]):
         username (Union[Unset, int]):
         slug (Union[Unset, str]):
     """
 
     project_version: int
     config: "RunLogOutConfig"
@@ -43,14 +46,16 @@
     run_log_pointer: str
     run_log_schema_version: int
     created_at: datetime.datetime
     updated_at: datetime.datetime
     status: str
     username_resolved: str
     id: Union[Unset, int] = UNSET
+    inputs: Union[Unset, "RunLogOutInputs"] = UNSET
+    outputs: Union[Unset, List[Any]] = UNSET
     tags: Union[Unset, "RunLogOutTags"] = UNSET
     username: Union[Unset, int] = UNSET
     slug: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project_version = self.project_version
@@ -66,14 +71,22 @@
         created_at = self.created_at.isoformat()
 
         updated_at = self.updated_at.isoformat()
 
         status = self.status
         username_resolved = self.username_resolved
         id = self.id
+        inputs: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.inputs, Unset):
+            inputs = self.inputs.to_dict()
+
+        outputs: Union[Unset, List[Any]] = UNSET
+        if not isinstance(self.outputs, Unset):
+            outputs = self.outputs
+
         tags: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.tags, Unset):
             tags = self.tags.to_dict()
 
         username = self.username
         slug = self.slug
 
@@ -92,26 +105,31 @@
                 "updated_at": updated_at,
                 "status": status,
                 "username_resolved": username_resolved,
             }
         )
         if id is not UNSET:
             field_dict["id"] = id
+        if inputs is not UNSET:
+            field_dict["inputs"] = inputs
+        if outputs is not UNSET:
+            field_dict["outputs"] = outputs
         if tags is not UNSET:
             field_dict["tags"] = tags
         if username is not UNSET:
             field_dict["username"] = username
         if slug is not UNSET:
             field_dict["slug"] = slug
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.run_log_out_config import RunLogOutConfig
+        from ..models.run_log_out_inputs import RunLogOutInputs
         from ..models.run_log_out_tags import RunLogOutTags
 
         d = src_dict.copy()
         project_version = d.pop("project_version")
 
         config = RunLogOutConfig.from_dict(d.pop("config"))
 
@@ -131,14 +149,23 @@
 
         status = d.pop("status")
 
         username_resolved = d.pop("username_resolved")
 
         id = d.pop("id", UNSET)
 
+        _inputs = d.pop("inputs", UNSET)
+        inputs: Union[Unset, RunLogOutInputs]
+        if isinstance(_inputs, Unset):
+            inputs = UNSET
+        else:
+            inputs = RunLogOutInputs.from_dict(_inputs)
+
+        outputs = cast(List[Any], d.pop("outputs", UNSET))
+
         _tags = d.pop("tags", UNSET)
         tags: Union[Unset, RunLogOutTags]
         if isinstance(_tags, Unset):
             tags = UNSET
         else:
             tags = RunLogOutTags.from_dict(_tags)
 
@@ -155,14 +182,16 @@
             run_log_pointer=run_log_pointer,
             run_log_schema_version=run_log_schema_version,
             created_at=created_at,
             updated_at=updated_at,
             status=status,
             username_resolved=username_resolved,
             id=id,
+            inputs=inputs,
+            outputs=outputs,
             tags=tags,
             username=username,
             slug=slug,
         )
 
         run_log_out.additional_properties = d
         return run_log_out
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_config.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.run_log_data import RunLogData
     from ..models.run_log_out_with_run_config import RunLogOutWithRunConfig
+    from ..models.run_log_out_with_run_inputs import RunLogOutWithRunInputs
     from ..models.run_log_out_with_run_tags import RunLogOutWithRunTags
 
 
 T = TypeVar("T", bound="RunLogOutWithRun")
 
 
 @attr.s(auto_attribs=True)
@@ -28,14 +29,16 @@
         run_log_schema_version (int):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
         status (str):
         username_resolved (str):
         run_log (RunLogData):
         id (Union[Unset, int]):
+        inputs (Union[Unset, RunLogOutWithRunInputs]):
+        outputs (Union[Unset, List[Any]]):
         tags (Union[Unset, RunLogOutWithRunTags]):
         username (Union[Unset, int]):
         slug (Union[Unset, str]):
     """
 
     project_version: int
     config: "RunLogOutWithRunConfig"
@@ -46,14 +49,16 @@
     run_log_schema_version: int
     created_at: datetime.datetime
     updated_at: datetime.datetime
     status: str
     username_resolved: str
     run_log: "RunLogData"
     id: Union[Unset, int] = UNSET
+    inputs: Union[Unset, "RunLogOutWithRunInputs"] = UNSET
+    outputs: Union[Unset, List[Any]] = UNSET
     tags: Union[Unset, "RunLogOutWithRunTags"] = UNSET
     username: Union[Unset, int] = UNSET
     slug: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project_version = self.project_version
@@ -71,14 +76,22 @@
         updated_at = self.updated_at.isoformat()
 
         status = self.status
         username_resolved = self.username_resolved
         run_log = self.run_log.to_dict()
 
         id = self.id
+        inputs: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.inputs, Unset):
+            inputs = self.inputs.to_dict()
+
+        outputs: Union[Unset, List[Any]] = UNSET
+        if not isinstance(self.outputs, Unset):
+            outputs = self.outputs
+
         tags: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.tags, Unset):
             tags = self.tags.to_dict()
 
         username = self.username
         slug = self.slug
 
@@ -98,27 +111,32 @@
                 "status": status,
                 "username_resolved": username_resolved,
                 "run_log": run_log,
             }
         )
         if id is not UNSET:
             field_dict["id"] = id
+        if inputs is not UNSET:
+            field_dict["inputs"] = inputs
+        if outputs is not UNSET:
+            field_dict["outputs"] = outputs
         if tags is not UNSET:
             field_dict["tags"] = tags
         if username is not UNSET:
             field_dict["username"] = username
         if slug is not UNSET:
             field_dict["slug"] = slug
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.run_log_data import RunLogData
         from ..models.run_log_out_with_run_config import RunLogOutWithRunConfig
+        from ..models.run_log_out_with_run_inputs import RunLogOutWithRunInputs
         from ..models.run_log_out_with_run_tags import RunLogOutWithRunTags
 
         d = src_dict.copy()
         project_version = d.pop("project_version")
 
         config = RunLogOutWithRunConfig.from_dict(d.pop("config"))
 
@@ -140,14 +158,23 @@
 
         username_resolved = d.pop("username_resolved")
 
         run_log = RunLogData.from_dict(d.pop("run_log"))
 
         id = d.pop("id", UNSET)
 
+        _inputs = d.pop("inputs", UNSET)
+        inputs: Union[Unset, RunLogOutWithRunInputs]
+        if isinstance(_inputs, Unset):
+            inputs = UNSET
+        else:
+            inputs = RunLogOutWithRunInputs.from_dict(_inputs)
+
+        outputs = cast(List[Any], d.pop("outputs", UNSET))
+
         _tags = d.pop("tags", UNSET)
         tags: Union[Unset, RunLogOutWithRunTags]
         if isinstance(_tags, Unset):
             tags = UNSET
         else:
             tags = RunLogOutWithRunTags.from_dict(_tags)
 
@@ -165,14 +192,16 @@
             run_log_schema_version=run_log_schema_version,
             created_at=created_at,
             updated_at=updated_at,
             status=status,
             username_resolved=username_resolved,
             run_log=run_log,
             id=id,
+            inputs=inputs,
+            outputs=outputs,
             tags=tags,
             username=username,
             slug=slug,
         )
 
         run_log_out_with_run.additional_properties = d
         return run_log_out_with_run
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run_config.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run_result_summary.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run_result_summary.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/organization_out.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,65 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.project_in import ProjectIn
-    from ..models.visibility_in import VisibilityIn
+from ..types import UNSET, Unset
 
-
-T = TypeVar("T", bound="TrackingserverApiApiCreateProjectBodyParams")
+T = TypeVar("T", bound="OrganizationOut")
 
 
 @attr.s(auto_attribs=True)
-class TrackingserverApiApiCreateProjectBodyParams:
+class OrganizationOut:
     """
     Attributes:
-        project (ProjectIn):
-        visibility (VisibilityIn):
+        name (str):
+        propel_auth_org_id (str):
+        id (Union[Unset, int]):
     """
 
-    project: "ProjectIn"
-    visibility: "VisibilityIn"
+    name: str
+    propel_auth_org_id: str
+    id: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        project = self.project.to_dict()
-
-        visibility = self.visibility.to_dict()
+        name = self.name
+        propel_auth_org_id = self.propel_auth_org_id
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "project": project,
-                "visibility": visibility,
+                "name": name,
+                "propel_auth_org_id": propel_auth_org_id,
             }
         )
+        if id is not UNSET:
+            field_dict["id"] = id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_in import ProjectIn
-        from ..models.visibility_in import VisibilityIn
-
         d = src_dict.copy()
-        project = ProjectIn.from_dict(d.pop("project"))
+        name = d.pop("name")
+
+        propel_auth_org_id = d.pop("propel_auth_org_id")
 
-        visibility = VisibilityIn.from_dict(d.pop("visibility"))
+        id = d.pop("id", UNSET)
 
-        trackingserver_api_api_create_project_body_params = cls(
-            project=project,
-            visibility=visibility,
+        organization_out = cls(
+            name=name,
+            propel_auth_org_id=propel_auth_org_id,
+            id=id,
         )
 
-        trackingserver_api_api_create_project_body_params.additional_properties = d
-        return trackingserver_api_api_create_project_body_params
+        organization_out.additional_properties = d
+        return organization_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,79 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
 if TYPE_CHECKING:
+    from ..models.documentation_asset_in import DocumentationAssetIn
     from ..models.project_in import ProjectIn
     from ..models.visibility_in import VisibilityIn
 
 
 T = TypeVar("T", bound="TrackingserverApiApiUpdateProjectBodyParams")
 
 
 @attr.s(auto_attribs=True)
 class TrackingserverApiApiUpdateProjectBodyParams:
     """
     Attributes:
         project (ProjectIn):
         visibility (VisibilityIn):
+        documentation (List['DocumentationAssetIn']):
     """
 
     project: "ProjectIn"
     visibility: "VisibilityIn"
+    documentation: List["DocumentationAssetIn"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project = self.project.to_dict()
 
         visibility = self.visibility.to_dict()
 
+        documentation = []
+        for documentation_item_data in self.documentation:
+            documentation_item = documentation_item_data.to_dict()
+
+            documentation.append(documentation_item)
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "project": project,
                 "visibility": visibility,
+                "documentation": documentation,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.documentation_asset_in import DocumentationAssetIn
         from ..models.project_in import ProjectIn
         from ..models.visibility_in import VisibilityIn
 
         d = src_dict.copy()
         project = ProjectIn.from_dict(d.pop("project"))
 
         visibility = VisibilityIn.from_dict(d.pop("visibility"))
 
+        documentation = []
+        _documentation = d.pop("documentation")
+        for documentation_item_data in _documentation:
+            documentation_item = DocumentationAssetIn.from_dict(documentation_item_data)
+
+            documentation.append(documentation_item)
+
         trackingserver_api_api_update_project_body_params = cls(
             project=project,
             visibility=visibility,
+            documentation=documentation,
         )
 
         trackingserver_api_api_update_project_body_params.additional_properties = d
         return trackingserver_api_api_update_project_body_params
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/user_out.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,34 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UserOut")
+T = TypeVar("T", bound="RunLogOutWithRunInputs")
 
 
 @attr.s(auto_attribs=True)
-class UserOut:
-    """
-    Attributes:
-        email (str):
-        id (Union[Unset, int]):
-    """
+class RunLogOutWithRunInputs:
+    """ """
 
-    email: str
-    id: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        email = self.email
-        id = self.id
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "email": email,
-            }
-        )
-        if id is not UNSET:
-            field_dict["id"] = id
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        email = d.pop("email")
-
-        id = d.pop("id", UNSET)
-
-        user_out = cls(
-            email=email,
-            id=id,
-        )
+        run_log_out_with_run_inputs = cls()
 
-        user_out.additional_properties = d
-        return user_out
+        run_log_out_with_run_inputs.additional_properties = d
+        return run_log_out_with_run_inputs
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/visibility_full.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/visibility_full.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/who_am_i_result.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/who_am_i_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/api_client/types.py` & `dagworks-sdk-0.0.3/src/dagworks/api/api_client/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Contains some shared types for properties """
 from http import HTTPStatus
-from typing import BinaryIO, Generic, MutableMapping, Optional, Tuple, TypeVar
+from typing import BinaryIO, Generic, Literal, MutableMapping, Optional, Tuple, TypeVar
 
 import attr
 
 
 class Unset:
-    def __bool__(self) -> bool:
+    def __bool__(self) -> Literal[False]:
         return False
 
 
 UNSET: Unset = Unset()
 
 FileJsonType = Tuple[Optional[str], BinaryIO, Optional[str]]
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/clients.py` & `dagworks-sdk-0.0.3/src/dagworks/api/clients.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import abc
 import dataclasses
 import logging
-from typing import Any, Dict
+from typing import Any, Dict, List
 
 from dagworks.api.api_client import AuthenticatedClient
 from dagworks.api.api_client.api.auth import trackingserver_api_api_phone_home as phone_home
 from dagworks.api.api_client.api.projects import (
     trackingserver_api_api_create_project_version as create_project_version,
 )
 from dagworks.api.api_client.api.projects import (
@@ -41,14 +41,15 @@
     ProjectVersionInGitDag,
     ProjectVersionInGitTags,
     ProjectVersionOut,
     RunLogIn,
     RunLogInConfig,
     RunLogInRunLog,
     RunLogInTags,
+    RunLogInInputs,
 )
 from dagworks.api.projecttypes import GitInfo
 from dagworks.parsing.dagtypes import LogicalDAG
 from dagworks.telemetry.telemetry import global_tracker
 from dagworks.tracking.trackingtypes import DAGRun
 
 logger = logging.getLogger(__name__)
@@ -94,22 +95,30 @@
         :param name: Name of the version to save the project with
         :return: Version ID -- likely commit hash for the project
         """
         pass
 
     @abc.abstractmethod
     def log_dag_run(
-        self, dag_run: DAGRun, project_version_id: int, config: Dict[str, Any], tags: Dict[str, str]
+        self,
+        dag_run: DAGRun,
+        project_version_id: int,
+        config: Dict[str, Any],
+        tags: Dict[str, str],
+        inputs: Dict[str, Any],
+        outputs: List[str],
     ):
         """Logs a DAG run to the DAGWorks API.
 
-        :param config:
         :param project_version_id:
         :param dag_run: DAG run to log
+        :param config: config used to create DAG
         :param tags: Tags to log with the DAG run
+        :param inputs: Inputs used to pass into the DAG
+        :param outputs: Outputs used to query the DAG
         """
         pass
 
 
 class BasicDAGWorksClient(DAGWorksClient):
     """Basic no-op DAGWorks client -- mocks out the above DAGWorks client for testing"""
 
@@ -201,33 +210,43 @@
                 f"it (request write access from the creator), or perhaps you haven't made it yet..."
             )
         logger.debug(f"Project {project} already exists. Using project: {project}")
         return project
 
     @global_tracker.track_calls(params_to_capture_raw=["project_version_id"])
     def log_dag_run(
-        self, dag_run: DAGRun, project_version_id: int, config: Dict[str, Any], tags: Dict[str, str]
+        self,
+        dag_run: DAGRun,
+        project_version_id: int,
+        config: Dict[str, Any],
+        tags: Dict[str, str],
+        inputs: Dict[str, Any],
+        outputs: List[str],
     ):
         run_log_to_save = RunLogInRunLog()
         run_log_to_save.additional_properties = {
             "tasks": [task.to_dict() for task in dag_run.tasks]
         }
         config_to_save = RunLogInConfig()
         config_to_save.additional_properties = config
         run_log_in_tags = RunLogInTags()
         run_log_in_tags.additional_properties = tags
+        inputs_to_save = RunLogInInputs()
+        inputs_to_save.additional_properties = inputs
         json_body = RunLogIn(
             status=dag_run.status.value,
             project_version_id=project_version_id,
             config=config_to_save,
             run_id=dag_run.run_id,
             start_time=dag_run.start_time,
             end_time=dag_run.end_time,
             run_log_schema_version=dag_run.schema_version,
             run_log=run_log_to_save,
             tags=run_log_in_tags,
+            inputs=inputs_to_save,
+            outputs=outputs,
         )
         log_run_log.sync(
             client=self.api_client,
             project_version_id=project_version_id,
             json_body=json_body,
         )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/constants.py` & `dagworks-sdk-0.0.3/src/dagworks/api/constants.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/api/projecttypes.py` & `dagworks-sdk-0.0.3/src/dagworks/api/projecttypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/__init__.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/cli.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 @click.group()
 def cli():
     pass
 
 
 @click.command()
-@click.option("--api-key", required=True, type=str)
-@click.option("--username", required=True, type=str)
-@click.option("--project-id", required=True, type=int)
-@click.option("--template", required=False, type=click.Choice(initialize.TEMPLATES))
-@click.option("--location", type=click.Path(exists=False, dir_okay=True), default=None)
+@click.option("--api-key", "-k", required=True, type=str)
+@click.option("--username", "-u", required=True, type=str)
+@click.option("--project-id", "-p", required=True, type=int)
+@click.option("--template", "-t", required=False, type=click.Choice(initialize.TEMPLATES))
+@click.option("--location", "-l", type=click.Path(exists=False, dir_okay=True), default=None)
 def init(api_key: str, username: str, project_id: int, template: str, location: str):
     if location is None:
         # If location is none we default to, say, ./hello_world
         location = os.path.join(os.getcwd(), template)
     initialize.generate_template(
         username=username,
         api_key=api_key,
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/initialize.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/initialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 try:
     # for python 3.9+
     BASE_TEMPLATES_DIRECTORY = importlib.resources.files("dagworks.cli.templates")
 except AttributeError:
     # for python <3.9
     import pkg_resources
+
     BASE_TEMPLATES_DIRECTORY = pkg_resources.resource_filename("dagworks.cli.templates", "")
 
 logger = loguru.logger
 
 HAMILTON_DIR_LOCATION = "components"
 CONFIG_DIR_LOCATION = "config"
 DATA_DIR_LOCATION = "data"
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/run.py.jinja2` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/run.sh.jinja2` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/common.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/data_loader.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/data_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/template_data.json` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/components/transforms.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/components/transforms.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 You can also play around with a very similar example on tryhamilton.dev.
 """
 
 
 def spend(spend_path: str) -> pd.Series:
     """Function that loads the spend column from a CSV."""
-    return pd.read_csv(spend_path)["spend"]
+    return pd.read_csv(spend_path, index_col=0)["spend"]
 
 
 def signups(signups_path: str) -> pd.Series:
     """Function that loads the signups column from a CSV."""
-    return pd.read_csv(signups_path)["signups"]
+    return pd.read_csv(signups_path, index_col=0)["signups"]
 
 
 def avg_3wk_spend(spend: pd.Series) -> pd.Series:
     """Rolling 3 week average spend."""
     return spend.rolling(3).mean()
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/template_data.json` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/iris_loader.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/iris_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/model_fitting.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/models.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json` & `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/driver.py` & `dagworks-sdk-0.0.3/src/dagworks/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,15 @@
             "final_vars": [("num_vars", safe_len)],
             "overrides": [("num_overrides", safe_len)],
             "inputs": [("num_inputs", safe_len)],
         },
     )
     def raw_execute(
         self,
-        final_vars: List[Union[str, Callable]],
+        final_vars: List[str],
         overrides: Dict[str, Any] = None,
         display_graph: bool = False,
         inputs: Dict[str, Any] = None,
     ) -> Any:
         """Executes the DAG -- we decorate raw_execute, as execute delegates to raw_execute
         and we don't want to run twice. We should change this later, but for now this is OK.
 
@@ -339,8 +339,10 @@
                 raise e
             finally:
                 self.client.log_dag_run(
                     tracking_state.get(),
                     self.project_version.id,
                     config=filter_config_to_json_serializable(self.config),
                     tags=self.run_tags,
+                    inputs=filter_config_to_json_serializable(inputs),
+                    outputs=final_vars,
                 )
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/parsing/__init__.py` & `dagworks-sdk-0.0.3/src/dagworks/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/parsing/dagtypes.py` & `dagworks-sdk-0.0.3/src/dagworks/parsing/dagtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/parsing/parse.py` & `dagworks-sdk-0.0.3/src/dagworks/parsing/parse.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/telemetry/__init__.py` & `dagworks-sdk-0.0.3/src/dagworks/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/telemetry/telemetry.py` & `dagworks-sdk-0.0.3/src/dagworks/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/tracking/__init__.py` & `dagworks-sdk-0.0.3/src/dagworks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/tracking/example_tracking.py` & `dagworks-sdk-0.0.3/src/dagworks/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks/tracking/runs.py` & `dagworks-sdk-0.0.3/src/dagworks/tracking/runs.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from contextlib import contextmanager
 from datetime import datetime, time
 from typing import Any, Callable, Dict, List
 
 import pandas as pd
 from hamilton import base
 from hamilton import node as h_node
+from hamilton.data_quality import base as dq_base
 from packaging.version import Version
 
 from dagworks.tracking.trackingtypes import DAGRun, Status, TaskRun
 
 logger = logging.getLogger(__name__)
 
 
@@ -166,14 +167,32 @@
     :param error:
     :return:
     """
     exc_type, exc_value, exc_tb = sys.exc_info()
     return traceback.format_exception(exc_type, exc_value, exc_tb)
 
 
+def serialize_data_quality_error(e: dq_base.DataValidationError) -> List[str]:
+    """Santizes data quality errors to make them more readable for the platform.
+
+    Note: this is hacky code.
+
+    :param e: Data quality error to inspect
+    :return: list of failures.
+    """
+    validation_failures = e.args[0]
+    sanitized_failures = []
+    for failure in validation_failures:
+        if "pandera_schema_validator" in failure:  # hack to know what type of validator.
+            sanitized_failures.append(failure.split("Usage Tip")[0])  # remove usage tip
+        else:
+            sanitized_failures.append(failure)
+    return sanitized_failures
+
+
 class RunTracker:
     """This class allows you to track results of runs"""
 
     def __init__(self, tracking_state: TrackingState):
         """Tracks runs given run IDs. Note that this needs to be re-initialized
         on each run, we'll want to fix that.
 
@@ -210,14 +229,22 @@
             task_run.status = Status.SUCCESS
             task_run.result_type = type(result)
             task_run.result_summary = process_result(result, node)  # add node
             task_run.end_time = datetime.now()
             self.tracking_state.update_task(node.name, task_run)
             logger.debug(f"Node: {node.name} ran successfully")
             return result
+        except dq_base.DataValidationError as e:
+            task_run.status = Status.FAILURE
+            task_run.end_time = datetime.now()
+            task_run.error = serialize_data_quality_error(e)
+            self.tracking_state.update_status(Status.FAILURE)
+            self.tracking_state.update_task(node.name, task_run)
+            logger.debug(f"Node: {node.name} encountered data quality issue...")
+            raise e
         except Exception as e:
             task_run.status = Status.FAILURE
             task_run.end_time = datetime.now()
             task_run.error = serialize_error()
             self.tracking_state.update_status(Status.FAILURE)
             self.tracking_state.update_task(node.name, task_run)
             logger.debug(f"Node: {node.name} failed to run...")
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks/tracking/trackingtypes.py` & `dagworks-sdk-0.0.3/src/dagworks/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/PKG-INFO` & `dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/SOURCES.txt` & `dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/dagworks/api/api_client/api/auth/__init__.py
 src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
 src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
 src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
 src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
 src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
 src/dagworks/api/api_client/api/projects/__init__.py
+src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
 src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
 src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
 src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
 src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
 src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
 src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
 src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
@@ -37,14 +38,18 @@
 src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
 src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
 src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
 src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
 src/dagworks/api/api_client/models/__init__.py
 src/dagworks/api/api_client/models/api_key_out.py
 src/dagworks/api/api_client/models/dependency.py
+src/dagworks/api/api_client/models/documentation_asset_in.py
+src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
+src/dagworks/api/api_client/models/documentation_asset_out.py
+src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
 src/dagworks/api/api_client/models/hamilton_dag.py
 src/dagworks/api/api_client/models/hamilton_function.py
 src/dagworks/api/api_client/models/hamilton_node.py
 src/dagworks/api/api_client/models/hamilton_node_dependencies.py
 src/dagworks/api/api_client/models/hamilton_node_tags.py
 src/dagworks/api/api_client/models/organization_out.py
 src/dagworks/api/api_client/models/paged_api_key_out.py
@@ -64,21 +69,24 @@
 src/dagworks/api/api_client/models/project_version_out_with_dag.py
 src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
 src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
 src/dagworks/api/api_client/models/python_type.py
 src/dagworks/api/api_client/models/run_log_data.py
 src/dagworks/api/api_client/models/run_log_in.py
 src/dagworks/api/api_client/models/run_log_in_config.py
+src/dagworks/api/api_client/models/run_log_in_inputs.py
 src/dagworks/api/api_client/models/run_log_in_run_log.py
 src/dagworks/api/api_client/models/run_log_in_tags.py
 src/dagworks/api/api_client/models/run_log_out.py
 src/dagworks/api/api_client/models/run_log_out_config.py
+src/dagworks/api/api_client/models/run_log_out_inputs.py
 src/dagworks/api/api_client/models/run_log_out_tags.py
 src/dagworks/api/api_client/models/run_log_out_with_run.py
 src/dagworks/api/api_client/models/run_log_out_with_run_config.py
+src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
 src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
 src/dagworks/api/api_client/models/task_run.py
 src/dagworks/api/api_client/models/task_run_result_summary.py
 src/dagworks/api/api_client/models/task_run_status.py
 src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
 src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
 src/dagworks/api/api_client/models/user_out.py
```

### Comparing `dagworks-sdk-0.0.2/tests/test_driver.py` & `dagworks-sdk-0.0.3/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/tests/test_runs.py` & `dagworks-sdk-0.0.3/tests/test_runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/tests/test_telemetry.py` & `dagworks-sdk-0.0.3/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.2/tests/test_tracking.py` & `dagworks-sdk-0.0.3/tests/test_tracking.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 from datetime import datetime
-from typing import Any, Callable, Dict
+from typing import Any, Callable, Dict, List
 
 import pytest
 from hamilton import base
 
 import tests.resources.basic_dag_with_config
 from dagworks import driver
 from dagworks.api.api_client.models import (
@@ -71,19 +71,27 @@
             name="",
             description="",
             tags=ProjectOutTags(),
             created_at=datetime.now(),
             updated_at=datetime.now(),
             owner="elijah",
             permissions=VisibilityFull([], [], [], []),
+            documentation=[],
+            can_write=True,
         )
 
     @track_calls
     def log_dag_run(
-        self, dag_run: DAGRun, project_version_id: int, config: Dict[str, Any], tags: Dict[str, Any]
+        self,
+        dag_run: DAGRun,
+        project_version_id: int,
+        config: Dict[str, Any],
+        tags: Dict[str, Any],
+        inputs: Dict[str, Any],
+        outputs: List[str],
     ):
         pass
 
 
 def test_tracking_state():
     state = TrackingState("test")
     state.clock_start()
```

