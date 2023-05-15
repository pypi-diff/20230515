# Comparing `tmp/alice-onboarding-1.9.0.tar.gz` & `tmp/alice-onboarding-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alice-onboarding-1.9.0.tar", last modified: Wed Nov 23 11:00:48 2022, max compression
+gzip compressed data, was "alice-onboarding-2.0.0.tar", last modified: Mon May 15 10:44:29 2023, max compression
```

## Comparing `alice-onboarding-1.9.0.tar` & `alice-onboarding-2.0.0.tar`

### file list

```diff
@@ -1,105 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3697 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.613460 alice-onboarding-1.9.0/alice/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-23 11:00:42.000000 alice-onboarding-1.9.0/alice/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      213 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.613460 alice-onboarding-1.9.0/alice/auth/
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/auth/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      740 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/auth/auth_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.613460 alice-onboarding-1.9.0/alice/onboarding/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.613460 alice-onboarding-1.9.0/alice/onboarding/enums/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/enums/certificate_locale.py
--rw-r--r--   0 runner    (1001) docker     (122)      114 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/enums/decision.py
--rw-r--r--   0 runner    (1001) docker     (122)      114 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/enums/document_side.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/enums/document_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/enums/document_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/enums/duplicates_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (122)       95 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/enums/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.613460 alice-onboarding-1.9.0/alice/onboarding/models/
--rw-r--r--   0 runner    (1001) docker     (122)      464 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (122)      222 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/device_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.613460 alice-onboarding-1.9.0/alice/onboarding/models/report/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.613460 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/
--rw-r--r--   0 runner    (1001) docker     (122)      473 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.613460 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/
--rw-r--r--   0 runner    (1001) docker     (122)      397 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/authentic_nfc_chip_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      343 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/checked_info_code_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/coherent_document_dates_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      445 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/consistent_document_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      338 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/expected_document_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/face_in_document_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/face_matching_document_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      340 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/not_a_printed_document_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      362 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/not_a_screen_document_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      368 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/not_a_synthetic_document_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      396 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/uncompromised_document_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      310 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/document/unexpired_document_check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/
--rw-r--r--   0 runner    (1001) docker     (122)      301 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/cheked_field_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      337 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/complete_mrz_name_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/consistent_field_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      333 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/expected_field_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/over_18_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/unexpired_date_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/valid_date_format_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/field/valid_date_range_check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/selfie/
--rw-r--r--   0 runner    (1001) docker     (122)      320 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/selfie/liveness_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      332 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/selfie/only_one_face_check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/summary/
--rw-r--r--   0 runner    (1001) docker     (122)      372 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/summary/only_one_device_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/checks/summary/only_one_ip_check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/compliance/
--rw-r--r--   0 runner    (1001) docker     (122)      474 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/compliance/device_out.py
--rw-r--r--   0 runner    (1001) docker     (122)      376 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/compliance/domain_events_report.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/compliance/user_event_out.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/document/
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     3071 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_report.py
--rw-r--r--   0 runner    (1001) docker     (122)      534 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_report_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)      114 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_side.py
--rw-r--r--   0 runner    (1001) docker     (122)     1672 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_side_report.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_side_report_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/face_matching/
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/face_matching/face_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/other_trusted_document/
--rw-r--r--   0 runner    (1001) docker     (122)      861 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py
--rw-r--r--   0 runner    (1001) docker     (122)      403 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/selfie/
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/selfie/selfie_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/shared/
--rw-r--r--   0 runner    (1001) docker     (122)      464 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/shared/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (122)      515 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/shared/href.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/onboarding/models/report/summary/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/summary/external_user_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1349 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/report/summary/report_summary.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/models/user_info.py
--rw-r--r--   0 runner    (1001) docker     (122)    53268 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (122)    51329 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/onboarding_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/onboarding_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/onboarding/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/sandbox/
--rw-r--r--   0 runner    (1001) docker     (122)     6251 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/sandbox/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4612 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/sandbox/sandbox_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      933 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/sandbox/sandbox_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice/webhooks/
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/webhooks/webhook.py
--rw-r--r--   0 runner    (1001) docker     (122)    11796 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/webhooks/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (122)    11234 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/alice/webhooks/webhooks_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 11:00:48.617460 alice-onboarding-1.9.0/alice_onboarding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2022-11-23 11:00:48.000000 alice-onboarding-1.9.0/alice_onboarding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4086 2022-11-23 11:00:48.000000 alice-onboarding-1.9.0/alice_onboarding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-23 11:00:48.000000 alice-onboarding-1.9.0/alice_onboarding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-23 11:00:48.000000 alice-onboarding-1.9.0/alice_onboarding.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       88 2022-11-23 11:00:48.000000 alice-onboarding-1.9.0/alice_onboarding.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      657 2022-11-23 11:00:48.000000 alice-onboarding-1.9.0/alice_onboarding.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      449 2022-11-23 11:00:48.621460 alice-onboarding-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2022-11-23 11:00:41.000000 alice-onboarding-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.083726 alice-onboarding-2.0.0/alice/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.083726 alice-onboarding-2.0.0/alice/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/auth/auth_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/auth/cached_token_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/auth/token_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.083726 alice-onboarding-2.0.0/alice/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.083726 alice-onboarding-2.0.0/alice/onboarding/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/certificate_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/document_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/document_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/document_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/duplicates_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/match_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/enums/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.083726 alice-onboarding-2.0.0/alice/onboarding/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/device_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.083726 alice-onboarding-2.0.0/alice/onboarding/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.083726 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.087726 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/authentic_nfc_chip_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/checked_info_code_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/coherent_document_dates_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/consistent_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/expected_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/face_in_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/face_matching_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/not_a_printed_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/not_a_screen_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/not_a_synthetic_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/uncompromised_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/document/unexpired_document_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.087726 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/cheked_field_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/complete_mrz_name_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/consistent_field_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/expected_field_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/over_18_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/unexpired_date_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/valid_date_format_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/field/valid_date_range_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.087726 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/selfie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/selfie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/selfie/liveness_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/selfie/only_one_face_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.087726 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/summary/only_one_device_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/checks/summary/only_one_ip_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.087726 alice-onboarding-2.0.0/alice/onboarding/models/report/compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/compliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/compliance/device_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/compliance/domain_events_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/compliance/user_event_out.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.087726 alice-onboarding-2.0.0/alice/onboarding/models/report/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_report_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_side_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_side_report_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.087726 alice-onboarding-2.0.0/alice/onboarding/models/report/face_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/face_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/face_matching/face_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.087726 alice-onboarding-2.0.0/alice/onboarding/models/report/other_trusted_document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/other_trusted_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/alice/onboarding/models/report/selfie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/selfie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/selfie/selfie_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/alice/onboarding/models/report/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/shared/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/shared/href.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/alice/onboarding/models/report/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/summary/external_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/report/summary/report_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/models/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57159 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64391 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/onboarding_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/onboarding_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/onboarding/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/public_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/alice/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/sandbox/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/sandbox/sandbox_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/sandbox/sandbox_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/alice/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/webhooks/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/webhooks/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/alice/webhooks/webhooks_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/alice_onboarding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-15 10:44:29.000000 alice-onboarding-2.0.0/alice_onboarding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-15 10:44:29.000000 alice-onboarding-2.0.0/alice_onboarding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:44:29.000000 alice-onboarding-2.0.0/alice_onboarding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:44:29.000000 alice-onboarding-2.0.0/alice_onboarding.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-15 10:44:29.000000 alice-onboarding-2.0.0/alice_onboarding.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 10:44:29.000000 alice-onboarding-2.0.0/alice_onboarding.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 10:44:29.091727 alice-onboarding-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 10:44:23.000000 alice-onboarding-2.0.0/setup.py
```

### Comparing `alice-onboarding-1.9.0/PKG-INFO` & `alice-onboarding-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: alice-onboarding
-Version: 1.9.0
+Version: 2.0.0
 Summary: Alice Onboarding Python SDK
 Home-page: https://github.com/alice-biometrics/onboarding-python
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: Alice Copyright
 Keywords: onboarding,biometrics,kyc,alice
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # onboarding-python <img src="https://github.com/alice-biometrics/custom-emojis/blob/master/images/python.png?raw=true" width="30"> 
 
 [![version](https://img.shields.io/github/release/alice-biometrics/onboarding-python/all.svg)](https://github.com/alice-biometrics/onboarding-python/releases) [![doc](https://img.shields.io/badge/doc-onboarding-51CB56)](https://docs.alicebiometrics.com/onboarding/sections/server/server_side_sdks/python.html)
```

### Comparing `alice-onboarding-1.9.0/README.md` & `alice-onboarding-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/auth/auth.py` & `alice-onboarding-2.0.0/alice/auth/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import json
 from typing import Optional, Union
 
 import requests
 from meiga import Failure, Result, Success
-from requests import Response, Session
+from requests import Session
 
 from alice.config import Config
 
 from .auth_client import AuthClient
 from .auth_errors import AuthError
+from .token_tools import get_token_from_response
 
 DEFAULT_URL = "https://apis.alicebiometrics.com/onboarding"
 
 
 class Auth:
     @staticmethod
     def from_config(config: Config) -> "Auth":
@@ -20,91 +20,89 @@
             session = config.session
         else:
             session = requests.Session()
         return Auth(
             api_key=config.api_key,  # type: ignore
             session=session,
             url=config.onboarding_url,
+            timeout=config.timeout,
             verbose=config.verbose,
         )
 
     def __init__(
         self,
         api_key: str,
         session: Session,
         url: str = DEFAULT_URL,
+        timeout: Union[float, None] = None,
         verbose: Optional[bool] = False,
     ):
-        self._auth_client = AuthClient(url=url, api_key=api_key, session=session)
+        self._auth_client = AuthClient(
+            url=url, api_key=api_key, session=session, timeout=timeout
+        )
         self.url = url
         self.verbose = verbose
 
-    def create_backend_token(
-        self, user_id: Union[str, None] = None, verbose: Optional[bool] = False
+    def create_user_token(
+        self, user_id: str, verbose: Optional[bool] = False
     ) -> Result[str, AuthError]:
         """
-        Returns a BACKEND_TOKEN or BACKEND_TOKEN_WITH_USER depending of user_id given parameter.
-        Both BACKEND_TOKEN and BACKEND_TOKEN_WITH_USER are used to secure global requests.
+        Returns a USER_TOKEN.
+        The USER_TOKEN is used to secure requests made by the users on their mobile devices or web clients.
+
 
         Parameters
         ----------
         user_id
             User identifier
         verbose
             Used for print service response as well as the time elapsed
 
+
         Returns
         -------
-            A Result where if the operation is successful it returns BACKEND_TOKEN or BACKEND_TOKEN_WITH_USER.
+            A Result where if the operation is successful it returns USER_TOKEN.
             Otherwise, it returns an OnboardingError.
         """
         verbose = self.verbose or verbose
-        response = self._auth_client.create_backend_token(user_id, verbose=verbose)
+        response = self._auth_client.create_user_token(user_id, verbose=verbose)
 
         if response.status_code == 200:
-            return Success(self.__get_token_from_response(response))
+            return Success(get_token_from_response(response))
         else:
-            suffix = " (with user)" if user_id else ""
             return Failure(
                 AuthError.from_response(
-                    operation=f"create_backend_token{suffix}", response=response
+                    operation="create_user_token", response=response
                 )
             )
 
-    def create_user_token(
-        self, user_id: str, verbose: Optional[bool] = False
+    def create_backend_token(
+        self, user_id: Union[str, None] = None, verbose: Optional[bool] = False
     ) -> Result[str, AuthError]:
         """
-        Returns a USER_TOKEN.
-        The USER_TOKEN is used to secure requests made by the users on their mobile devices or web clients.
-
+        Returns a BACKEND_TOKEN or BACKEND_TOKEN_WITH_USER depending of user_id given parameter.
+        Both BACKEND_TOKEN and BACKEND_TOKEN_WITH_USER are used to secure global requests.
 
         Parameters
         ----------
         user_id
             User identifier
         verbose
             Used for print service response as well as the time elapsed
 
-
         Returns
         -------
-            A Result where if the operation is successful it returns USER_TOKEN.
+            A Result where if the operation is successful it returns BACKEND_TOKEN or BACKEND_TOKEN_WITH_USER.
             Otherwise, it returns an OnboardingError.
         """
         verbose = self.verbose or verbose
-        response = self._auth_client.create_user_token(user_id, verbose=verbose)
+        response = self._auth_client.create_backend_token(user_id, verbose=verbose)
 
         if response.status_code == 200:
-            return Success(self.__get_token_from_response(response))
+            return Success(get_token_from_response(response))
         else:
+            suffix = " (with user)" if user_id else ""
             return Failure(
                 AuthError.from_response(
-                    operation="create_user_token", response=response
+                    operation=f"create_backend_token{suffix}", response=response
                 )
             )
-
-    @staticmethod
-    def __get_token_from_response(response: Response) -> str:
-        response_json = json.loads(response.content)
-        token: str = response_json["token"]
-        return token
```

### Comparing `alice-onboarding-1.9.0/alice/auth/auth_errors.py` & `alice-onboarding-2.0.0/alice/auth/auth_errors.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/compliance/user_event_out.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/compliance/user_event_out.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_field.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_field.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_report.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_report.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_report_meta.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_report_meta.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/document/document_side_report.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/document/document_side_report.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/face_matching/face_matching.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/face_matching/face_matching.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/report.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/report.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/selfie/selfie_report.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/selfie/selfie_report.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/shared/href.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/shared/href.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/models/report/summary/report_summary.py` & `alice-onboarding-2.0.0/alice/onboarding/models/report/summary/report_summary.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/onboarding/onboarding.py` & `alice-onboarding-2.0.0/alice/onboarding/onboarding.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from alice.config import Config
 from alice.onboarding.enums.certificate_locale import CertificateLocale
 from alice.onboarding.enums.decision import Decision
 from alice.onboarding.enums.document_side import DocumentSide
 from alice.onboarding.enums.document_source import DocumentSource
 from alice.onboarding.enums.document_type import DocumentType
 from alice.onboarding.enums.duplicates_resource_type import DuplicatesResourceType
+from alice.onboarding.enums.match_case import MatchCase
 from alice.onboarding.enums.version import Version
 from alice.onboarding.models.bounding_box import BoundingBox
 from alice.onboarding.models.device_info import DeviceInfo
 from alice.onboarding.models.report.report import Report
 from alice.onboarding.models.user_info import UserInfo
 from alice.onboarding.onboarding_client import OnboardingClient
 from alice.onboarding.onboarding_errors import OnboardingError
@@ -30,29 +31,31 @@
         if config.session:
             session = config.session
         else:
             session = Session()
         return Onboarding(
             auth=Auth.from_config(config),
             url=config.onboarding_url,
+            timeout=config.timeout,
             send_agent=config.send_agent,
             verbose=config.verbose,
             session=session,
         )
 
     def __init__(
         self,
         auth: Auth,
         session: Session,
         url: str = DEFAULT_URL,
+        timeout: Union[float, None] = None,
         send_agent: bool = True,
         verbose: bool = False,
     ):
         self.onboarding_client = OnboardingClient(
-            auth=auth, url=url, send_agent=send_agent, session=session
+            auth=auth, url=url, timeout=timeout, send_agent=send_agent, session=session
         )
         self.url = url
         self.verbose = verbose
 
     @early_return
     def healthcheck(
         self, verbose: Optional[bool] = False
@@ -149,15 +152,15 @@
             Otherwise, it returns an OnboardingError or AuthError.
         """
         verbose = self.verbose or verbose
         response = self.onboarding_client.delete_user(
             user_id=user_id, verbose=verbose
         ).unwrap_or_return()
 
-        if response.status_code == 200:
+        if response.status_code in [200, 202]:
             return isSuccess
         else:
             return Failure(
                 OnboardingError.from_response(
                     operation="delete_user", response=response
                 )
             )
@@ -409,37 +412,42 @@
         else:
             return Failure(
                 OnboardingError.from_response(operation="add_selfie", response=response)
             )
 
     @early_return
     def delete_selfie(
-        self, user_id: str, verbose: Optional[bool] = False
+        self,
+        user_id: str,
+        selfie_id: Optional[str] = None,
+        verbose: Optional[bool] = False,
     ) -> Result[bool, Union[OnboardingError, AuthError]]:
         """
 
         This call is used to delete the video of the user's face to the onboarding service.
         This will also erase the biometric face profile.
 
         Parameters
         ----------
         user_id
             User identifier
+        selfie_id
+            Optional selfie identifier
         verbose
             Used for print service response as well as the time elapsed
 
 
         Returns
         -------
             A Result where if the operation is successful it returns True.
             Otherwise, it returns an OnboardingError or AuthError.
         """
         verbose = self.verbose or verbose
         response = self.onboarding_client.delete_selfie(
-            user_id=user_id, verbose=verbose
+            user_id=user_id, selfie_id=selfie_id, verbose=verbose
         ).unwrap_or_return()
 
         if response.status_code == 200:
             return isSuccess
         else:
             return Failure(
                 OnboardingError.from_response(
@@ -1219,50 +1227,89 @@
             return Failure(
                 OnboardingError.from_response(
                     operation="identify_user", response=response
                 )
             )
 
     @early_return
-    def authorize_user(
+    def user_matching(
+        self,
+        user_id: str,
+        match_case: MatchCase,
+        verbose: bool = False,
+    ) -> Result[bool, Union[OnboardingError, AuthError]]:
+        """
+        It performs face matching between all the user selfies or documents. This call requires a BACKEND_TOKEN_WITH_USER_ID..
+
+        Parameters
+        ----------
+        user_id
+            User identifier
+        match_case
+            Evidence (selfies or docs) on which to perform the matching
+        verbose
+            Used for print service response as well as the time elapsed
+        Returns
+        -------
+            A Result where if the operation is successful it returns a list of face matchings.
+            Otherwise, it returns an OnboardingError or AuthError.
+        """
+        verbose = self.verbose or verbose
+        response = self.onboarding_client.user_matching(
+            user_id=user_id,
+            match_case=match_case,
+            verbose=verbose,
+        ).unwrap_or_return()
+
+        if response.status_code == 200:
+            return Success(response.json())
+        else:
+            return Failure(
+                OnboardingError.from_response(
+                    operation="user_matching", response=response
+                )
+            )
+
+    def enable_authentication(
         self, user_id: str, verbose: bool = False
     ) -> Result[bool, Union[OnboardingError, AuthError]]:
         """
-        Authorizes a user. Now it can be icated.
+        It enables the authentication for a user.
+
         Parameters
         ----------
         user_id
             User identifier
         verbose
             Used for print service response as well as the time elapsed
         Returns
         -------
             A Result where if the operation is successful it returns True.
             Otherwise, it returns an OnboardingError or AuthError.
         """
         verbose = self.verbose or verbose
-        response = self.onboarding_client.authorize_user(
+        response = self.onboarding_client.enable_authentication(
             user_id=user_id, verbose=verbose
         ).unwrap_or_return()
 
         if response.status_code == 200:
             return isSuccess
         else:
             return Failure(
                 OnboardingError.from_response(
-                    operation="authorize_user", response=response
+                    operation="enable_authentication", response=response
                 )
             )
 
     @early_return
-    def deauthorize_user(
+    def disable_authentication(
         self, user_id: str, verbose: bool = False
     ) -> Result[bool, Union[OnboardingError, AuthError]]:
         """
-        Deauthorizes a user. Now it cannot be authenticated.
+        It disables the authentication for a user.
 
         Parameters
         ----------
         user_id
             User identifier
         verbose
             Used for print service response as well as the time elapsed
@@ -1270,24 +1317,24 @@
 
         Returns
         -------
             A Result where if the operation is successful it returns True.
             Otherwise, it returns an OnboardingError or AuthError.
         """
         verbose = self.verbose or verbose
-        response = self.onboarding_client.deauthorize_user(
+        response = self.onboarding_client.disable_authentication(
             user_id=user_id, verbose=verbose
         ).unwrap_or_return()
 
         if response.status_code == 200:
             return isSuccess
         else:
             return Failure(
                 OnboardingError.from_response(
-                    operation="deauthorize_user", response=response
+                    operation="disable_authentication", response=response
                 )
             )
 
     @early_return
     def authenticate_user(
         self, user_id: str, media_data: bytes, verbose: bool = False
     ) -> Result[str, Union[OnboardingError, AuthError]]:
@@ -1642,7 +1689,80 @@
             return Success(response.json()["searches"])
         else:
             return Failure(
                 OnboardingError.from_response(
                     operation="get_duplicates_searches", response=response
                 )
             )
+
+    def accept_user(
+        self, user_id: str, operator: str = "auto", verbose: bool = False
+    ) -> Result[bool, OnboardingError]:
+        """
+        Mark a user state as ACCEPTED
+        Parameters
+        ----------
+        user_id
+            User identifier
+        operator
+            Who is accepting the user
+        verbose
+            Used for print service response as well as the time elapsed
+        Returns
+        -------
+            A Result where if the operation is successful it returns True.
+            Otherwise, it returns an OnboardingError.
+        """
+        verbose = self.verbose or verbose
+        response = self.onboarding_client.accept_user(
+            user_id=user_id, operator=operator, verbose=verbose
+        ).unwrap_or_return()
+
+        if response.status_code == 200:
+            return isSuccess
+        else:
+            return Failure(
+                OnboardingError.from_response(
+                    operation="accept_user", response=response
+                )
+            )
+
+    def reject_user(
+        self,
+        user_id: str,
+        rejection_reasons: Optional[List[Dict[str, str]]] = None,
+        operator: str = "auto",
+        verbose: bool = False,
+    ) -> Result[bool, OnboardingError]:
+        """
+        Mark a user state as REJECTED
+        Parameters
+        ----------
+        user_id
+            User identifier
+        rejection_reasons
+            List of rejection reasons
+        operator
+            Who is rejecting the user
+        verbose
+            Used for print service response as well as the time elapsed
+        Returns
+        -------
+            A Result where if the operation is successful it returns True.
+            Otherwise, it returns an OnboardingError.
+        """
+        verbose = self.verbose or verbose
+        response = self.onboarding_client.reject_user(
+            user_id=user_id,
+            rejection_reasons=rejection_reasons,
+            operator=operator,
+            verbose=verbose,
+        ).unwrap_or_return()
+
+        if response.status_code == 200:
+            return isSuccess
+        else:
+            return Failure(
+                OnboardingError.from_response(
+                    operation="accept_user", response=response
+                )
+            )
```

### Comparing `alice-onboarding-1.9.0/alice/onboarding/onboarding_client.py` & `alice-onboarding-2.0.0/alice/onboarding/onboarding_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import json
 import platform
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 
 import requests
-from meiga import Error, Result, Success, early_return
+from meiga import Error, Failure, Result, Success, early_return
 from requests import Response, Session
 
 import alice
 from alice.auth.auth import Auth
-from alice.auth.auth_errors import AuthError
 from alice.onboarding.enums.certificate_locale import CertificateLocale
 from alice.onboarding.enums.decision import Decision
 from alice.onboarding.enums.document_side import DocumentSide
 from alice.onboarding.enums.document_source import DocumentSource
 from alice.onboarding.enums.document_type import DocumentType
 from alice.onboarding.enums.duplicates_resource_type import DuplicatesResourceType
+from alice.onboarding.enums.match_case import MatchCase
 from alice.onboarding.enums.version import Version
 from alice.onboarding.models.bounding_box import BoundingBox
 from alice.onboarding.models.device_info import DeviceInfo
 from alice.onboarding.models.user_info import UserInfo
+from alice.onboarding.onboarding_errors import OnboardingError
 from alice.onboarding.tools import print_intro, print_response, print_token, timeit
 
 DEFAULT_URL = "https://apis.alicebiometrics.com/onboarding"
 
 
 class OnboardingClient:
     def __init__(
         self,
         auth: Auth,
         session: Session,
         url: str = DEFAULT_URL,
+        timeout: Union[float, None] = None,
         send_agent: bool = True,
     ):
         self.auth = auth
         self.url = url
+        self.timeout = timeout
         self.send_agent = send_agent
         self.session = session
 
     def _auth_headers(self, token: str) -> Dict[str, Any]:
         auth_headers = {"Authorization": f"Bearer {token}"}
         if self.send_agent:
             auth_headers.update(
@@ -62,28 +65,30 @@
 
         Returns
         -------
             A Result object with Response object [requests library] if Success
         """
         print_intro("healthcheck", verbose=verbose)
 
-        response = self.session.get(f"{self.url}/healthcheck")
-
+        try:
+            response = self.session.get(f"{self.url}/healthcheck", timeout=self.timeout)
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="healthcheck"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def create_user(
         self,
         user_info: Union[UserInfo, None] = None,
         device_info: Union[DeviceInfo, None] = None,
         verbose: Optional[bool] = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         It creates a new User in the onboarding service.
         You must create a User before you start the onboarding flow.
 
 
         Parameters
@@ -111,26 +116,29 @@
         data = None
         if user_info:
             data = data if data is not None else {}
             data.update(user_info.dict())
         if device_info:
             data = data if data is not None else {}
             data.update(device_info.dict())
-
-        response = self.session.post(f"{self.url}/user", headers=headers, data=data)
-
+        try:
+            response = self.session.post(
+                f"{self.url}/user", headers=headers, data=data, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="create_user"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def delete_user(
         self, user_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Delete all the information of a user
 
         Parameters
         ----------
         user_id
@@ -145,25 +153,30 @@
         """
         print_intro("delete_user", verbose=verbose)
 
         backend_token = self.auth.create_backend_token(user_id).unwrap_or_return()
         print_token("backend_token_with_user", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
-        response = self.session.delete(f"{self.url}/user", headers=headers)
 
+        try:
+            response = self.session.delete(
+                f"{self.url}/user", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="delete_user"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def get_user_status(
         self, user_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns User status to be used as feedback from the onboarding process
 
         Parameters
         ----------
         user_id
@@ -179,25 +192,29 @@
         print_intro("get_user_status", verbose=verbose)
 
         user_token = self.auth.create_user_token(user_id).unwrap_or_return()
         print_token("user_token", user_token, verbose=verbose)
 
         headers = self._auth_headers(user_token)
 
-        response = self.session.get(f"{self.url}/user/status", headers=headers)
-
+        try:
+            response = self.session.get(
+                f"{self.url}/user/status", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_user_status"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def get_users_stats(
         self, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns statistics about users in the Onboarding platform.
 
         Parameters
         ----------
         verbose
@@ -210,23 +227,27 @@
         """
         print_intro("get_users_stats", verbose=verbose)
 
         backend_token = self.auth.create_backend_token().unwrap_or_return()
         print_token("backend_token", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
-        response = self.session.get(f"{self.url}/users/stats", headers=headers)
-
+        try:
+            response = self.session.get(
+                f"{self.url}/users/stats", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_users_stats"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
-    def get_users(self, verbose: Optional[bool] = False) -> Result[Response, AuthError]:
+    def get_users(self, verbose: Optional[bool] = False) -> Result[Response, Error]:
         """
 
         Returns all users you have created, sorted by creation date in descending order.
 
         Parameters
         ----------
         verbose
@@ -239,15 +260,20 @@
         """
         print_intro("get_users", verbose=verbose)
 
         backend_token = self.auth.create_backend_token().unwrap_or_return()
         print_token("backend_token", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
-        response = self.session.get(f"{self.url}/users", headers=headers)
+        try:
+            response = self.session.get(
+                f"{self.url}/users", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_users"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
@@ -257,15 +283,15 @@
         page: int = 1,
         page_size: int = 0,
         descending: bool = True,
         authorized: bool = False,
         sort_by: Union[str, None] = None,
         filter_field: Union[str, None] = None,
         filter_value: Union[str, None] = None,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns every UserStatus available for all the Users in the onboarding platform ordered by creation date.
 
         Parameters
         ----------
         verbose
@@ -301,33 +327,37 @@
             url_query_params = (
                 url_query_params
                 + f"&filter_field={filter_field}&filter_value={filter_value}"
             )
         if sort_by:
             url_query_params = url_query_params + f"&sort_by={sort_by}"
 
-        response = self.session.get(
-            f"{self.url}/users/status{url_query_params}", headers=headers
-        )
-
+        try:
+            response = self.session.get(
+                f"{self.url}/users/status{url_query_params}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_users_status"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def add_user_feedback(
         self,
         user_id: str,
         document_id: str,
         selfie_media_id: str,
         decision: Decision,
         additional_feedback: List[str] = [],
         verbose: Optional[bool] = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Adds client's feedback about an user onboarding. Usually it comes after human review.
 
         Parameters
         ----------
         user_id
@@ -358,27 +388,33 @@
         data = {
             "document_id": document_id,
             "selfie_media_id": selfie_media_id,
             "decision": decision.value,
             "additional_feedback": additional_feedback,
         }
 
-        response = self.session.post(
-            self.url + "/user/feedback", data=data, headers=headers
-        )
+        try:
+            response = self.session.post(
+                self.url + "/user/feedback",
+                data=data,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="add_user_feedback"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def add_selfie(
         self, user_id: str, media_data: bytes, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         This call is used to upload for the first time the video of the user's face to the onboarding service.
         This video will be used to extract the biometric face profile.
 
         Parameters
         ----------
@@ -399,62 +435,84 @@
         user_token = self.auth.create_user_token(user_id).unwrap_or_return()
         print_token("user_token", user_token, verbose=verbose)
 
         headers = self._auth_headers(user_token)
 
         files = {"video": ("video", media_data)}
 
-        response = self.session.post(
-            f"{self.url}/user/selfie", files=files, headers=headers
-        )
+        try:
+            response = self.session.post(
+                f"{self.url}/user/selfie",
+                files=files,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="add_selfie"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def delete_selfie(
-        self, user_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+        self,
+        user_id: str,
+        selfie_id: Optional[str] = None,
+        verbose: Optional[bool] = False,
+    ) -> Result[Response, Error]:
         """
 
         This call is used to delete the video of the user's face to the onboarding service.
         This will also erase the biometric face profile.
 
         Parameters
         ----------
         user_id
             User identifier
+        selfie_id
+            Optional selfie identifier
         verbose
             Used for print service response as well as the time elapsed
 
 
         Returns
         -------
             A Result object with Response object [requests library] if Success
         """
         print_intro("delete_selfie", verbose=verbose)
 
         backend_token = self.auth.create_backend_token(user_id).unwrap_or_return()
         print_token("backend_token_with_user", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
-
-        response = self.session.delete(f"{self.url}/user/selfie", headers=headers)
+        try:
+            if not selfie_id:
+                response = self.session.delete(
+                    f"{self.url}/user/selfie", headers=headers, timeout=self.timeout
+                )
+            else:
+                response = self.session.delete(
+                    f"{self.url}/user/selfie/{selfie_id}",
+                    headers=headers,
+                    timeout=self.timeout,
+                )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="delete_selfie"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def void_selfie(
         self, user_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         This call is used to void the video of the user's face to the onboarding service.
         This will NOT erase the biometric face profile.
 
         Parameters
         ----------
@@ -471,25 +529,30 @@
         print_intro("void_selfie", verbose=verbose)
 
         backend_token = self.auth.create_backend_token(user_id).unwrap_or_return()
         print_token("backend_token_with_user", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
 
-        response = self.session.patch(f"{self.url}/user/selfie", headers=headers)
+        try:
+            response = self.session.patch(
+                f"{self.url}/user/selfie", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="void_selfie"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def supported_documents(
         self, user_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
         This method is used to obtain a hierarchical-ordered dict with the information of the documents supported by the API.
 
         Parameters
         ----------
         user_id
             User identifier
@@ -508,28 +571,33 @@
             print_token("user_token", token, verbose=verbose)
         else:
             token = self.auth.create_backend_token().unwrap_or_return()
             print_token("backend_token", token, verbose=verbose)
 
         headers = self._auth_headers(token)
 
-        response = self.session.get(f"{self.url}/documents/supported", headers=headers)
+        try:
+            response = self.session.get(
+                f"{self.url}/documents/supported", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="supported_documents"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def create_document(
         self,
         user_id: str,
         type: DocumentType,
         issuing_country: str,
         verbose: Optional[bool] = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         This call is used to obtain a new document_id
         With this document_id you will be able to extract information with the add_document method
 
         Parameters
         ----------
@@ -550,27 +618,33 @@
         print_intro("create_document", verbose=verbose)
         user_token = self.auth.create_user_token(user_id).unwrap_or_return()
         print_token("user_token", user_token, verbose=verbose)
 
         headers = self._auth_headers(user_token)
 
         data = {"type": type.value, "issuing_country": issuing_country}
-        response = self.session.post(
-            f"{self.url}/user/document", data=data, headers=headers
-        )
+        try:
+            response = self.session.post(
+                f"{self.url}/user/document",
+                data=data,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="create_document"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def delete_document(
         self, user_id: str, document_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Delete all the stored/extracted information from a document
 
 
         Parameters
         ----------
@@ -587,27 +661,31 @@
         """
         print_intro("delete_document", verbose=verbose)
 
         backend_token = self.auth.create_backend_token(user_id).unwrap_or_return()
         print_token("backend_token_with_user", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
-        response = self.session.delete(
-            f"{self.url}/user/document/{document_id}", headers=headers
-        )
-
+        try:
+            response = self.session.delete(
+                f"{self.url}/user/document/{document_id}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="delete_document"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def void_document(
         self, user_id: str, document_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Mark a document as invalid.
 
 
         Parameters
         ----------
@@ -624,17 +702,22 @@
         """
         print_intro("void_document", verbose=verbose)
 
         backend_token = self.auth.create_backend_token(user_id).unwrap_or_return()
         print_token("backend_token_with_user", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
-        response = self.session.patch(
-            f"{self.url}/user/document/{document_id}", headers=headers
-        )
+        try:
+            response = self.session.patch(
+                f"{self.url}/user/document/{document_id}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="void_document"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
@@ -645,15 +728,15 @@
         media_data: bytes,
         side: DocumentSide,
         manual: bool = False,
         source: DocumentSource = DocumentSource.file,
         bounding_box: Union[BoundingBox, None] = None,
         fields: Union[Dict[str, Any], None] = None,
         verbose: Optional[bool] = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         This call is used to upload for the first time the photo or video of a document to the onboarding service.
         From a given media, the platform automatically saves the document content.
 
         Parameters
         ----------
@@ -696,31 +779,38 @@
         }
 
         if bounding_box:
             data["bounding_box"] = bounding_box.json()
 
         files = {"image": ("image", media_data)}
 
-        response = self.session.put(
-            f"{self.url}/user/document", files=files, data=data, headers=headers
-        )
+        try:
+            response = self.session.put(
+                f"{self.url}/user/document",
+                files=files,
+                data=data,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="add_document"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def document_properties(
         self,
         user_id: str,
         type: DocumentType,
         issuing_country: str,
         verbose: Optional[bool] = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns the properties of a previously added document, such as face, MRZ or NFC availability
 
 
         Parameters
         ----------
@@ -742,27 +832,32 @@
 
         user_token = self.auth.create_user_token(user_id).unwrap_or_return()
         print_token("user_token", user_token, verbose=verbose)
 
         headers = self._auth_headers(user_token)
         data = {"type": type.value, "issuing_country": issuing_country}
 
-        response = self.session.post(
-            f"{self.url}/user/document/properties", data=data, headers=headers
-        )
-
+        try:
+            response = self.session.post(
+                f"{self.url}/user/document/properties",
+                data=data,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="document_properties"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def delete_other_trusted_document(
         self, user_id: str, document_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Delete all the stored/extracted information from an other trusted document
 
 
         Parameters
         ----------
@@ -779,27 +874,34 @@
         """
         print_intro("delete_other_trusted_document", verbose=verbose)
 
         backend_token = self.auth.create_backend_token(user_id).unwrap_or_return()
         print_token("backend_token_with_user", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
-        response = self.session.delete(
-            f"{self.url}/user/other-trusted-document/{document_id}", headers=headers
-        )
+        try:
+            response = self.session.delete(
+                f"{self.url}/user/other-trusted-document/{document_id}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(
+                OnboardingError.timeout(operation="delete_other_trusted_document")
+            )
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def void_other_trusted_document(
         self, user_id: str, document_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Mark other trusted document as invalid.
 
 
         Parameters
         ----------
@@ -816,31 +918,37 @@
         """
         print_intro("void_other_trusted_document", verbose=verbose)
 
         backend_token = self.auth.create_backend_token(user_id).unwrap_or_return()
         print_token("backend_token_with_user", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
-        response = self.session.patch(
-            f"{self.url}/user/other-trusted-document/{document_id}", headers=headers
-        )
-
+        try:
+            response = self.session.patch(
+                f"{self.url}/user/other-trusted-document/{document_id}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(
+                OnboardingError.timeout(operation="void_other_trusted_document")
+            )
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def add_other_trusted_document(
         self,
         user_id: str,
         media_data: bytes,
         category: Optional[str] = None,
         verbose: Optional[bool] = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         This call is used to upload an other trusted document (OTD) to the onboarding service.
         An OTD could be a bank receipt, a proof of address, a bill...
         From a given pdf media, the platform automatically saves the content.
 
         Parameters
@@ -865,32 +973,38 @@
         print_token("user_token", user_token, verbose=verbose)
 
         headers = self._auth_headers(user_token)
         files = {"pdf": ("pdf", media_data)}
 
         data = dict(category=category) if category else dict()
 
-        response = self.session.post(
-            f"{self.url}/user/other-trusted-document",
-            files=files,
-            data=data,
-            headers=headers,
-        )
+        try:
+            response = self.session.post(
+                f"{self.url}/user/other-trusted-document",
+                files=files,
+                data=data,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(
+                OnboardingError.timeout(operation="add_other_trusted_document")
+            )
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @timeit
     def create_report(
         self,
         user_id: str,
         version: Version = Version.DEFAULT,
         verbose: Optional[bool] = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         This call is used to get the report of the onboarding process for a specific user.
         It returns information on all evidence that has been added and analyzed for that user,
         including documents and facial verifications.
 
 
@@ -913,29 +1027,34 @@
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         headers = self._auth_headers(backend_user_token)
         headers["Alice-Report-Version"] = version.value
 
-        response = self.session.get(f"{self.url}/user/report", headers=headers)
+        try:
+            response = self.session.get(
+                f"{self.url}/user/report", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="create_report"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def create_certificate(
         self,
         user_id: str,
         locale: CertificateLocale = CertificateLocale.EN,
         template_name: str = "default",
         verbose: Optional[bool] = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
         This call is used to create a Certificate (Signed PDF Report) of the onboarding process for a specific user.
         It returns a identifier (certificate_id) as a reference of created resource.
         This resource contains all evidence defined in the template.
 
 
         Parameters
@@ -960,26 +1079,33 @@
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         options = {"template_name": template_name, "locale": locale.value}
         headers = self._auth_headers(backend_user_token)
         headers["Content-Type"] = "application/json"
-        response = self.session.post(
-            f"{self.url}/user/certificate", data=json.dumps(options), headers=headers
-        )
+        try:
+            response = self.session.post(
+                f"{self.url}/user/certificate",
+                data=json.dumps(options),
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="create_certificate"))
+
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def retrieve_certificate(
         self, user_id: str, certificate_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         This call is used to retrieve a Certificate (Signed PDF Report) of the onboarding process for a specific user.
         This resource contains all evidence defined in the template.
 
 
         Parameters
@@ -999,27 +1125,32 @@
         print_intro("retrieve_certificate", verbose=verbose)
 
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
         headers = self._auth_headers(backend_user_token)
-        response = self.session.get(
-            f"{self.url}/user/certificate/{certificate_id}", headers=headers
-        )
+        try:
+            response = self.session.get(
+                f"{self.url}/user/certificate/{certificate_id}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="retrieve_certificate"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def retrieve_certificates(
         self, user_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns summary info for created certificates
 
         Parameters
         ----------
         user_id
@@ -1034,25 +1165,29 @@
         print_intro("retrieve_certificates", verbose=verbose)
 
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
         headers = self._auth_headers(backend_user_token)
-        response = self.session.get(f"{self.url}/user/certificates", headers=headers)
-
+        try:
+            response = self.session.get(
+                f"{self.url}/user/certificates", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="retrieve_certificates"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def screening(
         self, user_id: str, detail: bool = False, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
         This call is used to check on the user using different databases & lists (sanctions, PEP, etc)..
         It returns retrieved information from public lists.
 
         Parameters
         ----------
         user_id
@@ -1075,25 +1210,27 @@
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
         headers = self._auth_headers(backend_user_token)
 
         url = f"{self.url}/user/screening/search"
         if detail:
             url += "/detail"
 
-        response = self.session.get(url, headers=headers)
-
+        try:
+            response = self.session.get(url, headers=headers, timeout=self.timeout)
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="screening"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def screening_monitor_add(
         self, user_id: str, verbose: Optional[bool] = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
         This call is adds a user to the AML monitoring list.
 
 
         Parameters
         ----------
         user_id
@@ -1107,30 +1244,39 @@
               A Result object with Response object [requests library] if Success
         """
         print_intro("screening_monitor_add", verbose=verbose)
 
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
-        print_token("backend_token_with_user", backend_user_token, verbose=verbose)
+        print_token(
+            "backend_token_with_user",
+            backend_user_token,
+            verbose=verbose,
+        )
         headers = self._auth_headers(backend_user_token)
 
-        response = self.session.get(
-            f"{self.url}/user/screening/monitor", headers=headers
-        )
+        try:
+            response = self.session.get(
+                f"{self.url}/user/screening/monitor",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="screening_monitor_add"))
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def screening_monitor_delete(
         self, user_id: str, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
         This call is adds a user to the AML monitoring list.
 
 
         Parameters
         ----------
         user_id
@@ -1147,27 +1293,34 @@
 
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
         headers = self._auth_headers(backend_user_token)
 
-        response = self.session.delete(
-            f"{self.url}/user/screening/monitor", headers=headers
-        )
+        try:
+            response = self.session.delete(
+                f"{self.url}/user/screening/monitor",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(
+                OnboardingError.timeout(operation="screening_monitor_delete")
+            )
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def screening_monitor_open_alerts(
         self, start_index: int = 0, size: int = 100, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
         Retrieves from the monitoring list the users with open alerts
 
         Parameters
         ----------
         start_index
             DB index to start (0-2147483647)
@@ -1183,32 +1336,37 @@
         """
         print_intro("screening_monitor_open_alerts", verbose=verbose)
 
         backend_token = self.auth.create_backend_token().unwrap_or_return()
         print_token("backend_token", backend_token, verbose=verbose)
         headers = self._auth_headers(backend_token)
 
-        response = self.session.get(
-            f"{self.url}/users/screening/monitor/alerts?start_index={start_index}&size={size}",
-            headers=headers,
-        )
-
+        try:
+            response = self.session.get(
+                f"{self.url}/users/screening/monitor/alerts?start_index={start_index}&size={size}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(
+                OnboardingError.timeout(operation="screening_monitor_open_alerts")
+            )
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def identify_user(
         self,
         target_user_id: str,
         probe_user_ids: List[str],
         version: Version = Version.DEFAULT,
         verbose: bool = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
         Identifies (1:N matching) a user against a N-length list of users.
 
         Parameters
         ----------
          target_user_id
             User identifier (Target)
@@ -1232,95 +1390,157 @@
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         headers = self._auth_headers(backend_user_token)
         headers["Alice-Identify-Version"] = version.value
 
         data = {"user_ids": probe_user_ids}
 
-        response = self.session.post(
-            f"{self.url}/user/identify", headers=headers, data=data
-        )
+        try:
+            response = self.session.post(
+                f"{self.url}/user/identify",
+                headers=headers,
+                data=data,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="identify_user"))
+        print_response(response=response, verbose=verbose)
 
+        return Success(response)
+
+    @early_return
+    def user_matching(
+        self,
+        user_id: str,
+        match_case: MatchCase,
+        verbose: bool = False,
+    ) -> Result[Response, Error]:
+        """
+        It performs face matching between all the user selfies or documents. This call requires a BACKEND_TOKEN_WITH_USER_ID..
+
+        Parameters
+        ----------
+        user_id
+            User identifier
+        match_case
+            Evidence (selfies or docs) on which to perform the matching
+        verbose
+            Used for print service response as well as the time elapsed
+
+
+        Returns
+        -------
+            A Result object with Response object [requests library] if Success
+        """
+        print_intro("user_matching", verbose=verbose)
+
+        backend_user_token = self.auth.create_backend_token(
+            user_id=user_id
+        ).unwrap_or_return()
+        print_token("backend_token_with_user", backend_user_token, verbose=verbose)
+
+        headers = self._auth_headers(backend_user_token)
+
+        try:
+            response = self.session.get(
+                f"{self.url}/user/match?match_case={match_case.value}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="user_matching"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
-    def authorize_user(
+    def enable_authentication(
         self, user_id: str, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
-        Authorizes a user. Now it can be authenticate.
+        It enables the authentication for a user.
 
         Parameters
         ----------
         user_id
             User identifier
         verbose
             Used for print service response as well as the time elapsed
 
 
         Returns
         -------
             A Result object with Response object [requests library] if Success
         """
-        print_intro("authorize_user", verbose=verbose)
+        print_intro("enable_authentication", verbose=verbose)
 
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         headers = self._auth_headers(backend_user_token)
-        response = self.session.post(f"{self.url}/user/authorize", headers=headers)
-
+        try:
+            response = self.session.post(
+                f"{self.url}/user/authentication/enable",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="enable_authentication"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
-    def deauthorize_user(
+    def disable_authentication(
         self, user_id: str, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
-        Deauthorizes a user. Now it cannot be authenticate.
+        It disables the authentication for a user.
 
         Parameters
         ----------
         user_id
             User identifier
         verbose
             Used for print service response as well as the time elapsed
 
 
         Returns
         -------
             A Result object with Response object [requests library] if Success
         """
-        print_intro("deauthorize_user", verbose=verbose)
+        print_intro("disable_authentication", verbose=verbose)
 
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         headers = self._auth_headers(backend_user_token)
-        response = self.session.post(f"{self.url}/user/deauthorize", headers=headers)
-
+        try:
+            response = self.session.post(
+                f"{self.url}/user/authentication/disable",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="disable_authentication"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def authenticate_user(
         self, user_id: str, media_data: bytes, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Authenticates a previously registered User against a given media to verify the identity
 
         Parameters
         ----------
         user_id
@@ -1340,27 +1560,32 @@
         user_token = self.auth.create_user_token(user_id=user_id).unwrap_or_return()
         print_token("user_token", user_token, verbose=verbose)
 
         headers = self._auth_headers(user_token)
 
         files = {"video": ("video", media_data)}
 
-        response = self.session.post(
-            f"{self.url}/user/authenticate", files=files, headers=headers
-        )
-
+        try:
+            response = self.session.post(
+                f"{self.url}/user/authenticate",
+                files=files,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="authenticate_user"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def get_authentications_ids(
         self, user_id: str, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns all authentication you have performed for a User, sorted by creation date in descending order.
 
         Parameters
         ----------
         user_id
@@ -1378,33 +1603,37 @@
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         headers = self._auth_headers(backend_user_token)
 
-        response = self.session.get(
-            f"{self.url}/user/authentications/ids", headers=headers
-        )
-
+        try:
+            response = self.session.get(
+                f"{self.url}/user/authentications/ids",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_authentications_ids"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def get_authentications(
         self,
         user_id: str,
         page: int = 1,
         page_size: int = 0,
         descending: bool = True,
         version: Version = Version.DEFAULT,
         verbose: bool = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns all authentications you have performed for a User.
 
         Parameters
         ----------
         user_id
@@ -1435,31 +1664,35 @@
         headers = self._auth_headers(backend_user_token)
         headers["Alice-Authentication-Version"] = version.value
 
         url_query_params = (
             f"?page={str(page)}&page_size={str(page_size)}&descending={str(descending)}"
         )
 
-        response = self.session.get(
-            f"{self.url}/user/authentications" + url_query_params, headers=headers
-        )
-
+        try:
+            response = self.session.get(
+                f"{self.url}/user/authentications" + url_query_params,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_authentications"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def get_authentication(
         self,
         user_id: str,
         authentication_id: str,
         version: Version = Version.DEFAULT,
         verbose: bool = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Gets a information from a previous authentication using the verification_id
 
         Parameters
         ----------
         user_id
@@ -1482,27 +1715,31 @@
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         headers = self._auth_headers(backend_user_token)
         headers["Alice-Authentication-Version"] = version.value
 
-        response = self.session.get(
-            f"{self.url}/user/authentication/{authentication_id}", headers=headers
-        )
-
+        try:
+            response = self.session.get(
+                f"{self.url}/user/authentication/{authentication_id}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_authentication"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def retrieve_media(
         self, user_id: str, media_id: str, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns the binary data of a media resource
 
         Parameters
         ----------
         user_id
@@ -1522,27 +1759,31 @@
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         headers = self._auth_headers(backend_user_token)
 
-        response = self.session.get(
-            f"{self.url}/media/{media_id}/download", headers=headers
-        )
-
+        try:
+            response = self.session.get(
+                f"{self.url}/media/{media_id}/download",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="retrieve_media"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def download(
         self, user_id: str, href: str, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns the binary data of a media resource
 
         Parameters
         ----------
         user_id
@@ -1562,29 +1803,31 @@
         backend_user_token = self.auth.create_backend_token(
             user_id=user_id
         ).unwrap_or_return()
         print_token("backend_token_with_user", backend_user_token, verbose=verbose)
 
         headers = self._auth_headers(backend_user_token)
 
-        response = self.session.get(href, headers=headers)
-
+        try:
+            response = self.session.get(href, headers=headers, timeout=self.timeout)
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="download"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def request_duplicates_search(
         self,
         start_date: datetime,
         end_date: datetime,
         resource_type: DuplicatesResourceType,
         verbose: bool = False,
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Returns the binary data of a media resource
 
         Parameters
         ----------
         start_date
@@ -1609,26 +1852,34 @@
         headers = self._auth_headers(backend_token)
 
         data = {
             "start_date": start_date.isoformat(),
             "end_date": end_date.isoformat(),
             "resource_type": resource_type.value,
         }
-        response = requests.post(
-            f"{self.url}/duplicates/search", data=data, headers=headers
-        )
+        try:
+            response = requests.post(
+                f"{self.url}/duplicates/search",
+                data=data,
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(
+                OnboardingError.timeout(operation="request_duplicates_search")
+            )
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def get_duplicates_search(
         self, search_id: str, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    ) -> Result[Response, Error]:
         """
 
         Retrieves a previously requested duplicates search from the onboarding platform
 
         Parameters
         ----------
         search_id
@@ -1645,26 +1896,29 @@
         print_intro("get_duplicates_search", verbose=verbose)
 
         backend_token = self.auth.create_backend_token().unwrap_or_return()
         print_token("backend_token", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
 
-        response = requests.get(
-            f"{self.url}/duplicates/search/{search_id}", headers=headers
-        )
+        try:
+            response = requests.get(
+                f"{self.url}/duplicates/search/{search_id}",
+                headers=headers,
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_duplicates_search"))
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
-    def get_duplicates_searches(
-        self, verbose: bool = False
-    ) -> Result[Response, AuthError]:
+    def get_duplicates_searches(self, verbose: bool = False) -> Result[Response, Error]:
         """
 
         Retrieves all previously requested duplicates searches from the onboarding platform
 
         Parameters
         ----------
         verbose
@@ -1679,11 +1933,110 @@
         print_intro("get_duplicates_searches", verbose=verbose)
 
         backend_token = self.auth.create_backend_token().unwrap_or_return()
         print_token("backend_token", backend_token, verbose=verbose)
 
         headers = self._auth_headers(backend_token)
 
-        response = requests.get(f"{self.url}/duplicates/searches", headers=headers)
+        try:
+            response = requests.get(
+                f"{self.url}/duplicates/searches", headers=headers, timeout=self.timeout
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="get_duplicates_searches"))
+        print_response(response=response, verbose=verbose)
+
+        return Success(response)
+
+    @timeit
+    def accept_user(
+        self, user_id: str, operator: str = "auto", verbose: bool = False
+    ) -> Result[Response, Error]:
+        """
+        Mark a user state as ACCEPTED
+
+        Parameters
+        ----------
+        user_id
+            User identifier
+        operator
+            Who is accepting the user
+        verbose
+            Used for print service response as well as the time elapsed
+
+
+        Returns
+        -------
+            A Response object [requests library]
+        """
+        print_intro("accept_user", verbose=verbose)
+
+        backend_user_token = self.auth.create_backend_token(
+            user_id=user_id
+        ).unwrap_or_return()
+        print_token("backend_token_with_user", backend_user_token, verbose=verbose)
+
+        headers = self._auth_headers(backend_user_token)
+        try:
+            response = requests.post(
+                f"{self.url}/user/state/accept",
+                headers=headers,
+                json={
+                    "operator": operator,
+                },
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="accept_user"))
+
+        print_response(response=response, verbose=verbose)
+
+        return Success(response)
+
+    @timeit
+    def reject_user(
+        self,
+        user_id: str,
+        rejection_reasons: Optional[List[Dict[str, str]]] = None,
+        operator: str = "auto",
+        verbose: bool = False,
+    ) -> Result[Response, Error]:
+        """
+        Mark a user state as REJECTED
+
+        Parameters
+        ----------
+        user_id
+            User identifier
+        rejection_reasons
+            List of rejection reasons
+        operator
+            Who is rejecting the user
+        verbose
+            Used for print service response as well as the time elapsed
+
+
+        Returns
+        -------
+            A Response object [requests library]
+        """
+        print_intro("accept_user", verbose=verbose)
+
+        backend_user_token = self.auth.create_backend_token(
+            user_id=user_id
+        ).unwrap_or_return()
+        print_token("backend_token_with_user", backend_user_token, verbose=verbose)
+
+        headers = self._auth_headers(backend_user_token)
+        try:
+            response = requests.post(
+                f"{self.url}/user/state/reject",
+                headers=headers,
+                json={"operator": operator, "rejection_reasons": rejection_reasons},
+                timeout=self.timeout,
+            )
+        except requests.exceptions.Timeout:
+            return Failure(OnboardingError.timeout(operation="accept_user"))
+
         print_response(response=response, verbose=verbose)
 
         return Success(response)
```

### Comparing `alice-onboarding-1.9.0/alice/onboarding/onboarding_errors.py` & `alice-onboarding-2.0.0/alice/onboarding/onboarding_errors.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,7 +28,13 @@
     def from_response(operation: str, response: Response) -> "OnboardingError":
         code = response.status_code
         try:
             message = response.json()
         except Exception:
             message = {"message": "no content"}
         return OnboardingError(operation=operation, code=code, message=message)
+
+    @staticmethod
+    def timeout(operation: str) -> "OnboardingError":
+        return OnboardingError(
+            operation=operation, code=408, message={"message": "Request timed out"}
+        )
```

### Comparing `alice-onboarding-1.9.0/alice/onboarding/tools.py` & `alice-onboarding-2.0.0/alice/onboarding/tools.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/public_api.py` & `alice-onboarding-2.0.0/alice/public_api.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/sandbox/sandbox.py` & `alice-onboarding-2.0.0/alice/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/sandbox/sandbox_client.py` & `alice-onboarding-2.0.0/alice/sandbox/sandbox_client.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/sandbox/sandbox_errors.py` & `alice-onboarding-2.0.0/alice/sandbox/sandbox_errors.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/webhooks/webhook.py` & `alice-onboarding-2.0.0/alice/webhooks/webhook.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/webhooks/webhooks.py` & `alice-onboarding-2.0.0/alice/webhooks/webhooks.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice/webhooks/webhooks_client.py` & `alice-onboarding-2.0.0/alice/webhooks/webhooks_client.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-1.9.0/alice_onboarding.egg-info/PKG-INFO` & `alice-onboarding-2.0.0/alice_onboarding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: alice-onboarding
-Version: 1.9.0
+Version: 2.0.0
 Summary: Alice Onboarding Python SDK
 Home-page: https://github.com/alice-biometrics/onboarding-python
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: Alice Copyright
 Keywords: onboarding,biometrics,kyc,alice
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # onboarding-python <img src="https://github.com/alice-biometrics/custom-emojis/blob/master/images/python.png?raw=true" width="30"> 
 
 [![version](https://img.shields.io/github/release/alice-biometrics/onboarding-python/all.svg)](https://github.com/alice-biometrics/onboarding-python/releases) [![doc](https://img.shields.io/badge/doc-onboarding-51CB56)](https://docs.alicebiometrics.com/onboarding/sections/server/server_side_sdks/python.html)
```

### Comparing `alice-onboarding-1.9.0/alice_onboarding.egg-info/SOURCES.txt` & `alice-onboarding-2.0.0/alice_onboarding.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,78 +3,100 @@
 README.md
 setup.cfg
 setup.py
 alice/VERSION
 alice/__init__.py
 alice/config.py
 alice/public_api.py
+alice/auth/__init__.py
 alice/auth/auth.py
 alice/auth/auth_client.py
 alice/auth/auth_errors.py
+alice/auth/cached_token_stack.py
+alice/auth/token_tools.py
+alice/onboarding/__init__.py
 alice/onboarding/onboarding.py
 alice/onboarding/onboarding_client.py
 alice/onboarding/onboarding_errors.py
 alice/onboarding/tools.py
+alice/onboarding/enums/__init__.py
 alice/onboarding/enums/certificate_locale.py
 alice/onboarding/enums/decision.py
 alice/onboarding/enums/document_side.py
 alice/onboarding/enums/document_source.py
 alice/onboarding/enums/document_type.py
 alice/onboarding/enums/duplicates_resource_type.py
+alice/onboarding/enums/match_case.py
 alice/onboarding/enums/version.py
+alice/onboarding/models/__init__.py
 alice/onboarding/models/bounding_box.py
 alice/onboarding/models/device_info.py
 alice/onboarding/models/user_info.py
+alice/onboarding/models/report/__init__.py
 alice/onboarding/models/report/report.py
+alice/onboarding/models/report/checks/__init__.py
 alice/onboarding/models/report/checks/check.py
+alice/onboarding/models/report/checks/document/__init__.py
 alice/onboarding/models/report/checks/document/authentic_nfc_chip_check.py
 alice/onboarding/models/report/checks/document/checked_info_code_check.py
 alice/onboarding/models/report/checks/document/coherent_document_dates_check.py
 alice/onboarding/models/report/checks/document/consistent_document_check.py
 alice/onboarding/models/report/checks/document/expected_document_check.py
 alice/onboarding/models/report/checks/document/face_in_document_check.py
 alice/onboarding/models/report/checks/document/face_matching_document_check.py
 alice/onboarding/models/report/checks/document/not_a_printed_document_check.py
 alice/onboarding/models/report/checks/document/not_a_screen_document_check.py
 alice/onboarding/models/report/checks/document/not_a_synthetic_document_check.py
 alice/onboarding/models/report/checks/document/uncompromised_document_check.py
 alice/onboarding/models/report/checks/document/unexpired_document_check.py
+alice/onboarding/models/report/checks/field/__init__.py
 alice/onboarding/models/report/checks/field/cheked_field_check.py
 alice/onboarding/models/report/checks/field/complete_mrz_name_check.py
 alice/onboarding/models/report/checks/field/consistent_field_check.py
 alice/onboarding/models/report/checks/field/expected_field_check.py
 alice/onboarding/models/report/checks/field/over_18_check.py
 alice/onboarding/models/report/checks/field/unexpired_date_check.py
 alice/onboarding/models/report/checks/field/valid_date_format_check.py
 alice/onboarding/models/report/checks/field/valid_date_range_check.py
+alice/onboarding/models/report/checks/selfie/__init__.py
 alice/onboarding/models/report/checks/selfie/liveness_check.py
 alice/onboarding/models/report/checks/selfie/only_one_face_check.py
+alice/onboarding/models/report/checks/summary/__init__.py
 alice/onboarding/models/report/checks/summary/only_one_device_check.py
 alice/onboarding/models/report/checks/summary/only_one_ip_check.py
+alice/onboarding/models/report/compliance/__init__.py
 alice/onboarding/models/report/compliance/device_out.py
 alice/onboarding/models/report/compliance/domain_events_report.py
 alice/onboarding/models/report/compliance/user_event_out.py
+alice/onboarding/models/report/document/__init__.py
 alice/onboarding/models/report/document/document_field.py
 alice/onboarding/models/report/document/document_report.py
 alice/onboarding/models/report/document/document_report_meta.py
 alice/onboarding/models/report/document/document_side.py
 alice/onboarding/models/report/document/document_side_report.py
 alice/onboarding/models/report/document/document_side_report_meta.py
 alice/onboarding/models/report/document/document_type.py
+alice/onboarding/models/report/face_matching/__init__.py
 alice/onboarding/models/report/face_matching/face_matching.py
+alice/onboarding/models/report/other_trusted_document/__init__.py
 alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py
 alice/onboarding/models/report/other_trusted_document/other_trusted_document_report_meta.py
+alice/onboarding/models/report/selfie/__init__.py
 alice/onboarding/models/report/selfie/selfie_report.py
+alice/onboarding/models/report/shared/__init__.py
 alice/onboarding/models/report/shared/bounding_box.py
 alice/onboarding/models/report/shared/href.py
+alice/onboarding/models/report/summary/__init__.py
 alice/onboarding/models/report/summary/external_user_data.py
 alice/onboarding/models/report/summary/report_summary.py
+alice/sandbox/__init__.py
 alice/sandbox/sandbox.py
 alice/sandbox/sandbox_client.py
 alice/sandbox/sandbox_errors.py
+alice/webhooks/__init__.py
 alice/webhooks/webhook.py
 alice/webhooks/webhooks.py
 alice/webhooks/webhooks_client.py
 alice_onboarding.egg-info/PKG-INFO
 alice_onboarding.egg-info/SOURCES.txt
 alice_onboarding.egg-info/dependency_links.txt
 alice_onboarding.egg-info/not-zip-safe
```

