# Comparing `tmp/ai_api_client_sdk-1.26.2-py3-none-any.whl.zip` & `tmp/ai_api_client_sdk-1.27.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,163 +1,172 @@
-Zip file size: 224267 bytes, number of entries: 161
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 12:33 ai_api_client_sdk/__init__.py
--rw-r--r--  2.0 unx     4511 b- defN 23-Mar-20 12:33 ai_api_client_sdk/ai_api_v2_client.py
--rw-r--r--  2.0 unx     7937 b- defN 23-Mar-20 12:33 ai_api_client_sdk/exception.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 12:33 ai_api_client_sdk/helpers/__init__.py
--rw-r--r--  2.0 unx     2780 b- defN 23-Mar-20 12:33 ai_api_client_sdk/helpers/authenticator.py
--rw-r--r--  2.0 unx      120 b- defN 23-Mar-20 12:33 ai_api_client_sdk/helpers/constants.py
--rw-r--r--  2.0 unx      824 b- defN 23-Mar-20 12:33 ai_api_client_sdk/helpers/datetime_parser.py
--rw-r--r--  2.0 unx    13435 b- defN 23-Mar-20 12:33 ai_api_client_sdk/helpers/rest_client.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/__init__.py
--rw-r--r--  2.0 unx     3176 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/ai_api_capabilities.py
--rw-r--r--  2.0 unx     1691 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/ai_api_capabilities_logs.py
--rw-r--r--  2.0 unx     2260 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/ai_api_limits.py
--rw-r--r--  2.0 unx     1397 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/ai_api_limits_deployments.py
--rw-r--r--  2.0 unx      868 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/ai_api_limits_enactments.py
--rw-r--r--  2.0 unx     1384 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/ai_api_limits_executions.py
--rw-r--r--  2.0 unx     2159 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/ai_api_meta.py
--rw-r--r--  2.0 unx     1618 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/api_version.py
--rw-r--r--  2.0 unx     4078 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/artifact.py
--rw-r--r--  2.0 unx     1278 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/artifact_create_response.py
--rw-r--r--  2.0 unx     1433 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/artifact_query_response.py
--rw-r--r--  2.0 unx     7240 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/base_models.py
--rw-r--r--  2.0 unx     2314 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/capabilities.py
--rw-r--r--  2.0 unx     3687 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/configuration.py
--rw-r--r--  2.0 unx      965 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/configuration_create_response.py
--rw-r--r--  2.0 unx     1513 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/configuration_query_response.py
--rw-r--r--  2.0 unx     1778 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/dataset_capabilities.py
--rw-r--r--  2.0 unx     1663 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/dataset_limits.py
--rw-r--r--  2.0 unx     5936 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/deployment.py
--rw-r--r--  2.0 unx     1632 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/deployment_bulk_modify_response.py
--rw-r--r--  2.0 unx     1732 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/deployment_create_response.py
--rw-r--r--  2.0 unx     1466 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/deployment_query_response.py
--rw-r--r--  2.0 unx     3059 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/enactment.py
--rw-r--r--  2.0 unx     4761 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/executable.py
--rw-r--r--  2.0 unx     1466 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/executable_query_response.py
--rw-r--r--  2.0 unx     4818 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/execution.py
--rw-r--r--  2.0 unx     1609 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/execution_bulk_modify_response.py
--rw-r--r--  2.0 unx     1448 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/execution_create_response.py
--rw-r--r--  2.0 unx     1450 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/execution_query_response.py
--rw-r--r--  2.0 unx     2748 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/extensions.py
--rw-r--r--  2.0 unx     1383 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/extensions_analytics.py
--rw-r--r--  2.0 unx     2371 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/extensions_dataset.py
--rw-r--r--  2.0 unx     1461 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/extensions_resource_groups.py
--rw-r--r--  2.0 unx     1457 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/healthz_status.py
--rw-r--r--  2.0 unx      947 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/input_artifact.py
--rw-r--r--  2.0 unx     1687 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/input_artifact_binding.py
--rw-r--r--  2.0 unx      862 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/label.py
--rw-r--r--  2.0 unx     3781 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/log_response.py
--rw-r--r--  2.0 unx     2942 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/metric.py
--rw-r--r--  2.0 unx     1004 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/metric_custom_info.py
--rw-r--r--  2.0 unx     1093 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/metric_label.py
--rw-r--r--  2.0 unx     2771 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/metric_resource.py
--rw-r--r--  2.0 unx      924 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/metric_tag.py
--rw-r--r--  2.0 unx     1460 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/metrics_query_response.py
--rw-r--r--  2.0 unx      960 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/output_artifact.py
--rw-r--r--  2.0 unx     1579 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/parameter.py
--rw-r--r--  2.0 unx     1054 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/parameter_binding.py
--rw-r--r--  2.0 unx     2205 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/resource_group.py
--rw-r--r--  2.0 unx     1549 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/resource_group_query_response.py
--rw-r--r--  2.0 unx      249 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/resource_group_status.py
--rw-r--r--  2.0 unx     2519 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/scenario.py
--rw-r--r--  2.0 unx     1433 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/scenario_query_response.py
--rw-r--r--  2.0 unx      312 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/status.py
--rw-r--r--  2.0 unx      263 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/target_status.py
--rw-r--r--  2.0 unx     1866 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/version.py
--rw-r--r--  2.0 unx     1459 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/version_list.py
--rw-r--r--  2.0 unx     1417 b- defN 23-Mar-20 12:33 ai_api_client_sdk/models/version_query_response.py
--rw-r--r--  2.0 unx      461 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/__init__.py
--rw-r--r--  2.0 unx    10698 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/artifact_client.py
--rw-r--r--  2.0 unx     3114 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/base_client.py
--rw-r--r--  2.0 unx    10003 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/configuration_client.py
--rw-r--r--  2.0 unx    17475 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/deployment_client.py
--rw-r--r--  2.0 unx     3995 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/executable_client.py
--rw-r--r--  2.0 unx    16635 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/execution_client.py
--rw-r--r--  2.0 unx     1041 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/healthz_client.py
--rw-r--r--  2.0 unx      555 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/meta_client.py
--rw-r--r--  2.0 unx     4458 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/metrics_client.py
--rw-r--r--  2.0 unx     7580 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/resource_groups_client.py
--rw-r--r--  2.0 unx     5149 b- defN 23-Mar-20 12:33 ai_api_client_sdk/resource_clients/scenario_client.py
--rw-r--r--  2.0 unx     6547 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.ai_api_v2_client.html
--rw-r--r--  2.0 unx    75814 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.exception.html
--rw-r--r--  2.0 unx     4693 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.authenticator.html
--rw-r--r--  2.0 unx     3546 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.constants.html
--rw-r--r--  2.0 unx     2191 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.datetime_parser.html
--rw-r--r--  2.0 unx     1797 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.html
--rw-r--r--  2.0 unx    16006 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.rest_client.html
--rw-r--r--  2.0 unx     1818 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.html
--rw-r--r--  2.0 unx     7319 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities.html
--rw-r--r--  2.0 unx     5657 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_logs.html
--rw-r--r--  2.0 unx     5822 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits.html
--rw-r--r--  2.0 unx     6524 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_deployments.html
--rw-r--r--  2.0 unx     4073 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_enactments.html
--rw-r--r--  2.0 unx     6493 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_executions.html
--rw-r--r--  2.0 unx     5748 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_meta.html
--rw-r--r--  2.0 unx     5420 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.api_version.html
--rw-r--r--  2.0 unx     7735 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact.html
--rw-r--r--  2.0 unx     5968 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact_create_response.html
--rw-r--r--  2.0 unx     6083 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact_query_response.html
--rw-r--r--  2.0 unx    27413 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.base_models.html
--rw-r--r--  2.0 unx     6110 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.capabilities.html
--rw-r--r--  2.0 unx     7062 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration.html
--rw-r--r--  2.0 unx     5754 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration_create_response.html
--rw-r--r--  2.0 unx     6253 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration_query_response.html
--rw-r--r--  2.0 unx     5791 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.dataset_capabilities.html
--rw-r--r--  2.0 unx     5530 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.dataset_limits.html
--rw-r--r--  2.0 unx    10076 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment.html
--rw-r--r--  2.0 unx     5430 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_bulk_modify_response.html
--rw-r--r--  2.0 unx     6501 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_create_response.html
--rw-r--r--  2.0 unx     6157 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_query_response.html
--rw-r--r--  2.0 unx     7043 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.enactment.html
--rw-r--r--  2.0 unx     8144 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.executable.html
--rw-r--r--  2.0 unx     6157 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.executable_query_response.html
--rw-r--r--  2.0 unx     8766 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution.html
--rw-r--r--  2.0 unx     5402 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_bulk_modify_response.html
--rw-r--r--  2.0 unx     6124 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_create_response.html
--rw-r--r--  2.0 unx     6123 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_query_response.html
--rw-r--r--  2.0 unx     6260 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions.html
--rw-r--r--  2.0 unx     5223 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_analytics.html
--rw-r--r--  2.0 unx     6017 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_dataset.html
--rw-r--r--  2.0 unx     5385 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_resource_groups.html
--rw-r--r--  2.0 unx     7359 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.healthz_status.html
--rw-r--r--  2.0 unx     6297 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.html
--rw-r--r--  2.0 unx     5613 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.input_artifact.html
--rw-r--r--  2.0 unx     5738 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.input_artifact_binding.html
--rw-r--r--  2.0 unx     5496 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.label.html
--rw-r--r--  2.0 unx    10825 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.log_response.html
--rw-r--r--  2.0 unx     6335 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric.html
--rw-r--r--  2.0 unx     5913 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_custom_info.html
--rw-r--r--  2.0 unx     5983 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_label.html
--rw-r--r--  2.0 unx     6156 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_resource.html
--rw-r--r--  2.0 unx     5560 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_tag.html
--rw-r--r--  2.0 unx     6093 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metrics_query_response.html
--rw-r--r--  2.0 unx     5643 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.output_artifact.html
--rw-r--r--  2.0 unx     5375 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.parameter.html
--rw-r--r--  2.0 unx     5905 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.parameter_binding.html
--rw-r--r--  2.0 unx     5598 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group.html
--rw-r--r--  2.0 unx     6217 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group_query_response.html
--rw-r--r--  2.0 unx     4015 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group_status.html
--rw-r--r--  2.0 unx     6014 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.scenario.html
--rw-r--r--  2.0 unx     6083 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.scenario_query_response.html
--rw-r--r--  2.0 unx     4037 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.status.html
--rw-r--r--  2.0 unx     3956 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.target_status.html
--rw-r--r--  2.0 unx     5449 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version.html
--rw-r--r--  2.0 unx     5068 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version_list.html
--rw-r--r--  2.0 unx     6049 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version_query_response.html
--rw-r--r--  2.0 unx    18046 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.artifact_client.html
--rw-r--r--  2.0 unx     5886 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.base_client.html
--rw-r--r--  2.0 unx    17115 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.configuration_client.html
--rw-r--r--  2.0 unx    25601 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.deployment_client.html
--rw-r--r--  2.0 unx    10336 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.executable_client.html
--rw-r--r--  2.0 unx    24454 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.execution_client.html
--rw-r--r--  2.0 unx     6957 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.healthz_client.html
--rw-r--r--  2.0 unx     2537 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.html
--rw-r--r--  2.0 unx     6109 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.meta_client.html
--rw-r--r--  2.0 unx    11596 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.metrics_client.html
--rw-r--r--  2.0 unx    14424 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.resource_groups_client.html
--rw-r--r--  2.0 unx    12195 b- defN 23-Mar-20 12:33 ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.scenario_client.html
--rw-r--r--  2.0 unx    12569 b- defN 23-Mar-20 12:34 ai_api_client_sdk-1.26.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3707 b- defN 23-Mar-20 12:34 ai_api_client_sdk-1.26.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-20 12:34 ai_api_client_sdk-1.26.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-20 12:34 ai_api_client_sdk-1.26.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    19654 b- defN 23-Mar-20 12:34 ai_api_client_sdk-1.26.2.dist-info/RECORD
-161 files, 904454 bytes uncompressed, 190933 bytes compressed:  78.9%
+Zip file size: 234966 bytes, number of entries: 170
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 15:31 ai_api_client_sdk/__init__.py
+-rw-r--r--  2.0 unx     4655 b- defN 23-May-09 15:31 ai_api_client_sdk/ai_api_v2_client.py
+-rw-r--r--  2.0 unx     7937 b- defN 23-May-09 15:31 ai_api_client_sdk/exception.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 15:31 ai_api_client_sdk/helpers/__init__.py
+-rw-r--r--  2.0 unx     2780 b- defN 23-May-09 15:31 ai_api_client_sdk/helpers/authenticator.py
+-rw-r--r--  2.0 unx      120 b- defN 23-May-09 15:31 ai_api_client_sdk/helpers/constants.py
+-rw-r--r--  2.0 unx      824 b- defN 23-May-09 15:31 ai_api_client_sdk/helpers/datetime_parser.py
+-rw-r--r--  2.0 unx    13435 b- defN 23-May-09 15:31 ai_api_client_sdk/helpers/rest_client.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 15:31 ai_api_client_sdk/models/__init__.py
+-rw-r--r--  2.0 unx     4061 b- defN 23-May-09 15:31 ai_api_client_sdk/models/ai_api_capabilities.py
+-rw-r--r--  2.0 unx     1789 b- defN 23-May-09 15:31 ai_api_client_sdk/models/ai_api_capabilities_bulk_updates.py
+-rw-r--r--  2.0 unx     1691 b- defN 23-May-09 15:31 ai_api_client_sdk/models/ai_api_capabilities_logs.py
+-rw-r--r--  2.0 unx     2260 b- defN 23-May-09 15:31 ai_api_client_sdk/models/ai_api_limits.py
+-rw-r--r--  2.0 unx     1397 b- defN 23-May-09 15:31 ai_api_client_sdk/models/ai_api_limits_deployments.py
+-rw-r--r--  2.0 unx      868 b- defN 23-May-09 15:31 ai_api_client_sdk/models/ai_api_limits_enactments.py
+-rw-r--r--  2.0 unx     1384 b- defN 23-May-09 15:31 ai_api_client_sdk/models/ai_api_limits_executions.py
+-rw-r--r--  2.0 unx     2159 b- defN 23-May-09 15:31 ai_api_client_sdk/models/ai_api_meta.py
+-rw-r--r--  2.0 unx     1618 b- defN 23-May-09 15:31 ai_api_client_sdk/models/api_version.py
+-rw-r--r--  2.0 unx     4078 b- defN 23-May-09 15:31 ai_api_client_sdk/models/artifact.py
+-rw-r--r--  2.0 unx     1278 b- defN 23-May-09 15:31 ai_api_client_sdk/models/artifact_create_response.py
+-rw-r--r--  2.0 unx     1433 b- defN 23-May-09 15:31 ai_api_client_sdk/models/artifact_query_response.py
+-rw-r--r--  2.0 unx     7240 b- defN 23-May-09 15:31 ai_api_client_sdk/models/base_models.py
+-rw-r--r--  2.0 unx     2314 b- defN 23-May-09 15:31 ai_api_client_sdk/models/capabilities.py
+-rw-r--r--  2.0 unx     3687 b- defN 23-May-09 15:31 ai_api_client_sdk/models/configuration.py
+-rw-r--r--  2.0 unx      965 b- defN 23-May-09 15:31 ai_api_client_sdk/models/configuration_create_response.py
+-rw-r--r--  2.0 unx     1513 b- defN 23-May-09 15:31 ai_api_client_sdk/models/configuration_query_response.py
+-rw-r--r--  2.0 unx     1778 b- defN 23-May-09 15:31 ai_api_client_sdk/models/dataset_capabilities.py
+-rw-r--r--  2.0 unx     1663 b- defN 23-May-09 15:31 ai_api_client_sdk/models/dataset_limits.py
+-rw-r--r--  2.0 unx     5936 b- defN 23-May-09 15:31 ai_api_client_sdk/models/deployment.py
+-rw-r--r--  2.0 unx     1632 b- defN 23-May-09 15:31 ai_api_client_sdk/models/deployment_bulk_modify_response.py
+-rw-r--r--  2.0 unx     1732 b- defN 23-May-09 15:31 ai_api_client_sdk/models/deployment_create_response.py
+-rw-r--r--  2.0 unx     2402 b- defN 23-May-09 15:31 ai_api_client_sdk/models/deployment_get_status_response.py
+-rw-r--r--  2.0 unx     1466 b- defN 23-May-09 15:31 ai_api_client_sdk/models/deployment_query_response.py
+-rw-r--r--  2.0 unx     3059 b- defN 23-May-09 15:31 ai_api_client_sdk/models/enactment.py
+-rw-r--r--  2.0 unx     1489 b- defN 23-May-09 15:31 ai_api_client_sdk/models/enactment_get_status_response.py
+-rw-r--r--  2.0 unx     4761 b- defN 23-May-09 15:31 ai_api_client_sdk/models/executable.py
+-rw-r--r--  2.0 unx     1466 b- defN 23-May-09 15:31 ai_api_client_sdk/models/executable_query_response.py
+-rw-r--r--  2.0 unx     5040 b- defN 23-May-09 15:31 ai_api_client_sdk/models/execution.py
+-rw-r--r--  2.0 unx     1609 b- defN 23-May-09 15:31 ai_api_client_sdk/models/execution_bulk_modify_response.py
+-rw-r--r--  2.0 unx     1448 b- defN 23-May-09 15:31 ai_api_client_sdk/models/execution_create_response.py
+-rw-r--r--  2.0 unx     2378 b- defN 23-May-09 15:31 ai_api_client_sdk/models/execution_get_status_response.py
+-rw-r--r--  2.0 unx     1450 b- defN 23-May-09 15:31 ai_api_client_sdk/models/execution_query_response.py
+-rw-r--r--  2.0 unx     3048 b- defN 23-May-09 15:31 ai_api_client_sdk/models/execution_schedule.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-09 15:31 ai_api_client_sdk/models/execution_schedule_create_response.py
+-rw-r--r--  2.0 unx     1584 b- defN 23-May-09 15:31 ai_api_client_sdk/models/execution_schedule_query_response.py
+-rw-r--r--  2.0 unx     2748 b- defN 23-May-09 15:31 ai_api_client_sdk/models/extensions.py
+-rw-r--r--  2.0 unx     1383 b- defN 23-May-09 15:31 ai_api_client_sdk/models/extensions_analytics.py
+-rw-r--r--  2.0 unx     2371 b- defN 23-May-09 15:31 ai_api_client_sdk/models/extensions_dataset.py
+-rw-r--r--  2.0 unx     1461 b- defN 23-May-09 15:31 ai_api_client_sdk/models/extensions_resource_groups.py
+-rw-r--r--  2.0 unx     1457 b- defN 23-May-09 15:31 ai_api_client_sdk/models/healthz_status.py
+-rw-r--r--  2.0 unx      947 b- defN 23-May-09 15:31 ai_api_client_sdk/models/input_artifact.py
+-rw-r--r--  2.0 unx     1687 b- defN 23-May-09 15:31 ai_api_client_sdk/models/input_artifact_binding.py
+-rw-r--r--  2.0 unx      862 b- defN 23-May-09 15:31 ai_api_client_sdk/models/label.py
+-rw-r--r--  2.0 unx     3781 b- defN 23-May-09 15:31 ai_api_client_sdk/models/log_response.py
+-rw-r--r--  2.0 unx     2942 b- defN 23-May-09 15:31 ai_api_client_sdk/models/metric.py
+-rw-r--r--  2.0 unx     1004 b- defN 23-May-09 15:31 ai_api_client_sdk/models/metric_custom_info.py
+-rw-r--r--  2.0 unx     1093 b- defN 23-May-09 15:31 ai_api_client_sdk/models/metric_label.py
+-rw-r--r--  2.0 unx     2771 b- defN 23-May-09 15:31 ai_api_client_sdk/models/metric_resource.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-09 15:31 ai_api_client_sdk/models/metric_tag.py
+-rw-r--r--  2.0 unx     1460 b- defN 23-May-09 15:31 ai_api_client_sdk/models/metrics_query_response.py
+-rw-r--r--  2.0 unx      960 b- defN 23-May-09 15:31 ai_api_client_sdk/models/output_artifact.py
+-rw-r--r--  2.0 unx     1579 b- defN 23-May-09 15:31 ai_api_client_sdk/models/parameter.py
+-rw-r--r--  2.0 unx     1054 b- defN 23-May-09 15:31 ai_api_client_sdk/models/parameter_binding.py
+-rw-r--r--  2.0 unx     2205 b- defN 23-May-09 15:31 ai_api_client_sdk/models/resource_group.py
+-rw-r--r--  2.0 unx     1549 b- defN 23-May-09 15:31 ai_api_client_sdk/models/resource_group_query_response.py
+-rw-r--r--  2.0 unx      249 b- defN 23-May-09 15:31 ai_api_client_sdk/models/resource_group_status.py
+-rw-r--r--  2.0 unx     2519 b- defN 23-May-09 15:31 ai_api_client_sdk/models/scenario.py
+-rw-r--r--  2.0 unx     1433 b- defN 23-May-09 15:31 ai_api_client_sdk/models/scenario_query_response.py
+-rw-r--r--  2.0 unx      461 b- defN 23-May-09 15:31 ai_api_client_sdk/models/status.py
+-rw-r--r--  2.0 unx      263 b- defN 23-May-09 15:31 ai_api_client_sdk/models/target_status.py
+-rw-r--r--  2.0 unx     1866 b- defN 23-May-09 15:31 ai_api_client_sdk/models/version.py
+-rw-r--r--  2.0 unx     1459 b- defN 23-May-09 15:31 ai_api_client_sdk/models/version_list.py
+-rw-r--r--  2.0 unx     1417 b- defN 23-May-09 15:31 ai_api_client_sdk/models/version_query_response.py
+-rw-r--r--  2.0 unx      524 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/__init__.py
+-rw-r--r--  2.0 unx    10698 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/artifact_client.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/base_client.py
+-rw-r--r--  2.0 unx    10003 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/configuration_client.py
+-rw-r--r--  2.0 unx    18280 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/deployment_client.py
+-rw-r--r--  2.0 unx     3995 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/executable_client.py
+-rw-r--r--  2.0 unx    17940 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/execution_client.py
+-rw-r--r--  2.0 unx    13760 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/execution_schedule_client.py
+-rw-r--r--  2.0 unx     1041 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/healthz_client.py
+-rw-r--r--  2.0 unx      555 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/meta_client.py
+-rw-r--r--  2.0 unx     4458 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/metrics_client.py
+-rw-r--r--  2.0 unx     7580 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/resource_groups_client.py
+-rw-r--r--  2.0 unx     5149 b- defN 23-May-09 15:31 ai_api_client_sdk/resource_clients/scenario_client.py
+-rw-r--r--  2.0 unx     6547 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.ai_api_v2_client.html
+-rw-r--r--  2.0 unx    75814 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.exception.html
+-rw-r--r--  2.0 unx     4693 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.authenticator.html
+-rw-r--r--  2.0 unx     3546 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.constants.html
+-rw-r--r--  2.0 unx     2191 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.datetime_parser.html
+-rw-r--r--  2.0 unx     1797 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.html
+-rw-r--r--  2.0 unx    16006 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.rest_client.html
+-rw-r--r--  2.0 unx     1818 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.html
+-rw-r--r--  2.0 unx     8193 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities.html
+-rw-r--r--  2.0 unx     5874 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.html
+-rw-r--r--  2.0 unx     5657 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_logs.html
+-rw-r--r--  2.0 unx     5822 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits.html
+-rw-r--r--  2.0 unx     6524 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_deployments.html
+-rw-r--r--  2.0 unx     4073 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_enactments.html
+-rw-r--r--  2.0 unx     6493 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_executions.html
+-rw-r--r--  2.0 unx     5748 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_meta.html
+-rw-r--r--  2.0 unx     5420 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.api_version.html
+-rw-r--r--  2.0 unx     7735 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact.html
+-rw-r--r--  2.0 unx     5968 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact_create_response.html
+-rw-r--r--  2.0 unx     6083 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact_query_response.html
+-rw-r--r--  2.0 unx    27413 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.base_models.html
+-rw-r--r--  2.0 unx     6110 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.capabilities.html
+-rw-r--r--  2.0 unx     7062 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration.html
+-rw-r--r--  2.0 unx     5754 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration_create_response.html
+-rw-r--r--  2.0 unx     6253 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration_query_response.html
+-rw-r--r--  2.0 unx     5791 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.dataset_capabilities.html
+-rw-r--r--  2.0 unx     5530 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.dataset_limits.html
+-rw-r--r--  2.0 unx    10076 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment.html
+-rw-r--r--  2.0 unx     5430 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_bulk_modify_response.html
+-rw-r--r--  2.0 unx     6501 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_create_response.html
+-rw-r--r--  2.0 unx     6157 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_query_response.html
+-rw-r--r--  2.0 unx     7043 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.enactment.html
+-rw-r--r--  2.0 unx     8144 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.executable.html
+-rw-r--r--  2.0 unx     6157 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.executable_query_response.html
+-rw-r--r--  2.0 unx     9044 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution.html
+-rw-r--r--  2.0 unx     5402 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_bulk_modify_response.html
+-rw-r--r--  2.0 unx     6124 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_create_response.html
+-rw-r--r--  2.0 unx     6123 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_query_response.html
+-rw-r--r--  2.0 unx     6260 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions.html
+-rw-r--r--  2.0 unx     5223 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_analytics.html
+-rw-r--r--  2.0 unx     6017 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_dataset.html
+-rw-r--r--  2.0 unx     5385 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_resource_groups.html
+-rw-r--r--  2.0 unx     7359 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.healthz_status.html
+-rw-r--r--  2.0 unx     7057 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.html
+-rw-r--r--  2.0 unx     5613 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.input_artifact.html
+-rw-r--r--  2.0 unx     5738 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.input_artifact_binding.html
+-rw-r--r--  2.0 unx     5496 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.label.html
+-rw-r--r--  2.0 unx    10825 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.log_response.html
+-rw-r--r--  2.0 unx     6335 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric.html
+-rw-r--r--  2.0 unx     5913 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_custom_info.html
+-rw-r--r--  2.0 unx     5983 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_label.html
+-rw-r--r--  2.0 unx     6156 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_resource.html
+-rw-r--r--  2.0 unx     5560 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_tag.html
+-rw-r--r--  2.0 unx     6093 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metrics_query_response.html
+-rw-r--r--  2.0 unx     5643 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.output_artifact.html
+-rw-r--r--  2.0 unx     5375 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.parameter.html
+-rw-r--r--  2.0 unx     5905 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.parameter_binding.html
+-rw-r--r--  2.0 unx     5598 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group.html
+-rw-r--r--  2.0 unx     6217 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group_query_response.html
+-rw-r--r--  2.0 unx     4015 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group_status.html
+-rw-r--r--  2.0 unx     6014 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.scenario.html
+-rw-r--r--  2.0 unx     6083 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.scenario_query_response.html
+-rw-r--r--  2.0 unx     6142 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.status.html
+-rw-r--r--  2.0 unx     3956 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.target_status.html
+-rw-r--r--  2.0 unx     5449 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version.html
+-rw-r--r--  2.0 unx     5068 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version_list.html
+-rw-r--r--  2.0 unx     6049 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version_query_response.html
+-rw-r--r--  2.0 unx    18046 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.artifact_client.html
+-rw-r--r--  2.0 unx     5886 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.base_client.html
+-rw-r--r--  2.0 unx    17115 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.configuration_client.html
+-rw-r--r--  2.0 unx    26095 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.deployment_client.html
+-rw-r--r--  2.0 unx    10336 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.executable_client.html
+-rw-r--r--  2.0 unx    25388 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.execution_client.html
+-rw-r--r--  2.0 unx     6957 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.healthz_client.html
+-rw-r--r--  2.0 unx     2647 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.html
+-rw-r--r--  2.0 unx     6109 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.meta_client.html
+-rw-r--r--  2.0 unx    11596 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.metrics_client.html
+-rw-r--r--  2.0 unx    14424 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.resource_groups_client.html
+-rw-r--r--  2.0 unx    12195 b- defN 23-May-09 15:31 ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.scenario_client.html
+-rw-r--r--  2.0 unx    12569 b- defN 23-May-09 15:32 ai_api_client_sdk-1.27.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3707 b- defN 23-May-09 15:32 ai_api_client_sdk-1.27.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 15:32 ai_api_client_sdk-1.27.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-09 15:32 ai_api_client_sdk-1.27.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    20734 b- defN 23-May-09 15:32 ai_api_client_sdk-1.27.0.dist-info/RECORD
+170 files, 947986 bytes uncompressed, 199816 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -24,14 +24,17 @@
 
 Filename: ai_api_client_sdk/models/__init__.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/ai_api_capabilities.py
 Comment: 
 
