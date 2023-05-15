# Comparing `tmp/cosmotech-api-2.4.0.tar.gz` & `tmp/cosmotech-api-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-api-2.4.0.tar", last modified: Fri Apr 28 10:11:17 2023, max compression
+gzip compressed data, was "cosmotech-api-2.4.1.tar", last modified: Mon May 15 13:16:26 2023, max compression
```

## Comparing `cosmotech-api-2.4.0.tar` & `cosmotech-api-2.4.1.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.129549 cosmotech-api-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 10:11:17.129549 cosmotech-api-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34207 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.105549 cosmotech-api-2.4.0/cosmotech_api/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.109549 cosmotech-api-2.4.0/cosmotech_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24319 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/connector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54204 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    92962 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/organization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   135364 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/scenario_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    83623 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/scenariorun_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    89623 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/solution_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    84630 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/twingraph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46553 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48790 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   110590 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37648 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.109549 cosmotech-api-2.4.0/cosmotech_api/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.117549 cosmotech-api-2.4.0/cosmotech_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/graph_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    22521 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13620 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/source_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/translated_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_import_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/user_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/user_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/validator_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    82066 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/cosmotech_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.117549 cosmotech-api-2.4.0/cosmotech_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/cosmotech_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/cosmotech_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.105549 cosmotech-api-2.4.0/cosmotech_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 10:11:17.129549 cosmotech-api-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.129549 cosmotech-api-2.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_connector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_graph_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_security.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenariorun_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_solution_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_source_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_translated_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_import_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twingraph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_user_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_user_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_validator_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_web_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.514235 cosmotech-api-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 13:16:26.514235 cosmotech-api-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34808 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.474233 cosmotech-api-2.4.1/cosmotech_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.478233 cosmotech-api-2.4.1/cosmotech_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54209 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92967 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135369 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/scenario_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83628 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/scenariorun_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89628 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/solution_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85025 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/twingraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46553 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48795 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110595 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37653 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.478233 cosmotech-api-2.4.1/cosmotech_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.490234 cosmotech-api-2.4.1/cosmotech_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/translated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_import_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/user_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/user_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82071 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.490234 cosmotech-api-2.4.1/cosmotech_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.474233 cosmotech-api-2.4.1/cosmotech_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 13:16:26.514235 cosmotech-api-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.514235 cosmotech-api-2.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenariorun_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_solution_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_translated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_import_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twingraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_user_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_user_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_web_app.py
```

### Comparing `cosmotech-api-2.4.0/LICENSE` & `cosmotech-api-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.0/README.md` & `cosmotech-api-2.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # cosmotech-api
 Cosmo Tech Platform API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.4.0-dev
+- API version: 2.4.2-SNAPSHOT
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://github.com/Cosmo-Tech/cosmotech-api](https://github.com/Cosmo-Tech/cosmotech-api)
 
 ## Requirements.
 
 Python >=3.6
