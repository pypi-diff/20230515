# Comparing `tmp/geti-sdk-1.5.4.tar.gz` & `tmp/geti-sdk-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geti-sdk-1.5.4.tar", last modified: Thu May 11 12:22:26 2023, max compression
+gzip compressed data, was "geti-sdk-1.5.5.tar", last modified: Mon May 15 14:05:10 2023, max compression
```

## Comparing `geti-sdk-1.5.4.tar` & `geti-sdk-1.5.5.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.245659 geti-sdk-1.5.4/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/LICENSE
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/MANIFEST.in
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-11 12:22:26.245659 geti-sdk-1.5.4/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/README.md
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.225659 geti-sdk-1.5.4/geti_sdk/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.225659 geti-sdk-1.5.4/geti_sdk/annotation_readers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/annotation_readers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/annotation_readers/base_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.229659 geti-sdk-1.5.4/geti_sdk/annotation_readers/datumaro_annotation_reader/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/annotation_readers/geti_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.229659 geti-sdk-1.5.4/geti_sdk/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5033 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/algorithms.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/annotation_scene.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/annotations.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/code_deployment_info.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/configurable_parameter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/configurable_parameter_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/configuration.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/configuration_identifiers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.229659 geti-sdk-1.5.4/geti_sdk/data_models/containers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/containers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/containers/algorithm_list.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/containers/media_list.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.233659 geti-sdk-1.5.4/geti_sdk/data_models/enums/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/annotation_kind.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/configuration_enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/deployment_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/domain.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/job_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/job_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/media_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/model_status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      961 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/optimization_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/prediction_mode.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/shape_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/enums/task_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/job.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/label.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/media.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/media_identifiers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/model_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/performance.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/predictions.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/project.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/shapes.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/task.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/task_annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/data_models/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.233659 geti-sdk-1.5.4/geti_sdk/demos/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/constants.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.225659 geti-sdk-1.5.4/geti_sdk/demos/data/
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.233659 geti-sdk-1.5.4/geti_sdk/demos/data/example/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/data/example/dogs.png
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.233659 geti-sdk-1.5.4/geti_sdk/demos/data_helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/data_helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/data_helpers/anomaly_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/data_helpers/coco_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5361 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/data_helpers/download_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/data_helpers/video_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.233659 geti-sdk-1.5.4/geti_sdk/demos/demo_projects/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/demo_projects/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/demo_projects/anomaly_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/demo_projects/coco_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/demos/demo_projects/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.233659 geti-sdk-1.5.4/geti_sdk/deployment/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.237659 geti-sdk-1.5.4/geti_sdk/deployment/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/data_models/intermediate_inference_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/data_models/region_of_interest.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26479 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/deployed_model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/deployment.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.237659 geti-sdk-1.5.4/geti_sdk/deployment/resources/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/resources/OVMS_README.md
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/resources/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/deployment/utils.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55163 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/geti.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.237659 geti-sdk-1.5.4/geti_sdk/http_session/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/http_session/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/http_session/exception.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/http_session/geti_session.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/http_session/server_config.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6554 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/platform_versions.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.237659 geti-sdk-1.5.4/geti_sdk/rest_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3660 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2203 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/active_learning_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.237659 geti-sdk-1.5.4/geti_sdk/rest_clients/annotation_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/annotation_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/annotation_clients/annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/configuration_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/dataset_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/deployment_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.237659 geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/image_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/media_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/video_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/model_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/prediction_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.237659 geti-sdk-1.5.4/geti_sdk/rest_clients/project_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/project_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24906 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/project_client/project_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/project_client/task_templates.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_clients/training_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.241659 geti-sdk-1.5.4/geti_sdk/rest_converters/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.241659 geti-sdk-1.5.4/geti_sdk/rest_converters/annotation_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/configuration_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/job_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/media_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/model_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.241659 geti-sdk-1.5.4/geti_sdk/rest_converters/prediction_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/project_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/rest_converters/status_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.241659 geti-sdk-1.5.4/geti_sdk/utils/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/algorithm_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/credentials_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/dictionary_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/label_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/plot_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/serialization_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/geti_sdk/utils/workspace_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.225659 geti-sdk-1.5.4/geti_sdk.egg-info/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-11 12:22:26.000000 geti-sdk-1.5.4/geti_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5766 2023-05-11 12:22:26.000000 geti-sdk-1.5.4/geti_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-05-11 12:22:26.000000 geti-sdk-1.5.4/geti_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-11 12:22:26.000000 geti-sdk-1.5.4/geti_sdk.egg-info/requires.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-05-11 12:22:26.000000 geti-sdk-1.5.4/geti_sdk.egg-info/top_level.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/pyproject.toml
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.241659 geti-sdk-1.5.4/requirements/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/requirements/requirements-dev.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/requirements/requirements-docs.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/requirements/requirements-notebooks.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/requirements/requirements.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-05-11 12:22:26.245659 geti-sdk-1.5.4/setup.cfg
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/setup.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.241659 geti-sdk-1.5.4/tests/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/conftest.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-11 12:22:26.245659 geti-sdk-1.5.4/tests/helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/constants.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/finalizers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/fixtures.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/plotting.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/project_service.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/training.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-05-11 12:03:44.000000 geti-sdk-1.5.4/tests/helpers/vcr_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/LICENSE
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/MANIFEST.in
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/README.md
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.372739 geti-sdk-1.5.5/geti_sdk/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.372739 geti-sdk-1.5.5/geti_sdk/annotation_readers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/base_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.372739 geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/geti_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.376739 geti-sdk-1.5.5/geti_sdk/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5033 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/algorithms.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/annotation_scene.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/annotations.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/code_deployment_info.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/configurable_parameter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/configurable_parameter_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/configuration.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/configuration_identifiers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.376739 geti-sdk-1.5.5/geti_sdk/data_models/containers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/containers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/containers/algorithm_list.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/containers/media_list.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.376739 geti-sdk-1.5.5/geti_sdk/data_models/enums/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/annotation_kind.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/configuration_enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/deployment_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/domain.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/job_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/job_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/media_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/model_status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      961 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/optimization_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/prediction_mode.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/shape_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/task_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/job.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/label.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/media.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/media_identifiers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/model_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/performance.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/predictions.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/project.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/shapes.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/task.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/task_annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.376739 geti-sdk-1.5.5/geti_sdk/demos/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/constants.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.368739 geti-sdk-1.5.5/geti_sdk/demos/data/
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/demos/data/example/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data/example/dogs.png
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/anomaly_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/coco_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5702 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/download_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/video_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/anomaly_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/coco_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/deployment/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/deployment/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/data_models/intermediate_inference_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/data_models/region_of_interest.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26479 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/deployed_model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/deployment.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/deployment/resources/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/resources/OVMS_README.md
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/resources/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/utils.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55163 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/geti.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/http_session/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/http_session/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/http_session/exception.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/http_session/geti_session.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/http_session/server_config.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6554 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/platform_versions.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3660 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2203 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/active_learning_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/configuration_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/dataset_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/deployment_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/image_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/media_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/video_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/model_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/prediction_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24906 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/project_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/task_templates.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/training_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_converters/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/configuration_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/job_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/media_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/model_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/project_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/status_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/geti_sdk/utils/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/algorithm_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/credentials_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/dictionary_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/label_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/plot_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/serialization_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/workspace_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.372739 geti-sdk-1.5.5/geti_sdk.egg-info/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5766 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/requires.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/pyproject.toml
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/requirements/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/requirements/requirements-dev.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/requirements/requirements-docs.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/requirements/requirements-notebooks.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/requirements/requirements.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/setup.cfg
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/setup.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/tests/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/conftest.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/tests/helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/constants.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/finalizers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/fixtures.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/plotting.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/project_service.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/training.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/vcr_helpers.py
```

### Comparing `geti-sdk-1.5.4/LICENSE` & `geti-sdk-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/PKG-INFO` & `geti-sdk-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.4
+Version: 1.5.5
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.4/README.md` & `geti-sdk-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/__init__.py` & `geti-sdk-1.5.5/geti_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,10 +74,10 @@
 
    .. automethod:: upload_and_predict_media_folder
 
 """
 
 from .geti import Geti
 
-__version__ = "1.5.4"
+__version__ = "1.5.5"
 
 __all__ = ["Geti"]
```

### Comparing `geti-sdk-1.5.4/geti_sdk/annotation_readers/__init__.py` & `geti-sdk-1.5.5/geti_sdk/annotation_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/annotation_readers/base_annotation_reader.py` & `geti-sdk-1.5.5/geti_sdk/annotation_readers/base_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py` & `geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py` & `geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py` & `geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/annotation_readers/directory_tree_annotation_reader.py` & `geti-sdk-1.5.5/geti_sdk/annotation_readers/directory_tree_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/annotation_readers/geti_annotation_reader.py` & `geti-sdk-1.5.5/geti_sdk/annotation_readers/geti_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/__init__.py` & `geti-sdk-1.5.5/geti_sdk/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/algorithms.py` & `geti-sdk-1.5.5/geti_sdk/data_models/algorithms.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/annotation_scene.py` & `geti-sdk-1.5.5/geti_sdk/data_models/annotation_scene.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/annotations.py` & `geti-sdk-1.5.5/geti_sdk/data_models/annotations.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/code_deployment_info.py` & `geti-sdk-1.5.5/geti_sdk/data_models/code_deployment_info.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/configurable_parameter.py` & `geti-sdk-1.5.5/geti_sdk/data_models/configurable_parameter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/configurable_parameter_group.py` & `geti-sdk-1.5.5/geti_sdk/data_models/configurable_parameter_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/configuration.py` & `geti-sdk-1.5.5/geti_sdk/data_models/configuration.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/configuration_identifiers.py` & `geti-sdk-1.5.5/geti_sdk/data_models/configuration_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/containers/__init__.py` & `geti-sdk-1.5.5/geti_sdk/data_models/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/containers/algorithm_list.py` & `geti-sdk-1.5.5/geti_sdk/data_models/containers/algorithm_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/containers/media_list.py` & `geti-sdk-1.5.5/geti_sdk/data_models/containers/media_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/__init__.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/annotation_kind.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/annotation_kind.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/annotation_state.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/configuration_enums.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/configuration_enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/deployment_state.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/deployment_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/domain.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/domain.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/job_state.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/job_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/job_type.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/job_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/media_type.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/media_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/model_status.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/model_status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/optimization_type.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/optimization_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/prediction_mode.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/prediction_mode.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/shape_type.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/shape_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/enums/task_type.py` & `geti-sdk-1.5.5/geti_sdk/data_models/enums/task_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/job.py` & `geti-sdk-1.5.5/geti_sdk/data_models/job.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/label.py` & `geti-sdk-1.5.5/geti_sdk/data_models/label.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/media.py` & `geti-sdk-1.5.5/geti_sdk/data_models/media.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/media_identifiers.py` & `geti-sdk-1.5.5/geti_sdk/data_models/media_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/model.py` & `geti-sdk-1.5.5/geti_sdk/data_models/model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/model_group.py` & `geti-sdk-1.5.5/geti_sdk/data_models/model_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/performance.py` & `geti-sdk-1.5.5/geti_sdk/data_models/performance.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/predictions.py` & `geti-sdk-1.5.5/geti_sdk/data_models/predictions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/project.py` & `geti-sdk-1.5.5/geti_sdk/data_models/project.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/shapes.py` & `geti-sdk-1.5.5/geti_sdk/data_models/shapes.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/status.py` & `geti-sdk-1.5.5/geti_sdk/data_models/status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/task.py` & `geti-sdk-1.5.5/geti_sdk/data_models/task.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/task_annotation_state.py` & `geti-sdk-1.5.5/geti_sdk/data_models/task_annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/data_models/utils.py` & `geti-sdk-1.5.5/geti_sdk/data_models/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/__init__.py` & `geti-sdk-1.5.5/geti_sdk/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/constants.py` & `geti-sdk-1.5.5/geti_sdk/demos/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/data/example/dogs.png` & `geti-sdk-1.5.5/geti_sdk/demos/data/example/dogs.png`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/data_helpers/__init__.py` & `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/data_helpers/anomaly_helpers.py` & `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/anomaly_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/data_helpers/coco_helpers.py` & `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/coco_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/data_helpers/download_helpers.py` & `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/download_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,56 +19,62 @@
 import zipfile
 from typing import Dict, Optional
 
 import requests
 from tqdm import tqdm
 
 
-def get_proxies(url: str = "") -> Dict[str, str]:
+def get_proxies(url: str = "", verify_cert: bool = True) -> Dict[str, str]:
     """
     Determine whether or not to use proxies to attempt to reach a certain url.
 
     :param url: URL that should be resolved