+Filename: ai_api_client_sdk/models/ai_api_capabilities_bulk_updates.py
+Comment: 
+
 Filename: ai_api_client_sdk/models/ai_api_capabilities_logs.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/ai_api_limits.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/ai_api_limits_deployments.py
@@ -84,20 +87,26 @@
 
 Filename: ai_api_client_sdk/models/deployment_bulk_modify_response.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/deployment_create_response.py
 Comment: 
 
+Filename: ai_api_client_sdk/models/deployment_get_status_response.py
+Comment: 
+
 Filename: ai_api_client_sdk/models/deployment_query_response.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/enactment.py
 Comment: 
 
+Filename: ai_api_client_sdk/models/enactment_get_status_response.py
+Comment: 
+
 Filename: ai_api_client_sdk/models/executable.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/executable_query_response.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/execution.py
@@ -105,17 +114,29 @@
 
 Filename: ai_api_client_sdk/models/execution_bulk_modify_response.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/execution_create_response.py
 Comment: 
 
+Filename: ai_api_client_sdk/models/execution_get_status_response.py
+Comment: 
+
 Filename: ai_api_client_sdk/models/execution_query_response.py
 Comment: 
 
+Filename: ai_api_client_sdk/models/execution_schedule.py
+Comment: 
+
+Filename: ai_api_client_sdk/models/execution_schedule_create_response.py
+Comment: 
+
+Filename: ai_api_client_sdk/models/execution_schedule_query_response.py
+Comment: 
+
 Filename: ai_api_client_sdk/models/extensions.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/extensions_analytics.py
 Comment: 
 
 Filename: ai_api_client_sdk/models/extensions_dataset.py
@@ -213,14 +234,17 @@
 
 Filename: ai_api_client_sdk/resource_clients/executable_client.py
 Comment: 
 
 Filename: ai_api_client_sdk/resource_clients/execution_client.py
 Comment: 
 
+Filename: ai_api_client_sdk/resource_clients/execution_schedule_client.py
+Comment: 
+
 Filename: ai_api_client_sdk/resource_clients/healthz_client.py
 Comment: 
 
 Filename: ai_api_client_sdk/resource_clients/meta_client.py
 Comment: 
 
 Filename: ai_api_client_sdk/resource_clients/metrics_client.py
@@ -228,257 +252,260 @@
 
 Filename: ai_api_client_sdk/resource_clients/resource_groups_client.py
 Comment: 
 
 Filename: ai_api_client_sdk/resource_clients/scenario_client.py
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.ai_api_v2_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.ai_api_v2_client.html
+Comment: 
+
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.exception.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.exception.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.authenticator.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.authenticator.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.constants.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.constants.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.datetime_parser.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.datetime_parser.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.rest_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.rest_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_logs.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_logs.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_deployments.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_deployments.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_enactments.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_enactments.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_executions.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_executions.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_meta.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_meta.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.api_version.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.api_version.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact_create_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact_create_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.base_models.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.base_models.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.capabilities.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.capabilities.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration_create_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration_create_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.dataset_capabilities.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.dataset_capabilities.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.dataset_limits.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.dataset_limits.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_bulk_modify_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_bulk_modify_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_create_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_create_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.enactment.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.enactment.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.executable.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.executable.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.executable_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.executable_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_bulk_modify_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_bulk_modify_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_create_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_create_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_analytics.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_analytics.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_dataset.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_dataset.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_resource_groups.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_resource_groups.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.healthz_status.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.healthz_status.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.input_artifact.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.input_artifact.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.input_artifact_binding.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.input_artifact_binding.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.label.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.label.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.log_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.log_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_custom_info.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_custom_info.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_label.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_label.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_resource.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_resource.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_tag.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_tag.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metrics_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metrics_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.output_artifact.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.output_artifact.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.parameter.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.parameter.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.parameter_binding.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.parameter_binding.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group_status.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group_status.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.scenario.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.scenario.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.scenario_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.scenario_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.status.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.status.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.target_status.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.target_status.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version_list.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version_list.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version_query_response.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version_query_response.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.artifact_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.artifact_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.base_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.base_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.configuration_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.configuration_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.deployment_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.deployment_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.executable_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.executable_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.execution_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.execution_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.healthz_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.healthz_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.meta_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.meta_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.metrics_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.metrics_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.resource_groups_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.resource_groups_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.scenario_client.html
+Filename: ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.scenario_client.html
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.dist-info/LICENSE
+Filename: ai_api_client_sdk-1.27.0.dist-info/LICENSE
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.dist-info/METADATA
+Filename: ai_api_client_sdk-1.27.0.dist-info/METADATA
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.dist-info/WHEEL
+Filename: ai_api_client_sdk-1.27.0.dist-info/WHEEL
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.dist-info/top_level.txt
+Filename: ai_api_client_sdk-1.27.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ai_api_client_sdk-1.26.2.dist-info/RECORD
+Filename: ai_api_client_sdk-1.27.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ai_api_client_sdk/ai_api_v2_client.py

```diff
@@ -1,14 +1,15 @@
 from typing import Callable
 
 from ai_api_client_sdk.exception import AIAPIAuthenticatorException
 from ai_api_client_sdk.helpers.authenticator import Authenticator
 from ai_api_client_sdk.helpers.rest_client import RestClient
 from ai_api_client_sdk.resource_clients import ArtifactClient, ConfigurationClient, DeploymentClient, \
-    ExecutableClient, ExecutionClient, HealthzClient, MetaClient, MetricsClient, ScenarioClient, ResourceGroupsClient
+    ExecutableClient, ExecutionClient, ExecutionScheduleClient, HealthzClient, MetaClient, MetricsClient, \
+    ScenarioClient, ResourceGroupsClient
 from ai_api_client_sdk.helpers.constants import Timeouts
 
 
 class AIAPIV2Client:
     """The AIAPIV2Client is the class implemented to interact with the AI API server. The user can use its attributes
     corresponding to the resources, for interacting with endpoints related to that resource. (i.e.,
     aiapiv2client.scenario)
@@ -54,13 +55,14 @@
                                                   num_request_retries=num_request_retries,
                                                   client_type='AI API Python SDK')
         self.artifact: ArtifactClient = ArtifactClient(rest_client=self.rest_client)
         self.configuration: ConfigurationClient = ConfigurationClient(rest_client=self.rest_client)
         self.deployment: DeploymentClient = DeploymentClient(rest_client=self.rest_client)
         self.executable: ExecutableClient = ExecutableClient(rest_client=self.rest_client)
         self.execution: ExecutionClient = ExecutionClient(rest_client=self.rest_client)
+        self.execution_schedule: ExecutionScheduleClient = ExecutionScheduleClient(rest_client=self.rest_client)
         self.healthz: HealthzClient = HealthzClient(rest_client=self.rest_client)
         self.metrics: MetricsClient = MetricsClient(rest_client=self.rest_client)
         self.scenario: ScenarioClient = ScenarioClient(rest_client=self.rest_client)
         self.meta: MetaClient = MetaClient(rest_client=self.rest_client)
         admin_rest_client = RestClient(base_url=base_url[:-3], get_token=token_creator, resource_group=resource_group)
         self.resource_groups: ResourceGroupsClient = ResourceGroupsClient(rest_client=admin_rest_client)
```

## ai_api_client_sdk/models/ai_api_capabilities.py

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict
 
+from ai_api_client_sdk.models.ai_api_capabilities_bulk_updates import AIAPICapabilitiesBulkUpdates
 from ai_api_client_sdk.models.ai_api_capabilities_logs import AIAPICapabilitiesLogs
 
 
 class AIAPICapabilities:
     """The AIAPICapabilities object represent the capabilities of the AI API
 
     :param multitenant: indicates whether resource groups are supported, defaults to True
@@ -14,42 +15,52 @@
     :type static_deployments: bool, optional
     :param user_deployments: indicates whether deployment creation by users are supported, defaults to True
     :type user_deployments: bool, optional
     :param time_to_live_deployments: indicate whether ttl value of deployment are supported, defaults to False
     :type time_to_live_deployments: bool, optional
     :param user_executions: indicates whether execution creation by users are supported, defaults to True
     :type user_executions: bool, optional
+    :param bulk_updates: An object, defining the bulk updates capabilities, defaults to None
+    :type bulk_updates: class:`ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.AIAPICapabilitiesBulkUpdates`,
+     optional
+    :param execution_schedules: indicates whether execution schedules are supported, defaults to False
+    :type execution_schedules: bool, optional
     :param logs: An object, defining the logs capabilities, defaults to None
     :type logs: class:`ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs`, optional
     :param `**kwargs`: The keyword arguments are there in case there are additional attributes returned from server
     """
+
     def __init__(self, multitenant: bool = True, shareable: bool = True, static_deployments: bool = True,
-                 user_deployments: bool = True, time_to_live_deployments: bool = False,
-                 user_executions: bool = True, logs: AIAPICapabilitiesLogs = None,
-                 **kwargs):
+                 user_deployments: bool = True, time_to_live_deployments: bool = False, user_executions: bool = True,
+                 bulk_updates: AIAPICapabilitiesBulkUpdates = None, execution_schedules: bool = False,
+                 logs: AIAPICapabilitiesLogs = None, **kwargs):
         self.multitenant: bool = multitenant
         self.shareable: bool = shareable
         self.static_deployments: bool = static_deployments
         self.user_deployments: bool = user_deployments
         self.time_to_live_deployments: bool = time_to_live_deployments
         self.user_executions: bool = user_executions
+        self.bulk_updates: AIAPICapabilitiesBulkUpdates = bulk_updates
+        self.execution_schedules: bool = execution_schedules
         self.logs: AIAPICapabilitiesLogs = logs
 
     @staticmethod
     def from_dict(ai_api_capabilities_dict: Dict[str, Any]):
         """Returns a :class:`ai_api_client_sdk.models.ai_api_capabilities.AIAPICapabilities` object, created from the
         values in the dict provided as parameter
 
         :param ai_api_capabilities_dict: Dict which includes the necessary values to create the object
         :type ai_api_capabilities_dict: Dict[str, Any]
         :return: An object, created from the values provided
         :rtype: class:`ai_api_client_sdk.models.ai_api_capabilities.AIAPICapabilities`
         """
         if 'logs' in ai_api_capabilities_dict:
             ai_api_capabilities_dict['logs'] = AIAPICapabilitiesLogs.from_dict(ai_api_capabilities_dict['logs'])
+        if 'bulk_updates' in ai_api_capabilities_dict:
+            ai_api_capabilities_dict['bulk_updates'] = AIAPICapabilitiesBulkUpdates.from_dict(ai_api_capabilities_dict['bulk_updates'])
         return AIAPICapabilities(**ai_api_capabilities_dict)
 
     def __eq__(self, other):
         if not isinstance(other, AIAPICapabilities):
             return False
         for k in self.__dict__.keys():
             if getattr(self, k) != getattr(other, k):