@@ -174,29 +174,29 @@
 *SolutionApi* | [**import_solution**](docs/SolutionApi.md#import_solution) | **POST** /organizations/{organization_id}/solutions/import | Import a solution
 *SolutionApi* | [**remove_all_run_templates**](docs/SolutionApi.md#remove_all_run_templates) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/runTemplates | Remove all Run Templates from the Solution specified
 *SolutionApi* | [**remove_all_solution_parameter_groups**](docs/SolutionApi.md#remove_all_solution_parameter_groups) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/parameterGroups | Remove all Parameter Groups from the Solution specified
 *SolutionApi* | [**remove_all_solution_parameters**](docs/SolutionApi.md#remove_all_solution_parameters) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/parameters | Remove all Parameters from the Solution specified
 *SolutionApi* | [**update_solution**](docs/SolutionApi.md#update_solution) | **PATCH** /organizations/{organization_id}/solutions/{solution_id} | Update a solution
 *SolutionApi* | [**update_solution_run_template**](docs/SolutionApi.md#update_solution_run_template) | **PATCH** /organizations/{organization_id}/solutions/{solution_id}/runTemplates/{run_template_id} | Update the specified Solution Run Template
 *SolutionApi* | [**upload_run_template_handler**](docs/SolutionApi.md#upload_run_template_handler) | **POST** /organizations/{organization_id}/solutions/{solution_id}/runtemplates/{run_template_id}/handlers/{handler_id}/upload | Upload a Run Template step handler zip file
-*TwingraphApi* | [**batch_query**](docs/TwingraphApi.md#batch_query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/batch-query | 
-*TwingraphApi* | [**batch_upload_update**](docs/TwingraphApi.md#batch_upload_update) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/batch | 
-*TwingraphApi* | [**create_entities**](docs/TwingraphApi.md#create_entities) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | 
-*TwingraphApi* | [**create_graph**](docs/TwingraphApi.md#create_graph) | **POST** /organizations/{organization_id}/twingraph/{graph_id} | 
-*TwingraphApi* | [**delete**](docs/TwingraphApi.md#delete) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id} | 
-*TwingraphApi* | [**delete_entities**](docs/TwingraphApi.md#delete_entities) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | 
-*TwingraphApi* | [**download_graph**](docs/TwingraphApi.md#download_graph) | **GET** /organizations/{organization_id}/twingraph/bulk-query/download/{hash} | 
-*TwingraphApi* | [**find_all_twingraphs**](docs/TwingraphApi.md#find_all_twingraphs) | **GET** /organizations/{organization_id}/twingraphs | 
-*TwingraphApi* | [**get_entities**](docs/TwingraphApi.md#get_entities) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | 
-*TwingraphApi* | [**get_graph_meta_data**](docs/TwingraphApi.md#get_graph_meta_data) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/metadata | 
-*TwingraphApi* | [**import_graph**](docs/TwingraphApi.md#import_graph) | **POST** /organizations/{organization_id}/twingraph/import | 
-*TwingraphApi* | [**job_status**](docs/TwingraphApi.md#job_status) | **GET** /organizations/{organization_id}/job/{job_id}/status | 
-*TwingraphApi* | [**query**](docs/TwingraphApi.md#query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/query | 
-*TwingraphApi* | [**update_entities**](docs/TwingraphApi.md#update_entities) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | 
-*TwingraphApi* | [**update_graph_meta_data**](docs/TwingraphApi.md#update_graph_meta_data) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/metadata | 
+*TwingraphApi* | [**batch_query**](docs/TwingraphApi.md#batch_query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/batch-query | Run a query on a graph instance and return the result as a zip file in async mode
+*TwingraphApi* | [**batch_upload_update**](docs/TwingraphApi.md#batch_upload_update) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/batch | Async batch update by loading a CSV file on a graph instance 
+*TwingraphApi* | [**create_entities**](docs/TwingraphApi.md#create_entities) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | Create new entities in a graph instance
+*TwingraphApi* | [**create_graph**](docs/TwingraphApi.md#create_graph) | **POST** /organizations/{organization_id}/twingraph/{graph_id} | Create a new graph
+*TwingraphApi* | [**delete**](docs/TwingraphApi.md#delete) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id} | Launch a mass delete job
+*TwingraphApi* | [**delete_entities**](docs/TwingraphApi.md#delete_entities) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | Delete entities in a graph instance
+*TwingraphApi* | [**download_graph**](docs/TwingraphApi.md#download_graph) | **GET** /organizations/{organization_id}/twingraph/bulk-query/download/{hash} | Download a graph compressed in a zip file
+*TwingraphApi* | [**find_all_twingraphs**](docs/TwingraphApi.md#find_all_twingraphs) | **GET** /organizations/{organization_id}/twingraphs | Return the list of all graphs stored in the organization
+*TwingraphApi* | [**get_entities**](docs/TwingraphApi.md#get_entities) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | Get entities in a graph instance
+*TwingraphApi* | [**get_graph_meta_data**](docs/TwingraphApi.md#get_graph_meta_data) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/metadata | Return the metaData of the specified graph
+*TwingraphApi* | [**import_graph**](docs/TwingraphApi.md#import_graph) | **POST** /organizations/{organization_id}/twingraph/import | Import a new version of a twin graph
+*TwingraphApi* | [**job_status**](docs/TwingraphApi.md#job_status) | **GET** /organizations/{organization_id}/job/{job_id}/status | Get the status of a job
+*TwingraphApi* | [**query**](docs/TwingraphApi.md#query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/query | Run a query on a graph instance
+*TwingraphApi* | [**update_entities**](docs/TwingraphApi.md#update_entities) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | Update entities in a graph instance
+*TwingraphApi* | [**update_graph_meta_data**](docs/TwingraphApi.md#update_graph_meta_data) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/metadata | Update the metaData of the specified graph
 *ValidatorApi* | [**create_validator**](docs/ValidatorApi.md#create_validator) | **POST** /organizations/{organization_id}/datasets/validators | Register a new validator
 *ValidatorApi* | [**create_validator_run**](docs/ValidatorApi.md#create_validator_run) | **POST** /organizations/{organization_id}/datasets/validators/{validator_id}/history | Register a new validator run
 *ValidatorApi* | [**delete_validator**](docs/ValidatorApi.md#delete_validator) | **DELETE** /organizations/{organization_id}/datasets/validators/{validator_id} | Delete a validator
 *ValidatorApi* | [**delete_validator_run**](docs/ValidatorApi.md#delete_validator_run) | **DELETE** /organizations/{organization_id}/datasets/validators/{validator_id}/history/{validatorrun_id} | Delete a validator run
 *ValidatorApi* | [**find_all_validator_runs**](docs/ValidatorApi.md#find_all_validator_runs) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id}/history | List all Validator Runs
 *ValidatorApi* | [**find_all_validators**](docs/ValidatorApi.md#find_all_validators) | **GET** /organizations/{organization_id}/datasets/validators | List all Validators
 *ValidatorApi* | [**find_validator_by_id**](docs/ValidatorApi.md#find_validator_by_id) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id} | Get the details of a validator
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/__init__.py` & `cosmotech-api-2.4.1/cosmotech_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/connector_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/connector_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/dataset_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/dataset_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/organization_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/organization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/scenario_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/scenario_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/scenariorun_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/scenariorun_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/solution_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/solution_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/twingraph_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/twingraph_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -1009,15 +1009,15 @@
     def batch_query(
         self,
         organization_id,
         graph_id,
         twin_graph_query,
         **kwargs
     ):
-        """batch_query  # noqa: E501
+        """Run a query on a graph instance and return the result as a zip file in async mode  # noqa: E501
 
         Run a query on a graph instance and return the result as a zip file in async mode  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.batch_query(organization_id, graph_id, twin_graph_query, async_req=True)
         >>> result = thread.get()
@@ -1096,15 +1096,15 @@
         self,
         organization_id,
         graph_id,
         twin_graph_query,
         body,
         **kwargs
     ):
-        """batch_upload_update  # noqa: E501
+        """Async batch update by loading a CSV file on a graph instance   # noqa: E501
 
         Async batch update by loading a CSV file on a graph instance   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.batch_upload_update(organization_id, graph_id, twin_graph_query, body, async_req=True)
         >>> result = thread.get()
@@ -1186,15 +1186,15 @@
         self,
         organization_id,
         graph_id,
         model_type,
         graph_properties,
         **kwargs
     ):
-        """create_entities  # noqa: E501
+        """Create new entities in a graph instance  # noqa: E501
 
         create new entities in a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_entities(organization_id, graph_id, model_type, graph_properties, async_req=True)
         >>> result = thread.get()
@@ -1274,15 +1274,15 @@
 
     def create_graph(
         self,
         organization_id,
         graph_id,
         **kwargs
     ):
-        """create_graph  # noqa: E501
+        """Create a new graph  # noqa: E501
 
         Create a new graph  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_graph(organization_id, graph_id, async_req=True)
         >>> result = thread.get()
@@ -1357,15 +1357,15 @@
 
     def delete(
         self,
         organization_id,
         graph_id,
         **kwargs
     ):
-        """delete  # noqa: E501
+        """Launch a mass delete job  # noqa: E501
 
         Launch a mass delete job  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete(organization_id, graph_id, async_req=True)
         >>> result = thread.get()
@@ -1441,15 +1441,15 @@
         self,
         organization_id,
         graph_id,
         model_type,
         ids,
         **kwargs
     ):
-        """delete_entities  # noqa: E501
+        """Delete entities in a graph instance  # noqa: E501
 
         delete entities in a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_entities(organization_id, graph_id, model_type, ids, async_req=True)
         >>> result = thread.get()
@@ -1529,15 +1529,15 @@
 
     def download_graph(
         self,
         organization_id,
         hash,
         **kwargs
     ):
-        """download_graph  # noqa: E501
+        """Download a graph compressed in a zip file  # noqa: E501
 
         Download a graph compressed in a zip file  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.download_graph(organization_id, hash, async_req=True)
         >>> result = thread.get()
@@ -1610,15 +1610,15 @@
         return self.download_graph_endpoint.call_with_http_info(**kwargs)
 
     def find_all_twingraphs(
         self,
         organization_id,
         **kwargs
     ):
-        """find_all_twingraphs  # noqa: E501
+        """Return the list of all graphs stored in the organization  # noqa: E501
 
         Return the list of all graphs stored in the organization  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.find_all_twingraphs(organization_id, async_req=True)
         >>> result = thread.get()
@@ -1691,15 +1691,15 @@
         self,
         organization_id,
         graph_id,
         model_type,
         ids,
         **kwargs
     ):
-        """get_entities  # noqa: E501
+        """Get entities in a graph instance  # noqa: E501
 
         get entities in a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_entities(organization_id, graph_id, model_type, ids, async_req=True)
         >>> result = thread.get()
@@ -1779,15 +1779,15 @@
 
     def get_graph_meta_data(
         self,
         organization_id,
         graph_id,
         **kwargs
     ):
-        """get_graph_meta_data  # noqa: E501
+        """Return the metaData of the specified graph  # noqa: E501
 
         Return the metaData of the specified graph  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_graph_meta_data(organization_id, graph_id, async_req=True)
         >>> result = thread.get()
@@ -1861,15 +1861,15 @@
 
     def import_graph(
         self,
         organization_id,
         twin_graph_import,
         **kwargs
     ):
-        """import_graph  # noqa: E501
+        """Import a new version of a twin graph  # noqa: E501
 
         Import a new version of a twin graph  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.import_graph(organization_id, twin_graph_import, async_req=True)
         >>> result = thread.get()
@@ -1943,15 +1943,15 @@
 
     def job_status(
         self,
         organization_id,
         job_id,
         **kwargs
     ):
-        """job_status  # noqa: E501
+        """Get the status of a job  # noqa: E501
 
         Get the status of a job  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.job_status(organization_id, job_id, async_req=True)
         >>> result = thread.get()
@@ -2026,15 +2026,15 @@
     def query(
         self,
         organization_id,
         graph_id,
         twin_graph_query,
         **kwargs
     ):
-        """query  # noqa: E501
+        """Run a query on a graph instance  # noqa: E501
 
         Run a query on a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.query(organization_id, graph_id, twin_graph_query, async_req=True)
         >>> result = thread.get()
@@ -2113,15 +2113,15 @@
         self,
         organization_id,
         graph_id,
         model_type,
         graph_properties,
         **kwargs
     ):
-        """update_entities  # noqa: E501
+        """Update entities in a graph instance  # noqa: E501
 
         update entities in a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_entities(organization_id, graph_id, model_type, graph_properties, async_req=True)
         >>> result = thread.get()
@@ -2202,15 +2202,15 @@
     def update_graph_meta_data(
         self,
         organization_id,
         graph_id,
         request_body,
         **kwargs
     ):
-        """update_graph_meta_data  # noqa: E501
+        """Update the metaData of the specified graph  # noqa: E501
 
         Update the metaData of the specified graph  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_graph_meta_data(organization_id, graph_id, request_body, async_req=True)
         >>> result = thread.get()
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/user_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.7
+    The version of the OpenAPI document: 2.3.8
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/validator_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/validator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api/workspace_api.py` & `cosmotech-api-2.4.1/cosmotech_api/api/workspace_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/api_client.py` & `cosmotech-api-2.4.1/cosmotech_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/apis/__init__.py` & `cosmotech-api-2.4.1/cosmotech_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.0/cosmotech_api/configuration.py` & `cosmotech-api-2.4.1/cosmotech_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -384,15 +384,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.4.0-dev\n"\
+               "Version of the API: 2.4.2-SNAPSHOT\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/exceptions.py` & `cosmotech-api-2.4.1/cosmotech_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/component_role_permissions.py` & `cosmotech-api-2.4.1/cosmotech_api/model/component_role_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/connector.py` & `cosmotech-api-2.4.1/cosmotech_api/model/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/connector_parameter.py` & `cosmotech-api-2.4.1/cosmotech_api/model/connector_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/connector_parameter_group.py` & `cosmotech-api-2.4.1/cosmotech_api/model/connector_parameter_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/container_resource_size_info.py` & `cosmotech-api-2.4.1/cosmotech_api/model/container_resource_size_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/container_resource_sizing.py` & `cosmotech-api-2.4.1/cosmotech_api/model/container_resource_sizing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/dataset.py` & `cosmotech-api-2.4.1/cosmotech_api/model/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -92,15 +92,15 @@
         return {
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'owner_id': (str,),  # noqa: E501
             'organization_id': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
-            'connector': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'connector': (DatasetConnector,),  # noqa: E501
             'fragments_ids': ([str],),  # noqa: E501
             'validator_id': (str,),  # noqa: E501
             'compatibility': ([DatasetCompatibility],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -166,15 +166,15 @@
                                 _visited_composed_classes = (Animal,)
             id (str): the Dataset unique identifier. [optional]  # noqa: E501
             name (str): the Dataset name. [optional]  # noqa: E501
             description (str): the Dataset description. [optional]  # noqa: E501
             owner_id (str): the User id which own this Dataset. [optional]  # noqa: E501
             organization_id (str): the Organization Id related to this Dataset. [optional]  # noqa: E501
             tags ([str]): the list of tags. [optional]  # noqa: E501
-            connector (bool, date, datetime, dict, float, int, list, str, none_type): the Connector setup bound to a Dataset. [optional]  # noqa: E501
+            connector (DatasetConnector): [optional]  # noqa: E501
             fragments_ids ([str]): the list of other Datasets ids to compose as fragments. [optional]  # noqa: E501
             validator_id (str): the validator id. [optional]  # noqa: E501
             compatibility ([DatasetCompatibility]): the list of compatible Solutions versions. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -257,15 +257,15 @@
                                 _visited_composed_classes = (Animal,)
             id (str): the Dataset unique identifier. [optional]  # noqa: E501
             name (str): the Dataset name. [optional]  # noqa: E501
             description (str): the Dataset description. [optional]  # noqa: E501
             owner_id (str): the User id which own this Dataset. [optional]  # noqa: E501
             organization_id (str): the Organization Id related to this Dataset. [optional]  # noqa: E501
             tags ([str]): the list of tags. [optional]  # noqa: E501
-            connector (bool, date, datetime, dict, float, int, list, str, none_type): the Connector setup bound to a Dataset. [optional]  # noqa: E501
+            connector (DatasetConnector): [optional]  # noqa: E501
             fragments_ids ([str]): the list of other Datasets ids to compose as fragments. [optional]  # noqa: E501
             validator_id (str): the validator id. [optional]  # noqa: E501
             compatibility ([DatasetCompatibility]): the list of compatible Solutions versions. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/dataset_compatibility.py` & `cosmotech-api-2.4.1/cosmotech_api/model/dataset_compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/dataset_connector.py` & `cosmotech-api-2.4.1/cosmotech_api/model/dataset_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/dataset_copy_parameters.py` & `cosmotech-api-2.4.1/cosmotech_api/model/dataset_copy_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/dataset_search.py` & `cosmotech-api-2.4.1/cosmotech_api/model/dataset_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/delete_historical_data.py` & `cosmotech-api-2.4.1/cosmotech_api/model/delete_historical_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/graph_properties.py` & `cosmotech-api-2.4.1/cosmotech_api/model/graph_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/organization.py` & `cosmotech-api-2.4.1/cosmotech_api/model/organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/organization_access_control.py` & `cosmotech-api-2.4.1/cosmotech_api/model/organization_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/organization_role.py` & `cosmotech-api-2.4.1/cosmotech_api/model/organization_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/organization_security.py` & `cosmotech-api-2.4.1/cosmotech_api/model/organization_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/organization_service.py` & `cosmotech-api-2.4.1/cosmotech_api/model/organization_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/organization_services.py` & `cosmotech-api-2.4.1/cosmotech_api/model/organization_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/organization_user.py` & `cosmotech-api-2.4.1/cosmotech_api/model/organization_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/resource_size_info.py` & `cosmotech-api-2.4.1/cosmotech_api/model/resource_size_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/run_template.py` & `cosmotech-api-2.4.1/cosmotech_api/model/run_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/run_template_handler_id.py` & `cosmotech-api-2.4.1/cosmotech_api/model/run_template_handler_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter.py` & `cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter_group.py` & `cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter_value.py` & `cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/run_template_resource_sizing.py` & `cosmotech-api-2.4.1/cosmotech_api/model/run_template_resource_sizing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/run_template_step_source.py` & `cosmotech-api-2.4.1/cosmotech_api/model/run_template_step_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_access_control.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_changed_parameter_value.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_changed_parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_comparison_result.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_comparison_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_data_download_info.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_data_download_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_data_download_job.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_data_download_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_job_state.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_job_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_last_run.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_last_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_resource_sizing.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_resource_sizing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_role.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container_artifact.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container_logs.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_logs.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_search.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_start_containers.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_start_containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_state.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_status.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_status_node.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_status_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_template_parameter_value.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_template_parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_security.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_user.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/scenario_validation_status.py` & `cosmotech-api-2.4.1/cosmotech_api/model/scenario_validation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/solution.py` & `cosmotech-api-2.4.1/cosmotech_api/model/solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/source_info.py` & `cosmotech-api-2.4.1/cosmotech_api/model/source_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/translated_labels.py` & `cosmotech-api-2.4.1/cosmotech_api/model/translated_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_batch_result.py` & `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_batch_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_hash.py` & `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_import.py` & `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_import_info.py` & `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_import_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_query.py` & `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/user.py` & `cosmotech-api-2.4.1/cosmotech_api/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.7
+    The version of the OpenAPI document: 2.3.8
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/user_organization.py` & `cosmotech-api-2.4.1/cosmotech_api/model/user_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.7
+    The version of the OpenAPI document: 2.3.8
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/user_workspace.py` & `cosmotech-api-2.4.1/cosmotech_api/model/user_workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.7
+    The version of the OpenAPI document: 2.3.8
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/validator.py` & `cosmotech-api-2.4.1/cosmotech_api/model/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/validator_run.py` & `cosmotech-api-2.4.1/cosmotech_api/model/validator_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace_access_control.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace_file.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace_role.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace_secret.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace_security.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace_solution.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace_solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace_user.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model/workspace_web_app.py` & `cosmotech-api-2.4.1/cosmotech_api/model/workspace_web_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/model_utils.py` & `cosmotech-api-2.4.1/cosmotech_api/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api/models/__init__.py` & `cosmotech-api-2.4.1/cosmotech_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.0/cosmotech_api/rest.py` & `cosmotech-api-2.4.1/cosmotech_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `cosmotech-api-2.4.0/cosmotech_api.egg-info/SOURCES.txt` & `cosmotech-api-2.4.1/cosmotech_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.0/setup.py` & `cosmotech-api-2.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "cosmotech-api"
-VERSION = "2.4.0"
+VERSION = "2.4.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `cosmotech-api-2.4.0/test/test_component_role_permissions.py` & `cosmotech-api-2.4.1/test/test_component_role_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_connector.py` & `cosmotech-api-2.4.1/test/test_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_connector_api.py` & `cosmotech-api-2.4.1/test/test_connector_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_connector_parameter.py` & `cosmotech-api-2.4.1/test/test_connector_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_connector_parameter_group.py` & `cosmotech-api-2.4.1/test/test_connector_parameter_group.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_container_resource_size_info.py` & `cosmotech-api-2.4.1/test/test_container_resource_size_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_container_resource_sizing.py` & `cosmotech-api-2.4.1/test/test_container_resource_sizing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_dataset.py` & `cosmotech-api-2.4.1/test/test_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_dataset_api.py` & `cosmotech-api-2.4.1/test/test_dataset_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_dataset_compatibility.py` & `cosmotech-api-2.4.1/test/test_dataset_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_dataset_connector.py` & `cosmotech-api-2.4.1/test/test_dataset_connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_dataset_copy_parameters.py` & `cosmotech-api-2.4.1/test/test_dataset_copy_parameters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_dataset_search.py` & `cosmotech-api-2.4.1/test/test_dataset_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_delete_historical_data.py` & `cosmotech-api-2.4.1/test/test_delete_historical_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_graph_properties.py` & `cosmotech-api-2.4.1/test/test_graph_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_organization.py` & `cosmotech-api-2.4.1/test/test_organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_organization_access_control.py` & `cosmotech-api-2.4.1/test/test_organization_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_organization_api.py` & `cosmotech-api-2.4.1/test/test_organization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_organization_role.py` & `cosmotech-api-2.4.1/test/test_organization_role.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_organization_security.py` & `cosmotech-api-2.4.1/test/test_organization_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_organization_service.py` & `cosmotech-api-2.4.1/test/test_organization_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_organization_services.py` & `cosmotech-api-2.4.1/test/test_organization_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_organization_user.py` & `cosmotech-api-2.4.1/test/test_organization_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.0/test/test_resource_size_info.py` & `cosmotech-api-2.4.1/test/test_scenario_resource_sizing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
 from cosmotech_api.model.resource_size_info import ResourceSizeInfo
+globals()['ResourceSizeInfo'] = ResourceSizeInfo
+from cosmotech_api.model.scenario_resource_sizing import ScenarioResourceSizing
 
 
-class TestResourceSizeInfo(unittest.TestCase):
-    """ResourceSizeInfo unit test stubs"""
+class TestScenarioResourceSizing(unittest.TestCase):
+    """ScenarioResourceSizing unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testResourceSizeInfo(self):
-        """Test ResourceSizeInfo"""
+    def testScenarioResourceSizing(self):
+        """Test ScenarioResourceSizing"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ResourceSizeInfo()  # noqa: E501
+        # model = ScenarioResourceSizing()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_run_template.py` & `cosmotech-api-2.4.1/test/test_run_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_run_template_handler_id.py` & `cosmotech-api-2.4.1/test/test_run_template_handler_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_run_template_parameter.py` & `cosmotech-api-2.4.1/test/test_run_template_parameter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_run_template_parameter_group.py` & `cosmotech-api-2.4.1/test/test_run_template_parameter_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_run_template_parameter_value.py` & `cosmotech-api-2.4.1/test/test_run_template_parameter_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_run_template_resource_sizing.py` & `cosmotech-api-2.4.1/test/test_run_template_resource_sizing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_run_template_step_source.py` & `cosmotech-api-2.4.1/test/test_run_template_step_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario.py` & `cosmotech-api-2.4.1/test/test_scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_access_control.py` & `cosmotech-api-2.4.1/test/test_scenario_security.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
 from cosmotech_api.model.scenario_access_control import ScenarioAccessControl
+globals()['ScenarioAccessControl'] = ScenarioAccessControl
+from cosmotech_api.model.scenario_security import ScenarioSecurity
 
 
-class TestScenarioAccessControl(unittest.TestCase):
-    """ScenarioAccessControl unit test stubs"""
+class TestScenarioSecurity(unittest.TestCase):
+    """ScenarioSecurity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioAccessControl(self):
-        """Test ScenarioAccessControl"""
+    def testScenarioSecurity(self):
+        """Test ScenarioSecurity"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioAccessControl()  # noqa: E501
+        # model = ScenarioSecurity()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_api.py` & `cosmotech-api-2.4.1/test/test_scenario_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_changed_parameter_value.py` & `cosmotech-api-2.4.1/test/test_scenario_changed_parameter_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_comparison_result.py` & `cosmotech-api-2.4.1/test/test_scenario_comparison_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_data_download_info.py` & `cosmotech-api-2.4.1/test/test_scenario_data_download_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_data_download_job.py` & `cosmotech-api-2.4.1/test/test_scenario_data_download_job.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_job_state.py` & `cosmotech-api-2.4.1/test/test_scenario_job_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_last_run.py` & `cosmotech-api-2.4.1/test/test_source_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_last_run import ScenarioLastRun
+from cosmotech_api.model.source_info import SourceInfo
 
 
-class TestScenarioLastRun(unittest.TestCase):
-    """ScenarioLastRun unit test stubs"""
+class TestSourceInfo(unittest.TestCase):
+    """SourceInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioLastRun(self):
-        """Test ScenarioLastRun"""
+    def testSourceInfo(self):
+        """Test SourceInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioLastRun()  # noqa: E501
+        # model = SourceInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_resource_sizing.py` & `cosmotech-api-2.4.1/test/test_resource_size_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
 from cosmotech_api.model.resource_size_info import ResourceSizeInfo
-globals()['ResourceSizeInfo'] = ResourceSizeInfo
-from cosmotech_api.model.scenario_resource_sizing import ScenarioResourceSizing
 
 
-class TestScenarioResourceSizing(unittest.TestCase):
-    """ScenarioResourceSizing unit test stubs"""
+class TestResourceSizeInfo(unittest.TestCase):
+    """ResourceSizeInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioResourceSizing(self):
-        """Test ScenarioResourceSizing"""
+    def testResourceSizeInfo(self):
+        """Test ResourceSizeInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioResourceSizing()  # noqa: E501
+        # model = ResourceSizeInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_role.py` & `cosmotech-api-2.4.1/test/test_scenario_role.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run.py` & `cosmotech-api-2.4.1/test/test_scenario_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_container.py` & `cosmotech-api-2.4.1/test/test_scenario_run_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_container_artifact.py` & `cosmotech-api-2.4.1/test/test_scenario_run_container_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_container_logs.py` & `cosmotech-api-2.4.1/test/test_scenario_run_container_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_logs.py` & `cosmotech-api-2.4.1/test/test_scenario_run_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_search.py` & `cosmotech-api-2.4.1/test/test_scenario_run_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_start_containers.py` & `cosmotech-api-2.4.1/test/test_scenario_run_start_containers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_state.py` & `cosmotech-api-2.4.1/test/test_scenario_run_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_status.py` & `cosmotech-api-2.4.1/test/test_scenario_run_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_status_node.py` & `cosmotech-api-2.4.1/test/test_scenario_run_status_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_run_template_parameter_value.py` & `cosmotech-api-2.4.1/test/test_scenario_run_template_parameter_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_security.py` & `cosmotech-api-2.4.1/test/test_scenario_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
-    Cosmo Tech Platform API
+    Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_access_control import ScenarioAccessControl
-globals()['ScenarioAccessControl'] = ScenarioAccessControl
-from cosmotech_api.model.scenario_security import ScenarioSecurity
+from cosmotech_api.model.scenario_user import ScenarioUser
 
 
-class TestScenarioSecurity(unittest.TestCase):
-    """ScenarioSecurity unit test stubs"""
+class TestScenarioUser(unittest.TestCase):
+    """ScenarioUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioSecurity(self):
-        """Test ScenarioSecurity"""
+    def testScenarioUser(self):
+        """Test ScenarioUser"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioSecurity()  # noqa: E501
+        # model = ScenarioUser()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_user.py` & `cosmotech-api-2.4.1/test/test_twin_graph_import.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.4-SNAPSHOT
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_user import ScenarioUser
+from cosmotech_api.model.source_info import SourceInfo
+globals()['SourceInfo'] = SourceInfo
+from cosmotech_api.model.twin_graph_import import TwinGraphImport
 
 
-class TestScenarioUser(unittest.TestCase):
-    """ScenarioUser unit test stubs"""
+class TestTwinGraphImport(unittest.TestCase):
+    """TwinGraphImport unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioUser(self):
-        """Test ScenarioUser"""
+    def testTwinGraphImport(self):
+        """Test TwinGraphImport"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioUser()  # noqa: E501
+        # model = TwinGraphImport()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_scenario_validation_status.py` & `cosmotech-api-2.4.1/test/test_scenario_validation_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_scenariorun_api.py` & `cosmotech-api-2.4.1/test/test_scenariorun_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_solution.py` & `cosmotech-api-2.4.1/test/test_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_solution_api.py` & `cosmotech-api-2.4.1/test/test_solution_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_source_info.py` & `cosmotech-api-2.4.1/test/test_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.source_info import SourceInfo
+from cosmotech_api.model.validator import Validator
 
 
-class TestSourceInfo(unittest.TestCase):
-    """SourceInfo unit test stubs"""
+class TestValidator(unittest.TestCase):
+    """Validator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSourceInfo(self):
-        """Test SourceInfo"""
+    def testValidator(self):
+        """Test Validator"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SourceInfo()  # noqa: E501
+        # model = Validator()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_translated_labels.py` & `cosmotech-api-2.4.1/test/test_translated_labels.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_twin_graph_batch_result.py` & `cosmotech-api-2.4.1/test/test_twin_graph_hash.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.twin_graph_batch_result import TwinGraphBatchResult
+from cosmotech_api.model.twin_graph_hash import TwinGraphHash
 
 
-class TestTwinGraphBatchResult(unittest.TestCase):
-    """TwinGraphBatchResult unit test stubs"""
+class TestTwinGraphHash(unittest.TestCase):
+    """TwinGraphHash unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphBatchResult(self):
-        """Test TwinGraphBatchResult"""
+    def testTwinGraphHash(self):
+        """Test TwinGraphHash"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphBatchResult()  # noqa: E501
+        # model = TwinGraphHash()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_twin_graph_hash.py` & `cosmotech-api-2.4.1/test/test_twin_graph_import_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.twin_graph_hash import TwinGraphHash
+from cosmotech_api.model.twin_graph_import_info import TwinGraphImportInfo
 
 
-class TestTwinGraphHash(unittest.TestCase):
-    """TwinGraphHash unit test stubs"""
+class TestTwinGraphImportInfo(unittest.TestCase):
+    """TwinGraphImportInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphHash(self):
-        """Test TwinGraphHash"""
+    def testTwinGraphImportInfo(self):
+        """Test TwinGraphImportInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphHash()  # noqa: E501
+        # model = TwinGraphImportInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_twin_graph_import.py` & `cosmotech-api-2.4.1/test/test_user.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.3.8
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.source_info import SourceInfo
-globals()['SourceInfo'] = SourceInfo
-from cosmotech_api.model.twin_graph_import import TwinGraphImport
+from cosmotech_api.model.user_organization import UserOrganization
+globals()['UserOrganization'] = UserOrganization
+from cosmotech_api.model.user import User
 
 
-class TestTwinGraphImport(unittest.TestCase):
-    """TwinGraphImport unit test stubs"""
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphImport(self):
-        """Test TwinGraphImport"""
+    def testUser(self):
+        """Test User"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphImport()  # noqa: E501
+        # model = User()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_twin_graph_import_info.py` & `cosmotech-api-2.4.1/test/test_twin_graph_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.twin_graph_import_info import TwinGraphImportInfo
+from cosmotech_api.model.twin_graph_query import TwinGraphQuery
 
 
-class TestTwinGraphImportInfo(unittest.TestCase):
-    """TwinGraphImportInfo unit test stubs"""
+class TestTwinGraphQuery(unittest.TestCase):
+    """TwinGraphQuery unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphImportInfo(self):
-        """Test TwinGraphImportInfo"""
+    def testTwinGraphQuery(self):
+        """Test TwinGraphQuery"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphImportInfo()  # noqa: E501
+        # model = TwinGraphQuery()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_twin_graph_query.py` & `cosmotech-api-2.4.1/test/test_workspace_secret.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.twin_graph_query import TwinGraphQuery
+from cosmotech_api.model.workspace_secret import WorkspaceSecret
 
 
-class TestTwinGraphQuery(unittest.TestCase):
-    """TwinGraphQuery unit test stubs"""
+class TestWorkspaceSecret(unittest.TestCase):
+    """WorkspaceSecret unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphQuery(self):
-        """Test TwinGraphQuery"""
+    def testWorkspaceSecret(self):
+        """Test WorkspaceSecret"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphQuery()  # noqa: E501
+        # model = WorkspaceSecret()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_user.py` & `cosmotech-api-2.4.1/test/test_user_workspace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.7
+    The version of the OpenAPI document: 2.3.8
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.user_organization import UserOrganization
-globals()['UserOrganization'] = UserOrganization
-from cosmotech_api.model.user import User
+from cosmotech_api.model.user_workspace import UserWorkspace
 
 
-class TestUser(unittest.TestCase):
-    """User unit test stubs"""
+class TestUserWorkspace(unittest.TestCase):
+    """UserWorkspace unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUser(self):
-        """Test User"""
+    def testUserWorkspace(self):
+        """Test UserWorkspace"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = User()  # noqa: E501
+        # model = UserWorkspace()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_user_api.py` & `cosmotech-api-2.4.1/test/test_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.7
+    The version of the OpenAPI document: 2.3.8
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_user_organization.py` & `cosmotech-api-2.4.1/test/test_user_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.7
+    The version of the OpenAPI document: 2.3.8
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_user_workspace.py` & `cosmotech-api-2.4.1/test/test_workspace_role.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.7
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.user_workspace import UserWorkspace
+from cosmotech_api.model.workspace_role import WorkspaceRole
 
 
-class TestUserWorkspace(unittest.TestCase):
-    """UserWorkspace unit test stubs"""
+class TestWorkspaceRole(unittest.TestCase):
+    """WorkspaceRole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserWorkspace(self):
-        """Test UserWorkspace"""
+    def testWorkspaceRole(self):
+        """Test WorkspaceRole"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UserWorkspace()  # noqa: E501
+        # model = WorkspaceRole()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_validator.py` & `cosmotech-api-2.4.1/test/test_workspace_solution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.validator import Validator
+from cosmotech_api.model.workspace_solution import WorkspaceSolution
 
 
-class TestValidator(unittest.TestCase):
-    """Validator unit test stubs"""
+class TestWorkspaceSolution(unittest.TestCase):
+    """WorkspaceSolution unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testValidator(self):
-        """Test Validator"""
+    def testWorkspaceSolution(self):
+        """Test WorkspaceSolution"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Validator()  # noqa: E501
+        # model = WorkspaceSolution()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_validator_api.py` & `cosmotech-api-2.4.1/test/test_validator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_validator_run.py` & `cosmotech-api-2.4.1/test/test_validator_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_workspace.py` & `cosmotech-api-2.4.1/test/test_workspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_workspace_access_control.py` & `cosmotech-api-2.4.1/test/test_workspace_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_workspace_api.py` & `cosmotech-api-2.4.1/test/test_workspace_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_workspace_file.py` & `cosmotech-api-2.4.1/test/test_workspace_file.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.0/test/test_workspace_role.py` & `cosmotech-api-2.4.1/test/test_workspace_security.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_role import WorkspaceRole
+from cosmotech_api.model.workspace_access_control import WorkspaceAccessControl
+globals()['WorkspaceAccessControl'] = WorkspaceAccessControl
+from cosmotech_api.model.workspace_security import WorkspaceSecurity
 
 
-class TestWorkspaceRole(unittest.TestCase):
-    """WorkspaceRole unit test stubs"""
+class TestWorkspaceSecurity(unittest.TestCase):
+    """WorkspaceSecurity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceRole(self):
-        """Test WorkspaceRole"""
+    def testWorkspaceSecurity(self):
+        """Test WorkspaceSecurity"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceRole()  # noqa: E501
+        # model = WorkspaceSecurity()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_workspace_secret.py` & `cosmotech-api-2.4.1/test/test_workspace_user.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Platform API
+    Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_secret import WorkspaceSecret
+from cosmotech_api.model.workspace_user import WorkspaceUser
 
 
-class TestWorkspaceSecret(unittest.TestCase):
-    """WorkspaceSecret unit test stubs"""
+class TestWorkspaceUser(unittest.TestCase):
+    """WorkspaceUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceSecret(self):
-        """Test WorkspaceSecret"""
+    def testWorkspaceUser(self):
+        """Test WorkspaceUser"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceSecret()  # noqa: E501
+        # model = WorkspaceUser()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.0/test/test_workspace_web_app.py` & `cosmotech-api-2.4.1/test/test_workspace_web_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.0-dev
+    The version of the OpenAPI document: 2.4.2-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

