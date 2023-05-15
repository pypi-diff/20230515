# Comparing `tmp/qwak_core-0.0.57.tar.gz` & `tmp/qwak_core-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.57.tar", max compression
+gzip compressed data, was "qwak_core-0.0.58.tar", max compression
```

## Comparing `qwak_core-0.0.57.tar` & `qwak_core-0.0.58.tar`

### file list

```diff
@@ -1,570 +1,570 @@
--rw-r--r--   0        0        0      264 2023-05-14 07:55:13.079099 qwak_core-0.0.57/README.md
--rw-r--r--   0        0        0        0 2023-05-14 07:57:00.979793 qwak_core-0.0.57/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-14 07:57:01.007793 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-14 07:56:38.379647 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.007793 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-14 07:57:01.003793 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-14 07:56:37.999645 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.003793 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-14 07:57:01.007793 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-14 07:56:38.187646 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.007793 qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-14 07:57:00.995793 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-14 07:56:37.435641 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-14 07:57:00.995793 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-14 07:57:00.999793 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-14 07:56:37.623642 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:00.999793 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-14 07:57:00.999793 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-14 07:56:37.811643 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.003793 qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-14 07:57:00.979793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-14 07:56:37.239640 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-14 07:57:00.983793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-14 07:57:00.983793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-14 07:56:38.571648 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:00.983793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-14 07:57:00.987793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-14 07:56:38.947651 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:00.987793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-14 07:57:00.991793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-14 07:56:39.139652 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-14 07:57:00.991793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-14 07:57:00.987793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-14 07:56:38.759649 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:00.987793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-14 07:57:00.991793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-14 07:56:39.331653 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:00.995793 qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-14 07:57:01.039793 qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-14 07:56:42.139671 qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.043793 qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-14 07:57:01.043793 qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-14 07:56:42.335672 qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-14 07:57:01.043793 qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-14 07:57:01.219794 qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-14 07:56:48.143710 qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.223795 qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-14 07:57:01.223795 qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-14 07:56:48.339711 qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-14 07:57:01.223795 qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-14 07:57:01.227795 qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-14 07:56:49.331718 qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-14 07:57:01.231794 qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-14 07:57:01.227795 qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-14 07:56:49.127716 qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.227795 qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-14 07:57:01.231794 qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-14 07:56:49.527719 qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.231794 qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-14 07:57:01.231794 qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-14 07:56:49.727720 qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-14 07:57:01.235795 qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-14 07:57:01.379795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-14 07:56:58.171775 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.379795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-14 07:57:01.367795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-14 07:56:57.779772 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.375795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-14 07:57:01.375795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-14 07:56:57.971773 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.379795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-14 07:57:01.359795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-14 07:56:57.371770 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-14 07:57:01.363795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-14 07:57:01.363795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-14 07:56:57.583771 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.367795 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-14 07:57:01.387796 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-14 07:56:58.779779 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.387796 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-14 07:57:01.383796 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-14 07:56:58.583778 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.387796 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-14 07:57:01.383796 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-14 07:56:58.383776 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.383796 qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-14 07:57:01.355795 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-14 07:56:57.151768 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.359795 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-14 07:57:01.343795 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-14 07:56:56.731766 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.343795 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-14 07:57:01.351795 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-14 07:56:56.947767 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-14 07:57:01.355795 qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-14 07:57:01.287795 qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-14 07:56:51.895734 qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-14 07:57:01.291795 qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-14 07:57:01.279795 qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-14 07:56:51.691733 qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.287795 qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-14 07:57:01.267795 qwak_core-0.0.57/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-14 07:56:51.231730 qwak_core-0.0.57/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.271795 qwak_core-0.0.57/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-14 07:57:01.271795 qwak_core-0.0.57/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-14 07:56:51.459731 qwak_core-0.0.57/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.275795 qwak_core-0.0.57/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-14 07:57:01.275795 qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-14 07:56:52.103736 qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-14 07:57:01.275795 qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-14 07:57:01.279795 qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-14 07:56:52.571739 qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-14 07:57:01.279795 qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-14 07:57:01.299795 qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-14 07:56:52.999741 qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.303795 qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-14 07:57:01.303795 qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-14 07:56:53.203743 qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-14 07:57:01.303795 qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-14 07:57:01.243795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-14 07:56:50.595726 qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.243795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-14 07:57:01.259795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-14 07:56:50.795727 qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-14 07:57:01.259795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-14 07:57:01.239795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-14 07:56:50.171723 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.239795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-05-14 07:57:01.235795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-05-14 07:56:49.963722 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.235795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-14 07:57:01.239795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-14 07:56:50.387724 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-14 07:57:01.243795 qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-14 07:57:01.027793 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-14 07:56:41.119665 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.031793 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-14 07:57:01.031793 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-14 07:56:41.315666 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.031793 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-14 07:57:01.035793 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-14 07:56:41.539667 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-14 07:57:01.035793 qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-14 07:57:01.199794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-14 07:56:46.919702 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.199794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-14 07:57:01.195794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-14 07:56:46.719701 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-14 07:57:01.195794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-14 07:57:01.171794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-14 07:56:44.823689 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.175794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-14 07:57:01.171794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-14 07:56:44.603687 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.171794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-14 07:57:01.155794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-14 07:56:43.939683 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.155794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-14 07:57:01.167794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-14 07:56:44.403686 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-14 07:57:01.167794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-14 07:57:01.175794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-14 07:56:45.023690 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.175794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-14 07:57:01.175794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-14 07:56:45.235691 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-14 07:57:01.179794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25213 2023-05-14 07:57:01.159794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37366 2023-05-14 07:56:44.187685 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.159794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-14 07:57:01.179794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-14 07:56:45.459693 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.179794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     5958 2023-05-14 07:57:01.183794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
--rw-r--r--   0        0        0     6232 2023-05-14 07:56:45.655694 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.183794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-14 07:57:01.199794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-14 07:57:00.231788 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.203794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-14 07:57:01.203794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-14 07:57:00.463790 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-14 07:57:01.203794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-14 07:57:01.207794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-14 07:56:47.547706 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.207794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-14 07:57:01.207794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-14 07:56:47.747707 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-14 07:57:01.207794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-14 07:57:01.211794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-14 07:56:47.943709 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.211794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-14 07:57:01.215794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-14 07:56:48.735714 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.215794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-14 07:57:01.211794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-14 07:56:48.535713 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-14 07:57:01.215794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-14 07:57:01.219794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-14 07:56:48.931715 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.219794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-14 07:57:01.183794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-14 07:56:45.859695 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.187794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-14 07:57:01.187794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-14 07:56:46.079697 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.187794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-14 07:57:01.191794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-14 07:56:46.295698 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-14 07:57:01.191794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-14 07:57:01.191794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-14 07:56:46.503699 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.195794 qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-14 07:57:01.391795 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-14 07:56:58.979780 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.391795 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-14 07:57:01.391795 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-14 07:56:59.183781 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-14 07:57:01.395796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-14 07:57:01.395796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-14 07:56:59.371783 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.395796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-14 07:57:01.399796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-14 07:56:59.579784 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-14 07:57:01.399796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-14 07:57:01.399796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-14 07:56:59.815786 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-14 07:57:01.399796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-14 07:57:01.403796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-14 07:57:00.007787 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.403796 qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-14 07:57:01.307795 qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-14 07:56:53.407744 qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.307795 qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-14 07:57:01.307795 qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-14 07:56:53.607745 qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-14 07:57:01.311795 qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-14 07:57:01.071793 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-14 07:56:43.127678 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.083793 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-14 07:57:01.095794 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-14 07:56:43.323679 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.103794 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-14 07:57:01.115794 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-14 07:56:43.523680 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-14 07:57:01.127794 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-14 07:57:01.135794 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-14 07:56:43.727681 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.147794 qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-14 07:57:01.263795 qwak_core-0.0.57/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-14 07:56:51.003728 qwak_core-0.0.57/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-14 07:57:01.263795 qwak_core-0.0.57/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-14 07:57:01.323795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-14 07:56:54.883754 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.323795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-14 07:57:01.323795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-14 07:56:55.083755 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.327795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-14 07:57:01.327795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-14 07:56:55.295756 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.327795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-14 07:57:01.327795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-14 07:56:55.511758 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.331795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-14 07:57:01.331795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-14 07:56:55.715759 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.331795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-14 07:57:01.335795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-14 07:56:55.931760 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-14 07:57:01.335795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-14 07:57:01.335795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-14 07:56:56.127762 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.339795 qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-14 07:57:01.311795 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-14 07:56:54.031748 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.315795 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-14 07:57:01.319795 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-14 07:56:54.675752 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.319795 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-14 07:57:01.315795 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-14 07:56:54.231749 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-14 07:57:01.315795 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-14 07:57:01.319795 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-14 07:56:54.471751 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.319795 qwak_core-0.0.57/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-14 07:57:01.295795 qwak_core-0.0.57/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-14 07:56:52.787740 qwak_core-0.0.57/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-14 07:57:01.295795 qwak_core-0.0.57/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-14 07:57:01.023793 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-14 07:56:42.723675 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-14 07:57:01.027793 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-14 07:57:01.023793 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-14 07:56:42.527674 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.023793 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-14 07:57:01.027793 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-14 07:56:42.919676 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-14 07:57:01.027793 qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-14 07:57:01.291795 qwak_core-0.0.57/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-14 07:56:52.331737 qwak_core-0.0.57/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-14 07:57:01.295795 qwak_core-0.0.57/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-14 07:57:01.311795 qwak_core-0.0.57/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-14 07:56:53.807747 qwak_core-0.0.57/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-14 07:57:01.311795 qwak_core-0.0.57/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-14 07:57:01.019793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-14 07:56:40.319660 qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.019793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-14 07:57:01.019793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-14 07:56:40.119658 qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-14 07:57:01.019793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-14 07:57:01.011793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-14 07:56:39.519654 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.011793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-14 07:57:01.011793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-14 07:56:39.719656 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.015793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-14 07:57:01.015793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-14 07:56:39.919657 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-14 07:57:01.015793 qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-14 07:57:01.339795 qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-14 07:56:56.535764 qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-14 07:57:01.343795 qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-14 07:57:01.339795 qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-14 07:56:56.335763 qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.339795 qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    12481 2023-05-14 07:57:01.035793 qwak_core-0.0.57/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    16473 2023-05-14 07:56:41.739669 qwak_core-0.0.57/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.035793 qwak_core-0.0.57/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-14 07:57:01.039793 qwak_core-0.0.57/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-14 07:56:41.939670 qwak_core-0.0.57/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-14 07:57:01.039793 qwak_core-0.0.57/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-14 07:57:06.207827 qwak_core-0.0.57/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-14 07:57:06.211827 qwak_core-0.0.57/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-14 07:55:13.079099 qwak_core-0.0.57/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-14 07:55:13.083099 qwak_core-0.0.57/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-14 07:55:13.087099 qwak_core-0.0.57/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.57/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.57/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-15 09:01:31.084706 qwak_core-0.0.58/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 09:03:24.689365 qwak_core-0.0.58/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-15 09:03:24.713365 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-15 09:03:01.973231 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.717365 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-15 09:03:24.709365 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-15 09:03:01.565228 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.713365 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-15 09:03:24.713365 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-15 09:03:01.765229 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.713365 qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-15 09:03:24.705365 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-15 09:03:00.965225 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-15 09:03:24.705365 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-15 09:03:24.705365 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-15 09:03:01.165226 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.705365 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-15 09:03:24.709365 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-15 09:03:01.365227 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.709365 qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-15 09:03:24.689365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-15 09:03:00.765224 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-15 09:03:24.689365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-15 09:03:24.693365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-15 09:03:02.181232 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.693365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-15 09:03:24.697365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-15 09:03:02.585234 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.697365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-15 09:03:24.697365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-15 09:03:02.797235 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-15 09:03:24.701365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-15 09:03:24.693365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-15 09:03:02.385233 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.693365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-15 09:03:24.701365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-15 09:03:03.021237 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.701365 qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-15 09:03:24.749365 qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-15 09:03:06.209255 qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.749365 qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-15 09:03:24.753365 qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-15 09:03:06.429256 qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-15 09:03:24.753365 qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-15 09:03:24.853366 qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-15 09:03:12.293290 qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.853366 qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-15 09:03:24.853366 qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-15 09:03:12.501291 qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-15 09:03:24.857366 qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-15 09:03:24.857366 qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-15 09:03:13.529297 qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-15 09:03:24.861366 qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-15 09:03:24.857366 qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-15 09:03:13.329296 qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.857366 qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-15 09:03:24.861366 qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-15 09:03:13.729298 qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.861366 qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-15 09:03:24.865366 qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-15 09:03:13.925299 qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-15 09:03:24.865366 qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-15 09:03:24.961367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-15 09:03:22.209350 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.961367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-15 09:03:24.957367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-15 09:03:21.813347 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.957367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-15 09:03:24.957367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-15 09:03:22.005348 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.961367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-15 09:03:24.949366 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-15 09:03:21.417344 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-15 09:03:24.953367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-15 09:03:24.953367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-15 09:03:21.617346 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.953367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-15 09:03:24.969367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-15 09:03:22.809353 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.969367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-15 09:03:24.965367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-15 09:03:22.609352 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.969367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-15 09:03:24.965367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-15 09:03:22.409351 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.965367 qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-15 09:03:24.949366 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-15 09:03:21.217343 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.949366 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-15 09:03:24.941367 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-15 09:03:20.801340 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.945366 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-15 09:03:24.945366 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-15 09:03:21.013342 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-15 09:03:24.945366 qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-15 09:03:24.893366 qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-15 09:03:16.097312 qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-15 09:03:24.893366 qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-15 09:03:24.889366 qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-15 09:03:15.893310 qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.893366 qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-15 09:03:24.881366 qwak_core-0.0.58/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-15 09:03:15.429308 qwak_core-0.0.58/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.881366 qwak_core-0.0.58/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-15 09:03:24.885366 qwak_core-0.0.58/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-15 09:03:15.633309 qwak_core-0.0.58/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.885366 qwak_core-0.0.58/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-15 09:03:24.885366 qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-15 09:03:16.301313 qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-15 09:03:24.885366 qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-15 09:03:24.889366 qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-15 09:03:16.745315 qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-15 09:03:24.889366 qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-15 09:03:24.901366 qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-15 09:03:17.169318 qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.901366 qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-15 09:03:24.905366 qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-15 09:03:17.369319 qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-15 09:03:24.905366 qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-15 09:03:24.873366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-15 09:03:14.821304 qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.873366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-15 09:03:24.877366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-15 09:03:15.021305 qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-15 09:03:24.877366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-15 09:03:24.869366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-15 09:03:14.349302 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.869366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-05-15 09:03:24.865366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-05-15 09:03:14.133300 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.869366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-15 09:03:24.869366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-15 09:03:14.569303 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-15 09:03:24.873366 qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-15 09:03:24.737365 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-15 09:03:05.037248 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.737365 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-15 09:03:24.737365 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-15 09:03:05.305250 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.737365 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-15 09:03:24.741365 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-15 09:03:05.529251 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-15 09:03:24.741365 qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-15 09:03:24.829366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-15 09:03:11.101283 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.833366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-15 09:03:24.829366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-15 09:03:10.909282 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-15 09:03:24.829366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-15 09:03:24.809366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-15 09:03:09.089271 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.809366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-15 09:03:24.805366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-15 09:03:08.889270 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.805366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-15 09:03:24.773366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-15 09:03:08.233266 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.773366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-15 09:03:24.801366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-15 09:03:08.681269 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-15 09:03:24.805366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-15 09:03:24.809366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-15 09:03:09.285272 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.809366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-15 09:03:24.813366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-15 09:03:09.501274 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-15 09:03:24.813366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25213 2023-05-15 09:03:24.773366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37366 2023-05-15 09:03:08.469268 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.801366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-15 09:03:24.813366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-15 09:03:09.701275 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.817366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     5958 2023-05-15 09:03:24.817366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
+-rw-r--r--   0        0        0     6232 2023-05-15 09:03:09.901276 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.817366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-15 09:03:24.833366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-15 09:03:24.189362 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.833366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-15 09:03:24.837366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-15 09:03:24.385363 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-15 09:03:24.837366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-15 09:03:24.837366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-15 09:03:11.685286 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.837366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-15 09:03:24.841366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-15 09:03:11.893288 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-15 09:03:24.841366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-15 09:03:24.841366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-15 09:03:12.093289 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.845366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-15 09:03:24.845366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-15 09:03:12.913293 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.849366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-15 09:03:24.845366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-15 09:03:12.705292 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-15 09:03:24.845366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-15 09:03:24.849366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-15 09:03:13.113294 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.849366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-15 09:03:24.817366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-15 09:03:10.105277 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.821366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-15 09:03:24.821366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-15 09:03:10.309278 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.821366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-15 09:03:24.825366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-15 09:03:10.509280 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-15 09:03:24.825366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-15 09:03:24.825366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-15 09:03:10.701281 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.825366 qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-15 09:03:24.973367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-15 09:03:23.005355 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.973367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-15 09:03:24.977367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-15 09:03:23.205356 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-15 09:03:24.977367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-15 09:03:24.977367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-15 09:03:23.405357 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.981367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-15 09:03:24.981367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-15 09:03:23.605359 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-15 09:03:24.981367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-15 09:03:24.981367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-15 09:03:23.805360 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-15 09:03:24.985367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-15 09:03:24.985367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-15 09:03:23.997361 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.985367 qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-15 09:03:24.905366 qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-15 09:03:17.565320 qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.905366 qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-15 09:03:24.909366 qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-15 09:03:17.769321 qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-15 09:03:24.909366 qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-15 09:03:24.757365 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-15 09:03:07.329261 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.757365 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-15 09:03:24.761366 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-15 09:03:07.533263 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.761366 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-15 09:03:24.765365 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-15 09:03:07.769264 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-15 09:03:24.765365 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-15 09:03:24.769365 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-15 09:03:08.009265 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.769365 qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-15 09:03:24.877366 qwak_core-0.0.58/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-15 09:03:15.225307 qwak_core-0.0.58/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-15 09:03:24.881366 qwak_core-0.0.58/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-15 09:03:24.921366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-15 09:03:18.977329 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.921366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-15 09:03:24.925366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-15 09:03:19.177330 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.925366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-15 09:03:24.925366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-15 09:03:19.377331 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.929366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-15 09:03:24.929366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-15 09:03:19.577333 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.929366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-15 09:03:24.929366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-15 09:03:19.789334 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.933366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-15 09:03:24.933366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-15 09:03:20.009335 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-15 09:03:24.933366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-15 09:03:24.937366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-15 09:03:20.209337 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.937366 qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-15 09:03:24.913366 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-15 09:03:18.157323 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.913366 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-15 09:03:24.921366 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-15 09:03:18.777327 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.921366 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-15 09:03:24.913366 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-15 09:03:18.369325 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-15 09:03:24.917366 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-15 09:03:24.917366 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-15 09:03:18.577326 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.917366 qwak_core-0.0.58/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-15 09:03:24.897366 qwak_core-0.0.58/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-15 09:03:16.965317 qwak_core-0.0.58/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-15 09:03:24.901366 qwak_core-0.0.58/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-15 09:03:24.729365 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-15 09:03:06.889259 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-15 09:03:24.733365 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-15 09:03:24.729365 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-15 09:03:06.645257 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.729365 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-15 09:03:24.733365 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-15 09:03:07.121260 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-15 09:03:24.733365 qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-15 09:03:24.897366 qwak_core-0.0.58/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-15 09:03:16.521314 qwak_core-0.0.58/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-15 09:03:24.897366 qwak_core-0.0.58/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-15 09:03:24.909366 qwak_core-0.0.58/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-15 09:03:17.961322 qwak_core-0.0.58/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-15 09:03:24.913366 qwak_core-0.0.58/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-15 09:03:24.725365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-15 09:03:04.065243 qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.729365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-15 09:03:24.725365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-15 09:03:03.849241 qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-15 09:03:24.725365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-15 09:03:24.717365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-15 09:03:03.221238 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.717365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-15 09:03:24.721365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-15 09:03:03.437239 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.721365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-15 09:03:24.721365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-15 09:03:03.641240 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-15 09:03:24.721365 qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-15 09:03:24.941367 qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-15 09:03:20.601339 qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-15 09:03:24.941367 qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-15 09:03:24.937366 qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-15 09:03:20.405338 qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.941367 qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    12481 2023-05-15 09:03:24.745365 qwak_core-0.0.58/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    16473 2023-05-15 09:03:05.753252 qwak_core-0.0.58/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.745365 qwak_core-0.0.58/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-15 09:03:24.745365 qwak_core-0.0.58/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-15 09:03:05.985254 qwak_core-0.0.58/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-15 09:03:24.749365 qwak_core-0.0.58/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-15 09:03:26.837377 qwak_core-0.0.58/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-15 09:03:26.837377 qwak_core-0.0.58/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-15 09:01:31.084706 qwak_core-0.0.58/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-15 09:01:31.088707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-15 09:01:31.092707 qwak_core-0.0.58/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.58/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.58/PKG-INFO
```

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.58/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.58/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/pyproject.toml` & `qwak_core-0.0.58/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.57"
+version = "0.0.58"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.57/qwak/automations/__init__.py` & `qwak_core-0.0.58/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/automations/automation_executions.py` & `qwak_core-0.0.58/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/automations/automations.py` & `qwak_core-0.0.58/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.58/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.58/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.58/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.58/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.58/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/alert_management/client.py` & `qwak_core-0.0.58/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/analytics/client.py` & `qwak_core-0.0.58/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/audience/client.py` & `qwak_core-0.0.58/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/automation_management/client.py` & `qwak_core-0.0.58/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.58/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.58/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.58/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.58/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/build_management/client.py` & `qwak_core-0.0.58/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.58/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.58/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/deployment/client.py` & `qwak_core-0.0.58/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.58/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.58/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.58/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.58/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.58/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/logging_client/client.py` & `qwak_core-0.0.58/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/model_management/client.py` & `qwak_core-0.0.58/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/project/client.py` & `qwak_core-0.0.58/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/secret_service/client.py` & `qwak_core-0.0.58/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.58/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.58/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.58/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.58/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.58/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.58/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.58/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.58/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.58/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.58/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.58/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.58/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.58/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.58/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.58/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/offline/client.py` & `qwak_core-0.0.58/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/feature_store/online/client.py` & `qwak_core-0.0.58/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/const.py` & `qwak_core-0.0.58/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.58/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.58/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.58/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.58/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/singleton_meta.py` & `qwak_core-0.0.58/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/tool/auth.py` & `qwak_core-0.0.58/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.58/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.58/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.58/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.58/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/adapters/__init__.py` & `qwak_core-0.0.58/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.58/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.58/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.58/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.58/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.58/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/base.py` & `qwak_core-0.0.58/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/decorators/api.py` & `qwak_core-0.0.58/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.58/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/experiment_tracking.py` & `qwak_core-0.0.58/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/schema.py` & `qwak_core-0.0.58/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/schema_entities.py` & `qwak_core-0.0.58/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.58/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.58/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.58/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.58/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.58/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.58/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.58/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.58/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/qwak_client/client.py` & `qwak_core-0.0.58/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.58/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/qwak_client/models/model.py` & `qwak_core-0.0.58/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.58/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.58/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/tools/logger/logger.py` & `qwak_core-0.0.58/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak/tools/logger/logging.yml` & `qwak_core-0.0.58/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.58/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/qwak_services_mock/services_mock.py` & `qwak_core-0.0.58/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.57/setup.py` & `qwak_core-0.0.58/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.57',
+    'version': '0.0.58',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.57/PKG-INFO` & `qwak_core-0.0.58/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.57
+Version: 0.0.58
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