```

## ai_api_client_sdk/models/execution.py

```diff
@@ -19,14 +19,16 @@
     :type configuration_name: str
     :param scenario_id: ID of the scenario which the execution belongs to
     :type scenario_id: str
     :param status: Status of the execution
     :type status: class:`ai_api_client_sdk.models.status.Status`
     :param target_status: Target status of the execution
     :type target_status: class:`ai_api_client_sdk.models.target_status.TargetStatus`
+    :param execution_schedule_id: ID of the execution schedule, defaults to None
+    :type execution_schedule_id: str, optional
     :param created_at: Time when the execution was created
     :type created_at: datetime
     :param modified_at: Time when the execution was last modified
     :type modified_at: datetime
     :param output_artifacts: List of the artifacts created by the execution, defaults to None
     :type output_artifacts: List[class:`ai_api_client_sdk.models.artifact.Artifact`], optional
     :param status_message: Gives information about the status of the execution, defaults to None
@@ -41,21 +43,22 @@
     :type completion_time: datetime, optional
     :param `**kwargs`: The keyword arguments are there in case there are additional attributes returned from server
     """
     def __init__(self, id: str, configuration_id: str, configuration_name: str, scenario_id: str, status: Status,
                  target_status: TargetStatus, created_at: datetime, modified_at: datetime,
                  output_artifacts: List[Artifact] = None, status_message: str = None,
                  status_details: Dict[str, Any] = None, submission_time: datetime = None, start_time: datetime = None,
-                 completion_time: datetime = None, **kwargs):
+                 execution_schedule_id: str = None, completion_time: datetime = None, **kwargs):
         super().__init__(id=id, configuration_id=configuration_id, configuration_name=configuration_name,
                          scenario_id=scenario_id, status=status, target_status=target_status, created_at=created_at,
                          modified_at=modified_at, status_message=status_message, status_details=status_details,
                          submission_time=submission_time, start_time=start_time, completion_time=completion_time,
                          **kwargs)
         self.output_artifacts: List[Artifact] = output_artifacts
+        self.execution_schedule_id = execution_schedule_id
 
     def __str__(self):
         return "Execution id: " + str(self.id)
 
     @staticmethod
     def from_dict(execution_dict: Dict[str, Any]):
         """Returns a :class:`ai_api_client_sdk.models.execution.Execution` object, created from the values in the dict
```

## ai_api_client_sdk/models/status.py

```diff
@@ -7,7 +7,14 @@
     PENDING = 'PENDING'
     RUNNING = 'RUNNING'
     COMPLETED = 'COMPLETED'
     DEAD = 'DEAD'
     STOPPING = 'STOPPING'
     STOPPED = 'STOPPED'
     UNKNOWN = 'UNKNOWN'
+
+
+class ScheduleStatus(Enum):
+    """Enum defining the status values for execution schedules
+    """
+    ACTIVE = 'ACTIVE'
+    INACTIVE = 'INACTIVE'
```

## ai_api_client_sdk/resource_clients/__init__.py

```diff
@@ -1,10 +1,11 @@
 from .artifact_client import ArtifactClient
 from .configuration_client import ConfigurationClient
 from .deployment_client import DeploymentClient
 from .executable_client import ExecutableClient
 from .execution_client import ExecutionClient
+from .execution_schedule_client import ExecutionScheduleClient
 from .healthz_client import HealthzClient
 from .metrics_client import MetricsClient
 from .scenario_client import ScenarioClient
 from .resource_groups_client import ResourceGroupsClient
 from .meta_client import MetaClient
```

## ai_api_client_sdk/resource_clients/deployment_client.py

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime
-from typing import List
+from typing import List, Union
 import re
 
 from ai_api_client_sdk.exception import AIAPIInvalidInputException
 from ai_api_client_sdk.models.base_models import BasicResponse, Order, BasicModifyRequest
 from ai_api_client_sdk.models.deployment import Deployment
 from ai_api_client_sdk.models.deployment_create_response import DeploymentCreateResponse
 from ai_api_client_sdk.models.deployment_query_response import DeploymentQueryResponse
 from ai_api_client_sdk.models.deployment_bulk_modify_response import DeploymentBulkModifyResponse
+from ai_api_client_sdk.models.deployment_get_status_response import DeploymentGetStatusResponse
 from ai_api_client_sdk.models.log_response import LogResponse
 from ai_api_client_sdk.models.status import Status
 from ai_api_client_sdk.models.target_status import TargetStatus
 from ai_api_client_sdk.resource_clients.base_client import BaseClient
 
 
 class DeploymentClient(BaseClient):
@@ -72,38 +73,48 @@
             trying to send a request to the server
         :return: An object representing the response from the server
         :rtype: class:`ai_api_client_sdk.models.base_models.BasicResponse`
         """
         response_dict = self.rest_client.delete(f'/deployments/{deployment_id}', resource_group=resource_group)
         return BasicResponse.from_dict(response_dict)
 
-    def get(self, deployment_id: str, resource_group: str = None) -> Deployment:
+    def get(self, deployment_id: str, resource_group: str = None, select: str = None) -> \
+            Union[Deployment, DeploymentGetStatusResponse]:
         """Retrieves the deployment from the server.
 
         :param deployment_id: ID of the deployment to be retrieved
         :type deployment_id: str
         :param resource_group: Resource Group which the request should be sent on behalf. Either this or a default
             resource group in the :class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client` should be specified,
             defaults to None
         :type resource_group: str
+        :param select: only status supported. Get deployment for a given deployment id and select status
+        :type select: str, optional
         :raises: class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException` if a 400 response is received from the
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPIAuthorizationException` if a 401 response is received from the
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPINotFoundException` if a 404 response is received from the
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPIServerException` if a non-2XX response is received from the
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
             trying to send a request to the server
         :return: The retrieved deployment
-        :rtype: class:`ai_api_client_sdk.models.deployment.Deployment`
+        :rtype: class:Union[`ai_api_client_sdk.models.deployment.Deployment`,
+            `ai_api_client_sdk.models.deployment_get_status_response.DeploymentGetStatusResponse`]
         """
-        deployment_dict = self.rest_client.get(path=f'/deployments/{deployment_id}', resource_group=resource_group)
-        return Deployment.from_dict(deployment_dict)
+        if select and 'status' in select:
+            param = self._form_query_params(select='status')
+            deployment_dict = self.rest_client.get(path=f'/deployments/{deployment_id}',  params=param,
+                                                   resource_group=resource_group)
+            return DeploymentGetStatusResponse.from_dict(deployment_dict)
+        else:
+            deployment_dict = self.rest_client.get(path=f'/deployments/{deployment_id}', resource_group=resource_group)
+            return Deployment.from_dict(deployment_dict)
 
     def modify(self, deployment_id: str, target_status: TargetStatus = None, configuration_id: str = None,
                resource_group: str = None) -> BasicResponse:
         """Modifies the deployment, by changing either the target status, or the configuration ID.
 
         :param deployment_id: ID of the deployment to be modified
         :type deployment_id: str
```

## ai_api_client_sdk/resource_clients/execution_client.py

```diff
@@ -1,14 +1,15 @@
-from typing import List
+from typing import List, Union
 from datetime import datetime
 
 from ai_api_client_sdk.models.base_models import BasicResponse, Order, BasicModifyRequest
 from ai_api_client_sdk.models.execution import Execution
 from ai_api_client_sdk.models.execution_create_response import ExecutionCreateResponse
 from ai_api_client_sdk.models.execution_query_response import ExecutionQueryResponse
+from ai_api_client_sdk.models.execution_get_status_response import ExecutionGetStatusResponse
 from ai_api_client_sdk.models.execution_bulk_modify_response import ExecutionBulkModifyResponse
 from ai_api_client_sdk.models.log_response import LogResponse
 from ai_api_client_sdk.models.status import Status
 from ai_api_client_sdk.models.target_status import TargetStatus
 from ai_api_client_sdk.resource_clients.base_client import BaseClient
 
 
@@ -65,38 +66,48 @@
             trying to send a request to the server
         :return: An object representing the response from the server
         :rtype: class:`ai_api_client_sdk.models.base_models.BasicResponse`
         """
         response_dict = self.rest_client.delete(path=f'/executions/{execution_id}', resource_group=resource_group)
         return BasicResponse.from_dict(response_dict)
 
-    def get(self, execution_id: str, resource_group: str = None) -> Execution:
+    def get(self, execution_id: str, resource_group: str = None, select: str = None) -> \
+            Union[Execution, ExecutionGetStatusResponse]:
         """Retrieves the execution from the server.
 
         :param execution_id: ID of the execution to be retrieved
         :type execution_id: str
         :param resource_group: Resource Group which the request should be sent on behalf. Either this or a default
             resource group in the :class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client` should be specified,
             defaults to None
         :type resource_group: str
+        :param select: only status supported. Get execution for a given execution id and select status
+        :type select: str, optional
         :raises: class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException` if a 400 response is received from the
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPIAuthorizationException` if a 401 response is received from the
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPINotFoundException` if a 404 response is received from the
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPIServerException` if a non-2XX response is received from the
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
             trying to send a request to the server
         :return: The retrieved execution
-        :rtype: class:`ai_api_client_sdk.models.execution.Execution`
+        :rtype: class:Union[`ai_api_client_sdk.models.execution.Execution`,
+            `ai_api_client_sdk.models.execution_get_status_response.ExecutionGetStatusResponse`]
         """
-        execution_dict = self.rest_client.get(path=f'/executions/{execution_id}', resource_group=resource_group)
-        return Execution.from_dict(execution_dict)
+        if select and 'status' in select:
+            param = self._form_query_params(select='status')
+            execution_dict = self.rest_client.get(path=f'/executions/{execution_id}', params=param,
+                                                  resource_group=resource_group)
+            return ExecutionGetStatusResponse.from_dict(execution_dict)
+        else:
+            execution_dict = self.rest_client.get(path=f'/executions/{execution_id}', resource_group=resource_group)
+            return Execution.from_dict(execution_dict)
 
     def modify(self, execution_id: str, target_status: TargetStatus, resource_group: str = None) -> BasicResponse:
         """Modifies the execution, by changing the target status.
 
         :param execution_id: ID of the execution to be modified
         :type execution_id: str
         :param target_status: Desired target status of the execution, defaults to None
@@ -122,24 +133,26 @@
         """
         body = {'target_status': target_status.value}
         response_dict = self.rest_client.patch(path=f'/executions/{execution_id}', body=body,
                                                resource_group=resource_group)
         return BasicResponse.from_dict(response_dict)
 
     def query(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None,
-              status: Status = None, top: int = None, skip: int = None,
+              execution_schedule_id: str = None, status: Status = None, top: int = None, skip: int = None,
               resource_group: str = None) -> ExecutionQueryResponse:
         """Queries the executions.
 
         :param scenario_id: ID of the scenario the executions should belong to, defaults to None
         :type scenario_id: str, optional
         :param configuration_id: ID of the configuration, the executions should be configured by, defaults to None
         :type configuration_id: str, optional
         :param executable_ids: IDs of the executables the executions should be created from, defaults to None
         :type executable_ids: List[str], optional
+        :param execution_schedule_id: ID of the execution schedule, defaults to None
+        :type execution_schedule_id: str, optional
         :param status: Status which the executions should currently have
         :type status: class:`ai_api_client_sdk.models.status.Status`, optional
         :param top: Number of executions to be retrieved, defaults to None
         :type top: int, optional
         :param skip: Number of executions to be skipped, from the list of the queried executions, defaults to None
         :type skip: int, optional
         :param resource_group: Resource Group which the request should be sent on behalf. Either this or a default
@@ -154,29 +167,32 @@
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
             trying to send a request to the server
         :return: An object representing the response from the server
         :rtype: class:`ai_api_client_sdk.models.execution_query_response.ExecutionQueryResponse`
         """
         params = self._form_query_params(scenario_id=scenario_id, configuration_id=configuration_id,
-                                         executable_ids=executable_ids, status=status.value if status else None,
+                                         executable_ids=executable_ids, execution_schedule_id=execution_schedule_id,
+                                         status=status.value if status else None,
                                          top=top, skip=skip)
         response_dict = self.rest_client.get(path='/executions', params=params, resource_group=resource_group)
         return ExecutionQueryResponse.from_dict(response_dict)
 
     def count(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None,
-              status: Status = None, resource_group: str = None) -> int:
+              execution_schedule_id: str = None, status: Status = None, resource_group: str = None) -> int:
         """Counts the number of executions.
 
         :param scenario_id: ID of the scenario, the executions should belong to, defaults to None
         :type scenario_id: str, optional
         :param configuration_id: ID of the configuration, the executions should be configured by, defaults to None
         :type configuration_id: str, optional
         :param executable_ids: IDs of the executables, the executions should be created from, defaults to None
         :type executable_ids: List[str], optional
+        :param execution_schedule_id: ID of the execution schedule, defaults to None
+        :type execution_schedule_id: str, optional
         :param status: Status which the executions should currently have
         :type status: class:`ai_api_client_sdk.models.status.Status`, optional
         :param resource_group: Resource group which the request should be sent on behalf. Either this or a default
             resource group in the :class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client` should be specified,
             defaults to None
         :type resource_group: str
         :raises: class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException` if a 400 response is received from the
@@ -187,15 +203,16 @@
             server
         :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
             trying to send a request to the server
         :return: An object representing the response from the server
         :rtype: int
         """
         params = self._form_query_params(scenario_id=scenario_id, configuration_id=configuration_id,
-                                         executable_ids=executable_ids, status=status.value if status else None)
+                                         executable_ids=executable_ids, execution_schedule_id=execution_schedule_id,
+                                         status=status.value if status else None)
         return self.rest_client.get(path='/executions/$count', params=params, resource_group=resource_group)
 
     def query_logs(self, execution_id: str, top: int = None, start: datetime = None, end: datetime = None,
                    order: Order = None, resource_group: str = None) -> LogResponse:
         """Queries the logs of the execution.
 
         :param execution_id: ID of the execution
```

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.ai_api_v2_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.ai_api_v2_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.exception.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.exception.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.authenticator.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.authenticator.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.constants.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.constants.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.datetime_parser.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.datetime_parser.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.rest_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.rest_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities.html`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ffc8d8">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#000000" face="helvetica, arial"><a name="AIAPICapabilities">class <strong>AIAPICapabilities</strong></a>(<a href="builtins.html#object">builtins.object</a>)</font></td></tr>
     
 <tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
-<td colspan=2><tt><a href="#AIAPICapabilities">AIAPICapabilities</a>(multitenant:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;shareable:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;static_deployments:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;user_deployments:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;time_to_live_deployments:&nbsp;bool&nbsp;=&nbsp;False,&nbsp;user_executions:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;logs:&nbsp;ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs&nbsp;=&nbsp;None,&nbsp;**kwargs)<br>
+<td colspan=2><tt><a href="#AIAPICapabilities">AIAPICapabilities</a>(multitenant:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;shareable:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;static_deployments:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;user_deployments:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;time_to_live_deployments:&nbsp;bool&nbsp;=&nbsp;False,&nbsp;user_executions:&nbsp;bool&nbsp;=&nbsp;True,&nbsp;bulk_updates:&nbsp;ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.AIAPICapabilitiesBulkUpdates&nbsp;=&nbsp;None,&nbsp;execution_schedules:&nbsp;bool&nbsp;=&nbsp;False,&nbsp;logs:&nbsp;ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs&nbsp;=&nbsp;None,&nbsp;**kwargs)<br>
 &nbsp;<br>
 The&nbsp;<a href="#AIAPICapabilities">AIAPICapabilities</a>&nbsp;<a href="builtins.html#object">object</a>&nbsp;represent&nbsp;the&nbsp;capabilities&nbsp;of&nbsp;the&nbsp;AI&nbsp;API<br>
 &nbsp;<br>
 :param&nbsp;multitenant:&nbsp;indicates&nbsp;whether&nbsp;resource&nbsp;groups&nbsp;are&nbsp;supported,&nbsp;defaults&nbsp;to&nbsp;True<br>
 :type&nbsp;multitenant:&nbsp;bool,&nbsp;optional<br>
 :param&nbsp;shareable:&nbsp;indicates&nbsp;whether&nbsp;clients&nbsp;can&nbsp;share&nbsp;an&nbsp;instance,&nbsp;defaults&nbsp;to&nbsp;True<br>
 :type&nbsp;shareable:&nbsp;bool,&nbsp;optional<br>
@@ -44,22 +44,27 @@
 :type&nbsp;static_deployments:&nbsp;bool,&nbsp;optional<br>
 :param&nbsp;user_deployments:&nbsp;indicates&nbsp;whether&nbsp;deployment&nbsp;creation&nbsp;by&nbsp;users&nbsp;are&nbsp;supported,&nbsp;defaults&nbsp;to&nbsp;True<br>
 :type&nbsp;user_deployments:&nbsp;bool,&nbsp;optional<br>
 :param&nbsp;time_to_live_deployments:&nbsp;indicate&nbsp;whether&nbsp;ttl&nbsp;value&nbsp;of&nbsp;deployment&nbsp;are&nbsp;supported,&nbsp;defaults&nbsp;to&nbsp;False<br>
 :type&nbsp;time_to_live_deployments:&nbsp;bool,&nbsp;optional<br>
 :param&nbsp;user_executions:&nbsp;indicates&nbsp;whether&nbsp;execution&nbsp;creation&nbsp;by&nbsp;users&nbsp;are&nbsp;supported,&nbsp;defaults&nbsp;to&nbsp;True<br>
 :type&nbsp;user_executions:&nbsp;bool,&nbsp;optional<br>
+:param&nbsp;bulk_updates:&nbsp;An&nbsp;<a href="builtins.html#object">object</a>,&nbsp;defining&nbsp;the&nbsp;bulk&nbsp;updates&nbsp;capabilities,&nbsp;defaults&nbsp;to&nbsp;None<br>
+:type&nbsp;bulk_updates:&nbsp;class:`ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.AIAPICapabilitiesBulkUpdates`,<br>
+&nbsp;optional<br>
+:param&nbsp;execution_schedules:&nbsp;indicates&nbsp;whether&nbsp;execution&nbsp;schedules&nbsp;are&nbsp;supported,&nbsp;defaults&nbsp;to&nbsp;False<br>
+:type&nbsp;execution_schedules:&nbsp;bool,&nbsp;optional<br>
 :param&nbsp;logs:&nbsp;An&nbsp;<a href="builtins.html#object">object</a>,&nbsp;defining&nbsp;the&nbsp;logs&nbsp;capabilities,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;logs:&nbsp;class:`ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs`,&nbsp;optional<br>
 :param&nbsp;`**kwargs`:&nbsp;The&nbsp;keyword&nbsp;arguments&nbsp;are&nbsp;there&nbsp;in&nbsp;case&nbsp;there&nbsp;are&nbsp;additional&nbsp;attributes&nbsp;returned&nbsp;from&nbsp;server<br>&nbsp;</tt></td></tr>
 <tr><td>&nbsp;</td>
 <td width="100%">Methods defined here:<br>
 <dl><dt><a name="AIAPICapabilities-__eq__"><strong>__eq__</strong></a>(self, other)</dt><dd><tt>Return&nbsp;self==value.</tt></dd></dl>
 
-<dl><dt><a name="AIAPICapabilities-__init__"><strong>__init__</strong></a>(self, multitenant: bool = True, shareable: bool = True, static_deployments: bool = True, user_deployments: bool = True, time_to_live_deployments: bool = False, user_executions: bool = True, logs: ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs = None, **kwargs)</dt><dd><tt>Initialize&nbsp;self.&nbsp;&nbsp;See&nbsp;help(type(self))&nbsp;for&nbsp;accurate&nbsp;signature.</tt></dd></dl>
+<dl><dt><a name="AIAPICapabilities-__init__"><strong>__init__</strong></a>(self, multitenant: bool = True, shareable: bool = True, static_deployments: bool = True, user_deployments: bool = True, time_to_live_deployments: bool = False, user_executions: bool = True, bulk_updates: ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.AIAPICapabilitiesBulkUpdates = None, execution_schedules: bool = False, logs: ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs = None, **kwargs)</dt><dd><tt>Initialize&nbsp;self.&nbsp;&nbsp;See&nbsp;help(type(self))&nbsp;for&nbsp;accurate&nbsp;signature.</tt></dd></dl>
 
 <dl><dt><a name="AIAPICapabilities-__str__"><strong>__str__</strong></a>(self)</dt><dd><tt>Return&nbsp;str(self).</tt></dd></dl>
 
 <hr>
 Static methods defined here:<br>
 <dl><dt><a name="AIAPICapabilities-from_dict"><strong>from_dict</strong></a>(ai_api_capabilities_dict: Dict[str, Any])</dt><dd><tt>Returns&nbsp;a&nbsp;:class:`ai_api_client_sdk.models.ai_api_capabilities.<a href="#AIAPICapabilities">AIAPICapabilities</a>`&nbsp;<a href="builtins.html#object">object</a>,&nbsp;created&nbsp;from&nbsp;the<br>
 values&nbsp;in&nbsp;the&nbsp;dict&nbsp;provided&nbsp;as&nbsp;parameter<br>
```

