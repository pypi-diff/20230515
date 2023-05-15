# Comparing `tmp/digitalai_release_sdk-23.1.0.tar.gz` & `tmp/digitalai_release_sdk-23.1.0rc1.tar.gz`

## Comparing `digitalai_release_sdk-23.1.0.tar` & `digitalai_release_sdk-23.1.0rc1.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/.github/workflows/python-test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/__init__.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/base_task.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/exceptions.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/input_context.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/job_data_encryptor.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/logging_config.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/masked_io.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/output_context.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/reporting_records.py
--rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/integration/wrapper.py
--rw-r--r--   0        0        0    43401 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/__init__.py
--rw-r--r--   0        0        0    40046 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api_client.py
--rw-r--r--   0        0        0    18319 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/configuration.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/exceptions.py
--rw-r--r--   0        0        0    84684 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model_utils.py
--rw-r--r--   0        0        0    14672 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/rest.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/__init__.py
--rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/activity_logs_api.py
--rw-r--r--   0        0        0    27710 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/application_api.py
--rw-r--r--   0        0        0    80045 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/configuration_api.py
--rw-r--r--   0        0        0   117358 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/delivery_api.py
--rw-r--r--   0        0        0   127626 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/delivery_pattern_api.py
--rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/dsl_api.py
--rw-r--r--   0        0        0    39032 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/environment_api.py
--rw-r--r--   0        0        0    28114 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/environment_label_api.py
--rw-r--r--   0        0        0    34558 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/environment_reservation_api.py
--rw-r--r--   0        0        0    28210 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/environment_stage_api.py
--rw-r--r--   0        0        0    32145 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/facet_api.py
--rw-r--r--   0        0        0   119798 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/folder_api.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/permissions_api.py
--rw-r--r--   0        0        0    44830 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/phase_api.py
--rw-r--r--   0        0        0    16975 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/planner_api.py
--rw-r--r--   0        0        0   155122 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/release_api.py
--rw-r--r--   0        0        0    49962 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/release_group_api.py
--rw-r--r--   0        0        0    22528 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/report_api.py
--rw-r--r--   0        0        0    52723 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/risk_api.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/risk_assessment_api.py
--rw-r--r--   0        0        0    42815 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/roles_api.py
--rw-r--r--   0        0        0   155071 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/task_api.py
--rw-r--r--   0        0        0   121845 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/template_api.py
--rw-r--r--   0        0        0    69042 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/triggers_api.py
--rw-r--r--   0        0        0    39680 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/api/user_api.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/apis/__init__.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/__init__.py
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/abort_release.py
--rw-r--r--   0        0        0    13364 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/activity_log_entry.py
--rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/application_filters.py
--rw-r--r--   0        0        0    11967 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/application_form.py
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/application_view.py
--rw-r--r--   0        0        0    14191 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/attachment.py
--rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/base_application_view.py
--rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/base_environment_view.py
--rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/blackout_metadata.py
--rw-r--r--   0        0        0    11977 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/blackout_period.py
--rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/bulk_action_result_view.py
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/change_password_view.py
--rw-r--r--   0        0        0    15183 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/ci_property.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/comment.py
--rw-r--r--   0        0        0    11714 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/comment1.py
--rw-r--r--   0        0        0    12018 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/complete_transition.py
--rw-r--r--   0        0        0    13860 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/condition.py
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/condition1.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/configuration_facet.py
--rw-r--r--   0        0        0    12525 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/configuration_view.py
--rw-r--r--   0        0        0    11933 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/copy_template.py
--rw-r--r--   0        0        0    13372 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/create_delivery.py
--rw-r--r--   0        0        0    12278 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/create_delivery_stage.py
--rw-r--r--   0        0        0    13969 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/create_release.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery.py
--rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_filters.py
--rw-r--r--   0        0        0    12760 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_flow_release_info.py
--rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_order_mode.py
--rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_pattern_filters.py
--rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_status.py
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_timeline.py
--rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/dependency.py
--rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/duplicate_delivery_pattern.py
--rw-r--r--   0        0        0    12119 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_filters.py
--rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_form.py
--rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_label_filters.py
--rw-r--r--   0        0        0    11927 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_label_form.py
--rw-r--r--   0        0        0    12099 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_label_view.py
--rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_reservation_form.py
--rw-r--r--   0        0        0    13456 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_reservation_search_view.py
--rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_reservation_view.py
--rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_stage_filters.py
--rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_stage_form.py
--rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_stage_view.py
--rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_view.py
--rw-r--r--   0        0        0    12367 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/external_variable_value.py
--rw-r--r--   0        0        0    13804 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/facet.py
--rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/facet_filters.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/facet_scope.py
--rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/flag_status.py
--rw-r--r--   0        0        0    13364 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/folder.py
--rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/folder_variables.py
--rw-r--r--   0        0        0    12273 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/gate_condition.py
--rw-r--r--   0        0        0    37643 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/gate_task.py
--rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/global_variables.py
--rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/import_result.py
--rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/member_type.py
--rw-r--r--   0        0        0    12427 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/model_property.py
--rw-r--r--   0        0        0    22798 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/phase.py
--rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/phase_status.py
--rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/phase_timeline.py
--rw-r--r--   0        0        0    12324 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/phase_version.py
--rw-r--r--   0        0        0    18794 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/plan_item.py
--rw-r--r--   0        0        0    12233 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/poll_type.py
--rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/principal_view.py
--rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/projected_phase.py
--rw-r--r--   0        0        0    13620 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/projected_release.py
--rw-r--r--   0        0        0    13187 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/projected_task.py
--rw-r--r--   0        0        0    37799 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release.py
--rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_configuration.py
--rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_count_result.py
--rw-r--r--   0        0        0    12456 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_count_results.py
--rw-r--r--   0        0        0    12335 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_extension.py
--rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_full_search_result.py
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group.py
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group_filters.py
--rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group_order_mode.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group_status.py
--rw-r--r--   0        0        0    13006 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group_timeline.py
--rw-r--r--   0        0        0    12254 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_order_direction.py
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_order_mode.py
--rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_search_result.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_status.py
--rw-r--r--   0        0        0    14321 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_timeline.py
--rw-r--r--   0        0        0    20032 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_trigger.py
--rw-r--r--   0        0        0    17803 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/releases_filters.py
--rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/reservation_filters.py
--rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/reservation_search_view.py
--rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk.py
--rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_assessment.py
--rw-r--r--   0        0        0    13222 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_assessor.py
--rw-r--r--   0        0        0    12785 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_global_thresholds.py
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_profile.py
--rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_status.py
--rw-r--r--   0        0        0    12464 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_status_with_thresholds.py
--rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/role_view.py
--rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/shared_configuration_status_response.py
--rw-r--r--   0        0        0    13902 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/stage.py
--rw-r--r--   0        0        0    12242 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/stage_status.py
--rw-r--r--   0        0        0    12479 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/stage_tracked_item.py
--rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/start_release.py
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/start_task.py
--rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/subscriber.py
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/system_message_settings.py
--rw-r--r--   0        0        0    35913 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task.py
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task_container.py
--rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task_recover_op.py
--rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task_reporting_record.py
--rw-r--r--   0        0        0    14337 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task_status.py
--rw-r--r--   0        0        0    13910 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/team.py
--rw-r--r--   0        0        0    12499 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/team_member_view.py
--rw-r--r--   0        0        0    12767 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/team_view.py
--rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/time_frame.py
--rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/tracked_item.py
--rw-r--r--   0        0        0    12363 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/tracked_item_status.py
--rw-r--r--   0        0        0    13727 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/transition.py
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/trigger.py
--rw-r--r--   0        0        0    12299 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/trigger_execution_status.py
--rw-r--r--   0        0        0    11957 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/usage_point.py
--rw-r--r--   0        0        0    14832 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/user_account.py
--rw-r--r--   0        0        0    36232 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/user_input_task.py
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/validate_pattern.py
--rw-r--r--   0        0        0    12310 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/value_provider_configuration.py
--rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/value_with_interpolation.py
--rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/variable.py
--rw-r--r--   0        0        0    15028 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/variable1.py
--rw-r--r--   0        0        0    12098 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/model/variable_or_value.py
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/digitalai/release/v1/models/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/tests/release/api/test_release_api_methods.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/tests/release/integration/expected_output.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/tests/release/integration/hello.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/tests/release/integration/input.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/tests/release/integration/output.json
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/tests/release/integration/test_wrapper.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/LICENSE
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/README.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/pyproject.toml
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/__init__.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/base_task.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/exceptions.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/input_context.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/job_data_encryptor.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/logging_config.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/masked_io.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/output_context.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/reporting_records.py
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/wrapper.py
+-rw-r--r--   0        0        0    43401 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/__init__.py
+-rw-r--r--   0        0        0    40046 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api_client.py
+-rw-r--r--   0        0        0    18319 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/configuration.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/exceptions.py
+-rw-r--r--   0        0        0    84684 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model_utils.py
+-rw-r--r--   0        0        0    14672 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/rest.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/__init__.py
+-rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/activity_logs_api.py
+-rw-r--r--   0        0        0    27710 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/application_api.py
+-rw-r--r--   0        0        0    80045 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/configuration_api.py
+-rw-r--r--   0        0        0   117358 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/delivery_api.py
+-rw-r--r--   0        0        0   127626 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/delivery_pattern_api.py
+-rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/dsl_api.py
+-rw-r--r--   0        0        0    39032 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/environment_api.py
+-rw-r--r--   0        0        0    28114 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/environment_label_api.py
+-rw-r--r--   0        0        0    34558 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/environment_reservation_api.py
+-rw-r--r--   0        0        0    28210 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/environment_stage_api.py
+-rw-r--r--   0        0        0    32145 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/facet_api.py
+-rw-r--r--   0        0        0   119798 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/folder_api.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/permissions_api.py
+-rw-r--r--   0        0        0    44830 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/phase_api.py
+-rw-r--r--   0        0        0    16975 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/planner_api.py
+-rw-r--r--   0        0        0   155122 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/release_api.py
+-rw-r--r--   0        0        0    49962 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/release_group_api.py
+-rw-r--r--   0        0        0    22528 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/report_api.py
+-rw-r--r--   0        0        0    52723 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/risk_api.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/risk_assessment_api.py
+-rw-r--r--   0        0        0    42815 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/roles_api.py
+-rw-r--r--   0        0        0   155071 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/task_api.py
+-rw-r--r--   0        0        0   121845 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/template_api.py
+-rw-r--r--   0        0        0    69042 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/triggers_api.py
+-rw-r--r--   0        0        0    39680 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/user_api.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/apis/__init__.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/__init__.py
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/abort_release.py
+-rw-r--r--   0        0        0    13364 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/activity_log_entry.py
+-rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/application_filters.py
+-rw-r--r--   0        0        0    11967 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/application_form.py
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/application_view.py
+-rw-r--r--   0        0        0    14191 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/attachment.py
+-rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/base_application_view.py
+-rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/base_environment_view.py
+-rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/blackout_metadata.py
+-rw-r--r--   0        0        0    11977 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/blackout_period.py
+-rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/bulk_action_result_view.py
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/change_password_view.py
+-rw-r--r--   0        0        0    15183 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/ci_property.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/comment.py
+-rw-r--r--   0        0        0    11714 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/comment1.py
+-rw-r--r--   0        0        0    12018 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/complete_transition.py
+-rw-r--r--   0        0        0    13860 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/condition.py
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/condition1.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/configuration_facet.py
+-rw-r--r--   0        0        0    12525 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/configuration_view.py
+-rw-r--r--   0        0        0    11933 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/copy_template.py
+-rw-r--r--   0        0        0    13372 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/create_delivery.py
+-rw-r--r--   0        0        0    12278 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/create_delivery_stage.py
+-rw-r--r--   0        0        0    13969 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/create_release.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery.py
+-rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_filters.py
+-rw-r--r--   0        0        0    12760 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_flow_release_info.py
+-rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_order_mode.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_pattern_filters.py
+-rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_status.py
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_timeline.py
+-rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/dependency.py
+-rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/duplicate_delivery_pattern.py
+-rw-r--r--   0        0        0    12119 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_filters.py
+-rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_form.py
+-rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_label_filters.py
+-rw-r--r--   0        0        0    11927 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_label_form.py
+-rw-r--r--   0        0        0    12099 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_label_view.py
+-rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_reservation_form.py
+-rw-r--r--   0        0        0    13456 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_reservation_search_view.py
+-rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_reservation_view.py
+-rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_stage_filters.py
+-rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_stage_form.py
+-rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_stage_view.py
+-rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_view.py
+-rw-r--r--   0        0        0    12367 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/external_variable_value.py
+-rw-r--r--   0        0        0    13804 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/facet.py
+-rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/facet_filters.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/facet_scope.py
+-rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/flag_status.py
+-rw-r--r--   0        0        0    13364 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/folder.py
+-rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/folder_variables.py
+-rw-r--r--   0        0        0    12273 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/gate_condition.py
+-rw-r--r--   0        0        0    37643 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/gate_task.py
+-rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/global_variables.py
+-rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/import_result.py
+-rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/member_type.py
+-rw-r--r--   0        0        0    12427 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/model_property.py
+-rw-r--r--   0        0        0    22798 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/phase.py
+-rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/phase_status.py
+-rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/phase_timeline.py
+-rw-r--r--   0        0        0    12324 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/phase_version.py
+-rw-r--r--   0        0        0    18794 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/plan_item.py
+-rw-r--r--   0        0        0    12233 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/poll_type.py
+-rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/principal_view.py
+-rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/projected_phase.py
+-rw-r--r--   0        0        0    13620 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/projected_release.py
+-rw-r--r--   0        0        0    13187 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/projected_task.py
+-rw-r--r--   0        0        0    37799 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release.py
+-rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_configuration.py
+-rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_count_result.py
+-rw-r--r--   0        0        0    12456 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_count_results.py
+-rw-r--r--   0        0        0    12335 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_extension.py
+-rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_full_search_result.py
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group.py
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group_filters.py
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group_order_mode.py
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group_status.py
+-rw-r--r--   0        0        0    13006 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group_timeline.py
+-rw-r--r--   0        0        0    12254 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_order_direction.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_order_mode.py
+-rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_search_result.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_status.py
+-rw-r--r--   0        0        0    14321 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_timeline.py
+-rw-r--r--   0        0        0    20032 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_trigger.py
+-rw-r--r--   0        0        0    17803 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/releases_filters.py
+-rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/reservation_filters.py
+-rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/reservation_search_view.py
+-rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk.py
+-rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_assessment.py
+-rw-r--r--   0        0        0    13222 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_assessor.py
+-rw-r--r--   0        0        0    12785 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_global_thresholds.py
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_profile.py
+-rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_status.py
+-rw-r--r--   0        0        0    12464 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_status_with_thresholds.py
+-rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/role_view.py
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/shared_configuration_status_response.py
+-rw-r--r--   0        0        0    13902 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/stage.py
+-rw-r--r--   0        0        0    12242 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/stage_status.py
+-rw-r--r--   0        0        0    12479 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/stage_tracked_item.py
+-rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/start_release.py
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/start_task.py
+-rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/subscriber.py
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/system_message_settings.py
+-rw-r--r--   0        0        0    35913 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task.py
+-rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task_container.py
+-rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task_recover_op.py
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task_reporting_record.py
+-rw-r--r--   0        0        0    14337 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task_status.py
+-rw-r--r--   0        0        0    13910 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/team.py
+-rw-r--r--   0        0        0    12499 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/team_member_view.py
+-rw-r--r--   0        0        0    12767 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/team_view.py
+-rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/time_frame.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/tracked_item.py
+-rw-r--r--   0        0        0    12363 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/tracked_item_status.py
+-rw-r--r--   0        0        0    13727 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/transition.py
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/trigger.py
+-rw-r--r--   0        0        0    12299 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/trigger_execution_status.py
+-rw-r--r--   0        0        0    11957 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/usage_point.py
+-rw-r--r--   0        0        0    14832 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/user_account.py
+-rw-r--r--   0        0        0    36232 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/user_input_task.py
+-rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/validate_pattern.py
+-rw-r--r--   0        0        0    12310 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/value_provider_configuration.py
+-rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/value_with_interpolation.py
+-rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/variable.py
+-rw-r--r--   0        0        0    15028 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/variable1.py
+-rw-r--r--   0        0        0    12098 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/variable_or_value.py
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/models/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/tests/release/api/test_release_api_methods.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/tests/release/integration/expected_output.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/tests/release/integration/hello.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/tests/release/integration/input.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/tests/release/integration/output.json
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/tests/release/integration/test_wrapper.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/README.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 digitalai_release_sdk-23.1.0rc1/PKG-INFO
```

### Comparing `digitalai_release_sdk-23.1.0/.github/workflows/python-test.yml` & `digitalai_release_sdk-23.1.0rc1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/integration/base_task.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/base_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         return self.release_context.automated_task_as_user
 
     def get_default_api_client(self) -> ApiClient:
         """
         Returns an ApiClient object with default configuration based on the task.
         """
         if not all([self.get_release_server_url(), self.get_task_user().username, self.get_task_user().password]):