+    :param verify_cert: False to disable SSL certificate validation
     :return:
     """
     logging.info(f"Connecting to url {url}...")
     proxies: Dict[str, str] = {}
     try:
-        requests.head(url=url, proxies=proxies, timeout=10)
+        requests.head(url=url, proxies=proxies, timeout=10, verify=verify_cert)
         return proxies
     except requests.exceptions.ConnectionError:
         logging.info("Unable to reach URL, attempting to connect via proxy...")
     proxies = {
         "http": "http://proxy-mu.intel.com:911",
         "https": "http://proxy-mu.intel.com:912",
     }
     try:
-        requests.head(url=url, proxies=proxies)
+        requests.head(url=url, proxies=proxies, verify=verify_cert)
         logging.info("Connection succeeded.")
     except requests.exceptions.ConnectionError as error:
         raise ValueError(
             "Unable to resolve URL with any proxy settings, please try to turn off "
             "your VPN connection before attempting again."
         ) from error
     return proxies
 
 
 def download_file(
-    url: str, target_folder: Optional[str], check_valid_archive: bool = False
+    url: str,
+    target_folder: Optional[str],
+    check_valid_archive: bool = False,
+    verify_cert: bool = True,
 ) -> str:
     """
     Download a file from `url` to a folder on local disk `target_folder`.
 
     NOTE: If a file with the same name as the file to be downloaded already exists in
         `target_folder`, this function will not download anything. If
         `check_valid_archive` is True, this function not only checks if the target
         file exists but also if it is a valid .zip archive.
 
     :param url:
     :param target_folder:
