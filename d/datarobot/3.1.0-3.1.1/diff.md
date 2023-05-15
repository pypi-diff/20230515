# Comparing `tmp/datarobot-3.1.0.tar.gz` & `tmp/datarobot-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarobot-3.1.0.tar", last modified: Mon Mar 13 18:54:15 2023, max compression
+gzip compressed data, was "datarobot-3.1.1.tar", last modified: Mon May 15 19:50:05 2023, max compression
```

## Comparing `datarobot-3.1.0.tar` & `datarobot-3.1.1.tar`

### file list

```diff
@@ -1,200 +1,197 @@
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:15.005040 datarobot-3.1.0/
--rw-r--r--   0 andrew.levan   (504) staff       (20)   161093 2023-03-13 18:52:23.000000 datarobot-3.1.0/CHANGES.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7555 2023-03-10 16:03:09.000000 datarobot-3.1.0/LICENSE.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)      421 2023-03-10 16:03:09.000000 datarobot-3.1.0/MANIFEST.in
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3283 2023-03-13 18:54:15.005180 datarobot-3.1.0/PKG-INFO
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8441 2023-03-13 18:52:20.000000 datarobot-3.1.0/README.md
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5625 2023-03-13 18:52:20.000000 datarobot-3.1.0/common_setup.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.883495 datarobot-3.1.0/datarobot/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2140 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      687 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/_compat.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      306 2023-03-13 18:52:23.000000 datarobot-3.1.0/datarobot/_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16695 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/client.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    22697 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/enums.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7993 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/errors.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.895291 datarobot-3.1.0/datarobot/helpers/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    22432 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/helpers/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13002 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/helpers/binary_data_utils.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1127 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/helpers/deployment_monitoring.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1156 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/helpers/eligibility_result.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14350 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/helpers/feature_discovery.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8696 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/helpers/image_utils.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    94333 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/helpers/partitioning_methods.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.899191 datarobot-3.1.0/datarobot/mixins/
--rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/mixins/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1134 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/mixins/browser_mixin.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1112 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/mixins/update_attributes_mixin.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.964288 datarobot-3.1.0/datarobot/models/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3943 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    12809 2023-03-13 17:59:36.000000 datarobot-3.1.0/datarobot/models/accuracy.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9166 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/advanced_tuning.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    23993 2023-03-13 17:59:36.000000 datarobot-3.1.0/datarobot/models/anomaly_assessment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2794 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/api_object.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14645 2023-03-13 17:59:36.000000 datarobot-3.1.0/datarobot/models/automated_documentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    81984 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/batch_prediction_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10455 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/blueprint.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    23822 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/calendar_file.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13301 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/change_request.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3978 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/cluster.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7233 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/cluster_insight.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11139 2023-03-13 17:59:36.000000 datarobot-3.1.0/datarobot/models/compliance_doc_template.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4180 2023-03-13 17:59:36.000000 datarobot-3.1.0/datarobot/models/confusion_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6953 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/connector.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11955 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/credential.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    24027 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/custom_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11963 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/custom_model_test.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    40997 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/custom_model_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15409 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/custom_task.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    21197 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/custom_task_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2315 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/custom_task_version_dependency_build.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8969 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/data_drift.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17613 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/data_engine_query_generator.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16402 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/data_source.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13812 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/data_store.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    55708 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    30524 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/datetime_trend_plots.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    83580 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/deployment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6583 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/driver.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9411 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/execution_environment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11344 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/execution_environment_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5374 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/external_baseline_validation.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.967902 datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      355 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6403 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4915 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4523 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5208 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4509 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6789 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    53938 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/feature.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.970001 datarobot-3.1.0/datarobot/models/feature_association_matrix/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      237 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/feature_association_matrix/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2600 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6177 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4753 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16677 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/feature_effect.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10333 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/feature_fit.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17463 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/featurelist.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7336 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/imported_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    21264 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2370 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5468 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/missing_report.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)   268103 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7215 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/modeljob.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14320 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/pairwise_statistics.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5438 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/pareto_front.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8726 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/payoff_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7403 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/predict_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10203 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/prediction_dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    33200 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/prediction_explanations.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2426 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/prediction_server.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15940 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/predictions.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2655 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/prime_file.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)   209294 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/project.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    55518 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/project_options.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8774 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/rating_table.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4337 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/recommended_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    19064 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/relationships_configuration.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2831 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/residuals.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4524 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/restore_discarded_features.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8203 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/roc_curve.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2927 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/ruleset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    19381 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/secondary_dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14217 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/segmentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10058 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/service_stats.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4070 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/shap_impact.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7057 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/shap_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2645 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/shap_matrix_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4214 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/sharing.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1431 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/trafarets.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    28260 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/training_predictions.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.972005 datarobot-3.1.0/datarobot/models/user_blueprints/
--rw-r--r--   0 andrew.levan   (504) staff       (20)       49 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/user_blueprints/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    69622 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/user_blueprints/models.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8758 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/user_blueprints/trafarets.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2668 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/validators.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.974386 datarobot-3.1.0/datarobot/models/visualai/
--rw-r--r--   0 andrew.levan   (504) staff       (20)       89 2023-03-13 17:59:36.000000 datarobot-3.1.0/datarobot/models/visualai/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    18528 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/visualai/augmentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7729 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/models/visualai/images.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10592 2023-03-13 17:59:36.000000 datarobot-3.1.0/datarobot/models/visualai/insights.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4936 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/models/word_cloud.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/py.typed
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17131 2023-03-13 18:52:20.000000 datarobot-3.1.0/datarobot/rest.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.978757 datarobot-3.1.0/datarobot/utils/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15333 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/utils/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2997 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/utils/deprecation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      495 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/utils/logger.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1200 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/utils/pagination.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1461 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/utils/retry.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1282 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/utils/source.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4109 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/utils/sourcedata.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4061 2023-03-10 16:03:09.000000 datarobot-3.1.0/datarobot/utils/waiters.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.887893 datarobot-3.1.0/datarobot.egg-info/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3283 2023-03-13 18:54:14.000000 datarobot-3.1.0/datarobot.egg-info/PKG-INFO
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6353 2023-03-13 18:54:14.000000 datarobot-3.1.0/datarobot.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)        1 2023-03-13 18:54:14.000000 datarobot-3.1.0/datarobot.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1093 2023-03-13 18:54:14.000000 datarobot-3.1.0/datarobot.egg-info/requires.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)       10 2023-03-13 18:54:14.000000 datarobot-3.1.0/datarobot.egg-info/top_level.txt
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.981860 datarobot-3.1.0/docs/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6404 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/Makefile
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.870448 datarobot-3.1.0/docs/_build/
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.982603 datarobot-3.1.0/docs/_build/latex/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1648 2023-03-13 18:53:57.000000 datarobot-3.1.0/docs/_build/latex/Makefile
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.983180 datarobot-3.1.0/docs/autodoc/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17499 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/autodoc/api_reference.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10245 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/conf.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.983903 datarobot-3.1.0/docs/examples/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1958 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/examples/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      415 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/getting_started.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      961 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)        2 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/predicted.csv
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.984610 datarobot-3.1.0/docs/reference/
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.986600 datarobot-3.1.0/docs/reference/admin/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3474 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/admin/credentials.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      415 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/admin/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3645 2023-03-13 17:59:36.000000 datarobot-3.1.0/docs/reference/admin/sharing.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.989207 datarobot-3.1.0/docs/reference/data/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7711 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/reference/data/database_connectivity.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9959 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/reference/data/dataset.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    22218 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/reference/data/feature_discovery.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      612 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/data/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      391 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/index.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.991238 datarobot-3.1.0/docs/reference/mlops/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    29303 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/mlops/custom_model.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    23173 2023-03-13 17:59:36.000000 datarobot-3.1.0/docs/reference/mlops/deployment.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      427 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/mlops/index.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.995943 datarobot-3.1.0/docs/reference/modeling/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4396 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/blueprint.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      570 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/index.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:14.998493 datarobot-3.1.0/docs/reference/modeling/insights/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5077 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/insights/automated_documentation.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4033 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/insights/external_testset.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      536 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/insights/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10234 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/reference/modeling/insights/prediction_explanations.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2277 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/insights/rating_table.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5305 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/job.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    21949 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/reference/modeling/model.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3448 2023-03-13 17:59:36.000000 datarobot-3.1.0/docs/reference/modeling/model_recommendation.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3385 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/prime.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16205 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/reference/modeling/project.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:15.003285 datarobot-3.1.0/docs/reference/modeling/spec/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11364 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/spec/binary_data.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7430 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/spec/custom_task.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10036 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/spec/datetime_partition.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      620 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/spec/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6625 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/spec/monotonic_constraints.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6204 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/spec/segmented_modeling.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    36391 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/reference/modeling/spec/time_series.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10392 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/spec/unsupervised_anomaly.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7376 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/modeling/spec/unsupervised_clustering.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14760 2023-03-13 18:52:20.000000 datarobot-3.1.0/docs/reference/modeling/spec/visualai.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-03-13 18:54:15.004702 datarobot-3.1.0/docs/reference/predictions/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    39016 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/predictions/batch_predictions.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1180 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/predictions/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9015 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/reference/predictions/predict_job.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      319 2023-03-10 16:03:09.000000 datarobot-3.1.0/docs/version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3386 2023-03-13 18:52:20.000000 datarobot-3.1.0/pyproject.toml
--rw-r--r--   0 andrew.levan   (504) staff       (20)      123 2023-03-13 18:54:15.005678 datarobot-3.1.0/setup.cfg
--rw-r--r--   0 andrew.levan   (504) staff       (20)      965 2023-03-10 16:03:09.000000 datarobot-3.1.0/setup.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1208 2023-03-10 16:03:09.000000 datarobot-3.1.0/setup_major.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.067422 datarobot-3.1.1/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   161611 2023-05-15 19:45:56.000000 datarobot-3.1.1/CHANGES.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7555 2023-03-10 16:03:09.000000 datarobot-3.1.1/LICENSE.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      421 2023-03-10 16:03:09.000000 datarobot-3.1.1/MANIFEST.in
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3283 2023-05-15 19:50:05.067684 datarobot-3.1.1/PKG-INFO
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8441 2023-05-15 19:45:52.000000 datarobot-3.1.1/README.md
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5603 2023-05-15 19:45:52.000000 datarobot-3.1.1/common_setup.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:04.987268 datarobot-3.1.1/datarobot/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2140 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      687 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/_compat.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      306 2023-05-15 19:45:56.000000 datarobot-3.1.1/datarobot/_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    16695 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/client.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    22697 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/enums.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7993 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/errors.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:04.994033 datarobot-3.1.1/datarobot/helpers/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    22432 2023-05-09 15:22:07.000000 datarobot-3.1.1/datarobot/helpers/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13002 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/helpers/binary_data_utils.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1127 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/helpers/deployment_monitoring.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1156 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/helpers/eligibility_result.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14350 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/helpers/feature_discovery.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8696 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/helpers/image_utils.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    94333 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/helpers/partitioning_methods.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:04.995403 datarobot-3.1.1/datarobot/mixins/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/mixins/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1134 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/mixins/browser_mixin.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1112 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/mixins/update_attributes_mixin.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.037797 datarobot-3.1.1/datarobot/models/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3943 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    12809 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/accuracy.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     9166 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/advanced_tuning.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    23993 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/anomaly_assessment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2794 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/api_object.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14645 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/automated_documentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    81984 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/batch_prediction_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10455 2023-05-11 14:05:22.000000 datarobot-3.1.1/datarobot/models/blueprint.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    23822 2023-05-11 14:05:22.000000 datarobot-3.1.1/datarobot/models/calendar_file.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13301 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/change_request.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3978 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/cluster.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7233 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/cluster_insight.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11139 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/compliance_doc_template.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4180 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/confusion_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6953 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/connector.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11955 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/credential.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    24027 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/custom_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11963 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/custom_model_test.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    40995 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/custom_model_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15409 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/custom_task.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    21195 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/custom_task_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2315 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/custom_task_version_dependency_build.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8969 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/data_drift.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17613 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/models/data_engine_query_generator.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    16402 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/data_source.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13812 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/data_store.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    55708 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    30524 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/datetime_trend_plots.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    83580 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/deployment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6583 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/driver.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     9411 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/execution_environment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11344 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/execution_environment_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5374 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/external_baseline_validation.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.041171 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      355 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6403 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4915 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4523 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5208 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4509 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6789 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    53938 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/feature.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.043055 datarobot-3.1.1/datarobot/models/feature_association_matrix/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      237 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/feature_association_matrix/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2600 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6177 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4753 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    16677 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/feature_effect.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10333 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/feature_fit.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17463 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/featurelist.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7336 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/imported_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    21264 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2370 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5468 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/missing_report.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   268103 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7215 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/models/modeljob.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14320 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/pairwise_statistics.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5438 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/pareto_front.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8726 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/payoff_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7403 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/models/predict_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10203 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/prediction_dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    33200 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/prediction_explanations.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2426 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/prediction_server.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15940 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/predictions.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2655 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/prime_file.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   209294 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/project.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    55518 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/project_options.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8774 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/rating_table.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4337 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/recommended_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    19064 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/models/relationships_configuration.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2831 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/residuals.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4524 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/restore_discarded_features.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8203 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/roc_curve.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2927 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/ruleset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    19381 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/secondary_dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14217 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/segmentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10058 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/service_stats.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4070 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/shap_impact.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7057 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/shap_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2645 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/shap_matrix_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4214 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/sharing.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1431 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/trafarets.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    28260 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/training_predictions.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.044445 datarobot-3.1.1/datarobot/models/user_blueprints/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)       49 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/user_blueprints/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    69622 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/user_blueprints/models.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8758 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/user_blueprints/trafarets.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2668 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/validators.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.046784 datarobot-3.1.1/datarobot/models/visualai/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)       89 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/visualai/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    18528 2023-05-11 14:04:17.000000 datarobot-3.1.1/datarobot/models/visualai/augmentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7729 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/visualai/images.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10592 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/visualai/insights.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4936 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/word_cloud.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/py.typed
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17131 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/rest.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.050697 datarobot-3.1.1/datarobot/utils/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15333 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/utils/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2997 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/deprecation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      495 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/logger.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1200 2023-04-18 15:18:29.000000 datarobot-3.1.1/datarobot/utils/pagination.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1461 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/retry.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1282 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/source.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4109 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/sourcedata.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4061 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/waiters.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:04.989196 datarobot-3.1.1/datarobot.egg-info/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3283 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/PKG-INFO
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6326 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        1 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1077 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/requires.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)       10 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/top_level.txt
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.052773 datarobot-3.1.1/docs/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6404 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/Makefile
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.053098 datarobot-3.1.1/docs/autodoc/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17499 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/autodoc/api_reference.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10245 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/conf.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.053461 datarobot-3.1.1/docs/examples/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1958 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/examples/index.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      415 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/getting_started.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      961 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/index.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        2 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/predicted.csv
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.053779 datarobot-3.1.1/docs/reference/
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.054859 datarobot-3.1.1/docs/reference/admin/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3474 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/admin/credentials.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      415 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/admin/index.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3645 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/admin/sharing.rst
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.056262 datarobot-3.1.1/docs/reference/data/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7711 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/data/database_connectivity.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     9959 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/data/dataset.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    22218 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/data/feature_discovery.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      612 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/data/index.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      391 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/index.rst
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.057403 datarobot-3.1.1/docs/reference/mlops/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    29303 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/mlops/custom_model.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    23173 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/mlops/deployment.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      427 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/mlops/index.rst
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.059850 datarobot-3.1.1/docs/reference/modeling/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4396 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/blueprint.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      570 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/index.rst
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.061731 datarobot-3.1.1/docs/reference/modeling/insights/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5077 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/automated_documentation.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4033 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/external_testset.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      536 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/index.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10234 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/prediction_explanations.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2277 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/rating_table.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5305 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/job.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    21949 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/model.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3448 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/model_recommendation.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3385 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/prime.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    16205 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/project.rst
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.065381 datarobot-3.1.1/docs/reference/modeling/spec/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11364 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/binary_data.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7430 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/custom_task.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10036 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/datetime_partition.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      620 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/index.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6625 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/monotonic_constraints.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6204 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/segmented_modeling.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    36391 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/time_series.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10392 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/unsupervised_anomaly.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7376 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/unsupervised_clustering.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14760 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/visualai.rst
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.066848 datarobot-3.1.1/docs/reference/predictions/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    39016 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/predictions/batch_predictions.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1180 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/predictions/index.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     9015 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/predictions/predict_job.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      319 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3386 2023-05-15 19:45:52.000000 datarobot-3.1.1/pyproject.toml
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      123 2023-05-15 19:50:05.068334 datarobot-3.1.1/setup.cfg
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      965 2023-03-10 16:03:09.000000 datarobot-3.1.1/setup.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1208 2023-05-15 19:45:52.000000 datarobot-3.1.1/setup_major.py
```

### Comparing `datarobot-3.1.0/CHANGES.rst` & `datarobot-3.1.1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #########
 Changelog
 #########