-            raise ValueError("Cannot connect to Release API without server URL, username, or password. "
+            raise ValueError("Cannot create reach Release API without server URL, username, or password. "
                              "Make sure that the 'Run as user' property is set on the release.")
 
         configuration = Configuration(
             host=self.get_release_server_url(),
             username=self.get_task_user().username,
             password=self.get_task_user().password)
```

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/integration/input_context.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/input_context.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/integration/job_data_encryptor.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/job_data_encryptor.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/integration/logging_config.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/logging_config.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/integration/masked_io.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/masked_io.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/integration/output_context.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/output_context.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/integration/reporting_records.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/reporting_records.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/integration/wrapper.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/integration/wrapper.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/README.md` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/README.md`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/__init__.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api_client.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api_client.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/configuration.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/exceptions.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/exceptions.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model_utils.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model_utils.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/rest.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/rest.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/activity_logs_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/activity_logs_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/application_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/application_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/configuration_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/configuration_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/delivery_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/delivery_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/delivery_pattern_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/delivery_pattern_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/dsl_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/dsl_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/environment_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/environment_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/environment_label_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/environment_label_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/environment_reservation_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/environment_reservation_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/environment_stage_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/environment_stage_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/facet_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/facet_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/folder_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/folder_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/permissions_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/phase_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/phase_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/planner_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/planner_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/release_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/release_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/release_group_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/release_group_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/report_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/report_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/risk_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/risk_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/risk_assessment_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/risk_assessment_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/roles_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/task_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/task_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/template_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/template_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/triggers_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/triggers_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/api/user_api.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/api/user_api.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/apis/__init__.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/abort_release.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/abort_release.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/activity_log_entry.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/activity_log_entry.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/application_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/application_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/application_form.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/application_form.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/application_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/application_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/attachment.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/attachment.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/base_application_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/base_application_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/base_environment_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/base_environment_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/blackout_metadata.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/blackout_metadata.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/blackout_period.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/blackout_period.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/bulk_action_result_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/bulk_action_result_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/change_password_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/change_password_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/ci_property.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/ci_property.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/comment.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/comment.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/comment1.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/comment1.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/complete_transition.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/complete_transition.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/condition.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/condition.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/condition1.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/condition1.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/configuration_facet.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/configuration_facet.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/configuration_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/configuration_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/copy_template.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/copy_template.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/create_delivery.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/create_delivery.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/create_delivery_stage.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/create_delivery_stage.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/create_release.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/create_release.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_flow_release_info.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_flow_release_info.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_order_mode.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_order_mode.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_pattern_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_pattern_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/delivery_timeline.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/delivery_timeline.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/dependency.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/dependency.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/duplicate_delivery_pattern.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/duplicate_delivery_pattern.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_form.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_form.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_label_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_label_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_label_form.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_label_form.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_label_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_label_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_reservation_form.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_reservation_form.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_reservation_search_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_reservation_search_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_reservation_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_reservation_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_stage_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_stage_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_stage_form.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_stage_form.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_stage_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_stage_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/environment_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/environment_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/external_variable_value.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/external_variable_value.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/facet.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/facet.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/facet_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/facet_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/facet_scope.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/facet_scope.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/flag_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/flag_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/folder.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/folder.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/folder_variables.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/folder_variables.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/gate_condition.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/gate_condition.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/gate_task.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/gate_task.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/global_variables.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/global_variables.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/import_result.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/import_result.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/member_type.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/member_type.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/model_property.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/model_property.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/phase.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/phase.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/phase_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/phase_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/phase_timeline.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/phase_timeline.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/phase_version.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/phase_version.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/plan_item.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/plan_item.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/poll_type.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/poll_type.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/principal_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/principal_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/projected_phase.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/projected_phase.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/projected_release.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/projected_release.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/projected_task.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/projected_task.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_configuration.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_configuration.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_count_result.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_count_result.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_count_results.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_count_results.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_extension.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_extension.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_full_search_result.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_full_search_result.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group_order_mode.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group_order_mode.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_group_timeline.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_group_timeline.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_order_direction.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_order_direction.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_order_mode.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_order_mode.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_search_result.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_search_result.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_timeline.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_timeline.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/release_trigger.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/release_trigger.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/releases_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/releases_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/reservation_filters.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/reservation_filters.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/reservation_search_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/reservation_search_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_assessment.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_assessment.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_assessor.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_assessor.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_global_thresholds.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_global_thresholds.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_profile.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_profile.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/risk_status_with_thresholds.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/risk_status_with_thresholds.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/role_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/role_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/shared_configuration_status_response.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/shared_configuration_status_response.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/stage.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/stage.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/stage_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/stage_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/stage_tracked_item.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/stage_tracked_item.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/start_release.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/start_release.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/start_task.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/start_task.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/subscriber.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/subscriber.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/system_message_settings.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/system_message_settings.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task_container.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task_container.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task_recover_op.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task_recover_op.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task_reporting_record.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task_reporting_record.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/task_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/task_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/team.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/team.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/team_member_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/team_member_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/team_view.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/team_view.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/time_frame.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/time_frame.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/tracked_item.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/tracked_item.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/tracked_item_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/tracked_item_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/transition.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/transition.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/trigger.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/trigger.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/trigger_execution_status.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/trigger_execution_status.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/usage_point.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/usage_point.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/user_account.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/user_account.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/user_input_task.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/user_input_task.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/validate_pattern.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/validate_pattern.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/value_provider_configuration.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/value_provider_configuration.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/value_with_interpolation.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/value_with_interpolation.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/variable.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/variable.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/variable1.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/variable1.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/model/variable_or_value.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/model/variable_or_value.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/digitalai/release/v1/models/__init__.py` & `digitalai_release_sdk-23.1.0rc1/digitalai/release/v1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/tests/release/api/test_release_api_methods.py` & `digitalai_release_sdk-23.1.0rc1/tests/release/api/test_release_api_methods.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/tests/release/integration/hello.py` & `digitalai_release_sdk-23.1.0rc1/tests/release/integration/hello.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/tests/release/integration/input.json` & `digitalai_release_sdk-23.1.0rc1/tests/release/integration/input.json`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/tests/release/integration/test_wrapper.py` & `digitalai_release_sdk-23.1.0rc1/tests/release/integration/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/LICENSE` & `digitalai_release_sdk-23.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/README.md` & `digitalai_release_sdk-23.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `digitalai_release_sdk-23.1.0/pyproject.toml` & `digitalai_release_sdk-23.1.0rc1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 exclude = [
   "digitalai/release/v1/docs/*"
 ]
 
 [project]
 name = "digitalai_release_sdk"
-version = "23.1.0"
+version = "23.1.0-rc.1"
 authors = [
   { name="Digital.ai", email="pypi-devops@digital.ai" },
 ]
 description = "Digital.ai Release SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `digitalai_release_sdk-23.1.0/PKG-INFO` & `digitalai_release_sdk-23.1.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalai_release_sdk
-Version: 23.1.0
+Version: 23.1.0rc1
 Summary: Digital.ai Release SDK
 Project-URL: Homepage, https://digital.ai/
 Author-email: "Digital.ai" <pypi-devops@digital.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

