# Comparing `tmp/datarobot_early_access-3.2.0.2023.5.15.tar.gz` & `tmp/datarobot_early_access-3.2.0.2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.5.15.tar", last modified: Mon May 15 16:46:32 2023, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.5.8.tar", last modified: Mon May  8 16:47:08 2023, max compression
```

## Comparing `datarobot_early_access-3.2.0.2023.5.15.tar` & `datarobot_early_access-3.2.0.2023.5.8.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   170943 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8705 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5678 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2271 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/data_matching.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7398 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17316 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2063 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25406 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   100246 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4044 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8771 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23045 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    83098 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40817 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57998 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12535 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4832 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    93319 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16683 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21038 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   256106 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9583 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   211358 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6051 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21042 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6880 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17421 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-05-15 16:46:09.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5670 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1108 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3148 2023-05-15 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.15/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-05-15 16:46:32.000000 datarobot_early_access-3.2.0.2023.5.15/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-05-15 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.15/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-05-15 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.15/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   169379 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8705 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5638 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2271 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/data_matching.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7536 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17252 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2063 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24305 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1127 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/deployment_monitoring.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   100246 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4044 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8437 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23045 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    83098 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40817 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    56459 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12528 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4829 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12639 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    93316 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10058 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16683 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21038 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   256106 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9565 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10203 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   209815 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/recommended_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6051 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19984 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1560 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17373 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5675 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1079 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3148 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/setup_weekly.py
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/CHANGES.rst` & `datarobot_early_access-3.2.0.2023.5.8/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,36 +32,23 @@
   :meth:`BatchMonitoringJobDefinition.run_once <datarobot.models.BatchMonitoringJobDefinition.run_once>`
 - Added a new method to retrieve a monitoring job
   :meth:`BatchMonitoringJob.get <datarobot.models.BatchMonitoringJob.get>`
 - Added the ability to filter return objects by a Use Case ID passed to the following methods:
   :meth:`Dataset.list <datarobot.models.Dataset.list>`
   :meth:`Notebook.list <datarobot.Notebook.list>`
   :meth:`Project.list <datarobot.models.Project.list>`
-- Added the ability to automatically add a newly created dataset or project to a Use Case by passing a UseCase, list of UseCase objects, UseCase ID or list of UseCase IDs using the keyword argument `use_cases` to the following methods:
-  :meth:`Dataset.create_from_file <datarobot.models.Dataset.create_from_file>`
-  :meth:`Dataset.create_from_in_memory_data <datarobot.models.Dataset.create_from_in_memory_data>`
-  :meth:`Dataset.create_from_url <datarobot.models.Dataset.create_from_url>`
-  :meth:`Dataset.create_from_data_source <datarobot.models.Dataset.create_from_data_source>`
-  :meth:`Dataset.create_from_query_generator <datarobot.models.Dataset.create_from_query_generator>`
-  :meth:`Dataset.create_project <datarobot.models.Dataset.create_project>`
-  :meth:`Project.create <datarobot.models.Project.create>`
-  :meth:`Project.create_from_data_source <datarobot.models.Project.create_from_data_source>`
-  :meth:`Project.create_from_dataset <datarobot.models.Project.create_from_dataset>`
-  :meth:`Project.create_segmented_project_from_clustering_model <datarobot.models.Project.create_segmented_project_from_clustering_model>`
-  :meth:`Project.start <datarobot.models.Project.start>`
+
 - Added the ability to set a default :class:`UseCase <datarobot.UseCase>` for requests. It can be set by:
 
-  - invoking `Client(..., default_use_case = <id>)`, or
-  - setting `default_use_case: <id>` in drconfig.yaml, or
-  - setting the env var ``DATAROBOT_DEFAULT_USE_CASE``, or
+  - invoking `Client(..., use_case = <id>)`, or
+  - setting `use_case: <id>` in drconfig.yaml, or
+  - setting the env var DATAROBOT_DEFAULT_USE_CASE, or
   - calling `with UseCase.get(<id>):`.
 
 - Added method meth:`Deployment.get_predictions_over_time <datarobot.models.Deployment.get_predictions_over_time>` to retrieve deployment predictions over time data.
-- Added a new class :class:`FairnessScoresOverTime <datarobot.models.deployment.bias_and_fairness.FairnessScoresOverTime>` to retrieve fairness over time information.
-- Added a new method :meth:`Deployment.get_fairness_scores_over_time <datarobot.models.Deployment.get_fairness_scores_over_time>` to retrieve fairness scores over time of a deployment.
 
 Enhancements
 ************
 - Improve error message of :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>`
   to clarify that a selected parameter cannot be used when a project has not proceeded to the
   correct stage prior to calling this method.
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/LICENSE.txt` & `datarobot_early_access-3.2.0.2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/PKG-INFO` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: datarobot_early_access
-Version: 3.2.0.2023.5.15
+Name: datarobot-early-access
+Version: 3.2.0.2023.5.8
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/README.md` & `datarobot_early_access-3.2.0.2023.5.8/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/common_setup.py` & `datarobot_early_access-3.2.0.2023.5.8/common_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,16 +181,15 @@
         "pandas>=0.15",
         "numpy",
         "pyyaml>=3.11",
         "requests>=2.28.1",
         "requests_toolbelt>=0.6",
         "trafaret>=0.7,<2.2,!=1.1.0",
         "urllib3>=1.23,<2.0.0",