+    :param check_valid_archive: Check if the target file is a valid zip archive
+    :param verify_cert: False to disable SSL certificate validation
     :return: path to the downloaded file
     """
     filename = url.split("/")[-1]
     if target_folder is None:
         target_folder = "data"
     path_to_file = os.path.join(target_folder, filename)
     valid_file_exists = False
@@ -89,15 +95,15 @@
         logging.info(
             f"File {filename} exists at {path_to_file}. No new data was downloaded."
         )
         return path_to_file
 
     proxies = get_proxies(url)
     logging.info(f"Downloading {filename}...")
-    with requests.get(url, stream=True, proxies=proxies) as r:
+    with requests.get(url, stream=True, proxies=proxies, verify=verify_cert) as r:
         if r.status_code != 200:
             r.raise_for_status()
             raise RuntimeError(
                 f"Request to {url} failed, returned status code {r.status_code}"
             )
         file_size = int(r.headers.get("Content-Length", 0))
         with tqdm.wrapattr(r.raw, "read", total=file_size, desc="") as r_raw:
```

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/data_helpers/video_helpers.py` & `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/video_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/demo_projects/__init__.py` & `geti-sdk-1.5.5/geti_sdk/demos/demo_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/demo_projects/anomaly_demos.py` & `geti-sdk-1.5.5/geti_sdk/demos/demo_projects/anomaly_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/demo_projects/coco_demos.py` & `geti-sdk-1.5.5/geti_sdk/demos/demo_projects/coco_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/demos/demo_projects/utils.py` & `geti-sdk-1.5.5/geti_sdk/demos/demo_projects/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/__init__.py` & `geti-sdk-1.5.5/geti_sdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/data_models/__init__.py` & `geti-sdk-1.5.5/geti_sdk/deployment/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/data_models/intermediate_inference_result.py` & `geti-sdk-1.5.5/geti_sdk/deployment/data_models/intermediate_inference_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/data_models/region_of_interest.py` & `geti-sdk-1.5.5/geti_sdk/deployment/data_models/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/deployed_model.py` & `geti-sdk-1.5.5/geti_sdk/deployment/deployed_model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/deployment.py` & `geti-sdk-1.5.5/geti_sdk/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/resources/OVMS_README.md` & `geti-sdk-1.5.5/geti_sdk/deployment/resources/OVMS_README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/resources/__init__.py` & `geti-sdk-1.5.5/geti_sdk/deployment/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/deployment/utils.py` & `geti-sdk-1.5.5/geti_sdk/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/geti.py` & `geti-sdk-1.5.5/geti_sdk/geti.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/http_session/__init__.py` & `geti-sdk-1.5.5/geti_sdk/http_session/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/http_session/exception.py` & `geti-sdk-1.5.5/geti_sdk/http_session/exception.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/http_session/geti_session.py` & `geti-sdk-1.5.5/geti_sdk/http_session/geti_session.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/http_session/server_config.py` & `geti-sdk-1.5.5/geti_sdk/http_session/server_config.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/platform_versions.py` & `geti-sdk-1.5.5/geti_sdk/platform_versions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/__init__.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/active_learning_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/active_learning_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/annotation_clients/__init__.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/annotation_clients/annotation_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/configuration_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/configuration_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/dataset_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/deployment_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/deployment_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/__init__.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/image_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/image_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/media_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/media_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/media_client/video_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/video_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/model_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/model_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/prediction_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/prediction_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/project_client/__init__.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/project_client/project_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/project_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/project_client/task_templates.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/task_templates.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_clients/training_client.py` & `geti-sdk-1.5.5/geti_sdk/rest_clients/training_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/__init__.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/annotation_rest_converter/__init__.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/configuration_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/configuration_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/job_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/job_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/media_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/media_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/model_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/model_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/prediction_rest_converter/__init__.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/project_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/project_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/rest_converters/status_rest_converter.py` & `geti-sdk-1.5.5/geti_sdk/rest_converters/status_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/__init__.py` & `geti-sdk-1.5.5/geti_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/algorithm_helpers.py` & `geti-sdk-1.5.5/geti_sdk/utils/algorithm_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/credentials_helpers.py` & `geti-sdk-1.5.5/geti_sdk/utils/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/dictionary_helpers.py` & `geti-sdk-1.5.5/geti_sdk/utils/dictionary_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/label_helpers.py` & `geti-sdk-1.5.5/geti_sdk/utils/label_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/plot_helpers.py` & `geti-sdk-1.5.5/geti_sdk/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/project_helpers.py` & `geti-sdk-1.5.5/geti_sdk/utils/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/serialization_helpers.py` & `geti-sdk-1.5.5/geti_sdk/utils/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk/utils/workspace_helpers.py` & `geti-sdk-1.5.5/geti_sdk/utils/workspace_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk.egg-info/PKG-INFO` & `geti-sdk-1.5.5/geti_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.4
+Version: 1.5.5
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.4/geti_sdk.egg-info/SOURCES.txt` & `geti-sdk-1.5.5/geti_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/geti_sdk.egg-info/requires.txt` & `geti-sdk-1.5.5/geti_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/setup.py` & `geti-sdk-1.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/__init__.py` & `geti-sdk-1.5.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/conftest.py` & `geti-sdk-1.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/__init__.py` & `geti-sdk-1.5.5/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/constants.py` & `geti-sdk-1.5.5/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/enums.py` & `geti-sdk-1.5.5/tests/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/finalizers.py` & `geti-sdk-1.5.5/tests/helpers/finalizers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/fixtures.py` & `geti-sdk-1.5.5/tests/helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/plotting.py` & `geti-sdk-1.5.5/tests/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/project_helpers.py` & `geti-sdk-1.5.5/tests/helpers/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/project_service.py` & `geti-sdk-1.5.5/tests/helpers/project_service.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/training.py` & `geti-sdk-1.5.5/tests/helpers/training.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.4/tests/helpers/vcr_helpers.py` & `geti-sdk-1.5.5/tests/helpers/vcr_helpers.py`

 * *Files identical despite different names*