### html2text {}

```diff
@@ -6,16 +6,17 @@
  
 Classes
            builtins.object
                  AIAPICapabilities
           
          class AIAPICapabilities(builtins.object)
              AIAPICapabilities(multitenant: bool = True, shareable: bool = True, static_deployments: bool = True, user_deployments:
-              bool = True, time_to_live_deployments: bool = False, user_executions: bool = True, logs:
-              ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs = None, **kwargs)
+              bool = True, time_to_live_deployments: bool = False, user_executions: bool = True, bulk_updates:
+              ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.AIAPICapabilitiesBulkUpdates = None, execution_schedules:
+              bool = False, logs: ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs = None, **kwargs)
               
              The AIAPICapabilities object represent the capabilities of the AI API
               
              :param multitenant: indicates whether resource groups are supported, defaults to True
              :type multitenant: bool, optional
              :param shareable: indicates whether clients can share an instance, defaults to True
              :type shareable: bool, optional
@@ -23,43 +24,49 @@
              :type static_deployments: bool, optional
              :param user_deployments: indicates whether deployment creation by users are supported, defaults to True
              :type user_deployments: bool, optional
              :param time_to_live_deployments: indicate whether ttl value of deployment are supported, defaults to False
              :type time_to_live_deployments: bool, optional
              :param user_executions: indicates whether execution creation by users are supported, defaults to True
              :type user_executions: bool, optional
+             :param bulk_updates: An object, defining the bulk updates capabilities, defaults to None
+             :type bulk_updates: class:`ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.AIAPICapabilitiesBulkUpdates`,
+              optional
+             :param execution_schedules: indicates whether execution schedules are supported, defaults to False
+             :type execution_schedules: bool, optional
              :param logs: An object, defining the logs capabilities, defaults to None
              :type logs: class:`ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs`, optional
-             :param `**kwargs`: The keyword arguments are there in case there are additional attributes returned from server
+   �     :param `**kwargs`: The keyword arguments are there in case there are additional attributes returned from server
               
-   �       Methods defined here:
+            Methods defined here:
                  __eq__(self, other)
-                  Return self==value.
+                     Return self==value.
                  __init__(self, multitenant: bool = True, shareable: bool = True, static_deployments: bool = True, user_deployments: bool =
-                 True, time_to_live_deployments: bool = False, user_executions: bool = True, logs:
-                 ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs = None, **kwargs)
+                 True, time_to_live_deployments: bool = False, user_executions: bool = True, bulk_updates:
+                 ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.AIAPICapabilitiesBulkUpdates = None, execution_schedules: bool =
+                 False, logs: ai_api_client_sdk.models.ai_api_capabilities_logs.AIAPICapabilitiesLogs = None, **kwargs)
                      Initialize self.  See help(type(self)) for accurate signature.
                  __str__(self)
                      Return str(self).
-               ===============================================================================================================================
+               ================================================================================================================================
                Static methods defined here:
                  from_dict(ai_api_capabilities_dict: Dict[str, Any])
                      Returns a :class:`ai_api_client_sdk.models.ai_api_capabilities.AIAPICapabilities` object, created from the
                     values in the dict provided as parameter
                       
                      :param ai_api_capabilities_dict: Dict which includes the necessary values to create the object
                      :type ai_api_capabilities_dict: Dict[str, Any]
                      :return: An object, created from the values provided
                      :rtype: class:`ai_api_client_sdk.models.ai_api_capabilities.AIAPICapabilities`
-               ===============================================================================================================================
+               ================================================================================================================================
                Data descriptors defined here:
                  __dict__
                      dictionary for instance variables (if defined)
                  __weakref__
                      list of weak references to the object (if defined)
-               ===============================================================================================================================
+               ================================================================================================================================
                Data and other attributes defined here:
                  __hash__ = None
  
 Data
    � Any = typing.Any
          Dict = typing.Dict
```

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_logs.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_logs.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_deployments.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_deployments.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_enactments.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_enactments.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_executions.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_executions.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_meta.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_meta.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.api_version.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.api_version.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact_create_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact_create_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.base_models.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.base_models.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.capabilities.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.capabilities.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration_create_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration_create_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.dataset_capabilities.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.dataset_capabilities.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.dataset_limits.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.dataset_limits.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_bulk_modify_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_bulk_modify_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_create_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_create_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.enactment.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.enactment.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.executable.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.executable.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.executable_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.executable_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution.html`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ffc8d8">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#000000" face="helvetica, arial"><a name="Execution">class <strong>Execution</strong></a>(<a href="ai_api_client_sdk.models.enactment.html#Enactment">ai_api_client_sdk.models.enactment.Enactment</a>)</font></td></tr>
     
 <tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
-<td colspan=2><tt><a href="#Execution">Execution</a>(id:&nbsp;str,&nbsp;configuration_id:&nbsp;str,&nbsp;configuration_name:&nbsp;str,&nbsp;scenario_id:&nbsp;str,&nbsp;status:&nbsp;ai_api_client_sdk.models.status.Status,&nbsp;target_status:&nbsp;ai_api_client_sdk.models.target_status.TargetStatus,&nbsp;created_at:&nbsp;datetime.datetime,&nbsp;modified_at:&nbsp;datetime.datetime,&nbsp;output_artifacts:&nbsp;List[ai_api_client_sdk.models.artifact.Artifact]&nbsp;=&nbsp;None,&nbsp;status_message:&nbsp;str&nbsp;=&nbsp;None,&nbsp;status_details:&nbsp;Dict[str,&nbsp;Any]&nbsp;=&nbsp;None,&nbsp;submission_time:&nbsp;datetime.datetime&nbsp;=&nbsp;None,&nbsp;start_time:&nbsp;datetime.datetime&nbsp;=&nbsp;None,&nbsp;completion_time:&nbsp;datetime.datetime&nbsp;=&nbsp;None,&nbsp;**kwargs)<br>
+<td colspan=2><tt><a href="#Execution">Execution</a>(id:&nbsp;str,&nbsp;configuration_id:&nbsp;str,&nbsp;configuration_name:&nbsp;str,&nbsp;scenario_id:&nbsp;str,&nbsp;status:&nbsp;ai_api_client_sdk.models.status.Status,&nbsp;target_status:&nbsp;ai_api_client_sdk.models.target_status.TargetStatus,&nbsp;created_at:&nbsp;datetime.datetime,&nbsp;modified_at:&nbsp;datetime.datetime,&nbsp;output_artifacts:&nbsp;List[ai_api_client_sdk.models.artifact.Artifact]&nbsp;=&nbsp;None,&nbsp;status_message:&nbsp;str&nbsp;=&nbsp;None,&nbsp;status_details:&nbsp;Dict[str,&nbsp;Any]&nbsp;=&nbsp;None,&nbsp;submission_time:&nbsp;datetime.datetime&nbsp;=&nbsp;None,&nbsp;start_time:&nbsp;datetime.datetime&nbsp;=&nbsp;None,&nbsp;execution_schedule_id:&nbsp;str&nbsp;=&nbsp;None,&nbsp;completion_time:&nbsp;datetime.datetime&nbsp;=&nbsp;None,&nbsp;**kwargs)<br>
 &nbsp;<br>
 The&nbsp;<a href="#Execution">Execution</a>&nbsp;object&nbsp;defines&nbsp;an&nbsp;execution<br>
 &nbsp;<br>
 :param&nbsp;id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;execution<br>
 :type&nbsp;id:&nbsp;str<br>
 :param&nbsp;configuration_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;configuration&nbsp;which&nbsp;configured&nbsp;the&nbsp;execution<br>
 :type&nbsp;configuration_id:&nbsp;str<br>
@@ -44,14 +44,16 @@
 :type&nbsp;configuration_name:&nbsp;str<br>
 :param&nbsp;scenario_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;scenario&nbsp;which&nbsp;the&nbsp;execution&nbsp;belongs&nbsp;to<br>
 :type&nbsp;scenario_id:&nbsp;str<br>
 :param&nbsp;status:&nbsp;Status&nbsp;of&nbsp;the&nbsp;execution<br>
 :type&nbsp;status:&nbsp;class:`ai_api_client_sdk.models.status.Status`<br>
 :param&nbsp;target_status:&nbsp;Target&nbsp;status&nbsp;of&nbsp;the&nbsp;execution<br>
 :type&nbsp;target_status:&nbsp;class:`ai_api_client_sdk.models.target_status.TargetStatus`<br>
+:param&nbsp;execution_schedule_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;execution&nbsp;schedule,&nbsp;defaults&nbsp;to&nbsp;None<br>
+:type&nbsp;execution_schedule_id:&nbsp;str,&nbsp;optional<br>
 :param&nbsp;created_at:&nbsp;Time&nbsp;when&nbsp;the&nbsp;execution&nbsp;was&nbsp;created<br>
 :type&nbsp;created_at:&nbsp;datetime<br>
 :param&nbsp;modified_at:&nbsp;Time&nbsp;when&nbsp;the&nbsp;execution&nbsp;was&nbsp;last&nbsp;modified<br>
 :type&nbsp;modified_at:&nbsp;datetime<br>
 :param&nbsp;output_artifacts:&nbsp;List&nbsp;of&nbsp;the&nbsp;artifacts&nbsp;created&nbsp;by&nbsp;the&nbsp;execution,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;output_artifacts:&nbsp;List[class:`ai_api_client_sdk.models.artifact.Artifact`],&nbsp;optional<br>
 :param&nbsp;status_message:&nbsp;Gives&nbsp;information&nbsp;about&nbsp;the&nbsp;status&nbsp;of&nbsp;the&nbsp;execution,&nbsp;defaults&nbsp;to&nbsp;None<br>
@@ -69,15 +71,15 @@
 <td width="100%"><dl><dt>Method resolution order:</dt>
 <dd><a href="ai_api_client_sdk.models.execution.html#Execution">Execution</a></dd>
 <dd><a href="ai_api_client_sdk.models.enactment.html#Enactment">ai_api_client_sdk.models.enactment.Enactment</a></dd>
 <dd><a href="builtins.html#object">builtins.object</a></dd>
 </dl>
 <hr>
 Methods defined here:<br>
-<dl><dt><a name="Execution-__init__"><strong>__init__</strong></a>(self, id: str, configuration_id: str, configuration_name: str, scenario_id: str, status: ai_api_client_sdk.models.status.Status, target_status: ai_api_client_sdk.models.target_status.TargetStatus, created_at: datetime.datetime, modified_at: datetime.datetime, output_artifacts: List[ai_api_client_sdk.models.artifact.Artifact] = None, status_message: str = None, status_details: Dict[str, Any] = None, submission_time: datetime.datetime = None, start_time: datetime.datetime = None, completion_time: datetime.datetime = None, **kwargs)</dt><dd><tt>Initialize&nbsp;self.&nbsp;&nbsp;See&nbsp;help(type(self))&nbsp;for&nbsp;accurate&nbsp;signature.</tt></dd></dl>
+<dl><dt><a name="Execution-__init__"><strong>__init__</strong></a>(self, id: str, configuration_id: str, configuration_name: str, scenario_id: str, status: ai_api_client_sdk.models.status.Status, target_status: ai_api_client_sdk.models.target_status.TargetStatus, created_at: datetime.datetime, modified_at: datetime.datetime, output_artifacts: List[ai_api_client_sdk.models.artifact.Artifact] = None, status_message: str = None, status_details: Dict[str, Any] = None, submission_time: datetime.datetime = None, start_time: datetime.datetime = None, execution_schedule_id: str = None, completion_time: datetime.datetime = None, **kwargs)</dt><dd><tt>Initialize&nbsp;self.&nbsp;&nbsp;See&nbsp;help(type(self))&nbsp;for&nbsp;accurate&nbsp;signature.</tt></dd></dl>
 
 <dl><dt><a name="Execution-__str__"><strong>__str__</strong></a>(self)</dt><dd><tt>Return&nbsp;str(self).</tt></dd></dl>
 
 <hr>
 Static methods defined here:<br>
 <dl><dt><a name="Execution-from_dict"><strong>from_dict</strong></a>(execution_dict: Dict[str, Any])</dt><dd><tt>Returns&nbsp;a&nbsp;:class:`ai_api_client_sdk.models.execution.<a href="#Execution">Execution</a>`&nbsp;object,&nbsp;created&nbsp;from&nbsp;the&nbsp;values&nbsp;in&nbsp;the&nbsp;dict<br>
 provided&nbsp;as&nbsp;parameter<br>
```

### html2text {}

```diff
@@ -8,16 +8,16 @@
                  Execution
           
          class Execution(ai_api_client_sdk.models.enactment.Enactment)
              Execution(id: str, configuration_id: str, configuration_name: str, scenario_id: str, status:
               ai_api_client_sdk.models.status.Status, target_status: ai_api_client_sdk.models.target_status.TargetStatus, created_at:
               datetime.datetime, modified_at: datetime.datetime, output_artifacts: List
              [ai_api_client_sdk.models.artifact.Artifact] = None, status_message: str = None, status_details: Dict
-             [str, Any] = None, submission_time: datetime.datetime = None, start_time: datetime.datetime = None, completion_time:
-              datetime.datetime = None, **kwargs)
+             [str, Any] = None, submission_time: datetime.datetime = None, start_time: datetime.datetime = None, execution_schedule_id:
+              str = None, completion_time: datetime.datetime = None, **kwargs)
               
              The Execution object defines an execution
               
              :param id: ID of the execution
              :type id: str
              :param configuration_id: ID of the configuration which configured the execution
              :type configuration_id: str
@@ -25,43 +25,46 @@
              :type configuration_name: str
              :param scenario_id: ID of the scenario which the execution belongs to
              :type scenario_id: str
              :param status: Status of the execution
              :type status: class:`ai_api_client_sdk.models.status.Status`
              :param target_status: Target status of the execution
              :type target_status: class:`ai_api_client_sdk.models.target_status.TargetStatus`
+             :param execution_schedule_id: ID of the execution schedule, defaults to None
+             :type execution_schedule_id: str, optional
              :param created_at: Time when the execution was created
              :type created_at: datetime
              :param modified_at: Time when the execution was last modified
              :type modified_at: datetime
              :param output_artifacts: List of the artifacts created by the execution, defaults to None
              :type output_artifacts: List[class:`ai_api_client_sdk.models.artifact.Artifact`], optional
              :param status_message: Gives information about the status of the execution, defaults to None
              :type status_message: str, optional
              :param status_details: A dict, which gives detailed information about the status of the execution, defaults to None
              :type status_details: Dict[str, Any], optional
-             :param submission_time: Time when the execution was submitted
-   �     :type submission_time: datetime, optional
-             :param start_time: Time when the execution status changed to RUNNING
-           :type start_time: datetime, optional
+   �     :param submission_time: Time when the execution was submitted
+             :type submission_time: datetime, optional
+           :param start_time: Time when the execution status changed to RUNNING
+             :type start_time: datetime, optional
              :param completion_time: Time when the execution status changed to COMPLETED/DEAD/STOPPED
              :type completion_time: datetime, optional
              :param `**kwargs`: The keyword arguments are there in case there are additional attributes returned from server
               
                  Method resolution order:
                      Execution
                      ai_api_client_sdk.models.enactment.Enactment
                      builtins.object
                ===========================================================================================================================
                Methods defined here:
                  __init__(self, id: str, configuration_id: str, configuration_name: str, scenario_id: str, status:
                  ai_api_client_sdk.models.status.Status, target_status: ai_api_client_sdk.models.target_status.TargetStatus, created_at:
                  datetime.datetime, modified_at: datetime.datetime, output_artifacts: List[ai_api_client_sdk.models.artifact.Artifact] =
                  None, status_message: str = None, status_details: Dict[str, Any] = None, submission_time: datetime.datetime = None,
-                 start_time: datetime.datetime = None, completion_time: datetime.datetime = None, **kwargs)
+                 start_time: datetime.datetime = None, execution_schedule_id: str = None, completion_time: datetime.datetime = None,
+                 **kwargs)
                      Initialize self.  See help(type(self)) for accurate signature.
                  __str__(self)
                      Return str(self).
               ===========================================================================================================================
                Static methods defined here:
                  from_dict(execution_dict: Dict[str, Any])
                      Returns a :class:`ai_api_client_sdk.models.execution.Execution` object, created from the values in the dict
```

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_bulk_modify_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_bulk_modify_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_create_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_create_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_analytics.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_analytics.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_dataset.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_dataset.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_resource_groups.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_resource_groups.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.healthz_status.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.healthz_status.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.html`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#aa55cc">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Package Contents</strong></big></font></td></tr>
     
 <tr><td bgcolor="#aa55cc"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%"><table width="100%" summary="list"><tr><td width="25%" valign=top><a href="ai_api_client_sdk.models.ai_api_capabilities.html">ai_api_capabilities</a><br>
+<a href="ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.html">ai_api_capabilities_bulk_updates</a><br>
 <a href="ai_api_client_sdk.models.ai_api_capabilities_logs.html">ai_api_capabilities_logs</a><br>
 <a href="ai_api_client_sdk.models.ai_api_limits.html">ai_api_limits</a><br>
 <a href="ai_api_client_sdk.models.ai_api_limits_deployments.html">ai_api_limits_deployments</a><br>
 <a href="ai_api_client_sdk.models.ai_api_limits_enactments.html">ai_api_limits_enactments</a><br>
 <a href="ai_api_client_sdk.models.ai_api_limits_executions.html">ai_api_limits_executions</a><br>
 <a href="ai_api_client_sdk.models.ai_api_meta.html">ai_api_meta</a><br>
 <a href="ai_api_client_sdk.models.api_version.html">api_version</a><br>
@@ -34,39 +35,45 @@
 <a href="ai_api_client_sdk.models.configuration_create_response.html">configuration_create_response</a><br>
 </td><td width="25%" valign=top><a href="ai_api_client_sdk.models.configuration_query_response.html">configuration_query_response</a><br>
 <a href="ai_api_client_sdk.models.dataset_capabilities.html">dataset_capabilities</a><br>
 <a href="ai_api_client_sdk.models.dataset_limits.html">dataset_limits</a><br>
 <a href="ai_api_client_sdk.models.deployment.html">deployment</a><br>
 <a href="ai_api_client_sdk.models.deployment_bulk_modify_response.html">deployment_bulk_modify_response</a><br>
 <a href="ai_api_client_sdk.models.deployment_create_response.html">deployment_create_response</a><br>
+<a href="ai_api_client_sdk.models.deployment_get_status_response.html">deployment_get_status_response</a><br>
 <a href="ai_api_client_sdk.models.deployment_query_response.html">deployment_query_response</a><br>
 <a href="ai_api_client_sdk.models.enactment.html">enactment</a><br>
+<a href="ai_api_client_sdk.models.enactment_get_status_response.html">enactment_get_status_response</a><br>
 <a href="ai_api_client_sdk.models.executable.html">executable</a><br>
 <a href="ai_api_client_sdk.models.executable_query_response.html">executable_query_response</a><br>
 <a href="ai_api_client_sdk.models.execution.html">execution</a><br>
 <a href="ai_api_client_sdk.models.execution_bulk_modify_response.html">execution_bulk_modify_response</a><br>
 <a href="ai_api_client_sdk.models.execution_create_response.html">execution_create_response</a><br>
-<a href="ai_api_client_sdk.models.execution_query_response.html">execution_query_response</a><br>
+<a href="ai_api_client_sdk.models.execution_get_status_response.html">execution_get_status_response</a><br>
+</td><td width="25%" valign=top><a href="ai_api_client_sdk.models.execution_query_response.html">execution_query_response</a><br>
+<a href="ai_api_client_sdk.models.execution_schedule.html">execution_schedule</a><br>
+<a href="ai_api_client_sdk.models.execution_schedule_create_response.html">execution_schedule_create_response</a><br>
+<a href="ai_api_client_sdk.models.execution_schedule_query_response.html">execution_schedule_query_response</a><br>
 <a href="ai_api_client_sdk.models.extensions.html">extensions</a><br>
-</td><td width="25%" valign=top><a href="ai_api_client_sdk.models.extensions_analytics.html">extensions_analytics</a><br>
+<a href="ai_api_client_sdk.models.extensions_analytics.html">extensions_analytics</a><br>
 <a href="ai_api_client_sdk.models.extensions_dataset.html">extensions_dataset</a><br>
 <a href="ai_api_client_sdk.models.extensions_resource_groups.html">extensions_resource_groups</a><br>
 <a href="ai_api_client_sdk.models.healthz_status.html">healthz_status</a><br>
 <a href="ai_api_client_sdk.models.input_artifact.html">input_artifact</a><br>
 <a href="ai_api_client_sdk.models.input_artifact_binding.html">input_artifact_binding</a><br>
 <a href="ai_api_client_sdk.models.label.html">label</a><br>
 <a href="ai_api_client_sdk.models.log_response.html">log_response</a><br>
 <a href="ai_api_client_sdk.models.metric.html">metric</a><br>
 <a href="ai_api_client_sdk.models.metric_custom_info.html">metric_custom_info</a><br>
 <a href="ai_api_client_sdk.models.metric_label.html">metric_label</a><br>
-<a href="ai_api_client_sdk.models.metric_resource.html">metric_resource</a><br>
+</td><td width="25%" valign=top><a href="ai_api_client_sdk.models.metric_resource.html">metric_resource</a><br>
 <a href="ai_api_client_sdk.models.metric_tag.html">metric_tag</a><br>
 <a href="ai_api_client_sdk.models.metrics_query_response.html">metrics_query_response</a><br>
 <a href="ai_api_client_sdk.models.output_artifact.html">output_artifact</a><br>
-</td><td width="25%" valign=top><a href="ai_api_client_sdk.models.parameter.html">parameter</a><br>
+<a href="ai_api_client_sdk.models.parameter.html">parameter</a><br>
 <a href="ai_api_client_sdk.models.parameter_binding.html">parameter_binding</a><br>
 <a href="ai_api_client_sdk.models.resource_group.html">resource_group</a><br>
 <a href="ai_api_client_sdk.models.resource_group_query_response.html">resource_group_query_response</a><br>
 <a href="ai_api_client_sdk.models.resource_group_status.html">resource_group_status</a><br>
 <a href="ai_api_client_sdk.models.scenario.html">scenario</a><br>
 <a href="ai_api_client_sdk.models.scenario_query_response.html">scenario_query_response</a><br>
 <a href="ai_api_client_sdk.models.status.html">status</a><br>
```