+
+3.1.1
+=====
+
+Configuration Changes
+*********************
+- Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
+- Update `typing-extensions <https://pypi.org/project/typing-extensions/>`_ to be inclusive of versions from 4.3.0 to < 5.0.0.
+
 3.1.0
 =====
 
 New Features
 ************
 
 Enhancements
@@ -49,15 +58,15 @@
 *******************
 - Deprecated method :meth:`Project.create_from_hdfs<datarobot.models.Project.create_from_hdfs>`.
 - Deprecated method :meth:`DatetimePartitioning.generate <datarobot.DatetimePartitioning.generate>`.
 - Deprecated parameter ``in_use`` from :meth:`ImageAugmentationList.create<datarobot.models.visualai.ImageAugmentationList.create>` as DataRobot will take care of it automatically.
 - Deprecated property ``Deployment.capabilities`` from :class:`Deployment <datarobot.models.Deployment>`.
 - ``ImageAugmentationSample.compute`` was removed in v3.1. You
   can get the same information with the method ``ImageAugmentationList.compute_samples``.
-- ``sample_id`` parameter removed from ``ImageAugmentationSample.list``. Please use ``auglist_id`` instead. 
+- ``sample_id`` parameter removed from ``ImageAugmentationSample.list``. Please use ``auglist_id`` instead.
 
 Configuration Changes
 *********************
 
 Experimental changes
 *********************
 - Added :meth:`DatetimePartitioning.datetime_partitioning_log_retrieve <datarobot._experimental.helpers.partitioning_methods.DatetimePartitioning.datetime_partitioning_log_retrieve>` to download the datetime partitioning log.
