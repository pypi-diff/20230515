# Comparing `tmp/lti-consumer-xblock-9.4.0.tar.gz` & `tmp/lti-consumer-xblock-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.4.0.tar", last modified: Mon May  8 15:40:36 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.5.0.tar", last modified: Mon May 15 20:31:54 2023, max compression
```

## Comparing `lti-consumer-xblock-9.4.0.tar` & `lti-consumer-xblock-9.5.0.tar`

### file list

```diff
@@ -1,245 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14500 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13716 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.102956 lti-consumer-xblock-9.4.0/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     6551 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.102956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15317 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.102956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.102956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.102956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.102956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    34236 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.102956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.106956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.106956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.106956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.106956 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    42504 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    72133 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11593 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35381 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.090955 lti-consumer-xblock-9.4.0/lti_consumer/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.090955 lti-consumer-xblock-9.4.0/lti_consumer/public/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.090955 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.110956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.114956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.114956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.114956 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.114956 lti-consumer-xblock-9.4.0/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.114956 lti-consumer-xblock-9.4.0/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.114956 lti-consumer-xblock-9.4.0/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.114956 lti-consumer-xblock-9.4.0/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.114956 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.118957 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.118957 lti-consumer-xblock-9.4.0/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.118957 lti-consumer-xblock-9.4.0/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.118957 lti-consumer-xblock-9.4.0/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.118957 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    84733 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.122957 lti-consumer-xblock-9.4.0/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.094956 lti-consumer-xblock-9.4.0/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14500 2023-05-08 15:40:36.000000 lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7590 2023-05-08 15:40:36.000000 lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-08 15:40:36.000000 lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-08 15:40:36.000000 lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-08 15:40:36.000000 lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-08 15:40:36.000000 lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-08 15:40:36.126957 lti-consumer-xblock-9.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-05-08 15:40:29.000000 lti-consumer-xblock-9.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14454 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13670 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6551 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15317 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34236 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42504 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    72133 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11593 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35442 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.685691 lti-consumer-xblock-9.5.0/lti_consumer/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.685691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_start_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11758 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84733 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14454 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7644 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-15 20:31:54.717692 lti-consumer-xblock-9.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/setup.py
```

### Comparing `lti-consumer-xblock-9.4.0/LICENSE` & `lti-consumer-xblock-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/NOTICE` & `lti-consumer-xblock-9.5.0/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/PKG-INFO` & `lti-consumer-xblock-9.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.4.0
+Version: 9.5.0
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -150,15 +150,15 @@
 
 If you want to download translations from Transifex install
 `transifex client <https://docs.transifex.com/client/installing-the-client/>`_ and run this command while
 inside project root directory:
 
 .. code:: bash
 
-    $ tx pull -f --mode=reviewed -l en,ar,es_419,fr,he,hi,ko_KR,pt_BR,ru,zh_CN
+    $ tx pull -f --mode=reviewed
 
 Further Development Info
 ------------------------
 
 See the `developer guide`_ for implementation details and other developer concerns.
 
 .. _developer guide: ./docs/developing.rst
```

### Comparing `lti-consumer-xblock-9.4.0/README.rst` & `lti-consumer-xblock-9.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 If you want to download translations from Transifex install
 `transifex client <https://docs.transifex.com/client/installing-the-client/>`_ and run this command while
 inside project root directory:
 
 .. code:: bash
 
-    $ tx pull -f --mode=reviewed -l en,ar,es_419,fr,he,hi,ko_KR,pt_BR,ru,zh_CN
+    $ tx pull -f --mode=reviewed
 
 Further Development Info
 ------------------------
 
 See the `developer guide`_ for implementation details and other developer concerns.
 
 .. _developer guide: ./docs/developing.rst