### html2text {}

```diff
@@ -1,20 +1,21 @@
                                                                        index
                         /home/jenkins/agent/workspace/ndation_ai-api-client-
 ai_api_client_sdk.models      sdk_master/ai_api_client_sdk/models/__init__.py
  
 Package Contents
-         ai_api_capabilities           configuration_query_response    extensions_analytics       parameter
-         ai_api_capabilities_logs      dataset_capabilities            extensions_dataset         parameter_binding
-         ai_api_limits                 dataset_limits                  extensions_resource_groups resource_group
-         ai_api_limits_deployments     deployment                      healthz_status             resource_group_query_response
-         ai_api_limits_enactments      deployment_bulk_modify_response input_artifact             resource_group_status
-         ai_api_limits_executions      deployment_create_response      input_artifact_binding     scenario
-         ai_api_meta                   deployment_query_response       label                      scenario_query_response
-   � api_version                   enactment                       log_response               status
-         artifact                      executable                      metric                     target_status
-         artifact_create_response      executable_query_response       metric_custom_info         version
-         artifact_query_response       execution                       metric_label               version_list
-         base_models                   execution_bulk_modify_response  metric_resource            version_query_response
-         capabilities                  execution_create_response       metric_tag
-         configuration                 execution_query_response        metrics_query_response
-         configuration_create_response extensions                      output_artifact
+         ai_api_capabilities              configuration_query_response    execution_query_response           metric_resource
+         ai_api_capabilities_bulk_updates dataset_capabilities            execution_schedule                 metric_tag
+         ai_api_capabilities_logs         dataset_limits                  execution_schedule_create_response metrics_query_response
+         ai_api_limits                    deployment                      execution_schedule_query_response  output_artifact
+         ai_api_limits_deployments        deployment_bulk_modify_response extensions                         parameter
+         ai_api_limits_enactments         deployment_create_response      extensions_analytics               parameter_binding
+         ai_api_limits_executions         deployment_get_status_response  extensions_dataset                 resource_group
+   � ai_api_meta                      deployment_query_response       extensions_resource_groups         resource_group_query_response
+         api_version                      enactment                       healthz_status                     resource_group_status
+         artifact                         enactment_get_status_response   input_artifact                     scenario
+         artifact_create_response         executable                      input_artifact_binding             scenario_query_response
+         artifact_query_response          executable_query_response       label                              status
+         base_models                      execution                       log_response                       target_status
+         capabilities                     execution_bulk_modify_response  metric                             version
+         configuration                    execution_create_response       metric_custom_info                 version_list
+         configuration_create_response    execution_get_status_response   metric_label                       version_query_response
```

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.input_artifact.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.input_artifact.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.input_artifact_binding.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.input_artifact_binding.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.label.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.label.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.log_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.log_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_custom_info.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_custom_info.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_label.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_label.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_resource.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_resource.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_tag.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_tag.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metrics_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metrics_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.output_artifact.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.output_artifact.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.parameter.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.parameter.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.parameter_binding.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.parameter_binding.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group_status.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group_status.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.scenario.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.scenario.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.scenario_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.scenario_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.status.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.status.html`

 * *Files 18% similar despite different names*

```diff
@@ -17,22 +17,61 @@
 <font color="#ffffff" face="helvetica, arial"><big><strong>Classes</strong></big></font></td></tr>
     
 <tr><td bgcolor="#ee77aa"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%"><dl>
 <dt><font face="helvetica, arial"><a href="enum.html#Enum">enum.Enum</a>(<a href="builtins.html#object">builtins.object</a>)
 </font></dt><dd>
 <dl>
-<dt><font face="helvetica, arial"><a href="ai_api_client_sdk.models.status.html#Status">Status</a>
+<dt><font face="helvetica, arial"><a href="ai_api_client_sdk.models.status.html#ScheduleStatus">ScheduleStatus</a>
+</font></dt><dt><font face="helvetica, arial"><a href="ai_api_client_sdk.models.status.html#Status">Status</a>
 </font></dt></dl>
 </dd>
 </dl>
  <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ffc8d8">
 <td colspan=3 valign=bottom>&nbsp;<br>
+<font color="#000000" face="helvetica, arial"><a name="ScheduleStatus">class <strong>ScheduleStatus</strong></a>(<a href="enum.html#Enum">enum.Enum</a>)</font></td></tr>
+    
+<tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
+<td colspan=2><tt><a href="#ScheduleStatus">ScheduleStatus</a>(value,&nbsp;names=None,&nbsp;*,&nbsp;module=None,&nbsp;qualname=None,&nbsp;type=None,&nbsp;start=1)<br>
+&nbsp;<br>
+<a href="enum.html#Enum">Enum</a>&nbsp;defining&nbsp;the&nbsp;status&nbsp;values&nbsp;for&nbsp;execution&nbsp;schedules<br>&nbsp;</tt></td></tr>
+<tr><td>&nbsp;</td>
+<td width="100%"><dl><dt>Method resolution order:</dt>
+<dd><a href="ai_api_client_sdk.models.status.html#ScheduleStatus">ScheduleStatus</a></dd>
+<dd><a href="enum.html#Enum">enum.Enum</a></dd>
+<dd><a href="builtins.html#object">builtins.object</a></dd>
+</dl>
+<hr>
+Data and other attributes defined here:<br>
+<dl><dt><strong>ACTIVE</strong> = &lt;ScheduleStatus.ACTIVE: 'ACTIVE'&gt;</dl>
+
+<dl><dt><strong>INACTIVE</strong> = &lt;ScheduleStatus.INACTIVE: 'INACTIVE'&gt;</dl>
+
+<hr>
+Data descriptors inherited from <a href="enum.html#Enum">enum.Enum</a>:<br>
+<dl><dt><strong>name</strong></dt>
+<dd><tt>The&nbsp;name&nbsp;of&nbsp;the&nbsp;Enum&nbsp;member.</tt></dd>
+</dl>
+<dl><dt><strong>value</strong></dt>
+<dd><tt>The&nbsp;value&nbsp;of&nbsp;the&nbsp;Enum&nbsp;member.</tt></dd>
+</dl>
+<hr>
+Readonly properties inherited from <a href="enum.html#EnumMeta">enum.EnumMeta</a>:<br>
+<dl><dt><strong>__members__</strong></dt>
+<dd><tt>Returns&nbsp;a&nbsp;mapping&nbsp;of&nbsp;member&nbsp;name-&gt;value.<br>
+&nbsp;<br>
+This&nbsp;mapping&nbsp;lists&nbsp;all&nbsp;enum&nbsp;members,&nbsp;including&nbsp;aliases.&nbsp;Note&nbsp;that&nbsp;this<br>
+is&nbsp;a&nbsp;read-only&nbsp;view&nbsp;of&nbsp;the&nbsp;internal&nbsp;mapping.</tt></dd>
+</dl>
+</td></tr></table> <p>
+<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
+<tr bgcolor="#ffc8d8">
+<td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#000000" face="helvetica, arial"><a name="Status">class <strong>Status</strong></a>(<a href="enum.html#Enum">enum.Enum</a>)</font></td></tr>
     
 <tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
 <td colspan=2><tt><a href="#Status">Status</a>(value,&nbsp;names=None,&nbsp;*,&nbsp;module=None,&nbsp;qualname=None,&nbsp;type=None,&nbsp;start=1)<br>
 &nbsp;<br>
 <a href="#Status">Status</a>&nbsp;is&nbsp;an&nbsp;<a href="enum.html#Enum">Enum</a>&nbsp;defining&nbsp;the&nbsp;valid&nbsp;values&nbsp;of&nbsp;the&nbsp;status&nbsp;of&nbsp;an&nbsp;execution/deployment<br>&nbsp;</tt></td></tr>
 <tr><td>&nbsp;</td>
```

### html2text {}

```diff
@@ -1,30 +1,58 @@
                                                                         index
                                /home/jenkins/agent/workspace/ndation_ai-api-
                                  client-sdk_master/ai_api_client_sdk/models/
 ai_api_client_sdk.models.status                                     status.py
  
 Classes
            enum.Enum(builtins.object)
+                 ScheduleStatus
                  Status
           
+         class ScheduleStatus(enum.Enum)
+             ScheduleStatus(value, names=None, *, module=None, qualname=None, type=None, start=1)
+              
+             Enum defining the status values for execution schedules
+              
+                 Method resolution order:
+                     ScheduleStatus
+                     enum.Enum
+                     builtins.object
+               ===============================================================================================
+               Data and other attributes defined here:
+                 ACTIVE = <ScheduleStatus.ACTIVE: 'ACTIVE'>
+                 INACTIVE = <ScheduleStatus.INACTIVE: 'INACTIVE'>
+            ===============================================================================================
+               Data descriptors inherited from enum.Enum:
+                name
+                     The name of the Enum member.
+                 value
+                     The value of the Enum member.
+               ===============================================================================================
+               Readonly properties inherited from enum.EnumMeta:
+                 __members__
+                     Returns a mapping of member name->value.
+                      
+                     This mapping lists all enum members, including aliases. Note that this
+                     is a read-only view of the internal mapping.
+   �  
          class Status(enum.Enum)
              Status(value, names=None, *, module=None, qualname=None, type=None, start=1)
               
              Status is an Enum defining the valid values of the status of an execution/deployment
               
                  Method resolution order:
                      Status
                      enum.Enum
                      builtins.object
                ===============================================================================================
                Data and other attributes defined here:
                  COMPLETED = <Status.COMPLETED: 'COMPLETED'>
                  DEAD = <Status.DEAD: 'DEAD'>
-   �         PENDING = <Status.PENDING: 'PENDING'>
+                 PENDING = <Status.PENDING: 'PENDING'>
                  RUNNING = <Status.RUNNING: 'RUNNING'>
               STOPPED = <Status.STOPPED: 'STOPPED'>
                  STOPPING = <Status.STOPPING: 'STOPPING'>
                 UNKNOWN = <Status.UNKNOWN: 'UNKNOWN'>
                ===============================================================================================
                Data descriptors inherited from enum.Enum:
                  name
```

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.target_status.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.target_status.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version_list.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version_list.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version_query_response.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version_query_response.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.artifact_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.artifact_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.base_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.base_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.configuration_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.configuration_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.deployment_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.deployment_client.html`

 * *Files 2% similar despite different names*

```diff
@@ -138,34 +138,37 @@
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIServerException`&nbsp;if&nbsp;a&nbsp;non-2XX&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIRequestException`&nbsp;if&nbsp;an&nbsp;unexpected&nbsp;exception&nbsp;occurs&nbsp;while<br>
 &nbsp;&nbsp;&nbsp;&nbsp;trying&nbsp;to&nbsp;send&nbsp;a&nbsp;request&nbsp;to&nbsp;the&nbsp;server<br>
 :return:&nbsp;An&nbsp;object&nbsp;representing&nbsp;the&nbsp;response&nbsp;from&nbsp;the&nbsp;server<br>
 :rtype:&nbsp;class:`ai_api_client_sdk.models.base_models.BasicResponse`</tt></dd></dl>
 
-<dl><dt><a name="DeploymentClient-get"><strong>get</strong></a>(self, deployment_id: str, resource_group: str = None) -&gt; ai_api_client_sdk.models.deployment.Deployment</dt><dd><tt>Retrieves&nbsp;the&nbsp;deployment&nbsp;from&nbsp;the&nbsp;server.<br>
+<dl><dt><a name="DeploymentClient-get"><strong>get</strong></a>(self, deployment_id: str, resource_group: str = None, select: str = None) -&gt; Union[ai_api_client_sdk.models.deployment.Deployment, ai_api_client_sdk.models.deployment_get_status_response.DeploymentGetStatusResponse]</dt><dd><tt>Retrieves&nbsp;the&nbsp;deployment&nbsp;from&nbsp;the&nbsp;server.<br>
 &nbsp;<br>
 :param&nbsp;deployment_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;deployment&nbsp;to&nbsp;be&nbsp;retrieved<br>
 :type&nbsp;deployment_id:&nbsp;str<br>
 :param&nbsp;resource_group:&nbsp;Resource&nbsp;Group&nbsp;which&nbsp;the&nbsp;request&nbsp;should&nbsp;be&nbsp;sent&nbsp;on&nbsp;behalf.&nbsp;Either&nbsp;this&nbsp;or&nbsp;a&nbsp;default<br>
 &nbsp;&nbsp;&nbsp;&nbsp;resource&nbsp;group&nbsp;in&nbsp;the&nbsp;:class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client`&nbsp;should&nbsp;be&nbsp;specified,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;resource_group:&nbsp;str<br>
+:param&nbsp;select:&nbsp;only&nbsp;status&nbsp;supported.&nbsp;Get&nbsp;deployment&nbsp;for&nbsp;a&nbsp;given&nbsp;deployment&nbsp;id&nbsp;and&nbsp;select&nbsp;status<br>
+:type&nbsp;select:&nbsp;str,&nbsp;optional<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException`&nbsp;if&nbsp;a&nbsp;400&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIAuthorizationException`&nbsp;if&nbsp;a&nbsp;401&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPINotFoundException`&nbsp;if&nbsp;a&nbsp;404&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIServerException`&nbsp;if&nbsp;a&nbsp;non-2XX&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIRequestException`&nbsp;if&nbsp;an&nbsp;unexpected&nbsp;exception&nbsp;occurs&nbsp;while<br>
 &nbsp;&nbsp;&nbsp;&nbsp;trying&nbsp;to&nbsp;send&nbsp;a&nbsp;request&nbsp;to&nbsp;the&nbsp;server<br>
 :return:&nbsp;The&nbsp;retrieved&nbsp;deployment<br>
-:rtype:&nbsp;class:`ai_api_client_sdk.models.deployment.Deployment`</tt></dd></dl>
+:rtype:&nbsp;class:Union[`ai_api_client_sdk.models.deployment.Deployment`,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;`ai_api_client_sdk.models.deployment_get_status_response.DeploymentGetStatusResponse`]</tt></dd></dl>
 
 <dl><dt><a name="DeploymentClient-modify"><strong>modify</strong></a>(self, deployment_id: str, target_status: ai_api_client_sdk.models.target_status.TargetStatus = None, configuration_id: str = None, resource_group: str = None) -&gt; ai_api_client_sdk.models.base_models.BasicResponse</dt><dd><tt>Modifies&nbsp;the&nbsp;deployment,&nbsp;by&nbsp;changing&nbsp;either&nbsp;the&nbsp;target&nbsp;status,&nbsp;or&nbsp;the&nbsp;configuration&nbsp;ID.<br>
 &nbsp;<br>
 :param&nbsp;deployment_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;deployment&nbsp;to&nbsp;be&nbsp;modified<br>
 :type&nbsp;deployment_id:&nbsp;str<br>
 :param&nbsp;target_status:&nbsp;Desired&nbsp;target&nbsp;status&nbsp;of&nbsp;the&nbsp;deployment,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;target_status:&nbsp;class:`ai_api_client_sdk.models.target_status.TargetStatus`,&nbsp;optional<br>
@@ -261,9 +264,10 @@
 </td></tr></table></td></tr></table><p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#55aa55">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Data</strong></big></font></td></tr>
     
 <tr><td bgcolor="#55aa55"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
-<td width="100%"><strong>List</strong> = typing.List</td></tr></table>
+<td width="100%"><strong>List</strong> = typing.List<br>
+<strong>Union</strong> = typing.Union</td></tr></table>
 </body></html>
```

### html2text {}

```diff
@@ -114,35 +114,40 @@
                          the server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIServerException` if a non-2XX response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
                          trying to send a request to the server
                      :return: An object representing the response from the server
                      :rtype: class:`ai_api_client_sdk.models.base_models.BasicResponse`
-                 get(self, deployment_id: str, resource_group: str = None) -> ai_api_client_sdk.models.deployment.Deployment
+                 get(self, deployment_id: str, resource_group: str = None, select: str = None) -> Union
+                 [ai_api_client_sdk.models.deployment.Deployment,
+                 ai_api_client_sdk.models.deployment_get_status_response.DeploymentGetStatusResponse]
                      Retrieves the deployment from the server.
                       
                      :param deployment_id: ID of the deployment to be retrieved
                      :type deployment_id: str
    �             :param resource_group: Resource Group which the request should be sent on behalf. Either this or a default
                          resource group in the :class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client` should be specified,
                       defaults to None
                      :type resource_group: str
-                    :raises: class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException` if a 400 response is received from the
+                     :param select: only status supported. Get deployment for a given deployment id and select status
+                    :type select: str, optional
+                     :raises: class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException` if a 400 response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIAuthorizationException` if a 401 response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPINotFoundException` if a 404 response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIServerException` if a non-2XX response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
                          trying to send a request to the server
                      :return: The retrieved deployment