-        "typing-extensions>=4.3.0,<5",
-        "mypy-extensions>=0.4.0,<2",
+        "typing-extensions==4.3.0",
     ],
     extras_require={
         "dev": dev_require,
         "examples": example_require,
         "release": release_require,
         "lint": lint_require,
         "images": images_require,
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_compat.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/documentai/document.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/model_package.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/retraining.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 import trafaret as t
 
 from datarobot._compat import String
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
 from datarobot.utils.pagination import unpaginate
 
 
-class RetrainingPolicy(APIObject):
+class RetrainingPolicy(APIObject, DeploymentQueryBuilderMixin):
     """Retraining Policy.
 
     Attributes
     ----------
     policy_id : str
         ID of the retraining policy
     name : str
@@ -144,15 +145,15 @@
             )
         """
 
         path = "{}{}/".format(cls._path.format(deployment_id), retraining_policy_id)
         cls._client.delete(path)
 
 
-class RetrainingPolicyRun(APIObject):
+class RetrainingPolicyRun(APIObject, DeploymentQueryBuilderMixin):
     """Retraining policy run.
 
     Attributes
     ----------
     policy_run_id : str
         ID of the retraining policy run
     status : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/client.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
-    default_use_case: Optional[str] = None,
+    use_case: Optional[str] = None,
 ) -> RESTClientObject:
     """Return a new `RESTClientObject` with optional configuration.
     Missing configuration will be read from environment variables or a config
     file.
 
     .. note::
         This function is intended for use with the ``client_configuration``
@@ -79,28 +79,28 @@
         Could be set to path with certificates of trusted certification authorities
     max_retries : int or datarobot.rest.Retry, optional
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools
-    default_use_case: str, optional
+    use_case: str, optional
         The entity ID of the default Use Case to use with any requests made by this Client instance.
     """
     env_config = _get_config_file_from_env()
     if token and endpoint:
         drconfig = DataRobotClientConfig(
             endpoint=endpoint,
             token=token,
             connect_timeout=connect_timeout,
             user_agent_suffix=user_agent_suffix,
             ssl_verify=ssl_verify,
             max_retries=max_retries,
             token_type=token_type,
-            default_use_case=default_use_case,
+            use_case=use_case,
         )
     elif config_path:
         if not _file_exists(config_path):
             raise ValueError(f"Invalid config path - no file at {config_path}")
         drconfig = _config_from_file(config_path)
     elif env_config:
         if not _file_exists(env_config):
@@ -131,15 +131,15 @@
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
-    default_use_case: Optional[str] = None,
+    use_case: Optional[str] = None,
 ) -> RESTClientObject:
     """
     Configures the global API client for the Python SDK with optional
     configuration. Missing configuration will be read from env
     or config file.
 
     Parameters
@@ -163,30 +163,30 @@
         Could be set to path with certificates of trusted certification authorities.
     max_retries : int or datarobot.rest.Retry, optional
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools.
-    default_use_case: str, optional
+    use_case: str, optional
         The entity ID of the default Use Case to use with any requests made by this Client instance.
     Returns
     -------
         The ``RESTClientObject`` instance created.
     """
     new_client = _create_client(
         token,
         endpoint,
         config_path,
         connect_timeout,
         user_agent_suffix,
         ssl_verify,
         max_retries,
         token_type,
-        default_use_case,
+        use_case,
     )
 
     set_client(new_client)
 
     return new_client
 
 
@@ -420,15 +420,15 @@
         )
         raise ValueError(e_msg)
     return DataRobotClientConfig(
         endpoint=endpoint,
         token=token,
         user_agent_suffix=user_agent_suffix,
         max_retries=max_retries,
-        default_use_case=use_case_id,
+        use_case=use_case_id,
     )
 
 
 def _config_from_file(config_path: str) -> DataRobotClientConfig:
     """
     Create and return a DataRobotClientConfig from a config path. The file must be
     a yaml formatted file
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/context.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/enums.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,27 @@
 #
-# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-from __future__ import annotations
-
-from enum import Enum, EnumMeta
-from typing import Optional
+from enum import Enum
 
 
 # A decorator to add an ALL attribute to (str, Enum) classes.
 def use_all(enum_instance):
     setattr(enum_instance, "ALL", list(map(lambda c: c, enum_instance)))
     return enum_instance
 
 
-class StrEnum(EnumMeta):
-    """
-    Enum that permits comparison of strings.
-    Ref: https://stackoverflow.com/questions/63335753/how-to-check-if-string-exists-in-enum-of-strings
-    """
-
-    def __contains__(cls: type, member: object) -> bool:
-        try:
-            cls(member)  # pylint: disable=no-value-for-parameter
-        except ValueError:
-            return False
-        return True
-
-
 def enum(*vals, **enums):
     """
     Enum without third party libs and compatible with py2 and py3 versions.
     """
     enums.update(dict(zip(vals, vals)))
     return type("Enum", (), enums)
 
@@ -892,39 +875,22 @@
 
 
 class ComplianceDocTemplateType(str, Enum):
     NORMAL = "normal"
     TIME_SERIES = "time_series"
 
 
-class UseCaseEntityType(str, Enum, metaclass=StrEnum):
+class UseCaseEntities(str, Enum):
     PROJECT = "project"
     DATASET = "dataset"
     NOTEBOOK = "notebook"
     APPLICATION = "application"
     RECIPE = "recipe"
 
 
-class UseCaseAPIPathEntityType(str, Enum):
-    PROJECT = "projects"
-    DATASET = "datasets"
-    NOTEBOOK = "notebooks"
-    APPLICATION = "applications"
-    RECIPE = "recipes"
-
-
-UseCaseReferenceEntityMap: dict[Optional[UseCaseEntityType], UseCaseAPIPathEntityType] = {
-    UseCaseEntityType.PROJECT: UseCaseAPIPathEntityType.PROJECT,
-    UseCaseEntityType.DATASET: UseCaseAPIPathEntityType.DATASET,
-    UseCaseEntityType.NOTEBOOK: UseCaseAPIPathEntityType.NOTEBOOK,
-    UseCaseEntityType.APPLICATION: UseCaseAPIPathEntityType.APPLICATION,
-    UseCaseEntityType.RECIPE: UseCaseAPIPathEntityType.RECIPE,
-}
-
-
 class NotebookPermissions(str, Enum):
     CAN_READ = "CAN_READ"
     CAN_UPDATE = "CAN_UPDATE"
     CAN_DELETE = "CAN_DELETE"
     CAN_SHARE = "CAN_SHARE"
     CAN_COPY = "CAN_COPY"
     CAN_EXECUTE = "CAN_EXECUTE"
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/errors.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/api_object.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/application.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
-from typing import List, Optional, Union
+from typing import List, Optional
 
 import trafaret as t
 from typing_extensions import TypedDict
 
 from datarobot.enums import ApplicationPermissions
 from datarobot.models.api_object import APIObject
-from datarobot.models.use_cases.utils import resolve_use_case
 from datarobot.utils.pagination import unpaginate
 
 
 class ApplicationDeployment(TypedDict):
     deployment_id: str
     reference_name: str
 
@@ -193,34 +192,31 @@
         self.deployments = deployments
 
     @classmethod
     def list(
         cls,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
-        use_cases: Optional[Union[str, List[str]]] = None,
     ) -> List[Application]:
         """
         Retrieve a list of user applications.
 
         Parameters
         ----------
         offset : Optional[int]
             Optional. Retrieve applications in a list after this number.
         limit : Optional[int]
             Optional. Retrieve only this number of applications.
-        use_cases: Optional[Union[str, List[str]]]
-            Optional. Filter available Applications by a specific Use Case ID or IDs.
+
         Returns
         -------
         applications : List[Application]
             The requested list of user applications.
         """
         query = {"offset": offset, "limit": limit}
-        query = resolve_use_case(use_case_id=use_cases, params=query)
         applications = unpaginate(initial_url=cls._path, initial_params=query, client=cls._client)
         return [cls.from_server_data(application) for application in applications]
 
     @classmethod
     def get(cls, application_id: str) -> Application:
         """
         Retrieve a single application.
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/blueprint.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/calendar_file.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/change_request.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/cluster.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/connector.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/credential.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_task.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/data_source.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/data_store.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -26,22 +26,22 @@
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject
 from datarobot.models.credential import CredentialDataSchema
 from datarobot.models.feature import DatasetFeature
 from datarobot.models.featurelist import DatasetFeaturelist
 from datarobot.models.project import Project
 from datarobot.models.sharing import SharingAccess
-from datarobot.models.use_cases.utils import add_to_use_case, resolve_use_case
 from datarobot.utils import assert_single_parameter, dataframe_to_buffer
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
 from datarobot.utils.sourcedata import list_of_records_to_buffer
 from datarobot.utils.waiters import wait_for_async_resolution
 
 from ..enums import DEFAULT_MAX_WAIT, DEFAULT_TIMEOUT
+from .use_cases.utils import resolve_use_case
 
 ProjectLocation = namedtuple("ProjectLocation", ["url", "id"])
 
 FeatureTypeCount = namedtuple("FeatureTypeCount", ["count", "feature_type"])
 
 
 TDataset = TypeVar("TDataset", bound="Dataset")
@@ -200,15 +200,14 @@
             return cls.create_from_file(file_path=cast(str, source))
         elif source_type == LocalSourceType.DATA_FRAME:
             return cls.create_from_in_memory_data(data_frame=source)
         elif source_type == LocalSourceType.FILELIKE:
             return cls.create_from_file(filelike=cast(IOBase, source))
 
     @classmethod
-    @add_to_use_case
     def create_from_file(
         cls: Type[TDataset],
         file_path: Optional[str] = None,
         filelike: Optional[IOBase] = None,
         categories: Optional[List[str]] = None,
         read_timeout: int = DEFAULT_TIMEOUT.UPLOAD,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -232,17 +231,14 @@
             An array of strings describing the intended use of the dataset. The
             current supported options are "TRAINING" and "PREDICTION".
         read_timeout: int, optional
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case ids or a single Use Case id to add this new Dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             A fully armed and operational Dataset
         """
         assert_single_parameter(("filelike", "file_path"), file_path, filelike)
@@ -273,15 +269,14 @@
         )
         dataset = cls.from_location(new_dataset_location)
         if categories:
             dataset.modify(categories=categories)
         return dataset
 
     @classmethod