```

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/admin.py` & `lti-consumer-xblock-9.5.0/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/api.py` & `lti-consumer-xblock-9.5.0/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/apps.py` & `lti-consumer-xblock-9.5.0/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/data.py` & `lti-consumer-xblock-9.5.0/lti_consumer/data.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/filters.py` & `lti-consumer-xblock-9.5.0/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/forms.py` & `lti-consumer-xblock-9.5.0/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/constants.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.5.0/lti_consumer/lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/models.py` & `lti-consumer-xblock-9.5.0/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.5.0/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.5.0/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.5.0/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.5.0/lti_consumer/plugin/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from edx_django_utils.cache import TieredCache, get_cache_key
 from jwkest.jwt import JWT, BadSyntax
 from opaque_keys import InvalidKeyError
 from opaque_keys.edx.keys import UsageKey
 from rest_framework import status, viewsets
 from rest_framework.decorators import action
 from rest_framework.response import Response
-from rest_framework.status import HTTP_400_BAD_REQUEST, HTTP_403_FORBIDDEN, HTTP_404_NOT_FOUND
+from rest_framework.status import HTTP_200_OK, HTTP_400_BAD_REQUEST, HTTP_403_FORBIDDEN, HTTP_404_NOT_FOUND
 
 from lti_consumer.api import get_lti_pii_sharing_state_for_course, validate_lti_1p3_launch_data
 from lti_consumer.exceptions import LtiError
 from lti_consumer.lti_1p3.consumer import LtiProctoringConsumer
 from lti_consumer.lti_1p3.exceptions import (BadJwtSignature, InvalidClaimValue, Lti1p3Exception,
                                              LtiDeepLinkingContentTypeNotSupported, MalformedJwtToken,
                                              MissingRequiredClaim, NoSuitableKeys, TokenSignatureExpired,
@@ -830,8 +830,8 @@
     LTI_1P3_PROCTORING_ASSESSMENT_STARTED.send(
         sender=None,
         attempt_number=proctoring_response["attempt_number"],
         resource_link=proctoring_response["resource_link"],
         user_id=request.user.id,
     )
 
-    return JsonResponse(data={})
+    return render(request, 'html/lti_start_assessment.html', status=HTTP_200_OK)
```

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ar/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/en/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/es_419/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/fr/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/he/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/hi/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/it/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ja/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ko/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/pt_BR/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/pt_PT/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/ru/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/public/js/translations/zh_CN/text.js` & `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.5.0/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.5.0/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.5.0/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.5.0/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.5.0/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.5.0/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.5.0/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.5.0/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,7 +276,21 @@
         expected_call_args = call(
             sender=None,
             attempt_number=2,
             resource_link={'id': 'resource_link_id'},
             user_id=self.user.id,
         )
         self.assertEqual(mock_assessment_started_signal.call_args, expected_call_args)
+
+    def test_start_assessment_endpoint_returns_valid_html(self):
+        """
+        Tests that a successful call to the start_assessment_endpoint returns the correct html response.
+        """
+        response = self.client.post(
+            self.url,
+            {
+                "JWT": self.create_tool_jwt_token()
+            },
+        )
+
+        self.assertEqual(response.status_code, 200)
+        self.assertIn('window.close', response.content.decode('utf-8'))
```

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/en/LC_MESSAGES/django.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/settings.py` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/settings.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer/utils.py` & `lti-consumer-xblock-9.5.0/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.4.0
+Version: 9.5.0
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -150,15 +150,15 @@
 
 If you want to download translations from Transifex install
 `transifex client <https://docs.transifex.com/client/installing-the-client/>`_ and run this command while
 inside project root directory:
 
 .. code:: bash
 
-    $ tx pull -f --mode=reviewed -l en,ar,es_419,fr,he,hi,ko_KR,pt_BR,ru,zh_CN
+    $ tx pull -f --mode=reviewed
 
 Further Development Info
 ------------------------
 
 See the `developer guide`_ for implementation details and other developer concerns.
 
 .. _developer guide: ./docs/developing.rst
```

### Comparing `lti-consumer-xblock-9.4.0/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 lti_consumer/templates/html/lti_1p3_launch.html
 lti_consumer/templates/html/lti_1p3_permission_error.html
 lti_consumer/templates/html/lti_1p3_studio.html
 lti_consumer/templates/html/lti_iframe.html
 lti_consumer/templates/html/lti_launch.html
 lti_consumer/templates/html/lti_launch_error.html
 lti_consumer/templates/html/lti_proctoring_start_error.html
+lti_consumer/templates/html/lti_start_assessment.html
 lti_consumer/templates/html/student.html
 lti_consumer/templates/html/lti-dl/dl_response_error.html
 lti_consumer/templates/html/lti-dl/dl_response_saved.html
 lti_consumer/templates/html/lti-dl/render_dl_content.html
 lti_consumer/templates/html/lti-dl/render_html.html
 lti_consumer/templates/html/lti-dl/render_image.html
 lti_consumer/templates/html/lti-dl/render_link.html
```

### Comparing `lti-consumer-xblock-9.4.0/setup.py` & `lti-consumer-xblock-9.5.0/setup.py`

 * *Files identical despite different names*