@@ -68,22 +77,28 @@
 
 Documentation Changes
 *********************
 - Update the documentation to suggest that setting `use_backtest_start_end_format` of :py:meth:`DatetimePartitioning.to_specification <datarobot.DatetimePartitioning.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
 - Update the documentation to suggest setting `use_start_end_format` of :py:meth:`Backtest.to_specification <datarobot.helpers.partitioning_methods.Backtest.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
+3.0.3
+=====
+
+Bugfixes
+********
+- Fixed an issue affecting backwards compatibility in :class:`datarobot.models.DatetimeModel`, where an unexpected keyword from the DataRobot API would break class deserialization.
 
 3.0.2
 =====
 
 Bugfixes
 ********
 - Restored :meth:`Model.get_leaderboard_ui_permalink <datarobot.models.Model.get_leaderboard_ui_permalink>`, :meth:`Model.open_model_browser <datarobot.models.Model.open_model_browser>`,
-  :meth:`Project.get_leaderboard_ui_permalink <datarobot.models.Project.get_leaderboard_ui_permalink>`, and :meth:`Project.open_leaderboard_browser <datarobot.models.Project.open_leaderboard_browser>`. 
+  :meth:`Project.get_leaderboard_ui_permalink <datarobot.models.Project.get_leaderboard_ui_permalink>`, and :meth:`Project.open_leaderboard_browser <datarobot.models.Project.open_leaderboard_browser>`.
   These methods were accidentally removed instead of deprecated.
 - Fix for ipykernel < 6.0.0 which does not persist contextvars across cells
 
 Deprecation Summary
 *******************
 - Deprecated method :meth:`Model.get_leaderboard_ui_permalink <datarobot.models.Model.get_leaderboard_ui_permalink>`. Please use :meth:`Model.get_uri <datarobot.models.Model.get_uri>` instead.
 - Deprecated method :meth:`Model.open_model_browser <datarobot.models.Model.open_model_browser>`. Please use :meth:`Model.open_in_browser <datarobot.models.Model.open_in_browser>` instead.