-                     :rtype: class:`ai_api_client_sdk.models.deployment.Deployment`
+                     :rtype: class:Union[`ai_api_client_sdk.models.deployment.Deployment`,
+                         `ai_api_client_sdk.models.deployment_get_status_response.DeploymentGetStatusResponse`]
                  modify(self, deployment_id: str, target_status: ai_api_client_sdk.models.target_status.TargetStatus = None, configuration_id: str
                  = None, resource_group: str = None) -> ai_api_client_sdk.models.base_models.BasicResponse
                      Modifies the deployment, by changing either the target status, or the configuration ID.
                       
                      :param deployment_id: ID of the deployment to be modified
                      :type deployment_id: str
                      :param target_status: Desired target status of the deployment, defaults to None
@@ -236,7 +241,8 @@
                  __dict__
                      dictionary for instance variables (if defined)
                  __weakref__
                      list of weak references to the object (if defined)
  
 Data
    � List = typing.List
+         Union = typing.Union
```

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.executable_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.executable_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.execution_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.execution_client.html`

 * *Files 2% similar despite different names*

```diff
@@ -60,22 +60,24 @@
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIPreconditionFailedException`&nbsp;if&nbsp;a&nbsp;412&nbsp;response&nbsp;is&nbsp;received&nbsp;from<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIRequestException`&nbsp;if&nbsp;an&nbsp;unexpected&nbsp;exception&nbsp;occurs&nbsp;while<br>
 &nbsp;&nbsp;&nbsp;&nbsp;trying&nbsp;to&nbsp;send&nbsp;a&nbsp;request&nbsp;to&nbsp;the&nbsp;server<br>
 :return:&nbsp;An&nbsp;object&nbsp;representing&nbsp;the&nbsp;response&nbsp;from&nbsp;the&nbsp;server<br>
 :rtype:&nbsp;class:`ai_api_client_sdk.models.execution_bulk_modify_response.ExecutionBulkModifyResponse`</tt></dd></dl>
 
-<dl><dt><a name="ExecutionClient-count"><strong>count</strong></a>(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None, status: ai_api_client_sdk.models.status.Status = None, resource_group: str = None) -&gt; int</dt><dd><tt>Counts&nbsp;the&nbsp;number&nbsp;of&nbsp;executions.<br>
+<dl><dt><a name="ExecutionClient-count"><strong>count</strong></a>(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None, execution_schedule_id: str = None, status: ai_api_client_sdk.models.status.Status = None, resource_group: str = None) -&gt; int</dt><dd><tt>Counts&nbsp;the&nbsp;number&nbsp;of&nbsp;executions.<br>
 &nbsp;<br>
 :param&nbsp;scenario_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;scenario,&nbsp;the&nbsp;executions&nbsp;should&nbsp;belong&nbsp;to,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;scenario_id:&nbsp;str,&nbsp;optional<br>
 :param&nbsp;configuration_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;configuration,&nbsp;the&nbsp;executions&nbsp;should&nbsp;be&nbsp;configured&nbsp;by,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;configuration_id:&nbsp;str,&nbsp;optional<br>
 :param&nbsp;executable_ids:&nbsp;IDs&nbsp;of&nbsp;the&nbsp;executables,&nbsp;the&nbsp;executions&nbsp;should&nbsp;be&nbsp;created&nbsp;from,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;executable_ids:&nbsp;List[str],&nbsp;optional<br>
+:param&nbsp;execution_schedule_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;execution&nbsp;schedule,&nbsp;defaults&nbsp;to&nbsp;None<br>
+:type&nbsp;execution_schedule_id:&nbsp;str,&nbsp;optional<br>
 :param&nbsp;status:&nbsp;Status&nbsp;which&nbsp;the&nbsp;executions&nbsp;should&nbsp;currently&nbsp;have<br>
 :type&nbsp;status:&nbsp;class:`ai_api_client_sdk.models.status.Status`,&nbsp;optional<br>
 :param&nbsp;resource_group:&nbsp;Resource&nbsp;group&nbsp;which&nbsp;the&nbsp;request&nbsp;should&nbsp;be&nbsp;sent&nbsp;on&nbsp;behalf.&nbsp;Either&nbsp;this&nbsp;or&nbsp;a&nbsp;default<br>
 &nbsp;&nbsp;&nbsp;&nbsp;resource&nbsp;group&nbsp;in&nbsp;the&nbsp;:class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client`&nbsp;should&nbsp;be&nbsp;specified,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;resource_group:&nbsp;str<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException`&nbsp;if&nbsp;a&nbsp;400&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
@@ -127,34 +129,37 @@
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIServerException`&nbsp;if&nbsp;a&nbsp;non-2XX&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIRequestException`&nbsp;if&nbsp;an&nbsp;unexpected&nbsp;exception&nbsp;occurs&nbsp;while<br>
 &nbsp;&nbsp;&nbsp;&nbsp;trying&nbsp;to&nbsp;send&nbsp;a&nbsp;request&nbsp;to&nbsp;the&nbsp;server<br>
 :return:&nbsp;An&nbsp;object&nbsp;representing&nbsp;the&nbsp;response&nbsp;from&nbsp;the&nbsp;server<br>
 :rtype:&nbsp;class:`ai_api_client_sdk.models.base_models.BasicResponse`</tt></dd></dl>
 
-<dl><dt><a name="ExecutionClient-get"><strong>get</strong></a>(self, execution_id: str, resource_group: str = None) -&gt; ai_api_client_sdk.models.execution.Execution</dt><dd><tt>Retrieves&nbsp;the&nbsp;execution&nbsp;from&nbsp;the&nbsp;server.<br>
+<dl><dt><a name="ExecutionClient-get"><strong>get</strong></a>(self, execution_id: str, resource_group: str = None, select: str = None) -&gt; Union[ai_api_client_sdk.models.execution.Execution, ai_api_client_sdk.models.execution_get_status_response.ExecutionGetStatusResponse]</dt><dd><tt>Retrieves&nbsp;the&nbsp;execution&nbsp;from&nbsp;the&nbsp;server.<br>
 &nbsp;<br>
 :param&nbsp;execution_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;execution&nbsp;to&nbsp;be&nbsp;retrieved<br>
 :type&nbsp;execution_id:&nbsp;str<br>
 :param&nbsp;resource_group:&nbsp;Resource&nbsp;Group&nbsp;which&nbsp;the&nbsp;request&nbsp;should&nbsp;be&nbsp;sent&nbsp;on&nbsp;behalf.&nbsp;Either&nbsp;this&nbsp;or&nbsp;a&nbsp;default<br>
 &nbsp;&nbsp;&nbsp;&nbsp;resource&nbsp;group&nbsp;in&nbsp;the&nbsp;:class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client`&nbsp;should&nbsp;be&nbsp;specified,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;resource_group:&nbsp;str<br>
+:param&nbsp;select:&nbsp;only&nbsp;status&nbsp;supported.&nbsp;Get&nbsp;execution&nbsp;for&nbsp;a&nbsp;given&nbsp;execution&nbsp;id&nbsp;and&nbsp;select&nbsp;status<br>
+:type&nbsp;select:&nbsp;str,&nbsp;optional<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException`&nbsp;if&nbsp;a&nbsp;400&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIAuthorizationException`&nbsp;if&nbsp;a&nbsp;401&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPINotFoundException`&nbsp;if&nbsp;a&nbsp;404&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIServerException`&nbsp;if&nbsp;a&nbsp;non-2XX&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIRequestException`&nbsp;if&nbsp;an&nbsp;unexpected&nbsp;exception&nbsp;occurs&nbsp;while<br>
 &nbsp;&nbsp;&nbsp;&nbsp;trying&nbsp;to&nbsp;send&nbsp;a&nbsp;request&nbsp;to&nbsp;the&nbsp;server<br>
 :return:&nbsp;The&nbsp;retrieved&nbsp;execution<br>
-:rtype:&nbsp;class:`ai_api_client_sdk.models.execution.Execution`</tt></dd></dl>
+:rtype:&nbsp;class:Union[`ai_api_client_sdk.models.execution.Execution`,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;`ai_api_client_sdk.models.execution_get_status_response.ExecutionGetStatusResponse`]</tt></dd></dl>
 
 <dl><dt><a name="ExecutionClient-modify"><strong>modify</strong></a>(self, execution_id: str, target_status: ai_api_client_sdk.models.target_status.TargetStatus, resource_group: str = None) -&gt; ai_api_client_sdk.models.base_models.BasicResponse</dt><dd><tt>Modifies&nbsp;the&nbsp;execution,&nbsp;by&nbsp;changing&nbsp;the&nbsp;target&nbsp;status.<br>
 &nbsp;<br>
 :param&nbsp;execution_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;execution&nbsp;to&nbsp;be&nbsp;modified<br>
 :type&nbsp;execution_id:&nbsp;str<br>
 :param&nbsp;target_status:&nbsp;Desired&nbsp;target&nbsp;status&nbsp;of&nbsp;the&nbsp;execution,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;target_status:&nbsp;class:`ai_api_client_sdk.models.target_status.TargetStatus`,&nbsp;optional<br>
@@ -173,22 +178,24 @@
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIServerException`&nbsp;if&nbsp;a&nbsp;non-2XX&nbsp;response&nbsp;is&nbsp;received&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;server<br>
 :raises:&nbsp;class:`ai_api_client_sdk.exception.AIAPIRequestException`&nbsp;if&nbsp;an&nbsp;unexpected&nbsp;exception&nbsp;occurs&nbsp;while<br>
 &nbsp;&nbsp;&nbsp;&nbsp;trying&nbsp;to&nbsp;send&nbsp;a&nbsp;request&nbsp;to&nbsp;the&nbsp;server<br>
 :return:&nbsp;An&nbsp;object&nbsp;representing&nbsp;the&nbsp;response&nbsp;from&nbsp;the&nbsp;server<br>
 :rtype:&nbsp;class:`ai_api_client_sdk.models.base_models.BasicResponse`</tt></dd></dl>
 
-<dl><dt><a name="ExecutionClient-query"><strong>query</strong></a>(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None, status: ai_api_client_sdk.models.status.Status = None, top: int = None, skip: int = None, resource_group: str = None) -&gt; ai_api_client_sdk.models.execution_query_response.ExecutionQueryResponse</dt><dd><tt>Queries&nbsp;the&nbsp;executions.<br>
+<dl><dt><a name="ExecutionClient-query"><strong>query</strong></a>(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None, execution_schedule_id: str = None, status: ai_api_client_sdk.models.status.Status = None, top: int = None, skip: int = None, resource_group: str = None) -&gt; ai_api_client_sdk.models.execution_query_response.ExecutionQueryResponse</dt><dd><tt>Queries&nbsp;the&nbsp;executions.<br>
 &nbsp;<br>
 :param&nbsp;scenario_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;scenario&nbsp;the&nbsp;executions&nbsp;should&nbsp;belong&nbsp;to,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;scenario_id:&nbsp;str,&nbsp;optional<br>
 :param&nbsp;configuration_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;configuration,&nbsp;the&nbsp;executions&nbsp;should&nbsp;be&nbsp;configured&nbsp;by,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;configuration_id:&nbsp;str,&nbsp;optional<br>
 :param&nbsp;executable_ids:&nbsp;IDs&nbsp;of&nbsp;the&nbsp;executables&nbsp;the&nbsp;executions&nbsp;should&nbsp;be&nbsp;created&nbsp;from,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;executable_ids:&nbsp;List[str],&nbsp;optional<br>
+:param&nbsp;execution_schedule_id:&nbsp;ID&nbsp;of&nbsp;the&nbsp;execution&nbsp;schedule,&nbsp;defaults&nbsp;to&nbsp;None<br>
+:type&nbsp;execution_schedule_id:&nbsp;str,&nbsp;optional<br>
 :param&nbsp;status:&nbsp;Status&nbsp;which&nbsp;the&nbsp;executions&nbsp;should&nbsp;currently&nbsp;have<br>
 :type&nbsp;status:&nbsp;class:`ai_api_client_sdk.models.status.Status`,&nbsp;optional<br>
 :param&nbsp;top:&nbsp;Number&nbsp;of&nbsp;executions&nbsp;to&nbsp;be&nbsp;retrieved,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;top:&nbsp;int,&nbsp;optional<br>
 :param&nbsp;skip:&nbsp;Number&nbsp;of&nbsp;executions&nbsp;to&nbsp;be&nbsp;skipped,&nbsp;from&nbsp;the&nbsp;list&nbsp;of&nbsp;the&nbsp;queried&nbsp;executions,&nbsp;defaults&nbsp;to&nbsp;None<br>
 :type&nbsp;skip:&nbsp;int,&nbsp;optional<br>
 :param&nbsp;resource_group:&nbsp;Resource&nbsp;Group&nbsp;which&nbsp;the&nbsp;request&nbsp;should&nbsp;be&nbsp;sent&nbsp;on&nbsp;behalf.&nbsp;Either&nbsp;this&nbsp;or&nbsp;a&nbsp;default<br>
@@ -250,9 +257,10 @@
 </td></tr></table></td></tr></table><p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#55aa55">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Data</strong></big></font></td></tr>
     
 <tr><td bgcolor="#55aa55"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
-<td width="100%"><strong>List</strong> = typing.List</td></tr></table>
+<td width="100%"><strong>List</strong> = typing.List<br>
+<strong>Union</strong> = typing.Union</td></tr></table>
 </body></html>
```

### html2text {}

```diff
@@ -39,24 +39,26 @@
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIPreconditionFailedException` if a 412 response is received from
                          the server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
                          trying to send a request to the server
                      :return: An object representing the response from the server
                      :rtype: class:`ai_api_client_sdk.models.execution_bulk_modify_response.ExecutionBulkModifyResponse`
-                 count(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None, status:
-                 ai_api_client_sdk.models.status.Status = None, resource_group: str = None) -> int
+                 count(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None, execution_schedule_id: str
+                 = None, status: ai_api_client_sdk.models.status.Status = None, resource_group: str = None) -> int
                      Counts the number of executions.
                       
                      :param scenario_id: ID of the scenario, the executions should belong to, defaults to None
                      :type scenario_id: str, optional
                      :param configuration_id: ID of the configuration, the executions should be configured by, defaults to None
                      :type configuration_id: str, optional
                      :param executable_ids: IDs of the executables, the executions should be created from, defaults to None
                      :type executable_ids: List[str], optional
+                     :param execution_schedule_id: ID of the execution schedule, defaults to None
+                     :type execution_schedule_id: str, optional
                      :param status: Status which the executions should currently have
                      :type status: class:`ai_api_client_sdk.models.status.Status`, optional
                      :param resource_group: Resource group which the request should be sent on behalf. Either this or a default
                          resource group in the :class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client` should be specified,
                          defaults to None
                      :type resource_group: str
                      :raises: class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException` if a 400 response is received from the
@@ -108,35 +110,40 @@
                          the server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIServerException` if a non-2XX response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
                          trying to send a request to the server
                      :return: An object representing the response from the server
                      :rtype: class:`ai_api_client_sdk.models.base_models.BasicResponse`
-                 get(self, execution_id: str, resource_group: str = None) -> ai_api_client_sdk.models.execution.Execution
+                 get(self, execution_id: str, resource_group: str = None, select: str = None) -> Union
+                 [ai_api_client_sdk.models.execution.Execution,
+                 ai_api_client_sdk.models.execution_get_status_response.ExecutionGetStatusResponse]
                      Retrieves the execution from the server.
                       
                      :param execution_id: ID of the execution to be retrieved
                      :type execution_id: str
                      :param resource_group: Resource Group which the request should be sent on behalf. Either this or a default
-   �                 resource group in the :class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client` should be specified,
-                         defaults to None
-                  :type resource_group: str
-                     :raises: class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException` if a 400 response is received from the
+                         resource group in the :class:`ai_api_client_sdk.ai_api_v2_client.AIAPIV2Client` should be specified,
+   �                 defaults to None
+                     :type resource_group: str
+                  :param select: only status supported. Get execution for a given execution id and select status
+                     :type select: str, optional
+                    :raises: class:`ai_api_client_sdk.exception.AIAPIInvalidRequestException` if a 400 response is received from the
                          server
-                    :raises: class:`ai_api_client_sdk.exception.AIAPIAuthorizationException` if a 401 response is received from the
+                     :raises: class:`ai_api_client_sdk.exception.AIAPIAuthorizationException` if a 401 response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPINotFoundException` if a 404 response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIServerException` if a non-2XX response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
                          trying to send a request to the server
                      :return: The retrieved execution
-                     :rtype: class:`ai_api_client_sdk.models.execution.Execution`
+                     :rtype: class:Union[`ai_api_client_sdk.models.execution.Execution`,
+                         `ai_api_client_sdk.models.execution_get_status_response.ExecutionGetStatusResponse`]
                  modify(self, execution_id: str, target_status: ai_api_client_sdk.models.target_status.TargetStatus, resource_group: str = None)
                  -> ai_api_client_sdk.models.base_models.BasicResponse
                      Modifies the execution, by changing the target status.
                       
                      :param execution_id: ID of the execution to be modified
                      :type execution_id: str
                      :param target_status: Desired target status of the execution, defaults to None
@@ -155,25 +162,27 @@
                          the server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIServerException` if a non-2XX response is received from the
                          server
                      :raises: class:`ai_api_client_sdk.exception.AIAPIRequestException` if an unexpected exception occurs while
                          trying to send a request to the server
                      :return: An object representing the response from the server
                      :rtype: class:`ai_api_client_sdk.models.base_models.BasicResponse`
-                 query(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None, status:
-                 ai_api_client_sdk.models.status.Status = None, top: int = None, skip: int = None, resource_group: str = None) -
+                 query(self, scenario_id: str = None, configuration_id: str = None, executable_ids: List[str] = None, execution_schedule_id: str
+                 = None, status: ai_api_client_sdk.models.status.Status = None, top: int = None, skip: int = None, resource_group: str = None) -
                  > ai_api_client_sdk.models.execution_query_response.ExecutionQueryResponse
                      Queries the executions.
                       
                      :param scenario_id: ID of the scenario the executions should belong to, defaults to None
                      :type scenario_id: str, optional
                      :param configuration_id: ID of the configuration, the executions should be configured by, defaults to None
                      :type configuration_id: str, optional
                      :param executable_ids: IDs of the executables the executions should be created from, defaults to None
                      :type executable_ids: List[str], optional
+                     :param execution_schedule_id: ID of the execution schedule, defaults to None
+                     :type execution_schedule_id: str, optional
                      :param status: Status which the executions should currently have
                      :type status: class:`ai_api_client_sdk.models.status.Status`, optional
                      :param top: Number of executions to be retrieved, defaults to None
                      :type top: int, optional
                      :param skip: Number of executions to be skipped, from the list of the queried executions, defaults to None
                      :type skip: int, optional
                      :param resource_group: Resource Group which the request should be sent on behalf. Either this or a default
@@ -230,7 +239,8 @@
                  __dict__
                      dictionary for instance variables (if defined)
                  __weakref__
                      list of weak references to the object (if defined)
  
 Data
    � List = typing.List
+         Union = typing.Union
```

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.healthz_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.healthz_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.html`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 <tr><td bgcolor="#aa55cc"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%"><table width="100%" summary="list"><tr><td width="25%" valign=top><a href="ai_api_client_sdk.resource_clients.artifact_client.html">artifact_client</a><br>
 <a href="ai_api_client_sdk.resource_clients.base_client.html">base_client</a><br>
 <a href="ai_api_client_sdk.resource_clients.configuration_client.html">configuration_client</a><br>
 </td><td width="25%" valign=top><a href="ai_api_client_sdk.resource_clients.deployment_client.html">deployment_client</a><br>
 <a href="ai_api_client_sdk.resource_clients.executable_client.html">executable_client</a><br>
 <a href="ai_api_client_sdk.resource_clients.execution_client.html">execution_client</a><br>
-</td><td width="25%" valign=top><a href="ai_api_client_sdk.resource_clients.healthz_client.html">healthz_client</a><br>
+</td><td width="25%" valign=top><a href="ai_api_client_sdk.resource_clients.execution_schedule_client.html">execution_schedule_client</a><br>
+<a href="ai_api_client_sdk.resource_clients.healthz_client.html">healthz_client</a><br>
 <a href="ai_api_client_sdk.resource_clients.meta_client.html">meta_client</a><br>
-<a href="ai_api_client_sdk.resource_clients.metrics_client.html">metrics_client</a><br>
-</td><td width="25%" valign=top><a href="ai_api_client_sdk.resource_clients.resource_groups_client.html">resource_groups_client</a><br>
+</td><td width="25%" valign=top><a href="ai_api_client_sdk.resource_clients.metrics_client.html">metrics_client</a><br>
+<a href="ai_api_client_sdk.resource_clients.resource_groups_client.html">resource_groups_client</a><br>
 <a href="ai_api_client_sdk.resource_clients.scenario_client.html">scenario_client</a><br>
 </td></tr></table></td></tr></table>
 </body></html>
```