-    @add_to_use_case
     def create_from_in_memory_data(
         cls: Type[TDataset],
         data_frame: Optional[pd.DataFrame] = None,
         records: Optional[List[Dict[str, Any]]] = None,
         categories: Optional[List[str]] = None,
         read_timeout: int = DEFAULT_TIMEOUT.UPLOAD,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -307,17 +302,14 @@
         read_timeout: int, optional
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful
         fname: string, optional
             The file name, "data.csv" by default
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data.
 
         Raises
@@ -338,15 +330,14 @@
             filelike=buff,
             categories=categories,
             read_timeout=read_timeout,
             max_wait=max_wait,
         )
 
     @classmethod
-    @add_to_use_case
     def create_from_url(
         cls: Type[TDataset],
         url: str,
         do_snapshot: Optional[bool] = None,
         persist_data_after_ingestion: Optional[bool] = None,
         categories: Optional[List[str]] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -373,17 +364,14 @@
             available. Specifying this parameter to false and `doSnapshot` to true will result in
             an error.
         categories: list[string], optional
             An array of strings describing the intended use of the dataset. The
             current supported options are "TRAINING" and "PREDICTION".
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data
         """
         base_data = {
@@ -398,15 +386,14 @@
 
         new_dataset_location = wait_for_async_resolution(
             cls._client, response.headers["Location"], max_wait
         )
         return cls.from_location(new_dataset_location)
 
     @classmethod
-    @add_to_use_case
     def create_from_data_source(
         cls: Type[TDataset],
         data_source_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         do_snapshot: Optional[bool] = None,
         persist_data_after_ingestion: Optional[bool] = None,
@@ -455,17 +442,15 @@
             If unset, uses the server default: False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         max_wait: int, optional
             Time in seconds after which project creation is considered unsuccessful.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
+
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data
         """
         base_data = {
@@ -489,15 +474,14 @@
 
         new_dataset_location = wait_for_async_resolution(
             cls._client, response.headers["Location"], max_wait
         )
         return cls.from_location(new_dataset_location)
 
     @classmethod
-    @add_to_use_case
     def create_from_query_generator(
         cls: Type[TDataset],
         generator_id: str,
         dataset_id: Optional[str] = None,
         dataset_version_id: Optional[str] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TDataset:
@@ -516,17 +500,14 @@
         dataset_id: str, optional
             The id of the dataset to apply the query to.
         dataset_version_id: str, optional
             The id of the dataset version to apply the query to. If not specified the
             latest version associated with dataset_id (if specified) is used.
         max_wait : int
             optional, the maximum number of seconds to wait before giving up.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the query generator
         """
         url = "dataEngineWorkspaceStates/fromDataEngineQueryGenerator/"
@@ -601,15 +582,15 @@
 
     @classmethod
     def list(
         cls: Type[TDataset],
         category: Optional[str] = None,
         filter_failed: Optional[bool] = None,
         order_by: Optional[str] = None,
-        use_cases: Optional[Union[str, List[str]]] = None,
+        use_case_ids: Optional[Union[str, List[str]]] = None,
     ) -> List[TDataset]:
         """
         List all datasets a user can view.
 
 
         Parameters
         ----------
@@ -624,41 +605,40 @@
             If True invalid datasets will be excluded.
 
         order_by: string, optional
             If unset, uses the server default: "-created".
             Sorting order which will be applied to catalog list, valid options are:
             - "created" -- ascending order by creation datetime;
             - "-created" -- descending order by creation datetime.
-
-        use_cases: string or List[string], optional
+        use_case_ids: string or List[string], optional
             Filter available datasets by a specific Use Case ID or IDs.
         Returns
         -------
         list[Dataset]
             a list of datasets the user can view
 
         """
         return list(
             cls.iterate(
                 category=category,
                 order_by=order_by,
                 filter_failed=filter_failed,
-                use_cases=use_cases,
+                use_case_ids=use_case_ids,
             )
         )
 
     @classmethod
     def iterate(
         cls: Type[TDataset],
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         category: Optional[str] = None,
         order_by: Optional[str] = None,
         filter_failed: Optional[bool] = None,
-        use_cases: Optional[Union[str, List[str]]] = None,
+        use_case_ids: Optional[Union[str, List[str]]] = None,
     ) -> Generator[TDataset, None, None]:
         """
         Get an iterator for the requested datasets a user can view.
         This lazily retrieves results. It does not get the next page from the server until the
         current page is exhausted.
 
         Parameters
@@ -682,32 +662,32 @@
 
         order_by: string, optional
             If unset, uses the server default: "-created".
             Sorting order which will be applied to catalog list, valid options are:
             - "created" -- ascending order by creation datetime;
             - "-created" -- descending order by creation datetime.
 
-        use_cases: string or List[string], optional
+        use_case_ids: string or List[string], optional
             Filter available datasets by a specific Use Case ID or IDs.
         Yields
         ------
         Dataset
             An iterator of the datasets the user can view
 
         """
         all_params = {
             "offset": offset,
             "limit": limit,
             "category": category,
             "order_by": order_by,
             "filter_failed": filter_failed,
-            "experiment_container_ids": use_cases,
+            "experiment_container_ids": use_case_ids,
         }
         all_params = resolve_use_case(
-            use_case_id=use_cases, use_case_key="experiment_container_ids", params=all_params
+            use_case_id=use_case_ids, use_case_key="experiment_container_ids", params=all_params
         )
         params = _remove_empty_params(all_params)
         _update_filter_failed(params)
 
         for dataset_json in unpaginate(cls._path, params, cls._client):
             yield cls.from_server_data(dataset_json)
 
@@ -994,15 +974,14 @@
         Returns
         -------
         locations: list[ProjectLocation]
         """
         url = f"{self._path}{self.id}/projects/"
         return [ProjectLocation(**kwargs) for kwargs in unpaginate(url, None, self._client)]
 
-    @add_to_use_case
     def create_project(
         self,
         project_name: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         credential_id: Optional[str] = None,
         use_kerberos: Optional[bool] = None,
@@ -1026,17 +1005,14 @@
             The ID of the set of credentials to use instead of user and password.
         use_kerberos: bool, optional
             Server default is False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case ids or a single Use Case id to add this new Dataset to. Must be a kwarg.
 
         Returns
         -------
         Project
         """
         return Project.create_from_dataset(
             self.id,
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import dateutil
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import ACCURACY_METRIC
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         start: datetime
@@ -41,15 +41,15 @@
 
     class Bucket(TypedDict):
         period: Period
         value: int
         sample_size: int
 
 
-class Accuracy(APIObject, MonitoringDataQueryBuilderMixin):
+class Accuracy(APIObject, DeploymentQueryBuilderMixin):
     """Deployment accuracy information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metrics
     period : dict
@@ -184,15 +184,15 @@
         -------
         percent_changes: Dict
         """
 
         return {name: value.get("percent_change") for name, value in self.metrics.items()}
 
 
-class AccuracyOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+class AccuracyOverTime(APIObject, DeploymentQueryBuilderMixin):
     """Deployment accuracy over time information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metric
     metric : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/bias_and_fairness.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import dateutil
 import trafaret as t
 from trafaret import Bool, Float
 
 from datarobot._compat import String
 from datarobot.enums import BUCKET_SIZE
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         start: datetime
@@ -33,15 +33,15 @@
 
     class Bucket(TypedDict):
         period: Period
         value: int
         sample_size: int
 
 
-class FairnessScoresOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+class FairnessScoresOverTime(APIObject, DeploymentQueryBuilderMixin):
     """Deployment fairness over time information.
 
     Attributes
     ----------
     buckets : List
         fairness over time bucket for each model and bucket queried
     protected_feature : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/data_drift.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from typing import List, Optional, TYPE_CHECKING
 
 import dateutil
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import BUCKET_SIZE, DATA_DRIFT_METRIC
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         start: datetime
@@ -49,15 +49,15 @@
         row_count: Optional[int]
         mean_predicted_value: Optional[int]
         percentiles: List[Percentile]
         mean_probabilities: List[MeanProbability]
         class_distribution: List[ClassDistribution]
 
 
-class TargetDrift(APIObject, MonitoringDataQueryBuilderMixin):
+class TargetDrift(APIObject, DeploymentQueryBuilderMixin):
     """Deployment target drift information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve target drift metric
     period : dict
@@ -173,15 +173,15 @@
         if metric:
             params["metric"] = metric
         data = cls._client.get(path, params=params).json()
         data = from_api(data, keep_null_keys=True)
         return cls.from_data(data)
 
 
-class FeatureDrift(APIObject, MonitoringDataQueryBuilderMixin):
+class FeatureDrift(APIObject, DeploymentQueryBuilderMixin):
     """Deployment feature drift information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve feature drift metric
     period : dict
@@ -320,15 +320,15 @@
             response_json = from_api(response_json, keep_null_keys=True)
             for item in response_json["data"]:
                 data.append(_from_data_item(item))
 
         return data
 
 
-class PredictionsOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+class PredictionsOverTime(APIObject, DeploymentQueryBuilderMixin):
     """Deployment predictions over time information.
 
     Attributes
     ----------
     baselines : List
         target baseline for each model queried
     buckets : List
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     ACCURACY_METRIC,
     BUCKET_SIZE,
     DEFAULT_MAX_WAIT,
     FileLocationType,
     LocalSourceType,
 )
 from datarobot.errors import InvalidUsageError
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject, ServerDataDictType
 from datarobot.models.batch_prediction_job import BatchPredictionJob
 from datarobot.models.custom_model_version import CustomModelVersion
 from datarobot.models.deployment.accuracy import Accuracy, AccuracyOverTime
 from datarobot.models.deployment.bias_and_fairness import FairnessScoresOverTime
 from datarobot.models.deployment.data_drift import FeatureDrift, PredictionsOverTime, TargetDrift
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
 from datarobot.models.deployment.sharing import (
     DeploymentGrantSharedRoleWithId,
     DeploymentGrantSharedRoleWithUsername,
     DeploymentSharedRole,
 )
 from datarobot.utils import deprecated, from_api, get_id_from_location
@@ -138,15 +138,15 @@
     # Allow users to pass a single value even if a list of values is expected.
     if isinstance(trafaret, t.List) and not isinstance(value, list):
         value = [value]
 
     return trafaret.check(value)
 
 
-class Deployment(APIObject, MonitoringDataQueryBuilderMixin, BrowserMixin):
+class Deployment(APIObject, DeploymentQueryBuilderMixin, BrowserMixin):
     """A deployment created from a DataRobot model.
 
     Attributes
     ----------
     id : str
         the id of the deployment
     label : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/deployment_monitoring.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import pytz
 
 if TYPE_CHECKING:
     from datetime import datetime
 
 
-class MonitoringDataQueryBuilderMixin:  # pylint: disable=missing-class-docstring
+class DeploymentQueryBuilderMixin:  # pylint: disable=missing-class-docstring
     @staticmethod
     def _build_query_params(  # pylint: disable=missing-function-docstring
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         **kwargs: Any,
     ) -> Dict[str, Any]:
         def timezone_aware(dt: datetime) -> datetime:
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/service_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from typing import cast, List, Optional, TYPE_CHECKING, Union
 
 import dateutil
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import SERVICE_STAT_METRIC
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         """Type dict for period"""
@@ -51,15 +51,15 @@
         serverErrorRate: float
         numConsumers: int
         cacheHitRatio: float
         medianLoad: float
         peakLoad: float
 
 
-class ServiceStats(APIObject, MonitoringDataQueryBuilderMixin):
+class ServiceStats(APIObject, DeploymentQueryBuilderMixin):
     """Deployment service stats information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve service stats metrics
     period : dict
@@ -175,15 +175,15 @@
         metrics = data.pop("metrics")
 
         data = from_api(data, keep_null_keys=True)
         data["metrics"] = metrics
         return cls.from_data(data)
 
 
-class ServiceStatsOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+class ServiceStatsOverTime(APIObject, DeploymentQueryBuilderMixin):
     """Deployment service stats over time information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metric
     metric : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/driver.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/execution_environment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/feature_effect.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/featurelist.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/imported_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/missing_report.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/modeljob.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/notebooks.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/notebooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional
 
 import trafaret as t
 
 from datarobot.enums import NotebookPermissions
 from datarobot.models.api_object import APIObject
 from datarobot.models.use_cases.utils import resolve_use_case
 from datarobot.utils.pagination import unpaginate
@@ -260,15 +260,15 @@
         cls,
         created_before: Optional[str] = None,
         created_after: Optional[str] = None,
         order_by: Optional[str] = None,
         tags: Optional[List[str]] = None,
         owners: Optional[List[str]] = None,
         query: Optional[str] = None,
-        use_cases: Optional[Union[str, List[str]]] = None,
+        use_case_id: Optional[str] = None,
     ) -> List[Notebook]:
         """
         List all Notebooks available to the user.
 
         Parameters
         ----------
         created_before : Optional[str]
@@ -284,26 +284,28 @@
         tags : Optional[List[str]]
             A list of tags that returned Notebooks should be associated with. Optional.
         owners : Optional[List[str]]
             A list of user IDs used to filter returned Notebooks.
             The respective users share ownership of the Notebooks. Optional.
         query : Optional[str]
             A specific regex query to use when filtering Notebooks. Optional.
-        use_cases : Optional[str or List[str]]
-            Filters returned Notebooks by a specific Use Case ID or IDs. Optional.
+        use_case_id : Optional[str]
+            Constrain returned Notebooks to a specific Use Case. Optional.
         Returns
         -------
         notebooks : List[Notebook]
             A list of Notebooks available to the user.
         """
         params = {
             "created_before": created_before,
             "created_after": created_after,
             "order_by": order_by,
             "tags": tags,
             "owners": owners,
             "query": query,
         }
-        params = resolve_use_case(use_case_id=use_cases, params=params, use_case_key="use_case_id")
+        params = resolve_use_case(
+            use_case_id=use_case_id, params=params, use_case_key="use_case_id"
+        )
         url = f"{cls._client.domain}/{cls._path}"
         r_data = unpaginate(url, params, cls._client)
         return [Notebook.from_server_data(data) for data in r_data]
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/pareto_front.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/predict_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             t.Key("num_columns"): Int(),
             t.Key("forecast_point", optional=True): parse_time,
             t.Key("predictions_start_date", optional=True): parse_time,
             t.Key("predictions_end_date", optional=True): parse_time,
             t.Key("relax_known_in_advance_features_check", optional=True): t.Bool(),
             # do not forget to update `test_data_quality_warnings`
             # in datarobot-python-api-tests repo
-            t.Key("data_quality_warnings", optional=True): t.Dict(
+            t.Key("data_quality_warnings"): t.Dict(
                 {
                     t.Key("has_kia_missing_values_in_forecast_window"): t.Bool(),
                     t.Key("insufficient_rows_for_evaluating_models"): t.Bool(),
                     t.Key("single_class_actual_value_column"): t.Bool(),
                 }
             ).allow_extra("*"),
             t.Key("forecast_point_range", optional=True): t.List(parse_time),
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/prediction_server.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/predictions.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/prime_file.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/project.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 from datarobot.models.relationships_configuration import RelationshipsConfiguration
 from datarobot.models.restore_discarded_features import (
     DiscardedFeaturesInfo,
     FeatureRestorationStatus,
 )
 from datarobot.models.segmentation import SegmentationTask
 from datarobot.models.sharing import SharingAccess
-from datarobot.models.use_cases.utils import add_to_use_case, resolve_use_case
+from datarobot.models.use_cases.utils import resolve_use_case
 from datarobot.utils import (
     assert_single_or_zero_parameter,
     camelize,
     datetime_to_string,
     deprecated,
     from_api,
     get_duplicate_features,
@@ -576,23 +576,22 @@
             keep_attrs=[
                 "advanced_options.default_monotonic_increasing_featurelist_id",
                 "advanced_options.default_monotonic_decreasing_featurelist_id",
             ],
         )
 
     @classmethod
-    @add_to_use_case
     def create(
         cls,
         sourcedata,
         project_name="Untitled Project",
         max_wait=DEFAULT_MAX_WAIT,
         read_timeout=DEFAULT_TIMEOUT.UPLOAD,
         dataset_filename=None,
-    ) -> TProject:
+    ):
         """
         Creates a project with provided data.
 
         Project creation is asynchronous process, which means that after
         initial request we will keep polling status of async process
         that is responsible for project creation until it's finished.
         For SDK users this only means that this method might raise
@@ -612,17 +611,15 @@
             unsuccessful
         read_timeout: int
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         dataset_filename : string or None, optional
             (New in version v2.14) File name to use for dataset.
             Ignored for url and file path sources.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new Project to. Must be a kwarg.
+
         Returns
         -------
         project : Project
             Instance with initialized data.
 
         Raises
         ------
@@ -728,15 +725,14 @@
         if project_name is not None:
             payload["project_name"] = project_name
 
         response = cls._client.post(hdfs_project_create_endpoint, data=payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
-    @add_to_use_case
     def create_from_data_source(
         cls: Type[TProject],
         data_source_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         credential_id: Optional[str] = None,
         use_kerberos: Optional[bool] = None,
@@ -767,17 +763,15 @@
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         project_name : str, optional
             optional, a name to give to the project.
         max_wait : int
             optional, the maximum number of seconds to wait before giving up.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new Project to. Must be a kwarg.
+
         Raises
         ------
         InvalidUsageError
             Raised if either ``username`` or ``password`` is passed without the other.
 
         Returns
         -------
@@ -802,15 +796,14 @@
         if "credential_data" in new_payload:
             new_payload["credential_data"] = CredentialDataSchema(new_payload["credential_data"])
 
         response = cls._client.post(cls._path, data=payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
-    @add_to_use_case
     def create_from_dataset(
         cls: Type[TProject],
         dataset_id: str,
         dataset_version_id: Optional[str] = None,
         project_name: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
@@ -844,17 +837,15 @@
             Server default is False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         max_wait: int
             optional, the maximum number of seconds to wait before giving up.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new Project to. Must be a kwarg.
+
         Returns
         -------
         Project
         """
         payload = {
             "dataset_id": dataset_id,
             "dataset_version_id": dataset_version_id,
@@ -870,15 +861,14 @@
         if "credential_data" in new_payload:
             new_payload["credential_data"] = CredentialDataSchema(new_payload["credential_data"])
 
         response = cls._client.post(cls._path, data=new_payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
-    @add_to_use_case
     def create_segmented_project_from_clustering_model(
         cls: Type[TProject],
         clustering_project_id: str,
         clustering_model_id: str,
         target: str,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TProject:
@@ -893,17 +883,15 @@
             The identifier of the clustering model you want to use as the
             segmentation method.
         target : str
             The name of the target column that will be used from the
             clustering project.
         max_wait: int
             optional, the maximum number of seconds to wait before giving up.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new Project to. Must be a kwarg.
+
         Returns
         -------
         project : Project
             The created project
         """
         prepare_model_package_path = (
             f"{cls._path}{clustering_project_id}/models/"
@@ -1018,15 +1006,14 @@
             )
             proj_id = get_id_from_location(finished_location)
             return cls.get(proj_id)
         except AppPlatformError as e:
             raise ProjectAsyncFailureError(repr(e), e.status_code, async_location)
 
     @classmethod
-    @add_to_use_case
     def start(
         cls: Type[TProject],
         sourcedata: Union[str, DataFrame],
         target: Optional[str] = None,
         project_name: str = "Untitled Project",
         worker_count: Optional[int] = None,
         metric: Optional[str] = None,
@@ -1147,17 +1134,15 @@
             - 'postProcessingRejectionOptionBasedClassification'
             The technique by which we'll mitigate bias, which will inform which bias mitigation task
             we insert into blueprints
         include_bias_mitigation_feature_as_predictor_variable : bool, optional
             Whether we should also use the mitigation feature as in input to the modeler just like
             any other categorical used for training, i.e. do we want the model to "train on" this
             feature in addition to using it for bias mitigation
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new Project to. Must be a kwarg.
+
         Returns
         -------
         project : Project
             The newly created and initialized project.
 
         Raises
         ------
@@ -1237,31 +1222,27 @@
             unsupervised_type=unsupervised_type,
             autopilot_cluster_list=autopilot_cluster_list,
         )
         return project
 
     @classmethod
     def list(
-        cls, search_params: Optional[Dict[str, str]] = None, use_cases: Optional[str] = None
+        cls, search_params: Optional[Dict[str, str]] = None, use_case_id: Optional[str] = None
     ) -> List[Project]:
         """
         Returns the projects associated with this account.
 
         Parameters
         ----------
         search_params : dict, optional.
             If not `None`, the returned projects are filtered by lookup.
             Currently you can query projects by:
 
             * ``project_name``
 
-        use_cases : str, optional.
-            If not `None`, the returned projects are filtered to those associated
-            with a specific Use Case.
-
         Returns
         -------
         projects : list of Project instances
             Contains a list of projects associated with this user
             account.
 
         Raises
@@ -1293,18 +1274,17 @@
             else:
                 raise TypeError(
                     "Provided search_params argument {} is invalid type {}".format(
                         search_params, type(search_params)
                     )
                 )
         # This is a special case we needed to cover. A user could pass in "experiment_container_id" themselves to
-        # `search_params`, so we need to check for that and default to `use_cases` if that was passed in.
-        # Then we proceed to check if resolve_use_case(`use_case_id`) arg was set, and use a global use case if
-        # it's available.
-        get_params = resolve_use_case(use_case_id=use_cases, params=get_params)
+        # `search_params`, so we need to check for that and default to `use_case_id` if that was passed in.
+        # Then we proceed to check if `use_case_id` was set, and use a global use case if it's available.
+        get_params = resolve_use_case(use_case_id=use_case_id, params=get_params)
         r_data = cls._client.get(cls._path, params=get_params).json()
         return [cls.from_server_data(item) for item in r_data]
 
     def _update(self, **data) -> Project:
         """
         Change the project properties.
 
@@ -2089,15 +2069,15 @@
         predictions_start_date=None,
         predictions_end_date=None,
         dataset_filename=None,
         relax_known_in_advance_features_check=None,
         credentials=None,
         actual_value_column=None,
         secondary_datasets_config_id=None,
-    ) -> PredictionDataset:
+    ):
         """Upload a new dataset to make predictions against
 
         Parameters
         ----------
         sourcedata : str, file or pandas.DataFrame
             Data to be used for predictions. If string, can be either a path to a local file,
             a publicly accessible URL (starting with ``http://``, ``https://``, ``file://``), or
@@ -2230,15 +2210,15 @@
         forecast_point=None,
         relax_known_in_advance_features_check=None,
         credentials=None,
         predictions_start_date=None,
         predictions_end_date=None,
         actual_value_column=None,
         secondary_datasets_config_id=None,
-    ) -> PredictionDataset:
+    ):
         """
         Upload a new dataset from a data source to make predictions against
 
         Parameters
         ----------
         data_source_id : str
             The identifier of the data source.
@@ -2321,15 +2301,15 @@
         forecast_point=None,
         relax_known_in_advance_features_check=None,
         credentials=None,
         predictions_start_date=None,
         predictions_end_date=None,
         actual_value_column=None,
         secondary_datasets_config_id=None,
-    ) -> PredictionDataset:
+    ):
         """Upload a new dataset from a catalog dataset to make predictions against
 
         Parameters
         ----------
         dataset_id : str
             The identifier of the dataset.
         dataset_version_id : str, optional
@@ -2360,14 +2340,15 @@
         actual_value_column : string, optional
             Actual value column name, valid for the prediction
             files if the project is unsupervised and the dataset is considered as bulk predictions
             dataset. Cannot be provided with the ``forecast_point`` parameter.
         secondary_datasets_config_id: string or None, optional
             The Id of the alternative secondary dataset config
             to use during prediction for Feature discovery project.
+
         Returns
         -------
         dataset : PredictionDataset
             the newly uploaded dataset
         """
         form_data = {"datasetId": dataset_id}
         if dataset_version_id:
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/project_options.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/rating_table.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/recommended_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/residuals.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/roc_curve.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/ruleset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/segmentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/shap_impact.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/sharing.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/trafarets.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/training_predictions.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/types.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/use_case.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,36 +5,32 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-#  pylint: disable=C0415
 from __future__ import annotations
 
 from types import TracebackType
-from typing import cast, Dict, List, Optional, Tuple, Type, TypeVar, Union
+from typing import cast, Dict, List, Optional, Tuple, Type, Union
 
 import trafaret as t
 
 from datarobot.context import Context
-from datarobot.enums import (
-    SHARING_ROLE,
-    UseCaseAPIPathEntityType,
-    UseCaseEntityType,
-    UseCaseReferenceEntityMap,
-)
+from datarobot.enums import SHARING_ROLE, UseCaseEntities
 from datarobot.errors import InvalidUsageError
 from datarobot.models.api_object import APIObject
+from datarobot.models.application import Application
+from datarobot.models.dataset import Dataset
+from datarobot.models.notebooks import Notebook
+from datarobot.models.project import Project
 from datarobot.models.sharing import SharingRole
 from datarobot.utils.pagination import unpaginate
 
-T = TypeVar("T")
-
 use_case_user_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("full_name", optional=True): t.Or(t.String, t.Null),
         t.Key("email", optional=True): t.Or(t.String, t.Null),
         t.Key("userhash", optional=True): t.Or(t.String, t.Null),
         t.Key("username", optional=True): t.Or(t.String, t.Null),
@@ -78,15 +74,15 @@
 
 class UseCaseReferenceEntity(APIObject):
     """
     An entity associated with a Use Case.
 
     Attributes
     ----------
-    entity_type : UseCaseEntityType
+    entity_type : UseCaseEntities
         The type of the entity.
     use_case_id : str
         The Use Case this entity is associated with.
     id : str
         The ID of the entity.
     created_at : str
         The date and time this entity was linked with the Use Case.
@@ -107,15 +103,15 @@
             t.Key("is_deleted"): t.Bool,
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         id: str,
-        entity_type: UseCaseEntityType,
+        entity_type: UseCaseEntities,
         entity_id: str,
         use_case_id: str,
         created_at: str,
         created: Dict[str, str],
         is_deleted: bool,
     ):
         self.id = id
@@ -332,23 +328,14 @@
         use_case_id : str
             The ID of the Use Case to be deleted.
         """
         path = f"{cls._path}{use_case_id}/"
         cls._client.delete(path)
         return None
 
-    @classmethod
-    def _resolve_api_entity(
-        cls, entity_type: Optional[UseCaseEntityType] = None
-    ) -> UseCaseAPIPathEntityType | None:
-        """
-        For a given reference entity type, return the corresponding API endpoint type.
-        """
-        return UseCaseReferenceEntityMap.get(entity_type)
-
     def __enter__(self) -> UseCase:
         # Not declared in __init__ because this attribute has a very
         # specific use in context management and nowhere else
         self.__previous: UseCase = cast(  # pylint: disable=attribute-defined-outside-init
             UseCase, Context.use_case
         )
         Context.use_case = self
@@ -381,73 +368,69 @@
         """
         payload = {"name": name, "description": description}
         path = f"{self._path}{self.id}/"
         r_data = self._client.patch(path, data=payload).json()
         return self.from_server_data(r_data)
 
     def _get_reference_entity_info(
-        self, entity: Union[UseCaseReferenceEntity, T]
-    ) -> Tuple[UseCaseAPIPathEntityType, Optional[str]]:
+        self, entity: Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
+    ) -> Tuple[UseCaseEntities, Optional[str]]:
         """
         Get the entity type and entity id for a reference entity instance
         Parameters
         ----------
         entity : Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
             The entity instance to add to a Use Case.
         Returns
         -------
-        entity_info : Tuple[UseCaseEntityType, str]
+        entity_info : Tuple[UseCaseEntities, str]
             The entity type and entity id
         """
-        from ..application import Application
-        from ..dataset import Dataset
-        from ..notebooks import Notebook
-        from ..prediction_dataset import PredictionDataset
-        from ..project import Project
-
         if isinstance(entity, Project):
-            return UseCaseAPIPathEntityType.PROJECT, entity.id
-        elif isinstance(entity, (Dataset, PredictionDataset)):
-            return UseCaseAPIPathEntityType.DATASET, entity.id
+            return UseCaseEntities.PROJECT, entity.id
+        elif isinstance(entity, Dataset):
+            return UseCaseEntities.DATASET, entity.id
         elif isinstance(entity, Notebook):
-            return UseCaseAPIPathEntityType.NOTEBOOK, entity.id
+            return UseCaseEntities.NOTEBOOK, entity.id
         elif isinstance(entity, Application):
-            return UseCaseAPIPathEntityType.APPLICATION, entity.id
+            return UseCaseEntities.APPLICATION, entity.id
         elif isinstance(entity, UseCaseReferenceEntity):
-            return UseCaseReferenceEntityMap[entity.entity_type], entity.entity_id
+            return entity.entity_type, entity.entity_id
         raise TypeError(
             "entity must be Project, Dataset, Notebook, Application, or UseCaseReferenceEntity"
         )
 
     def add(
         self,
-        entity: Optional[Union[UseCaseReferenceEntity, T]] = None,
-        entity_type: Optional[UseCaseEntityType] = None,
+        entity: Optional[
+            Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
+        ] = None,
+        entity_type: Optional[UseCaseEntities] = None,
         entity_id: Optional[str] = None,
     ) -> UseCaseReferenceEntity:
         """
         Add an entity (project, notebook, dataset, etc.) to a Use Case. Can only accept either an entity or
         an entity type and entity ID, but not both.
 
         Parameters
         ----------
         entity : Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
             An existing entity linked to a different Use Case to be linked to this Use Case.
             Can not be used if entity_type and entity_id are passed.
-        entity_type : UseCaseEntityType
+        entity_type : UseCaseEntities
             The entity type of the entity to link to this Use Case. Can not be used if entity is passed.
         entity_id : str
             The ID of the entity to link to this Use Case. Can not be used if entity is passed.
 
         Returns
         -------
         use_case_reference_entity : UseCaseReferenceEntity
             The newly created reference link between this Use Case and the entity.
         """
-        e_type = self._resolve_api_entity(entity_type)
+        e_type = entity_type
         e_id = entity_id
         if entity and (e_type or entity_id):
             raise InvalidUsageError(
                 "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not e_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
@@ -455,32 +438,34 @@
             e_type, e_id = self._get_reference_entity_info(entity)
         path = f"{self._path}{self.id}/{e_type}/{e_id}/"
         r_data = self._client.post(path)
         return UseCaseReferenceEntity.from_server_data(r_data.json())
 
     def remove(
         self,
-        entity: Optional[Union[UseCaseReferenceEntity, T]] = None,
-        entity_type: Optional[UseCaseEntityType] = None,
+        entity: Optional[
+            Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
+        ] = None,
+        entity_type: Optional[UseCaseEntities] = None,
         entity_id: Optional[str] = None,
     ) -> None:
         """
         Remove an entity from a Use Case. Only supports passing an entity instance, or an entity type and ID.
 
         Parameters
         ----------
         entity : Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
             An existing entity instance to be removed from a Use Case.
             Can not be used if entity_type and entity_id are passed.
-        entity_type : UseCaseEntityType
+        entity_type : UseCaseEntities
             The entity type of the entity to link to this Use Case. Can not be used if entity is passed.
         entity_id : str
             The ID of the entity to link to this Use Case.  Can not be used if entity is passed.
         """
-        e_type = self._resolve_api_entity(entity_type)
+        e_type = entity_type
         e_id = entity_id
         if entity and (entity_type or entity_id):
             raise InvalidUsageError(
                 "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not entity_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
@@ -554,58 +539,39 @@
             Return the access control information for a user with this user ID. Optional.
         """
         params = {"offset": offset, "limit": limit, "id": id}
         path = f"{self._path}{self.id}/sharedRoles/"
         r_data = unpaginate(path, params, self._client)
         return [SharingRole.from_server_data(data) for data in r_data]
 
-    def list_notebooks(self) -> List[T]:
+    def list_notebooks(self) -> List[Notebook]:
         """
         List all notebooks associated with this Use Case.
 
         Returns
         -------
         notebooks : List[Notebook]
             All notebooks associated with this Use Case.
         """
-        from ..notebooks import Notebook
+        return Notebook.list(use_case_id=self.id)
 
-        return Notebook.list(use_cases=self.id)  # type: ignore[return-value]
-
-    def list_projects(self) -> List[T]:
+    def list_projects(self) -> List[Project]:
         """
         List all projects associated with this Use Case.
 
         Returns
         -------
         projects : List[Project]
             All projects associated with this Use Case.
         """
-        from ..project import Project
-
-        return Project.list(search_params={"experiment_container_id": self.id})  # type: ignore[return-value]
+        return Project.list(search_params={"experiment_container_id": self.id})
 
-    def list_datasets(self) -> List[T]:
+    def list_datasets(self) -> List[Dataset]:
         """
         List all datasets associated with this Use Case.
 
         Returns
         -------
         datasets : List[Dataset]
             All datasets associated with this Use Case.
         """
-        from ..dataset import Dataset
-
-        return Dataset.list(use_cases=self.id)  # type: ignore[return-value]
-
-    def list_applications(self) -> List[T]:
-        """
-        List all applications associated with this Use Case.
-
-        Returns
-        -------
-        applications : List[Application]
-            All applications associated with this Use Case.
-        """
-        from ..application import Application
-
-        return Application.list(use_cases=self.id)  # type: ignore[return-value]
+        return Dataset.list(use_case_ids=self.id)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/validators.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/visualai/images.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/models/word_cloud.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/rest.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -408,39 +408,39 @@
             t.Key("endpoint"): String(),
             t.Key("token"): String(),
             t.Key("connect_timeout", optional=True): Int(),
             t.Key("ssl_verify", optional=True): t.Or(t.Bool(), String()),
             t.Key("user_agent_suffix", optional=True): String(),
             t.Key("max_retries", optional=True): Int(),
             t.Key("token_type", optional=True): String(),
-            t.Key("default_use_case", optional=True): String(),
+            t.Key("use_case", optional=True): String(),
         }
     ).allow_extra("*")
     _fields = {k.to_name or k.name for k in _converter.keys}
 
     def __init__(
         self,
         endpoint: str,
         token: str,
         connect_timeout: Optional[int] = None,
         ssl_verify: bool = True,
         user_agent_suffix: Optional[str] = None,
         max_retries: Optional[Union[int, Retry]] = None,
         token_type: Optional[str] = None,
-        default_use_case: Optional[str] = None,
+        use_case: Optional[str] = None,
     ) -> None:
         self.endpoint = endpoint
         self.token = token
         self.connect_timeout = connect_timeout
         self.ssl_verify = ssl_verify
         self.user_agent_suffix = user_agent_suffix
         self.max_retries = max_retries
         self.token_type = token_type
-        self.default_use_case = default_use_case
+        self.use_case = use_case
 
-        if self.default_use_case is not None:
-            Context.use_case = self.default_use_case
+        if self.use_case is not None:
+            Context.use_case = self.use_case
 
     @classmethod
     def from_data(cls, data: Dict[str, Any]) -> DataRobotClientConfig:
         checked = {k: v for k, v in cls._converter.check(data).items() if k in cls._fields}
         return cls(**checked)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/deprecation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/pagination.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/retry.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/source.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot/utils/waiters.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.2.0.2023.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: datarobot-early-access
-Version: 3.2.0.2023.5.15
+Name: datarobot_early_access
+Version: 3.2.0.2023.5.8
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 datarobot/_experimental/models/model_package.py
 datarobot/_experimental/models/project_options.py
 datarobot/_experimental/models/retraining.py
 datarobot/_experimental/models/documentai/__init__.py
 datarobot/_experimental/models/documentai/document.py
 datarobot/helpers/__init__.py
 datarobot/helpers/binary_data_utils.py
+datarobot/helpers/deployment_monitoring.py
 datarobot/helpers/eligibility_result.py
 datarobot/helpers/feature_discovery.py
 datarobot/helpers/image_utils.py
 datarobot/helpers/partitioning_methods.py
 datarobot/mixins/__init__.py
 datarobot/mixins/browser_mixin.py
 datarobot/mixins/update_attributes_mixin.py
@@ -109,15 +110,14 @@
 datarobot/models/validators.py
 datarobot/models/word_cloud.py
 datarobot/models/deployment/__init__.py
 datarobot/models/deployment/accuracy.py
 datarobot/models/deployment/bias_and_fairness.py
 datarobot/models/deployment/data_drift.py
 datarobot/models/deployment/deployment.py
-datarobot/models/deployment/mixins.py
 datarobot/models/deployment/service_stats.py
 datarobot/models/deployment/sharing.py
 datarobot/models/external_dataset_scores_insights/__init__.py
 datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
 datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
 datarobot/models/external_dataset_scores_insights/external_lift_chart.py
 datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 pandas>=0.15
 numpy
 pyyaml>=3.11
 requests>=2.28.1
 requests_toolbelt>=0.6
 trafaret!=1.1.0,<2.2,>=0.7
 urllib3<2.0.0,>=1.23
-typing-extensions<5,>=4.3.0
-mypy-extensions<2,>=0.4.0
+typing-extensions==4.3.0
 
 [dev]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
 pytest-asyncio
```

### Comparing `datarobot_early_access-3.2.0.2023.5.15/pyproject.toml` & `datarobot_early_access-3.2.0.2023.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/setup.py` & `datarobot_early_access-3.2.0.2023.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.15/setup_weekly.py` & `datarobot_early_access-3.2.0.2023.5.8/setup_weekly.py`

 * *Files identical despite different names*