```

### Comparing `datarobot-3.1.0/LICENSE.txt` & `datarobot-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/PKG-INFO` & `datarobot-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot
-Version: 3.1.0
+Version: 3.1.1
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot-3.1.0/README.md` & `datarobot-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/common_setup.py` & `datarobot-3.1.1/common_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -175,23 +175,22 @@
     license="DataRobot Tool and Utility Agreement",
     packages=None,
     package_data={"datarobot": ["py.typed"]},
     python_requires=">=3.7",
     long_description=None,
     classifiers=None,
     install_requires=[
-        "contextlib2>=0.5.5",
         "pandas>=0.15",
         "numpy",
         "pyyaml>=3.11",
         "requests>=2.21",
         "requests_toolbelt>=0.6",
         "trafaret>=0.7,<2.2,!=1.1.0",
         "urllib3>=1.23",
-        "typing-extensions==4.3.0",
+        "typing-extensions>=4.3.0,<5",
     ],
     extras_require={
         "dev": dev_require,
         "examples": example_require,
         "release": release_require,
         "lint": lint_require,
         "images": images_require,
```

### Comparing `datarobot-3.1.0/datarobot/__init__.py` & `datarobot-3.1.1/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/_compat.py` & `datarobot-3.1.1/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/client.py` & `datarobot-3.1.1/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/enums.py` & `datarobot-3.1.1/datarobot/enums.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/errors.py` & `datarobot-3.1.1/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/helpers/__init__.py` & `datarobot-3.1.1/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/helpers/binary_data_utils.py` & `datarobot-3.1.1/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/helpers/deployment_monitoring.py` & `datarobot-3.1.1/datarobot/helpers/deployment_monitoring.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/helpers/eligibility_result.py` & `datarobot-3.1.1/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/helpers/feature_discovery.py` & `datarobot-3.1.1/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/helpers/image_utils.py` & `datarobot-3.1.1/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/helpers/partitioning_methods.py` & `datarobot-3.1.1/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/mixins/browser_mixin.py` & `datarobot-3.1.1/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/mixins/update_attributes_mixin.py` & `datarobot-3.1.1/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/__init__.py` & `datarobot-3.1.1/datarobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/accuracy.py` & `datarobot-3.1.1/datarobot/models/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/advanced_tuning.py` & `datarobot-3.1.1/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/anomaly_assessment.py` & `datarobot-3.1.1/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/api_object.py` & `datarobot-3.1.1/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/automated_documentation.py` & `datarobot-3.1.1/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/batch_prediction_job.py` & `datarobot-3.1.1/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/blueprint.py` & `datarobot-3.1.1/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/calendar_file.py` & `datarobot-3.1.1/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/change_request.py` & `datarobot-3.1.1/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/cluster.py` & `datarobot-3.1.1/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/cluster_insight.py` & `datarobot-3.1.1/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/compliance_doc_template.py` & `datarobot-3.1.1/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/confusion_chart.py` & `datarobot-3.1.1/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/connector.py` & `datarobot-3.1.1/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/credential.py` & `datarobot-3.1.1/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/custom_model.py` & `datarobot-3.1.1/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/custom_model_test.py` & `datarobot-3.1.1/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/custom_model_version.py` & `datarobot-3.1.1/datarobot/models/custom_model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+import contextlib
 import copy
 import json
 import os
 
-import contextlib2
 from requests_toolbelt import MultipartEncoder
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import DEFAULT_MAX_WAIT, NETWORK_EGRESS_POLICY
 from datarobot.errors import InvalidUsageError
 from datarobot.models.api_object import APIObject
@@ -684,15 +684,15 @@
         network_egress_policy=None,
         maximum_memory=None,
         replicas=None,
         required_metadata_values=None,
     ):
         url = cls._path.format(custom_model_id)
 