### html2text {}

```diff
@@ -1,9 +1,9 @@
                                                                        index
                                   /home/jenkins/agent/workspace/ndation_ai-
                                    api-client-sdk_master/ai_api_client_sdk/
 ai_api_client_sdk.resource_clients              resource_clients/__init__.py
  
 Package Contents
-         artifact_client      deployment_client healthz_client resource_groups_client
-   � base_client          executable_client meta_client    scenario_client
-         configuration_client execution_client  metrics_client
+         artifact_client      deployment_client execution_schedule_client metrics_client
+   � base_client          executable_client healthz_client            resource_groups_client
+         configuration_client execution_client  meta_client               scenario_client
```

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.meta_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.meta_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.metrics_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.metrics_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.resource_groups_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.resource_groups_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.scenario_client.html` & `ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.scenario_client.html`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.dist-info/LICENSE` & `ai_api_client_sdk-1.27.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ai_api_client_sdk-1.26.2.dist-info/METADATA` & `ai_api_client_sdk-1.27.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-api-client-sdk
-Version: 1.26.2
+Version: 1.27.0
 Summary: AI API Client SDK
 Home-page: https://www.sap.com/
 Author: SAP SE
 License: SAP DEVELOPER LICENSE AGREEMENT
 Download-URL: https://pypi.python.org/pypi/ai-api-client-sdk
 Keywords: SAP AI Core
 Platform: Windows
```

## Comparing `ai_api_client_sdk-1.26.2.dist-info/RECORD` & `ai_api_client_sdk-1.27.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ai_api_client_sdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ai_api_client_sdk/ai_api_v2_client.py,sha256=_YVy75NzZH4Q81sADbNOH3n-ZuLlLdJ5QgL9iiBA0gE,4511
+ai_api_client_sdk/ai_api_v2_client.py,sha256=RpRdMSCvuq0RPlAk8ahVPYyH4DmGQmfG_WfbGMEBAhQ,4655
 ai_api_client_sdk/exception.py,sha256=EEvKQu1fFJZvxy_aDhNTADp9a4qnKSGzucL5fz1CP0w,7937
 ai_api_client_sdk/helpers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ai_api_client_sdk/helpers/authenticator.py,sha256=KtwxHZx7i9uQ4sbGuONbRl84p85T4iwK2VYwjTD97S0,2780
 ai_api_client_sdk/helpers/constants.py,sha256=Essj4uSU2LkO2p9uJX4-VEu-MSnoRp6KyzKTznMQS9U,120
 ai_api_client_sdk/helpers/datetime_parser.py,sha256=9QKWxIhH8mD3YIzSAGhFJokjHilVFniIbnlYfnCS_5Y,824
 ai_api_client_sdk/helpers/rest_client.py,sha256=GckbVzoyxO8H2oVzyLkh2MEK1QbJ0fwBGmMnMPK2ylM,13435
 ai_api_client_sdk/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ai_api_client_sdk/models/ai_api_capabilities.py,sha256=gPiXcX4kjsgSuSkRejSiQ2iXLjj_U66d6Y5UCmMfgHQ,3176
+ai_api_client_sdk/models/ai_api_capabilities.py,sha256=RD0jSlzO1EmvC47XveXUTV3mgcBastmTCC5-qlDCnjs,4061
+ai_api_client_sdk/models/ai_api_capabilities_bulk_updates.py,sha256=U1_nF05GEUeupsyslcMcUR0D4YG1ZsVkmjyQOPxyISI,1789
 ai_api_client_sdk/models/ai_api_capabilities_logs.py,sha256=0R7RF4ET6skgTvRbe0jmwEvRmQzw6EJcl_wEAzLZIfg,1691
 ai_api_client_sdk/models/ai_api_limits.py,sha256=K6BGb4cRsQjtMoVPkH3G8YXUz_4WHuprEkyDaUWcmFo,2260
 ai_api_client_sdk/models/ai_api_limits_deployments.py,sha256=_4jTjcec4lc5lWrcn-uKFBYprXDuiS3wXkafpcj1T2o,1397
 ai_api_client_sdk/models/ai_api_limits_enactments.py,sha256=p0aCGyG1R2IuNyGxiaTr3Y9rSNDte7om3EGx_kW4HmA,868
 ai_api_client_sdk/models/ai_api_limits_executions.py,sha256=R9MarJZ85Zx-hSkmrCV03MMUNxc_XqyE-Ohgx3O6_W0,1384
 ai_api_client_sdk/models/ai_api_meta.py,sha256=wkiHl_Y6O2xzfMmIMGdf5kUZ1hO9apKbMvwprgcBnnk,2159
 ai_api_client_sdk/models/api_version.py,sha256=09d_9H4C6e1nXcSdQ9E1_VIKzarHtV4geAkvGBQ-uwM,1618
@@ -24,22 +25,28 @@
 ai_api_client_sdk/models/configuration_create_response.py,sha256=RzejoI4iJTjo56lWIy44CnTySvHsoO1P9eejgdrLSd4,965
 ai_api_client_sdk/models/configuration_query_response.py,sha256=YbJmZVwx7D6aqS2JePFOyEktu4YyP8h_WXXkFVJ_Y1A,1513
 ai_api_client_sdk/models/dataset_capabilities.py,sha256=MtLwxCnA3178lCHRoZu746f7Ef4Bgye4D064v2JFelw,1778
 ai_api_client_sdk/models/dataset_limits.py,sha256=lFU1B08Uiy6OVDKWk8b-lxn1jlfxhNC_rTO3H9IZD_4,1663
 ai_api_client_sdk/models/deployment.py,sha256=qKoQcOdVTPcUDxEpuJLiT7pyl9HhPmeQKlwuIBBEWdc,5936
 ai_api_client_sdk/models/deployment_bulk_modify_response.py,sha256=X7ifCoaVzAtBKzcJAn6WM4eZRbBHp-y00TZj0EmCnPE,1632
 ai_api_client_sdk/models/deployment_create_response.py,sha256=DcLYCK3dcRQIR_P8pRxaWYNjcUhLnSpkpKPW5LQaxgE,1732
+ai_api_client_sdk/models/deployment_get_status_response.py,sha256=WFMtsCwtZO1ATPAzMqSKi7fxPgp5vNsrz-imXwqMC18,2402
 ai_api_client_sdk/models/deployment_query_response.py,sha256=nb6Zz2AiCQrqYTHncOpoVJRD6qooANeXA50dNx8eyRw,1466
 ai_api_client_sdk/models/enactment.py,sha256=UMVpH7q42SfzLSMxfzXyVjCR7ZqKhrVQvFZ4GfCNDO0,3059
+ai_api_client_sdk/models/enactment_get_status_response.py,sha256=KDD4QJ6qQs_Ljr0melVQCuhpXfJ4yXzkkWDpnb0T-XI,1489
 ai_api_client_sdk/models/executable.py,sha256=lp4LMEC1mhmKXc9eDqcRgb-IYj_ifvjrVd0uLET9N1E,4761
 ai_api_client_sdk/models/executable_query_response.py,sha256=TlnVsXXx2aIliauhi9WwMS_f7_xuSrvfFRxkCIeogPg,1466
-ai_api_client_sdk/models/execution.py,sha256=vdGoh6zVMecAfv6Czd_dsRJHTa83j6TWy9c-Cr3gNeI,4818
+ai_api_client_sdk/models/execution.py,sha256=JS5gbFpWCoXWoGyOu_dNzco_meZmMgcKVZX-f3waKgI,5040
 ai_api_client_sdk/models/execution_bulk_modify_response.py,sha256=GpvvrExAZ-mjGMtP4t08HyEhSa0hJ32OSNVeLW-Ovsc,1609
 ai_api_client_sdk/models/execution_create_response.py,sha256=RHzEY2jFf3APLES0nzaeCJU_8oCwqQEYwqtK34tZDWw,1448
+ai_api_client_sdk/models/execution_get_status_response.py,sha256=lzppD5xrwG4NcYB1c1uxsuHH-vl3LPCZd3AKR7WJA7M,2378
 ai_api_client_sdk/models/execution_query_response.py,sha256=lqDyKY1rNVZs_4mUrJ04e-ZAIFee3O_4WdlgCwpuEr4,1450
+ai_api_client_sdk/models/execution_schedule.py,sha256=HeQpLV6Xf5n1bqqtTfrvtGr5qv1f3pyuT1mAEb2pbAY,3048
+ai_api_client_sdk/models/execution_schedule_create_response.py,sha256=_qquZBaWm-3HkfT7wBtB3Zb21RnbRbPxJpasvtajt5Q,1000
+ai_api_client_sdk/models/execution_schedule_query_response.py,sha256=yKSdkwHyX9N7Ef8RdV9GbscKm1lJTR06xVw9aQsNDNg,1584
 ai_api_client_sdk/models/extensions.py,sha256=LrUPUHx_zZCziAGovsHhkYLm4sSpTaqUKHG2NE5B5jI,2748
 ai_api_client_sdk/models/extensions_analytics.py,sha256=kr_dJ_xmBoC7DUb1SHO3wnAityEcAcArf5d9Y42knH8,1383
 ai_api_client_sdk/models/extensions_dataset.py,sha256=c62uNNbspS7lkEF0k1jcQExlLsg2mJx1AFg5HwGRQlI,2371
 ai_api_client_sdk/models/extensions_resource_groups.py,sha256=hOFNhlKhRBKFaOJbD47Sf_pHZTpUlp0sHEp_I5vl-18,1461
 ai_api_client_sdk/models/healthz_status.py,sha256=Mxt_FakITpU_VBxPdziopGPwM8sFscQ9mg195YVVPv4,1457
 ai_api_client_sdk/models/input_artifact.py,sha256=Oy-zL-FW0cPh08soRp9c_uioUTL6KQn8q73Kh_-6-2c,947
 ai_api_client_sdk/models/input_artifact_binding.py,sha256=bdhHOGcZfZNXTTPTffcTXLSkNpwkYJTYPaaR3wWgFN0,1687
@@ -55,107 +62,109 @@
 ai_api_client_sdk/models/parameter.py,sha256=TsrJ8-jqJAmRVdui2Rdvb8M5vVhR35ic_NnEBV01zac,1579
 ai_api_client_sdk/models/parameter_binding.py,sha256=3NrPEbfwndpbOKtxN6UBGYrE_8Jv6QAV2zklNIxOnpc,1054
 ai_api_client_sdk/models/resource_group.py,sha256=j4F9UjOxb2ZJp1DnaxNPb4OuLedxuucKInKTcNQggiY,2205
 ai_api_client_sdk/models/resource_group_query_response.py,sha256=cOXWBsV1qPVtgLsaibwsxJyp6otmsaKIDnE0x75CMkQ,1549
 ai_api_client_sdk/models/resource_group_status.py,sha256=kYGyTY3r_VgfUAKdniOy_atRAPO2ybU102OfCDRcqbM,249
 ai_api_client_sdk/models/scenario.py,sha256=aEXz9lLWtFIi2xTRVrysPiZa3WU7zxZt4ZhmoQ6q6no,2519
 ai_api_client_sdk/models/scenario_query_response.py,sha256=2MbQuIh512VToBuhCJeuHNyOq2wIAQ-tyhu9zbC8vrY,1433
-ai_api_client_sdk/models/status.py,sha256=g2nOioxgCYN0E_nWvrAJvJfGwLfSlBP2Qyk8PHxiLsY,312
+ai_api_client_sdk/models/status.py,sha256=lXPa9mB6aJOKUxIhRvh2yZgvu6_juhFKCl5er_sfOcU,461
 ai_api_client_sdk/models/target_status.py,sha256=Isi3UZffuZkRb1Donu09dYUrCnI2gK3Mjz3ixJ3DTlM,263
 ai_api_client_sdk/models/version.py,sha256=O6c5M7-yoycRRqTbA2OJIPjI6DW7vlpg3z-3j1hoq40,1866
 ai_api_client_sdk/models/version_list.py,sha256=WcVdsN90hr_zawVfDYWoKcc9_5tICczevv6deBqfmMA,1459
 ai_api_client_sdk/models/version_query_response.py,sha256=MQK8pL8tG7x_aFElwtQO3WMp9tEFNG4kTojTv9zbmFA,1417
-ai_api_client_sdk/resource_clients/__init__.py,sha256=fGJc-MzrSSAPgUVUWiDHNERt5qrFUM7zEBqw__guUok,461
+ai_api_client_sdk/resource_clients/__init__.py,sha256=VG4gX68cO0evP4-UjrQJfxWKJd1kaP__rJqPfcDR1bg,524
 ai_api_client_sdk/resource_clients/artifact_client.py,sha256=QM84E-CBUF-6g0PwWMp9l7tPdYmrpF_YQyQo4GNtcsw,10698
 ai_api_client_sdk/resource_clients/base_client.py,sha256=tVGdKReqtG8r-GEN-r8oFdBcs20ZbZ4pHUwT50FHIeE,3114
 ai_api_client_sdk/resource_clients/configuration_client.py,sha256=HpvMv3TVqJE5dHqYmqXIXxYHX9SvE5wF7jArTxftgV0,10003
-ai_api_client_sdk/resource_clients/deployment_client.py,sha256=5KykBcPEGV2XwAZiq3XnV_AFg3VGmRovdG2fpjpFibc,17475
+ai_api_client_sdk/resource_clients/deployment_client.py,sha256=dFZV8CC5Uw-73kNbiwxmsAdyP_gbRWVQmc2Klt9Y2n8,18280
 ai_api_client_sdk/resource_clients/executable_client.py,sha256=QnP62eTjiJq_cOnhxcoQF5e9ixCZ05qeU_QmO9-AeKs,3995
