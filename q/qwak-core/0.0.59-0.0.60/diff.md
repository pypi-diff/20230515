# Comparing `tmp/qwak_core-0.0.59.tar.gz` & `tmp/qwak_core-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.59.tar", max compression
+gzip compressed data, was "qwak_core-0.0.60.tar", max compression
```

## Comparing `qwak_core-0.0.59.tar` & `qwak_core-0.0.60.tar`

### file list

```diff
@@ -1,570 +1,570 @@
--rw-r--r--   0        0        0      264 2023-05-15 11:57:36.731470 qwak_core-0.0.59/README.md
--rw-r--r--   0        0        0        0 2023-05-15 11:59:18.043027 qwak_core-0.0.59/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-15 11:59:18.067026 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-15 11:58:58.259113 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.067026 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-15 11:59:18.063027 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-15 11:58:57.903115 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.063027 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-15 11:59:18.063027 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-15 11:58:58.079114 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.063027 qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-15 11:59:18.055027 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-15 11:58:57.375117 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-15 11:59:18.055027 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-15 11:59:18.059027 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-15 11:58:57.551117 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.059027 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-15 11:59:18.059027 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-15 11:58:57.727116 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.059027 qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-15 11:59:18.043027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-15 11:58:57.195118 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-15 11:59:18.043027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-15 11:59:18.047027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-15 11:58:58.435113 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.047027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-15 11:59:18.051027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-15 11:58:58.803111 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.051027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-15 11:59:18.051027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-15 11:58:58.983110 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-15 11:59:18.051027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-15 11:59:18.047027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-15 11:58:58.615112 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.047027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-15 11:59:18.055027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-15 11:58:59.171109 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.055027 qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-15 11:59:18.095026 qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-15 11:59:01.767098 qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.095026 qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-15 11:59:18.095026 qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-15 11:59:01.951097 qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-15 11:59:18.095026 qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-15 11:59:18.159026 qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-15 11:59:07.179074 qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.159026 qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-15 11:59:18.159026 qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-15 11:59:07.355074 qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-15 11:59:18.159026 qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-15 11:59:18.163026 qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-15 11:59:08.255070 qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-15 11:59:18.167026 qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-15 11:59:18.163026 qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-15 11:59:08.079070 qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.163026 qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-15 11:59:18.167026 qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-15 11:59:08.431069 qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.167026 qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-15 11:59:18.167026 qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-15 11:59:08.607068 qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-15 11:59:18.171026 qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-15 11:59:18.247026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-15 11:59:15.835036 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.251026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-15 11:59:18.243026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-15 11:59:15.475038 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.247026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-15 11:59:18.247026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-15 11:59:15.651037 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.247026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-15 11:59:18.239026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-15 11:59:15.119040 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-15 11:59:18.243026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-15 11:59:18.243026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-15 11:59:15.299039 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.243026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-15 11:59:18.255026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-15 11:59:16.367034 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.255026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-15 11:59:18.251026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-15 11:59:16.191035 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.255026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-15 11:59:18.251026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-15 11:59:16.015035 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.251026 qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-15 11:59:18.239026 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-15 11:59:14.935040 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.239026 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-15 11:59:18.235026 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-15 11:59:14.563042 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.235026 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-15 11:59:18.235026 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-15 11:59:14.751041 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-15 11:59:18.239026 qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-15 11:59:18.191026 qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-15 11:59:10.415060 qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-15 11:59:18.195026 qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-15 11:59:18.191026 qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-15 11:59:10.239061 qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.191026 qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-15 11:59:18.183026 qwak_core-0.0.59/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-15 11:59:09.883062 qwak_core-0.0.59/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.183026 qwak_core-0.0.59/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-15 11:59:18.183026 qwak_core-0.0.59/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-15 11:59:10.059062 qwak_core-0.0.59/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.187026 qwak_core-0.0.59/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-15 11:59:18.187026 qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-15 11:59:10.595059 qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-15 11:59:18.187026 qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-15 11:59:18.187026 qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-15 11:59:10.979058 qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-15 11:59:18.191026 qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-15 11:59:18.199026 qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-15 11:59:11.347056 qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.199026 qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-15 11:59:18.199026 qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-15 11:59:11.523055 qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-15 11:59:18.203026 qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-15 11:59:18.175026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-15 11:59:09.347065 qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.179026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-15 11:59:18.179026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-15 11:59:09.523064 qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-15 11:59:18.179026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-15 11:59:18.171026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-15 11:59:08.979066 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.175026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-05-15 11:59:18.171026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-05-15 11:59:08.799067 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.171026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-15 11:59:18.175026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-15 11:59:09.167065 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-15 11:59:18.175026 qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-15 11:59:18.083027 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-15 11:59:00.839102 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.083027 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-15 11:59:18.087026 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-15 11:59:01.023101 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.087026 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-15 11:59:18.087026 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-15 11:59:01.207100 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-15 11:59:18.087026 qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-15 11:59:18.139026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-15 11:59:06.075079 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.139026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-15 11:59:18.139026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-15 11:59:05.895080 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-15 11:59:18.139026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-15 11:59:18.119026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-15 11:59:04.295087 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.119026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-15 11:59:18.119026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-15 11:59:04.115088 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.119026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-15 11:59:18.111026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-15 11:59:03.551090 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.111026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-15 11:59:18.115026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-15 11:59:03.935088 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-15 11:59:18.115026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-15 11:59:18.123026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-15 11:59:04.471086 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.123026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-15 11:59:18.123026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-15 11:59:04.651085 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-15 11:59:18.123026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25213 2023-05-15 11:59:18.115026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37366 2023-05-15 11:59:03.743089 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.115026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-15 11:59:18.127026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-15 11:59:04.827085 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.127026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     5958 2023-05-15 11:59:18.127026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
--rw-r--r--   0        0        0     6232 2023-05-15 11:59:05.003084 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.127026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-15 11:59:18.143026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-15 11:59:17.619028 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.143026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-15 11:59:18.143026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-15 11:59:17.799028 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-15 11:59:18.143026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-15 11:59:18.147026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-15 11:59:06.623077 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.147026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-15 11:59:18.147026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-15 11:59:06.803076 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-15 11:59:18.147026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-15 11:59:18.151026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-15 11:59:06.983075 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.151026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-15 11:59:18.155026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-15 11:59:07.723072 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.155026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-15 11:59:18.151026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-15 11:59:07.539073 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-15 11:59:18.151026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-15 11:59:18.155026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-15 11:59:07.903071 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.155026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-15 11:59:18.131026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-15 11:59:05.183083 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.131026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-15 11:59:18.131026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-15 11:59:05.359082 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.131026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-15 11:59:18.135026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-15 11:59:05.539081 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-15 11:59:18.135026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-15 11:59:18.135026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-15 11:59:05.719081 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.135026 qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-15 11:59:18.255026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-15 11:59:16.543033 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.259026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-15 11:59:18.259026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-15 11:59:16.719032 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-15 11:59:18.259026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-15 11:59:18.259026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-15 11:59:16.891032 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.263026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-15 11:59:18.263026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-15 11:59:17.075031 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-15 11:59:18.263026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-15 11:59:18.263026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-15 11:59:17.267030 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-15 11:59:18.267026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-15 11:59:18.267026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-15 11:59:17.439029 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.267026 qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-15 11:59:18.203026 qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-15 11:59:11.699055 qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.203026 qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-15 11:59:18.203026 qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-15 11:59:11.875054 qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-15 11:59:18.207026 qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-15 11:59:18.099027 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-15 11:59:02.791093 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.099027 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-15 11:59:18.103026 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-15 11:59:02.983093 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.103026 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-15 11:59:18.107026 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-15 11:59:03.167092 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-15 11:59:18.107026 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-15 11:59:18.107026 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-15 11:59:03.347091 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.111026 qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-15 11:59:18.179026 qwak_core-0.0.59/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-15 11:59:09.703063 qwak_core-0.0.59/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-15 11:59:18.183026 qwak_core-0.0.59/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-15 11:59:18.215026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-15 11:59:12.931049 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.219026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-15 11:59:18.219026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-15 11:59:13.111048 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.219026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-15 11:59:18.219026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-15 11:59:13.291047 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.223026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-15 11:59:18.223026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-15 11:59:13.467047 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.223026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-15 11:59:18.223026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-15 11:59:13.655046 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.227026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-15 11:59:18.227026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-15 11:59:13.851045 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-15 11:59:18.227026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-15 11:59:18.227026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-15 11:59:14.027044 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.231026 qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-15 11:59:18.207026 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-15 11:59:12.227052 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.211026 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-15 11:59:18.215026 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-15 11:59:12.751050 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.215026 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-15 11:59:18.211026 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-15 11:59:12.399052 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-15 11:59:18.211026 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-15 11:59:18.211026 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-15 11:59:12.575051 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.215026 qwak_core-0.0.59/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-15 11:59:18.199026 qwak_core-0.0.59/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-15 11:59:11.171057 qwak_core-0.0.59/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-15 11:59:18.199026 qwak_core-0.0.59/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-15 11:59:18.079027 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-15 11:59:02.375095 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-15 11:59:18.079027 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-15 11:59:18.079027 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-15 11:59:02.163096 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.079027 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-15 11:59:18.083027 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-15 11:59:02.591094 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-15 11:59:18.083027 qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-15 11:59:18.195026 qwak_core-0.0.59/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-15 11:59:10.783059 qwak_core-0.0.59/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-15 11:59:18.195026 qwak_core-0.0.59/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-15 11:59:18.207026 qwak_core-0.0.59/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-15 11:59:12.051053 qwak_core-0.0.59/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-15 11:59:18.207026 qwak_core-0.0.59/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-15 11:59:18.075027 qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-15 11:59:00.095105 qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.075027 qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-15 11:59:18.075027 qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-15 11:58:59.915106 qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-15 11:59:18.075027 qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-15 11:59:18.067026 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-15 11:58:59.355109 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.067026 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-15 11:59:18.071027 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-15 11:58:59.539108 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.071027 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-15 11:59:18.071027 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-15 11:58:59.727107 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-15 11:59:18.071027 qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-15 11:59:18.231026 qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-15 11:59:14.383043 qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-15 11:59:18.235026 qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-15 11:59:18.231026 qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-15 11:59:14.203044 qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.231026 qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-15 11:59:18.091026 qwak_core-0.0.59/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-15 11:59:01.395099 qwak_core-0.0.59/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.091026 qwak_core-0.0.59/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-15 11:59:18.091026 qwak_core-0.0.59/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-15 11:59:01.579099 qwak_core-0.0.59/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 11:59:18.091026 qwak_core-0.0.59/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-15 11:59:20.119017 qwak_core-0.0.59/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-15 11:59:20.119017 qwak_core-0.0.59/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-15 11:57:36.731470 qwak_core-0.0.59/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-15 11:57:36.735470 qwak_core-0.0.59/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-15 11:57:36.739470 qwak_core-0.0.59/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.59/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.59/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-15 12:22:28.684237 qwak_core-0.0.60/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 12:24:09.141068 qwak_core-0.0.60/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-15 12:24:09.165068 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-15 12:23:48.052897 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.165068 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-15 12:24:09.161069 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-15 12:23:47.688894 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.161069 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-15 12:24:09.165068 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-15 12:23:47.868895 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.165068 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-15 12:24:09.153068 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-15 12:23:47.144890 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-15 12:24:09.157069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-15 12:24:09.157069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-15 12:23:47.324891 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.157069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-15 12:24:09.161069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-15 12:23:47.508893 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.161069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-15 12:24:09.141068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-15 12:23:46.960888 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-15 12:24:09.141068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-15 12:24:09.145069 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-15 12:23:48.236899 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.145069 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-15 12:24:09.149068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-15 12:23:48.600901 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.149068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-15 12:24:09.149068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-15 12:23:48.784903 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-15 12:24:09.153068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-15 12:24:09.145069 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-15 12:23:48.416900 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.149068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-15 12:24:09.153068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-15 12:23:48.972905 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.153068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-15 12:24:09.197069 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-15 12:23:51.756927 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.197069 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-15 12:24:09.197069 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-15 12:23:51.980929 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-15 12:24:09.197069 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-15 12:24:09.337070 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-15 12:23:57.520974 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.337070 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-15 12:24:09.337070 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-15 12:23:57.708976 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-15 12:24:09.337070 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-15 12:24:09.341070 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-15 12:23:58.648984 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-15 12:24:09.345070 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-15 12:24:09.341070 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-15 12:23:58.460982 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.341070 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-15 12:24:09.345070 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-15 12:23:58.836985 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.345070 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-15 12:24:09.345070 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-15 12:23:59.020987 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-15 12:24:09.349070 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-15 12:24:09.433071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-15 12:24:06.681048 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.433071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-15 12:24:09.429071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-15 12:24:06.305045 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.429071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-15 12:24:09.433071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-15 12:24:06.489047 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.433071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-15 12:24:09.425071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-15 12:24:05.925042 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-15 12:24:09.425071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-15 12:24:09.429071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-15 12:24:06.117044 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.429071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-15 12:24:09.441071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-15 12:24:07.237053 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.441071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-15 12:24:09.437071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-15 12:24:07.053052 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.441071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-15 12:24:09.437071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-15 12:24:06.869050 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.437071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-15 12:24:09.421071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-15 12:24:05.729041 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.425071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-15 12:24:09.417071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-15 12:24:05.341038 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.421071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-15 12:24:09.421071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-15 12:24:05.541039 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-15 12:24:09.421071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-15 12:24:09.373070 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-15 12:24:00.937002 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-15 12:24:09.373070 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-15 12:24:09.369070 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-15 12:24:00.749001 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.373070 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-15 12:24:09.361070 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-15 12:24:00.364997 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.361070 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-15 12:24:09.365070 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-15 12:24:00.552999 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.365070 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-15 12:24:09.365070 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-15 12:24:01.129004 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-15 12:24:09.369070 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-15 12:24:09.369070 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-15 12:24:01.537007 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-15 12:24:09.369070 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-15 12:24:09.381070 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-15 12:24:01.925010 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.381070 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-15 12:24:09.381070 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-15 12:24:02.109012 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-15 12:24:09.381070 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-15 12:24:09.357070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-15 12:23:59.796993 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.357070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-15 12:24:09.357070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-15 12:23:59.980995 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-15 12:24:09.357070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-15 12:24:09.349070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-15 12:23:59.408990 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.353070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-15 12:24:09.349070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-15 12:23:59.220988 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.349070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-15 12:24:09.353070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-15 12:23:59.608991 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-15 12:24:09.353070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-15 12:24:09.185069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-15 12:23:50.724919 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.185069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-15 12:24:09.189069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-15 12:23:50.932921 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.189069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-15 12:24:09.189069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-15 12:23:51.140922 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-15 12:24:09.189069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-15 12:24:09.317070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-15 12:23:56.412965 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.317070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-15 12:24:09.313070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-15 12:23:56.228964 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-15 12:24:09.317070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-15 12:24:09.297070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-15 12:23:54.540950 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.297070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-15 12:24:09.293070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-15 12:23:54.352949 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.293070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-15 12:24:09.285070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-15 12:23:53.764944 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.289070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-15 12:24:09.289070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-15 12:23:54.164947 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-15 12:24:09.293070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-15 12:24:09.297070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-15 12:23:54.728952 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.297070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-15 12:24:09.301070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-15 12:23:54.916953 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-15 12:24:09.301070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25213 2023-05-15 12:24:09.289070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37366 2023-05-15 12:23:53.960945 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.289070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-15 12:24:09.301070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-15 12:23:55.100955 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.301070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     5958 2023-05-15 12:24:09.305070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
+-rw-r--r--   0        0        0     6232 2023-05-15 12:23:55.288956 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.305070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-15 12:24:09.317070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-15 12:24:08.565064 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.321070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-15 12:24:09.321070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-15 12:24:08.781066 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-15 12:24:09.321070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-15 12:24:09.325070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-15 12:23:56.964970 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.325070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-15 12:24:09.325070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-15 12:23:57.152972 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-15 12:24:09.325070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-15 12:24:09.329070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-15 12:23:57.336973 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.329070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-15 12:24:09.333070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-15 12:23:58.088979 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.333070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-15 12:24:09.329070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-15 12:23:57.896978 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-15 12:24:09.329070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-15 12:24:09.333070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-15 12:23:58.276981 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.333070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-15 12:24:09.305070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-15 12:23:55.480958 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.305070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-15 12:24:09.309070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-15 12:23:55.672959 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.309070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-15 12:24:09.309070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-15 12:23:55.860961 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-15 12:24:09.313070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-15 12:24:09.313070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-15 12:23:56.044963 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.313070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-15 12:24:09.441071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-15 12:24:07.417055 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.445071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-15 12:24:09.445071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-15 12:24:07.601056 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-15 12:24:09.445071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-15 12:24:09.445071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-15 12:24:07.785057 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.449071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-15 12:24:09.449071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-15 12:24:07.981059 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-15 12:24:09.449071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-15 12:24:09.449071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-15 12:24:08.173061 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-15 12:24:09.453071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-15 12:24:09.453071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-15 12:24:08.361062 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.453071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-15 12:24:09.385070 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-15 12:24:02.297013 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.385070 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-15 12:24:09.385070 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-15 12:24:02.481015 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-15 12:24:09.385070 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-15 12:24:09.213069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-15 12:23:52.924937 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.221069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-15 12:24:09.233069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-15 12:23:53.144939 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.241069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-15 12:24:09.253069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-15 12:23:53.356940 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-15 12:24:09.261069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-15 12:24:09.277069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-15 12:23:53.568942 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.285070 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-15 12:24:09.361070 qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-15 12:24:00.172996 qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-15 12:24:09.361070 qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-15 12:24:09.397071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-15 12:24:03.621024 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.401070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-15 12:24:09.401070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-15 12:24:03.809025 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.401070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-15 12:24:09.401070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-15 12:24:04.001027 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.405070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-15 12:24:09.405070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-15 12:24:04.193029 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.405070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-15 12:24:09.409071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-15 12:24:04.389030 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.409071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-15 12:24:09.409071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-15 12:24:04.597032 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-15 12:24:09.409071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-15 12:24:09.413071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-15 12:24:04.785033 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.413071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-15 12:24:09.389070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-15 12:24:02.853018 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.393070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-15 12:24:09.397071 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-15 12:24:03.433022 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.397071 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-15 12:24:09.393070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-15 12:24:03.041019 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-15 12:24:09.393070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-15 12:24:09.393070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-15 12:24:03.249021 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.397071 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-15 12:24:09.377070 qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-15 12:24:01.741009 qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-15 12:24:09.377070 qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-15 12:24:09.181069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-15 12:23:52.440933 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-15 12:24:09.181069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-15 12:24:09.177069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-15 12:23:52.204931 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.181069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-15 12:24:09.181069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-15 12:23:52.708935 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-15 12:24:09.185069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-15 12:24:09.373070 qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-15 12:24:01.329005 qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-15 12:24:09.377070 qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-15 12:24:09.389070 qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-15 12:24:02.669016 qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-15 12:24:09.389070 qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-15 12:24:09.177069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-15 12:23:49.900912 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.177069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-15 12:24:09.173069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-15 12:23:49.716911 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-15 12:24:09.177069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-15 12:24:09.169069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-15 12:23:49.152906 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.169069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-15 12:24:09.169069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-15 12:23:49.336907 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.169069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-15 12:24:09.173069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-15 12:23:49.524909 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-15 12:24:09.173069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-15 12:24:09.417071 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-15 12:24:05.157036 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-15 12:24:09.417071 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-15 12:24:09.413071 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-15 12:24:04.969035 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.417071 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-15 12:24:09.193069 qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15881 2023-05-15 12:23:51.348924 qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.193069 qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-15 12:24:09.193069 qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-15 12:23:51.552926 qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 12:24:09.193069 qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-15 12:24:14.013108 qwak_core-0.0.60/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-15 12:24:14.013108 qwak_core-0.0.60/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.60/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.60/PKG-INFO
```

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from _qwak_proto.qwak.audience.v1 import audience_pb2 as qwak_dot_audience_dot_v1_dot_audience__pb2
 from _qwak_proto.qwak.auto_scaling.v1 import auto_scaling_pb2 as qwak_dot_auto__scaling_dot_v1_dot_auto__scaling__pb2
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n qwak/deployment/deployment.proto\x12\x1aqwak.deployment.management\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fqwak/audience/v1/audience.proto\x1a\'qwak/auto_scaling/v1/auto_scaling.proto\x1a/qwak/user_application/common/v0/resources.proto\"\x9e\x01\n\x0eHostingService\x12>\n\tsagemaker\x18\x01 \x01(\x0b\x32%.qwak.deployment.management.SageMakerB\x02\x18\x01H\x00\x12\x45\n\x0fkube_deployment\x18\x02 \x01(\x0b\x32*.qwak.deployment.management.KubeDeploymentH\x00\x42\x05\n\x03val\"\xff\x03\n\x0eKubeDeployment\x12\x15\n\tpod_count\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x43\n\x0f\x64\x65ployment_size\x18\x05 \x01(\x0b\x32*.qwak.deployment.management.DeploymentSize\x12Z\n\x1b\x61\x64vanced_deployment_options\x18\x06 \x01(\x0b\x32\x35.qwak.deployment.management.AdvancedDeploymentOptions\x12L\n\x14kube_deployment_type\x18\x07 \x01(\x0e\x32..qwak.deployment.management.KubeDeploymentType\x12\x45\n\x10serving_strategy\x18\t \x01(\x0b\x32+.qwak.deployment.management.ServingStrategy\x12\x63\n\x15\x65nvironment_variables\x18\n \x03(\x0b\x32\x44.qwak.deployment.management.KubeDeployment.EnvironmentVariablesEntry\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe8\x01\n\x0fServingStrategy\x12\x45\n\x0frealtime_config\x18\x01 \x01(\x0b\x32*.qwak.deployment.management.RealTimeConfigH\x00\x12\x41\n\rstream_config\x18\x02 \x01(\x0b\x32(.qwak.deployment.management.StreamConfigH\x00\x12?\n\x0c\x62\x61tch_config\x18\x03 \x01(\x0b\x32\'.qwak.deployment.management.BatchConfigH\x00\x42\n\n\x08Strategy\"\x99\x01\n\x0eRealTimeConfig\x12\x41\n\x0etraffic_config\x18\x01 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\x12\x44\n\x13\x61uto_scaling_config\x18\x02 \x01(\x0b\x32\'.qwak.auto_scaling.v1.AutoScalingConfig\"\xcf\x01\n\rTrafficConfig\x12\x1f\n\x17selected_variation_name\x18\x01 \x01(\t\x12\x39\n\nvariations\x18\x02 \x03(\x0b\x32%.qwak.deployment.management.Variation\x12\x46\n\x17\x61udience_routes_entries\x18\x03 \x03(\x0b\x32%.qwak.audience.v1.AudienceRoutesEntry\x12\x1a\n\x12\x66\x61llback_variation\x18\x04 \x01(\t\"F\n\x0cStreamConfig\x12\x36\n\x05kafka\x18\x01 \x01(\x0b\x32\'.qwak.deployment.management.KafkaConfig\"\r\n\x0b\x42\x61tchConfig\"\xaf\x05\n\x0bKafkaConfig\x12\x42\n\x08\x63onsumer\x18\x01 \x01(\x0b\x32\x30.qwak.deployment.management.KafkaConfig.Consumer\x12\x42\n\x08producer\x18\x02 \x01(\x0b\x32\x30.qwak.deployment.management.KafkaConfig.Producer\x12\x0f\n\x07workers\x18\x03 \x01(\x05\x1a\x99\x02\n\x08\x43onsumer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x05\x12Y\n\x10\x61uto_offset_type\x18\x05 \x01(\x0e\x32?.qwak.deployment.management.KafkaConfig.Consumer.AutoOffSetType\x12\x16\n\x0emax_batch_size\x18\x06 \x01(\x05\x12\x18\n\x10max_poll_latency\x18\x07 \x01(\x01\"7\n\x0e\x41utoOffSetType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x45\x41RLIEST\x10\x01\x12\n\n\x06LATEST\x10\x02\x1a\xea\x01\n\x08Producer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12Z\n\x10\x63ompression_type\x18\x03 \x01(\x0e\x32@.qwak.deployment.management.KafkaConfig.Producer.CompressionType\"Y\n\x0f\x43ompressionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cUNCOMPRESSED\x10\x01\x12\x08\n\x04GZIP\x10\x02\x12\n\n\x06SNAPPY\x10\x03\x12\x07\n\x03LZ4\x10\x04\x12\x08\n\x04ZSTD\x10\x05\":\n\tSageMaker\x12\x16\n\x0einstance_count\x18\x04 \x01(\x05\x12\x15\n\rinstance_type\x18\x05 \x01(\t\"\xd0\x01\n\x0e\x44\x65ploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x15\n\rmemory_amount\x18\x03 \x01(\x05\x12<\n\x0cmemory_units\x18\x04 \x01(\x0e\x32&.qwak.deployment.management.MemoryUnit\x12\x44\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\"Y\n\x0cGpuResources\x12\x35\n\x08gpu_type\x18\x01 \x01(\x0e\x32#.qwak.deployment.management.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x8c\x02\n\x19\x41\x64vancedDeploymentOptions\x12%\n\x1dnumber_of_http_server_workers\x18\x01 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x02 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x04 \x01(\t\x12\x16\n\x0emax_batch_size\x18\x05 \x01(\x05\x12(\n deployment_process_timeout_limit\x18\x06 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x07 \x01(\t\"\xb8\x07\n\x11\x44\x65ploymentDetails\x12\x31\n\rlast_deployed\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x16\n\x0enumber_of_pods\x18\x03 \x01(\x05\x12\x14\n\x0c\x63pu_fraction\x18\x04 \x01(\x02\x12\x15\n\rmemory_amount\x18\x05 \x01(\x05\x12<\n\x0cmemory_units\x18\x06 \x01(\x0e\x32&.qwak.deployment.management.MemoryUnit\x12\x19\n\x11number_of_workers\x18\x07 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x08 \x01(\x05\x12L\n\x14kube_deployment_type\x18\t \x01(\x0e\x32..qwak.deployment.management.KubeDeploymentType\x12\x45\n\x10serving_strategy\x18\n \x01(\x0b\x32+.qwak.deployment.management.ServingStrategy\x12\x38\n\tvariation\x18\x0b \x01(\x0b\x32%.qwak.deployment.management.Variation\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x0c \x01(\t\x12\x16\n\x0emax_batch_size\x18\r \x01(\x05\x12:\n\x08gpu_type\x18\x0e \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x0f \x01(\x05\x12\x16\n\x0e\x65nvironment_id\x18\x10 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x11 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12(\n deployment_process_timeout_limit\x18\x13 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x14 \x01(\t\x12\x66\n\x15\x65nvironment_variables\x18\x15 \x03(\x0b\x32G.qwak.deployment.management.DeploymentDetails.EnvironmentVariablesEntry\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb9\x01\n\x19RuntimeDeploymentSettings\x12Y\n\x11root_logger_level\x18\x01 \x01(\x0e\x32>.qwak.deployment.management.RuntimeDeploymentSettings.LogLevel\"A\n\x08LogLevel\x12\x0b\n\x07NOT_SET\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x08\n\x04WARN\x10\x02\x12\x08\n\x04INFO\x10\x03\x12\t\n\x05\x44\x45\x42UG\x10\x04\"\xb6\x02\n\x0f\x44\x65ploymentBrief\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x13\n\x0b\x64\x65ployed_by\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x61ilure_reason_code\x18\x04 \x01(\t\x12\x17\n\x0f\x66\x61ilure_message\x18\x05 \x01(\t\x12\x19\n\x11technical_details\x18\x06 \x01(\t\x12\x38\n\x14\x64\x65ployment_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x65nvironment_id\x18\x08 \x01(\t\x12\x16\n\x0evariation_name\x18\t \x01(\t\"\xd7\x02\n\x1eKubernetesModelDeploymentState\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x41\n\x06status\x18\x03 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x41\n\x0estatus_details\x18\x04 \x01(\x0b\x32).qwak.deployment.management.StatusDetails\x12\x16\n\x0evariation_name\x18\x05 \x01(\t\x12\x15\n\rdeployment_id\x18\x06 \x01(\t\x12\x12\n\nmodel_uuid\x18\x07 \x01(\t\x12\x43\n\nmanaged_by\x18\x08 \x01(\x0e\x32/.qwak.deployment.management.DeploymentManagedBy\"\x9e\x02\n\rStatusDetails\x12R\n\x16pending_status_details\x18\x01 \x01(\x0b\x32\x30.qwak.deployment.management.PendingStatusDetailsH\x00\x12U\n\x16success_status_details\x18\x02 \x01(\x0b\x32\x33.qwak.deployment.management.SuccessfulStatusDetailsH\x00\x12P\n\x15\x66\x61iled_status_details\x18\x03 \x01(\x0b\x32/.qwak.deployment.management.FailedStatusDetailsH\x00\x42\x10\n\x0estatus_details\"\x9c\x01\n\x14PendingStatusDetails\x12\x41\n\x0cold_instance\x18\x01 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\x12\x41\n\x0cnew_instance\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"`\n\x17SuccessfulStatusDetails\x12\x45\n\x10running_instance\x18\x01 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"\xe3\x01\n\x13\x46\x61iledStatusDetails\x12\x43\n\x0f\x66\x61ilure_details\x18\x01 \x01(\x0b\x32*.qwak.deployment.management.FailureDetails\x12\x41\n\x0cold_instance\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\x12\x44\n\x0f\x66\x61iled_instance\x18\x03 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"\x91\x01\n\x0e\x46\x61ilureDetails\x12_\n\x1e\x64\x65ployment_failure_reason_code\x18\x01 \x01(\x0e\x32\x37.qwak.deployment.management.DeploymentFailureReasonCode\x12\x1e\n\x16\x66\x61ilure_reason_details\x18\x02 \x01(\t\"V\n\x0fInstanceDetails\x12\x15\n\rdeployment_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x03 \x01(\x05\"u\n\tVariation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x03 \x01(\t\x12:\n\x07traffic\x18\x02 \x01(\x0b\x32\'.qwak.deployment.management.TrafficSpecH\x00\x42\x06\n\x04spec\"4\n\x0bTrafficSpec\x12\x12\n\npercentage\x18\x01 \x01(\x05\x12\x11\n\tis_shadow\x18\x02 \x01(\x08\"]\n\x18\x46utureDeploymentSettings\x12\x41\n\x0etraffic_config\x18\x01 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\"\xb6\x01\n\x1c\x45nvironmentDeploymentMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x43\n\x0fhosting_service\x18\x04 \x01(\x0b\x32*.qwak.deployment.management.HostingService\x12\x16\n\nmodel_uuid\x18\x05 \x01(\tB\x02\x18\x01\"\x92\x01\n\"EnvironmentDeploymentResultMessage\x12\x1b\n\x13\x64\x65ployment_named_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x0c\n\x04info\x18\x03 \x01(\t\"\x90\x02\n\x1e\x45nvironmentUndeploymentMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12V\n\x14hosting_service_type\x18\x03 \x01(\x0e\x32\x38.qwak.deployment.management.DeploymentHostingServiceType\x12\x41\n\x0etraffic_config\x18\x04 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\x12\x16\n\x0evariation_name\x18\x05 \x01(\t\x12\x12\n\nmodel_uuid\x18\x06 \x01(\t\"w\n$EnvironmentUndeploymentResultMessage\x12\x41\n\x06status\x18\x01 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x0c\n\x04info\x18\x02 \x01(\t\"\xd6\x01\n+EnvironmentRuntimeDeploymentSettingsMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12R\n\x13\x64\x65ployment_settings\x18\x03 \x01(\x0b\x32\x35.qwak.deployment.management.RuntimeDeploymentSettings\x12\x16\n\x0evariation_name\x18\x04 \x01(\t\x12\x12\n\nmodel_uuid\x18\x05 \x01(\t\"G\n1EnvironmentRuntimeDeploymentSettingsResultMessage\x12\x12\n\nerror_info\x18\x01 \x01(\t\"4\n$EnvironmentApplyModelTrafficResponse\x12\x0c\n\x04info\x18\x01 \x01(\t\"\xce\x01\n#EnvironmentDeploymentDetailsMessage\x12J\n\x13\x64\x65ployments_details\x18\x01 \x03(\x0b\x32-.qwak.deployment.management.DeploymentDetails\x12?\n\x10\x61udiences_routes\x18\x02 \x03(\x0b\x32%.qwak.audience.v1.AudienceRoutesEntry\x12\x1a\n\x12\x66\x61llback_variation\x18\x03 \x01(\t\"g\n#EnvironmentDeploymentHistoryMessage\x12@\n\x0b\x64\x65ployments\x18\x01 \x03(\x0b\x32+.qwak.deployment.management.DeploymentBrief\"V\n\x19\x45nvironmentTrafficMessage\x12\x39\n\nvariations\x18\x01 \x03(\x0b\x32%.qwak.deployment.management.Variation\"\x9e\x02\n BuildDeploymentEnvironmentStatus\x12\x87\x01\n\x1f\x65nvironment_to_deployment_brief\x18\x01 \x03(\x0b\x32^.qwak.deployment.management.BuildDeploymentEnvironmentStatus.EnvironmentToDeploymentBriefEntry\x1ap\n!EnvironmentToDeploymentBriefEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.DeploymentBrief:\x02\x38\x01\"@\n\x15\x42uildDeploymentStatus\x12\x12\n\nbuild_uuid\x18\x01 \x01(\t\x12\x13\n\x0bis_deployed\x18\x02 \x01(\x08*\xc9\x02\n\x15ModelDeploymentStatus\x12\x16\n\x12INVALID_DEPLOYMENT\x10\x00\x12\x19\n\x15INITIATING_DEPLOYMENT\x10\x01\x12 \n\x1c\x46\x41ILED_INITIATING_DEPLOYMENT\x10\x08\x12\x16\n\x12PENDING_DEPLOYMENT\x10\x02\x12\x19\n\x15SUCCESSFUL_DEPLOYMENT\x10\x03\x12\x15\n\x11\x46\x41ILED_DEPLOYMENT\x10\x04\x12\x1b\n\x17INITIATING_UNDEPLOYMENT\x10\t\x12\x18\n\x14PENDING_UNDEPLOYMENT\x10\n\x12\x1b\n\x17SUCCESSFUL_UNDEPLOYMENT\x10\x05\x12\x17\n\x13\x46\x41ILED_UNDEPLOYMENT\x10\x06\x12\t\n\x05UNSET\x10\x07\x12\x19\n\x15\x41LL_BUILDS_UNDEPLOYED\x10\x0b*O\n\x1c\x44\x65ploymentHostingServiceType\x12\x0b\n\x07INVALID\x10\x00\x12\r\n\tSAGEMAKER\x10\x01\x12\x13\n\x0fKUBE_DEPLOYMENT\x10\x02*F\n\x12KubeDeploymentType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06ONLINE\x10\x01\x12\n\n\x06STREAM\x10\x02\x12\t\n\x05\x42\x41TCH\x10\x03*l\n\x07GpuType\x12\x0f\n\x0bINVALID_GPU\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05*+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x83\x01\n\x13\x44\x65ploymentManagedBy\x12!\n\x1d\x44\x45PLOYMENT_MANAGED_BY_INVALID\x10\x00\x12&\n\"DEPLOYMENT_MANAGED_BY_KUBE_CAPTAIN\x10\x01\x12!\n\x1d\x44\x45PLOYMENT_MANAGED_BY_ADMIRAL\x10\x02*\x93\x02\n\x1b\x44\x65ploymentFailureReasonCode\x12\x18\n\x14INVALID_FAILURE_CODE\x10\x00\x12\x12\n\x0eUNKNOWN_REASON\x10\x01\x12\x1e\n\x1aNO_REPLICA_SETS_PODS_FOUND\x10\x02\x12\x1d\n\x19MODEL_CONTAINER_NOT_FOUND\x10\x03\x12\x11\n\rUNSCHEDULABLE\x10\x04\x12\x1a\n\x16\x44OCKER_IMAGE_NOT_FOUND\x10\x05\x12\x19\n\x15MEMORY_LIMIT_EXCEEDED\x10\x06\x12\x0e\n\nCRASH_LOOP\x10\x07\x12-\n)CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x08\x42\x45\n%com.qwak.ai.management.deployment.apiP\x01Z\x1aqwak/deployment;deploymentb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n qwak/deployment/deployment.proto\x12\x1aqwak.deployment.management\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fqwak/audience/v1/audience.proto\x1a\'qwak/auto_scaling/v1/auto_scaling.proto\x1a/qwak/user_application/common/v0/resources.proto\"\x9e\x01\n\x0eHostingService\x12>\n\tsagemaker\x18\x01 \x01(\x0b\x32%.qwak.deployment.management.SageMakerB\x02\x18\x01H\x00\x12\x45\n\x0fkube_deployment\x18\x02 \x01(\x0b\x32*.qwak.deployment.management.KubeDeploymentH\x00\x42\x05\n\x03val\"\xff\x03\n\x0eKubeDeployment\x12\x15\n\tpod_count\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x43\n\x0f\x64\x65ployment_size\x18\x05 \x01(\x0b\x32*.qwak.deployment.management.DeploymentSize\x12Z\n\x1b\x61\x64vanced_deployment_options\x18\x06 \x01(\x0b\x32\x35.qwak.deployment.management.AdvancedDeploymentOptions\x12L\n\x14kube_deployment_type\x18\x07 \x01(\x0e\x32..qwak.deployment.management.KubeDeploymentType\x12\x45\n\x10serving_strategy\x18\t \x01(\x0b\x32+.qwak.deployment.management.ServingStrategy\x12\x63\n\x15\x65nvironment_variables\x18\n \x03(\x0b\x32\x44.qwak.deployment.management.KubeDeployment.EnvironmentVariablesEntry\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe8\x01\n\x0fServingStrategy\x12\x45\n\x0frealtime_config\x18\x01 \x01(\x0b\x32*.qwak.deployment.management.RealTimeConfigH\x00\x12\x41\n\rstream_config\x18\x02 \x01(\x0b\x32(.qwak.deployment.management.StreamConfigH\x00\x12?\n\x0c\x62\x61tch_config\x18\x03 \x01(\x0b\x32\'.qwak.deployment.management.BatchConfigH\x00\x42\n\n\x08Strategy\"\x99\x01\n\x0eRealTimeConfig\x12\x41\n\x0etraffic_config\x18\x01 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\x12\x44\n\x13\x61uto_scaling_config\x18\x02 \x01(\x0b\x32\'.qwak.auto_scaling.v1.AutoScalingConfig\"\xcf\x01\n\rTrafficConfig\x12\x1f\n\x17selected_variation_name\x18\x01 \x01(\t\x12\x39\n\nvariations\x18\x02 \x03(\x0b\x32%.qwak.deployment.management.Variation\x12\x46\n\x17\x61udience_routes_entries\x18\x03 \x03(\x0b\x32%.qwak.audience.v1.AudienceRoutesEntry\x12\x1a\n\x12\x66\x61llback_variation\x18\x04 \x01(\t\"F\n\x0cStreamConfig\x12\x36\n\x05kafka\x18\x01 \x01(\x0b\x32\'.qwak.deployment.management.KafkaConfig\"\r\n\x0b\x42\x61tchConfig\"\xaf\x05\n\x0bKafkaConfig\x12\x42\n\x08\x63onsumer\x18\x01 \x01(\x0b\x32\x30.qwak.deployment.management.KafkaConfig.Consumer\x12\x42\n\x08producer\x18\x02 \x01(\x0b\x32\x30.qwak.deployment.management.KafkaConfig.Producer\x12\x0f\n\x07workers\x18\x03 \x01(\x05\x1a\x99\x02\n\x08\x43onsumer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x05\x12Y\n\x10\x61uto_offset_type\x18\x05 \x01(\x0e\x32?.qwak.deployment.management.KafkaConfig.Consumer.AutoOffSetType\x12\x16\n\x0emax_batch_size\x18\x06 \x01(\x05\x12\x18\n\x10max_poll_latency\x18\x07 \x01(\x01\"7\n\x0e\x41utoOffSetType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x45\x41RLIEST\x10\x01\x12\n\n\x06LATEST\x10\x02\x1a\xea\x01\n\x08Producer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12Z\n\x10\x63ompression_type\x18\x03 \x01(\x0e\x32@.qwak.deployment.management.KafkaConfig.Producer.CompressionType\"Y\n\x0f\x43ompressionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cUNCOMPRESSED\x10\x01\x12\x08\n\x04GZIP\x10\x02\x12\n\n\x06SNAPPY\x10\x03\x12\x07\n\x03LZ4\x10\x04\x12\x08\n\x04ZSTD\x10\x05\":\n\tSageMaker\x12\x16\n\x0einstance_count\x18\x04 \x01(\x05\x12\x15\n\rinstance_type\x18\x05 \x01(\t\"\xc2\x02\n\x0e\x44\x65ploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0f\n\x03\x63pu\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x03 \x01(\x05\x42\x02\x18\x01\x12@\n\x0cmemory_units\x18\x04 \x01(\x0e\x32&.qwak.deployment.management.MemoryUnitB\x02\x18\x01\x12H\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12`\n\x1c\x63lient_pod_compute_resources\x18\x06 \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResources\"Y\n\x0cGpuResources\x12\x35\n\x08gpu_type\x18\x01 \x01(\x0e\x32#.qwak.deployment.management.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x8c\x02\n\x19\x41\x64vancedDeploymentOptions\x12%\n\x1dnumber_of_http_server_workers\x18\x01 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x02 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x04 \x01(\t\x12\x16\n\x0emax_batch_size\x18\x05 \x01(\x05\x12(\n deployment_process_timeout_limit\x18\x06 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x07 \x01(\t\"\xb8\x07\n\x11\x44\x65ploymentDetails\x12\x31\n\rlast_deployed\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x16\n\x0enumber_of_pods\x18\x03 \x01(\x05\x12\x14\n\x0c\x63pu_fraction\x18\x04 \x01(\x02\x12\x15\n\rmemory_amount\x18\x05 \x01(\x05\x12<\n\x0cmemory_units\x18\x06 \x01(\x0e\x32&.qwak.deployment.management.MemoryUnit\x12\x19\n\x11number_of_workers\x18\x07 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x08 \x01(\x05\x12L\n\x14kube_deployment_type\x18\t \x01(\x0e\x32..qwak.deployment.management.KubeDeploymentType\x12\x45\n\x10serving_strategy\x18\n \x01(\x0b\x32+.qwak.deployment.management.ServingStrategy\x12\x38\n\tvariation\x18\x0b \x01(\x0b\x32%.qwak.deployment.management.Variation\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x0c \x01(\t\x12\x16\n\x0emax_batch_size\x18\r \x01(\x05\x12:\n\x08gpu_type\x18\x0e \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x0f \x01(\x05\x12\x16\n\x0e\x65nvironment_id\x18\x10 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x11 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12(\n deployment_process_timeout_limit\x18\x13 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x14 \x01(\t\x12\x66\n\x15\x65nvironment_variables\x18\x15 \x03(\x0b\x32G.qwak.deployment.management.DeploymentDetails.EnvironmentVariablesEntry\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb9\x01\n\x19RuntimeDeploymentSettings\x12Y\n\x11root_logger_level\x18\x01 \x01(\x0e\x32>.qwak.deployment.management.RuntimeDeploymentSettings.LogLevel\"A\n\x08LogLevel\x12\x0b\n\x07NOT_SET\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x08\n\x04WARN\x10\x02\x12\x08\n\x04INFO\x10\x03\x12\t\n\x05\x44\x45\x42UG\x10\x04\"\xb6\x02\n\x0f\x44\x65ploymentBrief\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x13\n\x0b\x64\x65ployed_by\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x61ilure_reason_code\x18\x04 \x01(\t\x12\x17\n\x0f\x66\x61ilure_message\x18\x05 \x01(\t\x12\x19\n\x11technical_details\x18\x06 \x01(\t\x12\x38\n\x14\x64\x65ployment_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x65nvironment_id\x18\x08 \x01(\t\x12\x16\n\x0evariation_name\x18\t \x01(\t\"\xd7\x02\n\x1eKubernetesModelDeploymentState\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x41\n\x06status\x18\x03 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x41\n\x0estatus_details\x18\x04 \x01(\x0b\x32).qwak.deployment.management.StatusDetails\x12\x16\n\x0evariation_name\x18\x05 \x01(\t\x12\x15\n\rdeployment_id\x18\x06 \x01(\t\x12\x12\n\nmodel_uuid\x18\x07 \x01(\t\x12\x43\n\nmanaged_by\x18\x08 \x01(\x0e\x32/.qwak.deployment.management.DeploymentManagedBy\"\x9e\x02\n\rStatusDetails\x12R\n\x16pending_status_details\x18\x01 \x01(\x0b\x32\x30.qwak.deployment.management.PendingStatusDetailsH\x00\x12U\n\x16success_status_details\x18\x02 \x01(\x0b\x32\x33.qwak.deployment.management.SuccessfulStatusDetailsH\x00\x12P\n\x15\x66\x61iled_status_details\x18\x03 \x01(\x0b\x32/.qwak.deployment.management.FailedStatusDetailsH\x00\x42\x10\n\x0estatus_details\"\x9c\x01\n\x14PendingStatusDetails\x12\x41\n\x0cold_instance\x18\x01 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\x12\x41\n\x0cnew_instance\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"`\n\x17SuccessfulStatusDetails\x12\x45\n\x10running_instance\x18\x01 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"\xe3\x01\n\x13\x46\x61iledStatusDetails\x12\x43\n\x0f\x66\x61ilure_details\x18\x01 \x01(\x0b\x32*.qwak.deployment.management.FailureDetails\x12\x41\n\x0cold_instance\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\x12\x44\n\x0f\x66\x61iled_instance\x18\x03 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"\x91\x01\n\x0e\x46\x61ilureDetails\x12_\n\x1e\x64\x65ployment_failure_reason_code\x18\x01 \x01(\x0e\x32\x37.qwak.deployment.management.DeploymentFailureReasonCode\x12\x1e\n\x16\x66\x61ilure_reason_details\x18\x02 \x01(\t\"V\n\x0fInstanceDetails\x12\x15\n\rdeployment_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x03 \x01(\x05\"u\n\tVariation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x03 \x01(\t\x12:\n\x07traffic\x18\x02 \x01(\x0b\x32\'.qwak.deployment.management.TrafficSpecH\x00\x42\x06\n\x04spec\"4\n\x0bTrafficSpec\x12\x12\n\npercentage\x18\x01 \x01(\x05\x12\x11\n\tis_shadow\x18\x02 \x01(\x08\"]\n\x18\x46utureDeploymentSettings\x12\x41\n\x0etraffic_config\x18\x01 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\"\xb6\x01\n\x1c\x45nvironmentDeploymentMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x43\n\x0fhosting_service\x18\x04 \x01(\x0b\x32*.qwak.deployment.management.HostingService\x12\x16\n\nmodel_uuid\x18\x05 \x01(\tB\x02\x18\x01\"\x92\x01\n\"EnvironmentDeploymentResultMessage\x12\x1b\n\x13\x64\x65ployment_named_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x0c\n\x04info\x18\x03 \x01(\t\"\x90\x02\n\x1e\x45nvironmentUndeploymentMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12V\n\x14hosting_service_type\x18\x03 \x01(\x0e\x32\x38.qwak.deployment.management.DeploymentHostingServiceType\x12\x41\n\x0etraffic_config\x18\x04 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\x12\x16\n\x0evariation_name\x18\x05 \x01(\t\x12\x12\n\nmodel_uuid\x18\x06 \x01(\t\"w\n$EnvironmentUndeploymentResultMessage\x12\x41\n\x06status\x18\x01 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x0c\n\x04info\x18\x02 \x01(\t\"\xd6\x01\n+EnvironmentRuntimeDeploymentSettingsMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12R\n\x13\x64\x65ployment_settings\x18\x03 \x01(\x0b\x32\x35.qwak.deployment.management.RuntimeDeploymentSettings\x12\x16\n\x0evariation_name\x18\x04 \x01(\t\x12\x12\n\nmodel_uuid\x18\x05 \x01(\t\"G\n1EnvironmentRuntimeDeploymentSettingsResultMessage\x12\x12\n\nerror_info\x18\x01 \x01(\t\"4\n$EnvironmentApplyModelTrafficResponse\x12\x0c\n\x04info\x18\x01 \x01(\t\"\xce\x01\n#EnvironmentDeploymentDetailsMessage\x12J\n\x13\x64\x65ployments_details\x18\x01 \x03(\x0b\x32-.qwak.deployment.management.DeploymentDetails\x12?\n\x10\x61udiences_routes\x18\x02 \x03(\x0b\x32%.qwak.audience.v1.AudienceRoutesEntry\x12\x1a\n\x12\x66\x61llback_variation\x18\x03 \x01(\t\"g\n#EnvironmentDeploymentHistoryMessage\x12@\n\x0b\x64\x65ployments\x18\x01 \x03(\x0b\x32+.qwak.deployment.management.DeploymentBrief\"V\n\x19\x45nvironmentTrafficMessage\x12\x39\n\nvariations\x18\x01 \x03(\x0b\x32%.qwak.deployment.management.Variation\"\x9e\x02\n BuildDeploymentEnvironmentStatus\x12\x87\x01\n\x1f\x65nvironment_to_deployment_brief\x18\x01 \x03(\x0b\x32^.qwak.deployment.management.BuildDeploymentEnvironmentStatus.EnvironmentToDeploymentBriefEntry\x1ap\n!EnvironmentToDeploymentBriefEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.DeploymentBrief:\x02\x38\x01\"@\n\x15\x42uildDeploymentStatus\x12\x12\n\nbuild_uuid\x18\x01 \x01(\t\x12\x13\n\x0bis_deployed\x18\x02 \x01(\x08*\xc9\x02\n\x15ModelDeploymentStatus\x12\x16\n\x12INVALID_DEPLOYMENT\x10\x00\x12\x19\n\x15INITIATING_DEPLOYMENT\x10\x01\x12 \n\x1c\x46\x41ILED_INITIATING_DEPLOYMENT\x10\x08\x12\x16\n\x12PENDING_DEPLOYMENT\x10\x02\x12\x19\n\x15SUCCESSFUL_DEPLOYMENT\x10\x03\x12\x15\n\x11\x46\x41ILED_DEPLOYMENT\x10\x04\x12\x1b\n\x17INITIATING_UNDEPLOYMENT\x10\t\x12\x18\n\x14PENDING_UNDEPLOYMENT\x10\n\x12\x1b\n\x17SUCCESSFUL_UNDEPLOYMENT\x10\x05\x12\x17\n\x13\x46\x41ILED_UNDEPLOYMENT\x10\x06\x12\t\n\x05UNSET\x10\x07\x12\x19\n\x15\x41LL_BUILDS_UNDEPLOYED\x10\x0b*O\n\x1c\x44\x65ploymentHostingServiceType\x12\x0b\n\x07INVALID\x10\x00\x12\r\n\tSAGEMAKER\x10\x01\x12\x13\n\x0fKUBE_DEPLOYMENT\x10\x02*F\n\x12KubeDeploymentType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06ONLINE\x10\x01\x12\n\n\x06STREAM\x10\x02\x12\t\n\x05\x42\x41TCH\x10\x03*l\n\x07GpuType\x12\x0f\n\x0bINVALID_GPU\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05*+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x83\x01\n\x13\x44\x65ploymentManagedBy\x12!\n\x1d\x44\x45PLOYMENT_MANAGED_BY_INVALID\x10\x00\x12&\n\"DEPLOYMENT_MANAGED_BY_KUBE_CAPTAIN\x10\x01\x12!\n\x1d\x44\x45PLOYMENT_MANAGED_BY_ADMIRAL\x10\x02*\x93\x02\n\x1b\x44\x65ploymentFailureReasonCode\x12\x18\n\x14INVALID_FAILURE_CODE\x10\x00\x12\x12\n\x0eUNKNOWN_REASON\x10\x01\x12\x1e\n\x1aNO_REPLICA_SETS_PODS_FOUND\x10\x02\x12\x1d\n\x19MODEL_CONTAINER_NOT_FOUND\x10\x03\x12\x11\n\rUNSCHEDULABLE\x10\x04\x12\x1a\n\x16\x44OCKER_IMAGE_NOT_FOUND\x10\x05\x12\x19\n\x15MEMORY_LIMIT_EXCEEDED\x10\x06\x12\x0e\n\nCRASH_LOOP\x10\x07\x12-\n)CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x08\x42\x45\n%com.qwak.ai.management.deployment.apiP\x01Z\x1aqwak/deployment;deploymentb\x06proto3')
 
 _MODELDEPLOYMENTSTATUS = DESCRIPTOR.enum_types_by_name['ModelDeploymentStatus']
 ModelDeploymentStatus = enum_type_wrapper.EnumTypeWrapper(_MODELDEPLOYMENTSTATUS)
 _DEPLOYMENTHOSTINGSERVICETYPE = DESCRIPTOR.enum_types_by_name['DeploymentHostingServiceType']
 DeploymentHostingServiceType = enum_type_wrapper.EnumTypeWrapper(_DEPLOYMENTHOSTINGSERVICETYPE)
 _KUBEDEPLOYMENTTYPE = DESCRIPTOR.enum_types_by_name['KubeDeploymentType']
 KubeDeploymentType = enum_type_wrapper.EnumTypeWrapper(_KUBEDEPLOYMENTTYPE)
@@ -428,42 +428,50 @@
   DESCRIPTOR._serialized_options = b'\n%com.qwak.ai.management.deployment.apiP\001Z\032qwak/deployment;deployment'
   _HOSTINGSERVICE.fields_by_name['sagemaker']._options = None
   _HOSTINGSERVICE.fields_by_name['sagemaker']._serialized_options = b'\030\001'
   _KUBEDEPLOYMENT_ENVIRONMENTVARIABLESENTRY._options = None
   _KUBEDEPLOYMENT_ENVIRONMENTVARIABLESENTRY._serialized_options = b'8\001'
   _KUBEDEPLOYMENT.fields_by_name['pod_count']._options = None
   _KUBEDEPLOYMENT.fields_by_name['pod_count']._serialized_options = b'\030\001'
+  _DEPLOYMENTSIZE.fields_by_name['cpu']._options = None
+  _DEPLOYMENTSIZE.fields_by_name['cpu']._serialized_options = b'\030\001'
+  _DEPLOYMENTSIZE.fields_by_name['memory_amount']._options = None
+  _DEPLOYMENTSIZE.fields_by_name['memory_amount']._serialized_options = b'\030\001'
+  _DEPLOYMENTSIZE.fields_by_name['memory_units']._options = None
+  _DEPLOYMENTSIZE.fields_by_name['memory_units']._serialized_options = b'\030\001'
+  _DEPLOYMENTSIZE.fields_by_name['gpu_resources']._options = None
+  _DEPLOYMENTSIZE.fields_by_name['gpu_resources']._serialized_options = b'\030\001'
   _DEPLOYMENTDETAILS_ENVIRONMENTVARIABLESENTRY._options = None
   _DEPLOYMENTDETAILS_ENVIRONMENTVARIABLESENTRY._serialized_options = b'8\001'
   _KUBERNETESMODELDEPLOYMENTSTATE.fields_by_name['branch_id']._options = None
   _KUBERNETESMODELDEPLOYMENTSTATE.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _ENVIRONMENTDEPLOYMENTMESSAGE.fields_by_name['branch_id']._options = None
   _ENVIRONMENTDEPLOYMENTMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _ENVIRONMENTDEPLOYMENTMESSAGE.fields_by_name['model_uuid']._options = None
   _ENVIRONMENTDEPLOYMENTMESSAGE.fields_by_name['model_uuid']._serialized_options = b'\030\001'
   _ENVIRONMENTUNDEPLOYMENTMESSAGE.fields_by_name['branch_id']._options = None
   _ENVIRONMENTUNDEPLOYMENTMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE.fields_by_name['branch_id']._options = None
   _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._options = None
   _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_options = b'8\001'
-  _MODELDEPLOYMENTSTATUS._serialized_start=7852
-  _MODELDEPLOYMENTSTATUS._serialized_end=8181
-  _DEPLOYMENTHOSTINGSERVICETYPE._serialized_start=8183
-  _DEPLOYMENTHOSTINGSERVICETYPE._serialized_end=8262
-  _KUBEDEPLOYMENTTYPE._serialized_start=8264
-  _KUBEDEPLOYMENTTYPE._serialized_end=8334
-  _GPUTYPE._serialized_start=8336
-  _GPUTYPE._serialized_end=8444
-  _MEMORYUNIT._serialized_start=8446
-  _MEMORYUNIT._serialized_end=8489
-  _DEPLOYMENTMANAGEDBY._serialized_start=8492
-  _DEPLOYMENTMANAGEDBY._serialized_end=8623
-  _DEPLOYMENTFAILUREREASONCODE._serialized_start=8626
-  _DEPLOYMENTFAILUREREASONCODE._serialized_end=8901
+  _MODELDEPLOYMENTSTATUS._serialized_start=7966
+  _MODELDEPLOYMENTSTATUS._serialized_end=8295
+  _DEPLOYMENTHOSTINGSERVICETYPE._serialized_start=8297
+  _DEPLOYMENTHOSTINGSERVICETYPE._serialized_end=8376
+  _KUBEDEPLOYMENTTYPE._serialized_start=8378
+  _KUBEDEPLOYMENTTYPE._serialized_end=8448
+  _GPUTYPE._serialized_start=8450
+  _GPUTYPE._serialized_end=8558
+  _MEMORYUNIT._serialized_start=8560
+  _MEMORYUNIT._serialized_end=8603
+  _DEPLOYMENTMANAGEDBY._serialized_start=8606
+  _DEPLOYMENTMANAGEDBY._serialized_end=8737
+  _DEPLOYMENTFAILUREREASONCODE._serialized_start=8740
+  _DEPLOYMENTFAILUREREASONCODE._serialized_end=9015
   _HOSTINGSERVICE._serialized_start=253
   _HOSTINGSERVICE._serialized_end=411
   _KUBEDEPLOYMENT._serialized_start=414
   _KUBEDEPLOYMENT._serialized_end=925
   _KUBEDEPLOYMENT_ENVIRONMENTVARIABLESENTRY._serialized_start=866
   _KUBEDEPLOYMENT_ENVIRONMENTVARIABLESENTRY._serialized_end=925
   _SERVINGSTRATEGY._serialized_start=928
@@ -485,69 +493,69 @@
   _KAFKACONFIG_PRODUCER._serialized_start=2069
   _KAFKACONFIG_PRODUCER._serialized_end=2303
   _KAFKACONFIG_PRODUCER_COMPRESSIONTYPE._serialized_start=2214
   _KAFKACONFIG_PRODUCER_COMPRESSIONTYPE._serialized_end=2303
   _SAGEMAKER._serialized_start=2305
   _SAGEMAKER._serialized_end=2363
   _DEPLOYMENTSIZE._serialized_start=2366
-  _DEPLOYMENTSIZE._serialized_end=2574
-  _GPURESOURCES._serialized_start=2576
-  _GPURESOURCES._serialized_end=2665
-  _ADVANCEDDEPLOYMENTOPTIONS._serialized_start=2668
-  _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=2936
-  _DEPLOYMENTDETAILS._serialized_start=2939
-  _DEPLOYMENTDETAILS._serialized_end=3891
+  _DEPLOYMENTSIZE._serialized_end=2688
+  _GPURESOURCES._serialized_start=2690
+  _GPURESOURCES._serialized_end=2779
+  _ADVANCEDDEPLOYMENTOPTIONS._serialized_start=2782
+  _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=3050
+  _DEPLOYMENTDETAILS._serialized_start=3053
+  _DEPLOYMENTDETAILS._serialized_end=4005
   _DEPLOYMENTDETAILS_ENVIRONMENTVARIABLESENTRY._serialized_start=866
   _DEPLOYMENTDETAILS_ENVIRONMENTVARIABLESENTRY._serialized_end=925
-  _RUNTIMEDEPLOYMENTSETTINGS._serialized_start=3894
-  _RUNTIMEDEPLOYMENTSETTINGS._serialized_end=4079
-  _RUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_start=4014
-  _RUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_end=4079
-  _DEPLOYMENTBRIEF._serialized_start=4082
-  _DEPLOYMENTBRIEF._serialized_end=4392
-  _KUBERNETESMODELDEPLOYMENTSTATE._serialized_start=4395
-  _KUBERNETESMODELDEPLOYMENTSTATE._serialized_end=4738
-  _STATUSDETAILS._serialized_start=4741
-  _STATUSDETAILS._serialized_end=5027
-  _PENDINGSTATUSDETAILS._serialized_start=5030
-  _PENDINGSTATUSDETAILS._serialized_end=5186
-  _SUCCESSFULSTATUSDETAILS._serialized_start=5188
-  _SUCCESSFULSTATUSDETAILS._serialized_end=5284
-  _FAILEDSTATUSDETAILS._serialized_start=5287
-  _FAILEDSTATUSDETAILS._serialized_end=5514
-  _FAILUREDETAILS._serialized_start=5517
-  _FAILUREDETAILS._serialized_end=5662
-  _INSTANCEDETAILS._serialized_start=5664
-  _INSTANCEDETAILS._serialized_end=5750
-  _VARIATION._serialized_start=5752
-  _VARIATION._serialized_end=5869
-  _TRAFFICSPEC._serialized_start=5871
-  _TRAFFICSPEC._serialized_end=5923
-  _FUTUREDEPLOYMENTSETTINGS._serialized_start=5925
-  _FUTUREDEPLOYMENTSETTINGS._serialized_end=6018
-  _ENVIRONMENTDEPLOYMENTMESSAGE._serialized_start=6021
-  _ENVIRONMENTDEPLOYMENTMESSAGE._serialized_end=6203
-  _ENVIRONMENTDEPLOYMENTRESULTMESSAGE._serialized_start=6206
-  _ENVIRONMENTDEPLOYMENTRESULTMESSAGE._serialized_end=6352
-  _ENVIRONMENTUNDEPLOYMENTMESSAGE._serialized_start=6355
-  _ENVIRONMENTUNDEPLOYMENTMESSAGE._serialized_end=6627
-  _ENVIRONMENTUNDEPLOYMENTRESULTMESSAGE._serialized_start=6629
-  _ENVIRONMENTUNDEPLOYMENTRESULTMESSAGE._serialized_end=6748
-  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE._serialized_start=6751
-  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE._serialized_end=6965
-  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSRESULTMESSAGE._serialized_start=6967
-  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSRESULTMESSAGE._serialized_end=7038
-  _ENVIRONMENTAPPLYMODELTRAFFICRESPONSE._serialized_start=7040
-  _ENVIRONMENTAPPLYMODELTRAFFICRESPONSE._serialized_end=7092
-  _ENVIRONMENTDEPLOYMENTDETAILSMESSAGE._serialized_start=7095
-  _ENVIRONMENTDEPLOYMENTDETAILSMESSAGE._serialized_end=7301
-  _ENVIRONMENTDEPLOYMENTHISTORYMESSAGE._serialized_start=7303
-  _ENVIRONMENTDEPLOYMENTHISTORYMESSAGE._serialized_end=7406
-  _ENVIRONMENTTRAFFICMESSAGE._serialized_start=7408
-  _ENVIRONMENTTRAFFICMESSAGE._serialized_end=7494
-  _BUILDDEPLOYMENTENVIRONMENTSTATUS._serialized_start=7497
-  _BUILDDEPLOYMENTENVIRONMENTSTATUS._serialized_end=7783
-  _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_start=7671
-  _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_end=7783
-  _BUILDDEPLOYMENTSTATUS._serialized_start=7785
-  _BUILDDEPLOYMENTSTATUS._serialized_end=7849
+  _RUNTIMEDEPLOYMENTSETTINGS._serialized_start=4008
+  _RUNTIMEDEPLOYMENTSETTINGS._serialized_end=4193
+  _RUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_start=4128
+  _RUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_end=4193
+  _DEPLOYMENTBRIEF._serialized_start=4196
+  _DEPLOYMENTBRIEF._serialized_end=4506
+  _KUBERNETESMODELDEPLOYMENTSTATE._serialized_start=4509
+  _KUBERNETESMODELDEPLOYMENTSTATE._serialized_end=4852
+  _STATUSDETAILS._serialized_start=4855
+  _STATUSDETAILS._serialized_end=5141
+  _PENDINGSTATUSDETAILS._serialized_start=5144
+  _PENDINGSTATUSDETAILS._serialized_end=5300
+  _SUCCESSFULSTATUSDETAILS._serialized_start=5302
+  _SUCCESSFULSTATUSDETAILS._serialized_end=5398
+  _FAILEDSTATUSDETAILS._serialized_start=5401
+  _FAILEDSTATUSDETAILS._serialized_end=5628
+  _FAILUREDETAILS._serialized_start=5631
+  _FAILUREDETAILS._serialized_end=5776
+  _INSTANCEDETAILS._serialized_start=5778
+  _INSTANCEDETAILS._serialized_end=5864
+  _VARIATION._serialized_start=5866
+  _VARIATION._serialized_end=5983
+  _TRAFFICSPEC._serialized_start=5985
+  _TRAFFICSPEC._serialized_end=6037
+  _FUTUREDEPLOYMENTSETTINGS._serialized_start=6039
+  _FUTUREDEPLOYMENTSETTINGS._serialized_end=6132
+  _ENVIRONMENTDEPLOYMENTMESSAGE._serialized_start=6135
+  _ENVIRONMENTDEPLOYMENTMESSAGE._serialized_end=6317
+  _ENVIRONMENTDEPLOYMENTRESULTMESSAGE._serialized_start=6320
+  _ENVIRONMENTDEPLOYMENTRESULTMESSAGE._serialized_end=6466
+  _ENVIRONMENTUNDEPLOYMENTMESSAGE._serialized_start=6469
+  _ENVIRONMENTUNDEPLOYMENTMESSAGE._serialized_end=6741
+  _ENVIRONMENTUNDEPLOYMENTRESULTMESSAGE._serialized_start=6743
+  _ENVIRONMENTUNDEPLOYMENTRESULTMESSAGE._serialized_end=6862
+  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE._serialized_start=6865
+  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE._serialized_end=7079
+  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSRESULTMESSAGE._serialized_start=7081
+  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSRESULTMESSAGE._serialized_end=7152
+  _ENVIRONMENTAPPLYMODELTRAFFICRESPONSE._serialized_start=7154
+  _ENVIRONMENTAPPLYMODELTRAFFICRESPONSE._serialized_end=7206
+  _ENVIRONMENTDEPLOYMENTDETAILSMESSAGE._serialized_start=7209
+  _ENVIRONMENTDEPLOYMENTDETAILSMESSAGE._serialized_end=7415
+  _ENVIRONMENTDEPLOYMENTHISTORYMESSAGE._serialized_start=7417
+  _ENVIRONMENTDEPLOYMENTHISTORYMESSAGE._serialized_end=7520
+  _ENVIRONMENTTRAFFICMESSAGE._serialized_start=7522
+  _ENVIRONMENTTRAFFICMESSAGE._serialized_end=7608
+  _BUILDDEPLOYMENTENVIRONMENTSTATUS._serialized_start=7611
+  _BUILDDEPLOYMENTENVIRONMENTSTATUS._serialized_end=7897
+  _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_start=7785
+  _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_end=7897
+  _BUILDDEPLOYMENTSTATUS._serialized_start=7899
+  _BUILDDEPLOYMENTSTATUS._serialized_end=7963
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -532,36 +532,41 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NUMBER_OF_PODS_FIELD_NUMBER: builtins.int
     CPU_FIELD_NUMBER: builtins.int
     MEMORY_AMOUNT_FIELD_NUMBER: builtins.int
     MEMORY_UNITS_FIELD_NUMBER: builtins.int
     GPU_RESOURCES_FIELD_NUMBER: builtins.int
+    CLIENT_POD_COMPUTE_RESOURCES_FIELD_NUMBER: builtins.int
     number_of_pods: builtins.int
     """Count of pods to deploy."""
     cpu: builtins.float
     """Amount of CPU cores"""
     memory_amount: builtins.int
     """Amount of memory"""
     memory_units: global___MemoryUnit.ValueType
     """Units type of memory"""
     @property
     def gpu_resources(self) -> qwak.user_application.common.v0.resources_pb2.GpuResources:
         """GPU Resource for deployed model"""
+    @property
+    def client_pod_compute_resources(self) -> qwak.user_application.common.v0.resources_pb2.ClientPodComputeResources:
+        """Deployment pod compute resources"""
     def __init__(
         self,
         *,
         number_of_pods: builtins.int = ...,
         cpu: builtins.float = ...,
         memory_amount: builtins.int = ...,
         memory_units: global___MemoryUnit.ValueType = ...,
         gpu_resources: qwak.user_application.common.v0.resources_pb2.GpuResources | None = ...,
+        client_pod_compute_resources: qwak.user_application.common.v0.resources_pb2.ClientPodComputeResources | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cpu", b"cpu", "gpu_resources", b"gpu_resources", "memory_amount", b"memory_amount", "memory_units", b"memory_units", "number_of_pods", b"number_of_pods"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["client_pod_compute_resources", b"client_pod_compute_resources", "gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_pod_compute_resources", b"client_pod_compute_resources", "cpu", b"cpu", "gpu_resources", b"gpu_resources", "memory_amount", b"memory_amount", "memory_units", b"memory_units", "number_of_pods", b"number_of_pods"]) -> None: ...
 
 global___DeploymentSize = DeploymentSize
 
 class GpuResources(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GPU_TYPE_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/pyproject.toml` & `qwak_core-0.0.60/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.59"
+version = "0.0.60"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.59/qwak/automations/__init__.py` & `qwak_core-0.0.60/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/automations/automation_executions.py` & `qwak_core-0.0.60/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/automations/automations.py` & `qwak_core-0.0.60/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.60/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.60/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.60/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.60/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.60/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/alert_management/client.py` & `qwak_core-0.0.60/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/analytics/client.py` & `qwak_core-0.0.60/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/audience/client.py` & `qwak_core-0.0.60/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/automation_management/client.py` & `qwak_core-0.0.60/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.60/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.60/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.60/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.60/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/build_management/client.py` & `qwak_core-0.0.60/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.60/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.60/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/deployment/client.py` & `qwak_core-0.0.60/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.60/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.60/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.60/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.60/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.60/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/logging_client/client.py` & `qwak_core-0.0.60/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/model_management/client.py` & `qwak_core-0.0.60/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/project/client.py` & `qwak_core-0.0.60/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/secret_service/client.py` & `qwak_core-0.0.60/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.60/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.60/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.60/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.60/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.60/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.60/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.60/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.60/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.60/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.60/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.60/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.60/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.60/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.60/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/offline/client.py` & `qwak_core-0.0.60/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/feature_store/online/client.py` & `qwak_core-0.0.60/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/const.py` & `qwak_core-0.0.60/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.60/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.60/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.60/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.60/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/singleton_meta.py` & `qwak_core-0.0.60/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/tool/auth.py` & `qwak_core-0.0.60/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.60/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.60/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/adapters/__init__.py` & `qwak_core-0.0.60/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.60/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.60/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.60/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.60/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.60/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/base.py` & `qwak_core-0.0.60/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/decorators/api.py` & `qwak_core-0.0.60/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.60/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/experiment_tracking.py` & `qwak_core-0.0.60/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/schema.py` & `qwak_core-0.0.60/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/schema_entities.py` & `qwak_core-0.0.60/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.60/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.60/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.60/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.60/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.60/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.60/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.60/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/qwak_client/client.py` & `qwak_core-0.0.60/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.60/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/qwak_client/models/model.py` & `qwak_core-0.0.60/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.60/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.60/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/tools/logger/logger.py` & `qwak_core-0.0.60/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak/tools/logger/logging.yml` & `qwak_core-0.0.60/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.60/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/qwak_services_mock/services_mock.py` & `qwak_core-0.0.60/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.59/setup.py` & `qwak_core-0.0.60/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.59',
+    'version': '0.0.60',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.59/PKG-INFO` & `qwak_core-0.0.60/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.59
+Version: 0.0.60
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