-        with contextlib2.ExitStack() as stack:
+        with contextlib.ExitStack() as stack:
             upload_data = [
                 ("isMajorUpdate", str(is_major_update)),
                 ("baseEnvironmentId", base_environment_id),
             ]
 
             if folder_path:
                 for root_path, _, file_paths in os.walk(folder_path):
```

### Comparing `datarobot-3.1.0/datarobot/models/custom_task.py` & `datarobot-3.1.1/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/custom_task_version.py` & `datarobot-3.1.1/datarobot/models/custom_task_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
+import contextlib
 import json
 import os
 
-import contextlib2
 from requests_toolbelt import MultipartEncoder
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model_version import (
     CustomDependency,
@@ -352,15 +352,15 @@
             )
 
         if maximum_memory:
             upload_data.append(("maximumMemory", str(maximum_memory)))
 
         cls._verify_folder_path(folder_path)
 
-        with contextlib2.ExitStack() as stack:
+        with contextlib.ExitStack() as stack:
             if folder_path:
                 for dir_name, _, file_names in os.walk(folder_path):
                     for file_name in file_names:
                         file_path = os.path.join(dir_name, file_name)
                         file = stack.enter_context(
                             open(file_path, "rb")  # pylint: disable=consider-using-with
                         )
```

### Comparing `datarobot-3.1.0/datarobot/models/custom_task_version_dependency_build.py` & `datarobot-3.1.1/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/data_drift.py` & `datarobot-3.1.1/datarobot/models/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/data_engine_query_generator.py` & `datarobot-3.1.1/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/data_source.py` & `datarobot-3.1.1/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/data_store.py` & `datarobot-3.1.1/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/dataset.py` & `datarobot-3.1.1/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/datetime_trend_plots.py` & `datarobot-3.1.1/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/deployment.py` & `datarobot-3.1.1/datarobot/models/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/driver.py` & `datarobot-3.1.1/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/execution_environment.py` & `datarobot-3.1.1/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/execution_environment_version.py` & `datarobot-3.1.1/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/external_baseline_validation.py` & `datarobot-3.1.1/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/feature.py` & `datarobot-3.1.1/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/feature_effect.py` & `datarobot-3.1.1/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/feature_fit.py` & `datarobot-3.1.1/datarobot/models/feature_fit.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/featurelist.py` & `datarobot-3.1.1/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/imported_model.py` & `datarobot-3.1.1/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/job.py` & `datarobot-3.1.1/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/lift_chart.py` & `datarobot-3.1.1/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/missing_report.py` & `datarobot-3.1.1/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/model.py` & `datarobot-3.1.1/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/modeljob.py` & `datarobot-3.1.1/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/pairwise_statistics.py` & `datarobot-3.1.1/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/pareto_front.py` & `datarobot-3.1.1/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/payoff_matrix.py` & `datarobot-3.1.1/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/predict_job.py` & `datarobot-3.1.1/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/prediction_dataset.py` & `datarobot-3.1.1/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/prediction_explanations.py` & `datarobot-3.1.1/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/prediction_server.py` & `datarobot-3.1.1/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/predictions.py` & `datarobot-3.1.1/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/prime_file.py` & `datarobot-3.1.1/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/project.py` & `datarobot-3.1.1/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/project_options.py` & `datarobot-3.1.1/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/rating_table.py` & `datarobot-3.1.1/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/recommended_model.py` & `datarobot-3.1.1/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/relationships_configuration.py` & `datarobot-3.1.1/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/residuals.py` & `datarobot-3.1.1/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/restore_discarded_features.py` & `datarobot-3.1.1/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/roc_curve.py` & `datarobot-3.1.1/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/ruleset.py` & `datarobot-3.1.1/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/secondary_dataset.py` & `datarobot-3.1.1/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/segmentation.py` & `datarobot-3.1.1/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/service_stats.py` & `datarobot-3.1.1/datarobot/models/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/shap_impact.py` & `datarobot-3.1.1/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/shap_matrix.py` & `datarobot-3.1.1/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/shap_matrix_job.py` & `datarobot-3.1.1/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/sharing.py` & `datarobot-3.1.1/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/trafarets.py` & `datarobot-3.1.1/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/training_predictions.py` & `datarobot-3.1.1/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/user_blueprints/models.py` & `datarobot-3.1.1/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/user_blueprints/trafarets.py` & `datarobot-3.1.1/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/validators.py` & `datarobot-3.1.1/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/visualai/augmentation.py` & `datarobot-3.1.1/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/visualai/images.py` & `datarobot-3.1.1/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/visualai/insights.py` & `datarobot-3.1.1/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/models/word_cloud.py` & `datarobot-3.1.1/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/rest.py` & `datarobot-3.1.1/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/utils/__init__.py` & `datarobot-3.1.1/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/utils/deprecation.py` & `datarobot-3.1.1/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/utils/pagination.py` & `datarobot-3.1.1/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/utils/retry.py` & `datarobot-3.1.1/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/utils/source.py` & `datarobot-3.1.1/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/utils/sourcedata.py` & `datarobot-3.1.1/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot/utils/waiters.py` & `datarobot-3.1.1/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/datarobot.egg-info/PKG-INFO` & `datarobot-3.1.1/datarobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot
-Version: 3.1.0
+Version: 3.1.1
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot-3.1.0/datarobot.egg-info/SOURCES.txt` & `datarobot-3.1.1/datarobot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,14 @@
 datarobot/utils/waiters.py
 docs/Makefile
 docs/conf.py
 docs/getting_started.rst
 docs/index.rst
 docs/predicted.csv
 docs/version.py