-ai_api_client_sdk/resource_clients/execution_client.py,sha256=IIYuW3PzgwQ4j-AKULUpw9jHBbWR-0Ijzbh8O4kBzwA,16635
+ai_api_client_sdk/resource_clients/execution_client.py,sha256=6AEX3SCduZIHWv3lFGSfOo1XiIW8jvHUY_ta4UCZN6s,17940
+ai_api_client_sdk/resource_clients/execution_schedule_client.py,sha256=4bXZnnayC3c3erGTWaALONfGBzQFz4i8FufuPqVJ9iU,13760
 ai_api_client_sdk/resource_clients/healthz_client.py,sha256=JWxwN_b2T1iGSoSTVV04oJPU7KTKETtUx0n9pycezCM,1041
 ai_api_client_sdk/resource_clients/meta_client.py,sha256=LcNTUqY-GY3wQmKo7oLXLb2sdLx0taf_-gJjUpPwfDE,555
 ai_api_client_sdk/resource_clients/metrics_client.py,sha256=9rJr2vcT49rxm3CNdWbBoUooUAPGEwEVtmzeC3aRjyc,4458
 ai_api_client_sdk/resource_clients/resource_groups_client.py,sha256=E8Pe45e3GkUpy5UahH-MQSI-r8STrf6jTDLLGpv0VAY,7580
 ai_api_client_sdk/resource_clients/scenario_client.py,sha256=a1LqL3rTZCjjiQdK5X0dPU7lHIcTahXaL65G3qEvqqo,5149
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.ai_api_v2_client.html,sha256=6FZCNbEp9oYKDtL9Nh2Gsstqr8nH8zqqsuU1dJR5MdU,6547
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.exception.html,sha256=xhnOECK8HWko9ElahOINn6ldvU9cS-tj6T145AAW-Js,75814
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.authenticator.html,sha256=3dWU2aohWg0Q_zELLds7tLL3qzOTSWz7kLvDnyqEg1A,4693
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.constants.html,sha256=2xopmeIel93t02Z9dGD-bVanKYjze9mdGUEFnfD4_Q8,3546
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.datetime_parser.html,sha256=TNLq6lABdpKXlnCZ3IWsuTU_0wuTWTOQYbLBhEYL86A,2191
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.html,sha256=2R_Y_rVi_5CKy_w3ElS9hPRMPzOAbWPDpMfyasGYIgc,1797
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.helpers.rest_client.html,sha256=38YjpmVBSMsilb79cmixWgLfG8nfJBju67D_mkE60cs,16006
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.html,sha256=U_R99vZbZEVxDsJsjegLcnPoQ2I_Uc9jbEOTY9etN2M,1818
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities.html,sha256=5IapMoxrdJXsyGp4g2g0WGLWwOJRfa1Wn-PbUJe0WXI,7319
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_logs.html,sha256=fkCK4TT2esODJJS2oH4Ha1M1Zc6idLToglPyvioWuoU,5657
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits.html,sha256=9E7qDvpBwovt-SB5rMc9dKDnOe640e_YM0B403BrhOE,5822
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_deployments.html,sha256=8yqxomsqi_cOs2gqpPPH5y4Ik2CMuantIjWvep2Smn0,6524
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_enactments.html,sha256=-xfKZxZlMiQaY5uf2yOlK1D9GOO5I0Omdy3qMmmLq-c,4073
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_limits_executions.html,sha256=4QFUUYMhVbshZrQC6BQZmud90oshCCwPpI6Q4jd-UjQ,6493
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.ai_api_meta.html,sha256=kP1dOuKNvgfAf4AZIWuhQ1iw2lBXo2oCAWzQGDuzZ-E,5748
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.api_version.html,sha256=_nmXw9RAvY4eeXichAWMGiM3iKxYJB17DrgHpjcm00M,5420
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact.html,sha256=hMGKWDAH34CKlrTIlIExLnFMK1iGPX3PZsCiswOZfJY,7735
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact_create_response.html,sha256=VK8q0v27HZlxlyzCsgfiSC27J7P1dExHbM5Vj66KlMg,5968
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.artifact_query_response.html,sha256=hDEnqNOqUzaaGJlhkLRWKtcxTyeZsKC-oOWI7i7qf-A,6083
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.base_models.html,sha256=BP-H9RIl__1HCcxuOiaYfWTmqRCVilpsbr3y7_vgzgc,27413
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.capabilities.html,sha256=xVwCpQnloWsr4iH3aOLUHUEgzW5ABFDB0HwHKbz0oWg,6110
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration.html,sha256=f_-8aG_YWvq-teE4j0jvd3JRWG9sj4OaB9gncy2yrPc,7062
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration_create_response.html,sha256=pXAQZiuPcOtam-jcLGkCDYVlMI8bCoyur1HF12Rbg3M,5754
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.configuration_query_response.html,sha256=kPX2SkHUbd5tEu8VyMHq4bV6pntPptHKeX9R4kamhTM,6253
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.dataset_capabilities.html,sha256=ONXGZVhYvW4Sdhaf6JbLvo6-RflOAn9bc0oakTxWp80,5791
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.dataset_limits.html,sha256=zM4wby7vV2gPZsX9ICLuGb7wnR2ZlGgMIwx1Psl5JPQ,5530
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment.html,sha256=ec0mVEAWrwgI00xJxBuxK-NVZ8FfaUvFmysBiiMqnw0,10076
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_bulk_modify_response.html,sha256=m9khXW681NoVDCcHx4Z_TuDHXdz7EQCeFSR0zCKefZc,5430
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_create_response.html,sha256=Y6wWwjL0oFKUFw1CXMKb9aH8PI11UG6DCaqzbbdz4YI,6501
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.deployment_query_response.html,sha256=4gG6g7JHZgUNaQYJQ2OiuVmH5sUSO0I5Gv801vBmri0,6157
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.enactment.html,sha256=BbbK6FAeRnmuWKde-SPC_yjODheYXn7Y_KwtQ_1xWJE,7043
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.executable.html,sha256=Bf2tSrhtQ5rYnOMAXxS5N6gfea_A65G5X6wTVLRo8KE,8144
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.executable_query_response.html,sha256=zrUqIVNwlOWv3FHPIkJELdsQp0zp6gKhzRZC08AX8HQ,6157
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution.html,sha256=Kr0usoJE11fy7Z3T5S5cKdqtSjfCVOVBV06s1gonLW0,8766
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_bulk_modify_response.html,sha256=hhA7ugSNDDvBlxnk6_hfJ8dmK5mfHENFxVnZnf0Jj_4,5402
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_create_response.html,sha256=HxGinVA3thshAszAlrQbWPzpWoE4BaV6wqS16_lBqWc,6124
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.execution_query_response.html,sha256=O9EmgdnwrOjtIC0VU0V7m5fnwtZ2r29lMLfVAP9ktsQ,6123
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions.html,sha256=yyChdJROjx8VIOh7AgYL81oR0Xq3qAiHD2qqPMjt4pE,6260
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_analytics.html,sha256=Wq1ApoJfY1zw8NHYN4DCkWJn7uWzd4SxsS6TmbsLSiE,5223
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_dataset.html,sha256=TioZTpioV2ZQj7GIpEZ-g8o_Zx88JTsv07eTonlVFbk,6017
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.extensions_resource_groups.html,sha256=LEwcL205RBLr_tnJwmHVpp6bCV4qHM2jSmK39pqa_4E,5385
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.healthz_status.html,sha256=fd_4XbHhuvbttuUmqWXAlgw2yKfOh1IcM0EQ83bjYgA,7359
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.html,sha256=h1bN-NHgGNMjXci85eFnuYKxnQZEb3DE-bdLOdNQADU,6297
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.input_artifact.html,sha256=ARYuKWDlFsNirgCf1u9b2_XfWPGJ9VceAZDtj9d5MGg,5613
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.input_artifact_binding.html,sha256=9Cbs6FZVeaMZEXopHPA0kh959rEjfndpo6S4KG_448A,5738
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.label.html,sha256=Wmh75hgbnKKu2owViCyDbkjknDuZ2KkfcGj_X4Kx_Zg,5496
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.log_response.html,sha256=u0ElQ4vzrvzhwj23rINXOu4txBUf45dzz1uVseCeUmA,10825
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric.html,sha256=SzOQR59j81ojFwkylRtTZOhU7A1aNomtYLdNEJKslTU,6335
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_custom_info.html,sha256=6PM9EPzWJdOlUpmz5nZ7BrvLH1mob6i2JvJRkZVcZh0,5913
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_label.html,sha256=dq8wIVWC_p-qspyT-SmgcbKWGDMRA8xIebP-yLBdKdA,5983
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_resource.html,sha256=8JOVXmTrnWvPS5Xpcf20XC7UNmmRmJeVDG2lFiaCiXY,6156
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metric_tag.html,sha256=vPqN0el1ulY3VawqouzpGESJOaDkkH34b67b-tFekKw,5560
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.metrics_query_response.html,sha256=borkr-Q-AFFzsFs33e6jWHWKZrccUicGz6qJnrP0VyI,6093
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.output_artifact.html,sha256=OEC_kIPiWJWi7FWq6_lZfJNTVtyDCOIS5HxO5SGOP7c,5643
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.parameter.html,sha256=vBrzVOMXWFKtekFyEwX7P3q8IzVB0s3nQS5KbiK8HGQ,5375
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.parameter_binding.html,sha256=B2sGKy2n5fWAcXqQt_7KRoIhA88btw1DxuESu5GzXxU,5905
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group.html,sha256=l00dRSYC6ZjrabGRbg2AdY_TrRY14TXk9jvyX3v-jsA,5598
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group_query_response.html,sha256=LljdcLm7x5e2pyJ7yM8bjahsSUFpUTfkZfV0Fd4NsCI,6217
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.resource_group_status.html,sha256=UFAuqwn1eD1jHAvj8jbab5Ivh9kRYBRQWLeAukrCSFc,4015
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.scenario.html,sha256=AtNVGZq99AIEOtfjKzECKOVHklP9KjCuO3EMrKDptmU,6014
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.scenario_query_response.html,sha256=uNiHm7r13baJ0ES83EIJTInuDyu0Ev7zpoWRzctTD7E,6083
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.status.html,sha256=rvpCBJZLgHaAPBNH7sv5u1cHBTm_9a_ptx2_YtNTO6U,4037
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.target_status.html,sha256=IyKHuSUY-l2Axehm7lJ9ywFhhzaLrfJs_eKQFF-UNGQ,3956
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version.html,sha256=P43lRs-ionuvSa6slr1uloUW2SFhTL1OuUbmvIBrw0Q,5449
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version_list.html,sha256=lXFHK-A7JO2q5U46eO5wlfHrMg-7tn5dCGDyMYaOs3I,5068
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.models.version_query_response.html,sha256=4OS1mfmCrvdwecRcRAvPfLe13OMZFnJvnkOcoSI3CTI,6049
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.artifact_client.html,sha256=jWcVRAMBPtVNzK6YOsbvJAhBnY2BUQUvApshv_I7wJQ,18046
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.base_client.html,sha256=awB_2yE9hLEm0FqdiYDMwg4mwNyf9Kfbu1KhEFSYUOY,5886
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.configuration_client.html,sha256=FJog8LTmwC-phNxWzB5vEdqNiZrAwZu2VxkdJVkiGJs,17115
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.deployment_client.html,sha256=QpGtAEDXIT0shUC2qFH50dMkUDMUo7R36MSGbK6xgsU,25601
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.executable_client.html,sha256=oyqOW6wg_JNcQcxHKgCPdPEFPHNQqy-6QOWg4pzE1As,10336
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.execution_client.html,sha256=6rDGxiepGZ3I7yri1NbP_jC_M8V_XFR2x13xHMCGF1Q,24454
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.healthz_client.html,sha256=83HKipF3xqtQAAzfywBamzfFcNAncqKs-jio_pBxloY,6957
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.html,sha256=GN_ZE0WeZvooEm-2hnYEFmOcrWx8GxAGXp2jtmSLqZs,2537
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.meta_client.html,sha256=Oxh3eq6vpcwzBvb7Jz95eaT9lexruu8ut7fXmBJKJTs,6109
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.metrics_client.html,sha256=vsG0oKL_6AVP2V8I0BaWbKIUArVua4ScrBvhUePfQ8I,11596
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.resource_groups_client.html,sha256=wPq8kekq1PcBS_bOV9GutU6VYEXzKyK9h00qnrPp_98,14424
-ai_api_client_sdk-1.26.2.data/data/docs/ai_api_client_sdk.resource_clients.scenario_client.html,sha256=amASMzNKAPI2rqL3Xg57m1pBUN8s7NatljCbLWJch78,12195
-ai_api_client_sdk-1.26.2.dist-info/LICENSE,sha256=DYP9C1BSy7cci4r8ihdmeTl1R7DMKUZgDAoeO9QrbS8,12569
-ai_api_client_sdk-1.26.2.dist-info/METADATA,sha256=K71XFPXHr4hV5EZzmQuk_pw62wClhkYthE3M_bOFsjI,3707
-ai_api_client_sdk-1.26.2.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-ai_api_client_sdk-1.26.2.dist-info/top_level.txt,sha256=jYykiIlGnnxHjf0W37RKkLw9SZwzxQWwRdDy6KQ-aqY,18
-ai_api_client_sdk-1.26.2.dist-info/RECORD,,
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.ai_api_v2_client.html,sha256=6FZCNbEp9oYKDtL9Nh2Gsstqr8nH8zqqsuU1dJR5MdU,6547
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.exception.html,sha256=xhnOECK8HWko9ElahOINn6ldvU9cS-tj6T145AAW-Js,75814
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.authenticator.html,sha256=3dWU2aohWg0Q_zELLds7tLL3qzOTSWz7kLvDnyqEg1A,4693
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.constants.html,sha256=2xopmeIel93t02Z9dGD-bVanKYjze9mdGUEFnfD4_Q8,3546
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.datetime_parser.html,sha256=TNLq6lABdpKXlnCZ3IWsuTU_0wuTWTOQYbLBhEYL86A,2191
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.html,sha256=2R_Y_rVi_5CKy_w3ElS9hPRMPzOAbWPDpMfyasGYIgc,1797
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.helpers.rest_client.html,sha256=38YjpmVBSMsilb79cmixWgLfG8nfJBju67D_mkE60cs,16006
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.html,sha256=U_R99vZbZEVxDsJsjegLcnPoQ2I_Uc9jbEOTY9etN2M,1818
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities.html,sha256=aBQi8Orh795NpYSpktZ-8eYH6mAuqEFYKkdwvqpeVMs,8193
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_bulk_updates.html,sha256=fVnZ-2UMUKipRlILIKMdemm4GVKRvdkdFT5CHeyVTso,5874
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_capabilities_logs.html,sha256=fkCK4TT2esODJJS2oH4Ha1M1Zc6idLToglPyvioWuoU,5657
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits.html,sha256=9E7qDvpBwovt-SB5rMc9dKDnOe640e_YM0B403BrhOE,5822
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_deployments.html,sha256=8yqxomsqi_cOs2gqpPPH5y4Ik2CMuantIjWvep2Smn0,6524
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_enactments.html,sha256=-xfKZxZlMiQaY5uf2yOlK1D9GOO5I0Omdy3qMmmLq-c,4073
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_limits_executions.html,sha256=4QFUUYMhVbshZrQC6BQZmud90oshCCwPpI6Q4jd-UjQ,6493
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.ai_api_meta.html,sha256=kP1dOuKNvgfAf4AZIWuhQ1iw2lBXo2oCAWzQGDuzZ-E,5748
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.api_version.html,sha256=_nmXw9RAvY4eeXichAWMGiM3iKxYJB17DrgHpjcm00M,5420
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact.html,sha256=hMGKWDAH34CKlrTIlIExLnFMK1iGPX3PZsCiswOZfJY,7735
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact_create_response.html,sha256=VK8q0v27HZlxlyzCsgfiSC27J7P1dExHbM5Vj66KlMg,5968
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.artifact_query_response.html,sha256=hDEnqNOqUzaaGJlhkLRWKtcxTyeZsKC-oOWI7i7qf-A,6083
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.base_models.html,sha256=BP-H9RIl__1HCcxuOiaYfWTmqRCVilpsbr3y7_vgzgc,27413
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.capabilities.html,sha256=xVwCpQnloWsr4iH3aOLUHUEgzW5ABFDB0HwHKbz0oWg,6110
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration.html,sha256=f_-8aG_YWvq-teE4j0jvd3JRWG9sj4OaB9gncy2yrPc,7062
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration_create_response.html,sha256=pXAQZiuPcOtam-jcLGkCDYVlMI8bCoyur1HF12Rbg3M,5754
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.configuration_query_response.html,sha256=kPX2SkHUbd5tEu8VyMHq4bV6pntPptHKeX9R4kamhTM,6253
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.dataset_capabilities.html,sha256=ONXGZVhYvW4Sdhaf6JbLvo6-RflOAn9bc0oakTxWp80,5791
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.dataset_limits.html,sha256=zM4wby7vV2gPZsX9ICLuGb7wnR2ZlGgMIwx1Psl5JPQ,5530
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment.html,sha256=ec0mVEAWrwgI00xJxBuxK-NVZ8FfaUvFmysBiiMqnw0,10076
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_bulk_modify_response.html,sha256=m9khXW681NoVDCcHx4Z_TuDHXdz7EQCeFSR0zCKefZc,5430
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_create_response.html,sha256=Y6wWwjL0oFKUFw1CXMKb9aH8PI11UG6DCaqzbbdz4YI,6501
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.deployment_query_response.html,sha256=4gG6g7JHZgUNaQYJQ2OiuVmH5sUSO0I5Gv801vBmri0,6157
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.enactment.html,sha256=BbbK6FAeRnmuWKde-SPC_yjODheYXn7Y_KwtQ_1xWJE,7043
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.executable.html,sha256=Bf2tSrhtQ5rYnOMAXxS5N6gfea_A65G5X6wTVLRo8KE,8144
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.executable_query_response.html,sha256=zrUqIVNwlOWv3FHPIkJELdsQp0zp6gKhzRZC08AX8HQ,6157
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution.html,sha256=ZFjmFwwpJjiAvcwuj3mpDsDWsSPvC4Jtjt3--0_qDsQ,9044
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_bulk_modify_response.html,sha256=hhA7ugSNDDvBlxnk6_hfJ8dmK5mfHENFxVnZnf0Jj_4,5402
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_create_response.html,sha256=HxGinVA3thshAszAlrQbWPzpWoE4BaV6wqS16_lBqWc,6124
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.execution_query_response.html,sha256=O9EmgdnwrOjtIC0VU0V7m5fnwtZ2r29lMLfVAP9ktsQ,6123
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions.html,sha256=yyChdJROjx8VIOh7AgYL81oR0Xq3qAiHD2qqPMjt4pE,6260
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_analytics.html,sha256=Wq1ApoJfY1zw8NHYN4DCkWJn7uWzd4SxsS6TmbsLSiE,5223
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_dataset.html,sha256=TioZTpioV2ZQj7GIpEZ-g8o_Zx88JTsv07eTonlVFbk,6017
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.extensions_resource_groups.html,sha256=LEwcL205RBLr_tnJwmHVpp6bCV4qHM2jSmK39pqa_4E,5385
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.healthz_status.html,sha256=fd_4XbHhuvbttuUmqWXAlgw2yKfOh1IcM0EQ83bjYgA,7359
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.html,sha256=UAg5cV51HrlB7R_nwXjKuXWHHcDHn1kWd9lmTBlZ6vg,7057
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.input_artifact.html,sha256=ARYuKWDlFsNirgCf1u9b2_XfWPGJ9VceAZDtj9d5MGg,5613
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.input_artifact_binding.html,sha256=9Cbs6FZVeaMZEXopHPA0kh959rEjfndpo6S4KG_448A,5738
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.label.html,sha256=Wmh75hgbnKKu2owViCyDbkjknDuZ2KkfcGj_X4Kx_Zg,5496
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.log_response.html,sha256=u0ElQ4vzrvzhwj23rINXOu4txBUf45dzz1uVseCeUmA,10825
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric.html,sha256=SzOQR59j81ojFwkylRtTZOhU7A1aNomtYLdNEJKslTU,6335
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_custom_info.html,sha256=6PM9EPzWJdOlUpmz5nZ7BrvLH1mob6i2JvJRkZVcZh0,5913
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_label.html,sha256=dq8wIVWC_p-qspyT-SmgcbKWGDMRA8xIebP-yLBdKdA,5983
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_resource.html,sha256=8JOVXmTrnWvPS5Xpcf20XC7UNmmRmJeVDG2lFiaCiXY,6156
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metric_tag.html,sha256=vPqN0el1ulY3VawqouzpGESJOaDkkH34b67b-tFekKw,5560
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.metrics_query_response.html,sha256=borkr-Q-AFFzsFs33e6jWHWKZrccUicGz6qJnrP0VyI,6093
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.output_artifact.html,sha256=OEC_kIPiWJWi7FWq6_lZfJNTVtyDCOIS5HxO5SGOP7c,5643
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.parameter.html,sha256=vBrzVOMXWFKtekFyEwX7P3q8IzVB0s3nQS5KbiK8HGQ,5375
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.parameter_binding.html,sha256=B2sGKy2n5fWAcXqQt_7KRoIhA88btw1DxuESu5GzXxU,5905
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group.html,sha256=l00dRSYC6ZjrabGRbg2AdY_TrRY14TXk9jvyX3v-jsA,5598
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group_query_response.html,sha256=LljdcLm7x5e2pyJ7yM8bjahsSUFpUTfkZfV0Fd4NsCI,6217
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.resource_group_status.html,sha256=UFAuqwn1eD1jHAvj8jbab5Ivh9kRYBRQWLeAukrCSFc,4015
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.scenario.html,sha256=AtNVGZq99AIEOtfjKzECKOVHklP9KjCuO3EMrKDptmU,6014
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.scenario_query_response.html,sha256=uNiHm7r13baJ0ES83EIJTInuDyu0Ev7zpoWRzctTD7E,6083
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.status.html,sha256=QgrCr8nourGpqmflANvMC9NUxNZrMgiJ-Uit8dLs81c,6142
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.target_status.html,sha256=IyKHuSUY-l2Axehm7lJ9ywFhhzaLrfJs_eKQFF-UNGQ,3956
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version.html,sha256=P43lRs-ionuvSa6slr1uloUW2SFhTL1OuUbmvIBrw0Q,5449
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version_list.html,sha256=lXFHK-A7JO2q5U46eO5wlfHrMg-7tn5dCGDyMYaOs3I,5068
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.models.version_query_response.html,sha256=4OS1mfmCrvdwecRcRAvPfLe13OMZFnJvnkOcoSI3CTI,6049
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.artifact_client.html,sha256=jWcVRAMBPtVNzK6YOsbvJAhBnY2BUQUvApshv_I7wJQ,18046
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.base_client.html,sha256=awB_2yE9hLEm0FqdiYDMwg4mwNyf9Kfbu1KhEFSYUOY,5886
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.configuration_client.html,sha256=FJog8LTmwC-phNxWzB5vEdqNiZrAwZu2VxkdJVkiGJs,17115
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.deployment_client.html,sha256=4y7id05gWy0nO5F5nGrRT4QhXJYZFTkko4cQq0GBqaE,26095
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.executable_client.html,sha256=oyqOW6wg_JNcQcxHKgCPdPEFPHNQqy-6QOWg4pzE1As,10336
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.execution_client.html,sha256=XcVtEdWbdV_R6Bm2SyDXq82o_5DqufSUgC2BFUD1SJU,25388
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.healthz_client.html,sha256=83HKipF3xqtQAAzfywBamzfFcNAncqKs-jio_pBxloY,6957
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.html,sha256=_OGaQBB3VPSvXWpNwquZKtBtCnuCglDYCSqwypCB_yU,2647
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.meta_client.html,sha256=Oxh3eq6vpcwzBvb7Jz95eaT9lexruu8ut7fXmBJKJTs,6109
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.metrics_client.html,sha256=vsG0oKL_6AVP2V8I0BaWbKIUArVua4ScrBvhUePfQ8I,11596
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.resource_groups_client.html,sha256=wPq8kekq1PcBS_bOV9GutU6VYEXzKyK9h00qnrPp_98,14424
+ai_api_client_sdk-1.27.0.data/data/docs/ai_api_client_sdk.resource_clients.scenario_client.html,sha256=amASMzNKAPI2rqL3Xg57m1pBUN8s7NatljCbLWJch78,12195
+ai_api_client_sdk-1.27.0.dist-info/LICENSE,sha256=DYP9C1BSy7cci4r8ihdmeTl1R7DMKUZgDAoeO9QrbS8,12569
+ai_api_client_sdk-1.27.0.dist-info/METADATA,sha256=owUMu_2AaAFyZn0CB6Pkosl6u8mTDrMglWsmFPZn-y8,3707
+ai_api_client_sdk-1.27.0.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
+ai_api_client_sdk-1.27.0.dist-info/top_level.txt,sha256=jYykiIlGnnxHjf0W37RKkLw9SZwzxQWwRdDy6KQ-aqY,18
+ai_api_client_sdk-1.27.0.dist-info/RECORD,,
```