-docs/_build/latex/Makefile
 docs/autodoc/api_reference.rst
 docs/examples/index.rst
 docs/reference/index.rst
 docs/reference/admin/credentials.rst
 docs/reference/admin/index.rst
 docs/reference/admin/sharing.rst
 docs/reference/data/database_connectivity.rst
```

### Comparing `datarobot-3.1.0/datarobot.egg-info/requires.txt` & `datarobot-3.1.1/datarobot.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-contextlib2>=0.5.5
 pandas>=0.15
 numpy
 pyyaml>=3.11
 requests>=2.21
 requests_toolbelt>=0.6
 trafaret!=1.1.0,<2.2,>=0.7
 urllib3>=1.23
-typing-extensions==4.3.0
+typing-extensions<5,>=4.3.0
 
 [dev]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
 pytest-asyncio
```

### Comparing `datarobot-3.1.0/docs/Makefile` & `datarobot-3.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/autodoc/api_reference.rst` & `datarobot-3.1.1/docs/autodoc/api_reference.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/conf.py` & `datarobot-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/examples/index.rst` & `datarobot-3.1.1/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/index.rst` & `datarobot-3.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/admin/credentials.rst` & `datarobot-3.1.1/docs/reference/admin/credentials.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/admin/sharing.rst` & `datarobot-3.1.1/docs/reference/admin/sharing.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/data/database_connectivity.rst` & `datarobot-3.1.1/docs/reference/data/database_connectivity.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/data/dataset.rst` & `datarobot-3.1.1/docs/reference/data/dataset.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/data/feature_discovery.rst` & `datarobot-3.1.1/docs/reference/data/feature_discovery.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/data/index.rst` & `datarobot-3.1.1/docs/reference/data/index.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/mlops/custom_model.rst` & `datarobot-3.1.1/docs/reference/mlops/custom_model.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/mlops/deployment.rst` & `datarobot-3.1.1/docs/reference/mlops/deployment.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/blueprint.rst` & `datarobot-3.1.1/docs/reference/modeling/blueprint.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/index.rst` & `datarobot-3.1.1/docs/reference/modeling/index.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/insights/automated_documentation.rst` & `datarobot-3.1.1/docs/reference/modeling/insights/automated_documentation.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/insights/external_testset.rst` & `datarobot-3.1.1/docs/reference/modeling/insights/external_testset.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/insights/index.rst` & `datarobot-3.1.1/docs/reference/modeling/insights/index.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/insights/prediction_explanations.rst` & `datarobot-3.1.1/docs/reference/modeling/insights/prediction_explanations.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/insights/rating_table.rst` & `datarobot-3.1.1/docs/reference/modeling/insights/rating_table.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/job.rst` & `datarobot-3.1.1/docs/reference/modeling/job.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/model.rst` & `datarobot-3.1.1/docs/reference/modeling/model.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/model_recommendation.rst` & `datarobot-3.1.1/docs/reference/modeling/model_recommendation.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/prime.rst` & `datarobot-3.1.1/docs/reference/modeling/prime.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/project.rst` & `datarobot-3.1.1/docs/reference/modeling/project.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/binary_data.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/binary_data.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/custom_task.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/custom_task.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/datetime_partition.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/datetime_partition.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/index.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/index.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/monotonic_constraints.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/monotonic_constraints.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/segmented_modeling.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/segmented_modeling.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/time_series.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/time_series.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/unsupervised_anomaly.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/unsupervised_anomaly.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/unsupervised_clustering.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/unsupervised_clustering.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/modeling/spec/visualai.rst` & `datarobot-3.1.1/docs/reference/modeling/spec/visualai.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/predictions/batch_predictions.rst` & `datarobot-3.1.1/docs/reference/predictions/batch_predictions.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/predictions/index.rst` & `datarobot-3.1.1/docs/reference/predictions/index.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/docs/reference/predictions/predict_job.rst` & `datarobot-3.1.1/docs/reference/predictions/predict_job.rst`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/pyproject.toml` & `datarobot-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/setup.py` & `datarobot-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.0/setup_major.py` & `datarobot-3.1.1/setup_major.py`

 * *Files identical despite different names*

