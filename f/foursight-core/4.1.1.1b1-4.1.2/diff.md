# Comparing `tmp/foursight_core-4.1.1.1b1.tar.gz` & `tmp/foursight_core-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.1.1b1.tar", max compression
+gzip compressed data, was "foursight_core-4.1.2.tar", max compression
```

## Comparing `foursight_core-4.1.1.1b1.tar` & `foursight_core-4.1.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-05-03 19:29:57.728898 foursight_core-4.1.1.1b1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-05-03 19:29:57.736898 foursight_core-4.1.1.1b1/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-05-03 19:29:57.736898 foursight_core-4.1.1.1b1/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-05-03 19:29:57.736898 foursight_core-4.1.1.1b1/foursight_core/app.py
--rw-r--r--   0        0        0   105128 2023-05-03 19:29:57.736898 foursight_core-4.1.1.1b1/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4452 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    78954 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    33872 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-05-03 19:29:57.740898 foursight_core-4.1.1.1b1/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1931686 2023-05-03 19:29:57.752898 foursight_core-4.1.1.1b1/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1607 2023-05-03 19:29:57.756898 foursight_core-4.1.1.1b1/pyproject.toml
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 foursight_core-4.1.1.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-15 19:31:49.591048 foursight_core-4.1.2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/app.py
+-rw-r--r--   0        0        0   105128 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4476 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    78954 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    33872 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1932518 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1603 2023-05-15 19:31:49.615048 foursight_core-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1189 1970-01-01 00:00:00.000000 foursight_core-4.1.2/PKG-INFO
```

### Comparing `foursight_core-4.1.1.1b1/LICENSE.txt` & `foursight_core-4.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/abstract_connection.py` & `foursight_core-4.1.2/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/app_utils.py` & `foursight_core-4.1.2/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/buckets.py` & `foursight_core-4.1.2/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/check_schema.py` & `foursight_core-4.1.2/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/check_utils.py` & `foursight_core-4.1.2/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.2/foursight_core/checks/access_key_expiration_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .helpers.confchecks import (
     check_function, CheckResult, action_function, ActionResult
 )
+import json
 from datetime import datetime, timedelta
 from dcicutils import s3_utils
 from dcicutils.ff_utils import get_metadata, search_metadata, patch_metadata, post_metadata
 
 
 @check_function(action="refresh_access_keys")
 def access_key_status(connection, **kwargs):
@@ -68,15 +69,15 @@
                                       f'&sort=-date_created', key=connection.ff_keys)
         # generate new key
         access_key_req = {'user': user_uuid, 'description': kp_name}
         access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)['@graph'][0]
         s3_obj = {'secret': access_key_res['secret_access_key'],
                   'key': access_key_res['access_key_id'],
                   'server': s3.url}
-        s3.s3_put_secret(s3_obj, kp_name)
+        s3.s3_put_secret(json.dumps(s3_obj), kp_name)
         full_output['successfully_generated'].append(email)
         # clear out old keys after generating new one
         for access_key in access_keys:  # note this search result was computed before the new key was added
             if access_key['status'] != 'deleted':
                 patch_metadata(patch_item={'status': 'deleted'}, obj_id=access_key['uuid'], key=connection.ff_keys)
 
     action.full_output = full_output
```

### Comparing `foursight_core-4.1.1.1b1/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.2/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.2/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.2/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.2/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.2/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.2/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/checks/test_checks.py` & `foursight_core-4.1.2/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/decorators.py` & `foursight_core-4.1.2/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/deploy.py` & `foursight_core-4.1.2/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/environment.py` & `foursight_core-4.1.2/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/es_connection.py` & `foursight_core-4.1.2/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/exceptions.py` & `foursight_core-4.1.2/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/fs_connection.py` & `foursight_core-4.1.2/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/identity.py` & `foursight_core-4.1.2/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/mapping.json` & `foursight_core-4.1.2/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/package.py` & `foursight_core-4.1.2/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/auth.py` & `foursight_core-4.1.2/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.2/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.2/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.2/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.2/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/checks.py` & `foursight_core-4.1.2/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/cognito.py` & `foursight_core-4.1.2/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.2/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.2/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.2/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/encryption.py` & `foursight_core-4.1.2/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/envs.py` & `foursight_core-4.1.2/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/gac.py` & `foursight_core-4.1.2/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.2/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.2/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.1.2/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/react_api.py` & `foursight_core-4.1.2/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.2/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.2/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.2/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.2/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.2/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/ui/index.html` & `foursight_core-4.1.2/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.2/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.2/foursight_core/react/ui/static/js/main.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.6d493f41.js.LICENSE.txt */
+/*! For license information please see main.6f828eef.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -50229,128 +50229,169 @@
             ea = t.createContext({}),
             ta = function() {
                 var e = (0, t.useContext)(ea);
                 return e ? e[0] : {}
             },
             na = function() {
                 return [Array.from(Yi(Wi)[0].values())]
-            },
-            ra = function(e) {
-                var t, n, r, o, i, a, s, u, l = e.info,
-                    c = e.foursightUrl;
+            };
+
+        function ra(e, t) {
+            var n, r, o, i, a, s, u, l;
+            return !st.IsNull(null === e || void 0 === e || null === (n = e.app) || void 0 === n || null === (r = n.credentials) || void 0 === r ? void 0 : r.aws_account_number) && !st.IsNull(null === t || void 0 === t || null === (o = t.data) || void 0 === o || null === (i = o.foursight) || void 0 === i ? void 0 : i.aws_account_number) && (null === e || void 0 === e || null === (a = e.app) || void 0 === a || null === (s = a.credentials) || void 0 === s ? void 0 : s.aws_account_number) === (null === t || void 0 === t || null === (u = t.data) || void 0 === u || null === (l = u.foursight) || void 0 === l ? void 0 : l.aws_account_number)
+        }
+        var oa = function(e) {
+                var t, n, r, o, i, a, s, u, l = e.header,
+                    c = e.info,
+                    d = e.foursightUrl,
+                    f = function(e) {
+                        var t = e.url;
+                        return t && t.startsWith("https://") && (0, Kr.jsxs)("small", {
+                            children: ["\xa0| ", (0, Kr.jsx)("a", {
+                                style: {
+                                    color: "inherit"
+                                },
+                                href: kr.Path("certificates") + "/?hostname=" + t,
+                                rel: "noreferrer",
+                                target: "_blank",
+                                children: (0, Kr.jsx)("b", {
+                                    children: "SSL"
+                                })
+                            }), "\xa0", (0, Kr.jsx)("a", {
+                                style: {
+                                    color: "inherit"
+                                },
+                                href: kr.Path("certificates") + "/?hostname=" + t,
+                                rel: "noreferrer",
+                                target: "_blank",
+                                children: (0, Kr.jsx)("span", {
+                                    className: "fa fa-external-link",
+                                    style: {
+                                        position: "relative",
+                                        bottom: "-1px"
+                                    }
+                                })
+                            })]
+                        })
+                    },
+                    p = Xi("/portal_access_key");
                 return (0, Kr.jsx)("table", {
                     style: {
                         width: "100%"
                     },
                     children: (0, Kr.jsxs)("tbody", {
                         style: {
                             whiteSpace: "nowrap"
                         },
                         children: [(0, Kr.jsxs)("tr", {
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt",
                                     width: "10%"
                                 },
-                                children: "foursight-cgap" === l.get("foursight.package") ? (0, Kr.jsx)(Kr.Fragment, {
+                                children: "foursight-cgap" === c.get("foursight.package") ? (0, Kr.jsx)(Kr.Fragment, {
                                     children: "Foursight-CGAP:"
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
-                                    children: "foursight" === l.get("foursight.package") ? (0, Kr.jsx)(Kr.Fragment, {
+                                    children: "foursight" === c.get("foursight.package") ? (0, Kr.jsx)(Kr.Fragment, {
                                         children: "Foursight-Fourfront:"
                                     }) : (0, Kr.jsx)(Kr.Fragment, {
                                         children: "Foursight:"
                                     })
                                 })
                             }), (0, Kr.jsxs)("td", {
                                 children: [(0, Kr.jsx)("a", {
                                     style: {
                                         color: "inherit"
                                     },
-                                    href: l.get("foursight.url") || c,
+                                    href: c.get("foursight.url") || d,
                                     rel: "noreferrer",
                                     target: "_blank",
-                                    children: l.get("foursight.url") || c
+                                    children: c.get("foursight.url") || d
                                 }), "\xa0", (0, Kr.jsx)("a", {
                                     style: {
                                         color: "inherit"
                                     },
-                                    href: l.get("foursight.url") || c,
+                                    href: c.get("foursight.url") || d,
                                     rel: "noreferrer",
                                     target: "_blank",
                                     children: (0, Kr.jsx)("span", {
                                         className: "fa fa-external-link",
                                         style: {
                                             position: "relative",
                                             bottom: "-1px"
                                         }
                                     })
+                                }), (0, Kr.jsx)(f, {
+                                    url: c.get("foursight.url")
                                 })]
                             })]
                         }), (0, Kr.jsxs)("tr", {
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "Portal:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("portal.url") ? (0, Kr.jsxs)(Kr.Fragment, {
+                                children: c.get("portal.url") ? (0, Kr.jsxs)(Kr.Fragment, {
                                     children: [(0, Kr.jsx)("a", {
                                         style: {
                                             color: "inherit"
                                         },
-                                        href: l.get("portal.url"),
+                                        href: c.get("portal.url"),
                                         rel: "noreferrer",
                                         target: "_blank",
-                                        children: l.get("portal.url")
+                                        children: c.get("portal.url")
                                     }), "\xa0", (0, Kr.jsx)("a", {
                                         style: {
                                             color: "inherit"
                                         },
-                                        href: l.get("portal.url"),
+                                        href: c.get("portal.url"),
                                         rel: "noreferrer",
                                         target: "_blank",
                                         children: (0, Kr.jsx)("span", {
                                             className: "fa fa-external-link",
                                             style: {
                                                 position: "relative",
                                                 bottom: "-1px"
                                             }
                                         })
                                     }), "\xa0|\xa0", (0, Kr.jsx)("a", {
                                         style: {
                                             color: "inherit"
                                         },
-                                        href: l.get("portal.health_ui_url"),
+                                        href: c.get("portal.health_ui_url"),
                                         rel: "noreferrer",
                                         target: "_blank",
                                         children: "Health"
                                     }), "\xa0", (0, Kr.jsx)("a", {
                                         style: {
                                             color: "inherit"
                                         },
-                                        href: l.get("portal.health_ui_url"),
+                                        href: c.get("portal.health_ui_url"),
                                         rel: "noreferrer",
                                         target: "_blank",
                                         children: (0, Kr.jsx)("span", {
                                             className: "fa fa-external-link",
                                             style: {
                                                 position: "relative",
                                                 bottom: "-1px"
                                             }
                                         })
                                     }), "\xa0", (0, Kr.jsxs)("small", {
                                         children: ["(", (0, Kr.jsx)("a", {
                                             style: {
                                                 color: "inherit"
                                             },
-                                            href: l.get("portal.health_url"),
+                                            href: c.get("portal.health_url"),
                                             rel: "noreferrer",
                                             target: "_blank",
                                             children: "JSON"
-                                        }), ")\xa0"]
+                                        }), ")"]
+                                    }), (0, Kr.jsx)(f, {
+                                        url: c.get("portal.url")
                                     })]
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
                         }), (0, Kr.jsxs)("tr", {
                             style: {
@@ -50358,36 +50399,36 @@
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "ElasticSearch:"
                             }), (0, Kr.jsxs)("td", {
-                                children: [l.get("portal.elasticsearch") ? (0, Kr.jsx)(Kr.Fragment, {
-                                    children: l.get("portal.elasticsearch")
+                                children: [c.get("portal.elasticsearch") ? (0, Kr.jsx)(Kr.Fragment, {
+                                    children: c.get("portal.elasticsearch")
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
-                                }), (null === (t = l.data) || void 0 === t || null === (n = t.foursight) || void 0 === n || null === (r = n.versions) || void 0 === r ? void 0 : r.elasticsearch_server) && (0, Kr.jsxs)(Kr.Fragment, {
+                                }), (null === (t = c.data) || void 0 === t || null === (n = t.foursight) || void 0 === n || null === (r = n.versions) || void 0 === r ? void 0 : r.elasticsearch_server) && (0, Kr.jsxs)(Kr.Fragment, {
                                     children: ["\xa0(", (0, Kr.jsx)("b", {
-                                        children: null === (o = l.data) || void 0 === o || null === (i = o.foursight) || void 0 === i || null === (a = i.versions) || void 0 === a ? void 0 : a.elasticsearch_server
+                                        children: null === (o = c.data) || void 0 === o || null === (i = o.foursight) || void 0 === i || null === (a = i.versions) || void 0 === a ? void 0 : a.elasticsearch_server
                                     }), ")"]
                                 })]
                             })]
                         }), (0, Kr.jsxs)("tr", {
                             style: {
                                 fontSize: "small"
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "Database:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("portal.health.database") ? (0, Kr.jsx)(Kr.Fragment, {
-                                    children: l.get("portal.health.database")
+                                children: c.get("portal.health.database") ? (0, Kr.jsx)(Kr.Fragment, {
+                                    children: c.get("portal.health.database")
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
                         }), (0, Kr.jsx)("tr", {
                             children: (0, Kr.jsx)("td", {
                                 style: {
@@ -50417,38 +50458,38 @@
                                 },
                                 children: "Identity:"
                             }), (0, Kr.jsx)("td", {
                                 style: {
                                     whiteSpace: "break-spaces",
                                     wordBreak: "break-all"
                                 },
-                                children: l.get("foursight.identity") ? (0, Kr.jsx)(Kr.Fragment, {
-                                    children: l.get("foursight.identity")
+                                children: c.get("foursight.identity") ? (0, Kr.jsx)(Kr.Fragment, {
+                                    children: c.get("foursight.identity")
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
                         }), (0, Kr.jsxs)("tr", {
                             style: {
                                 fontSize: "small"
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "Global Env Bucket:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("foursight.s3.global_env_bucket") ? (0, Kr.jsxs)(Kr.Fragment, {
-                                    children: [l.get("foursight.s3.global_env_bucket"), l.get("foursight.s3.bucket_org") && (0, Kr.jsxs)(Kr.Fragment, {
+                                children: c.get("foursight.s3.global_env_bucket") ? (0, Kr.jsxs)(Kr.Fragment, {
+                                    children: [c.get("foursight.s3.global_env_bucket"), c.get("foursight.s3.bucket_org") && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0(", (0, Kr.jsx)("span", {
-                                            id: "tooltip-bucket-org-".concat(l.get("foursight.aws_account_number")),
-                                            children: l.get("foursight.s3.bucket_org")
+                                            id: "tooltip-bucket-org-".concat(c.get("foursight.aws_account_number")),
+                                            children: c.get("foursight.s3.bucket_org")
                                         }), ")", (0, Kr.jsx)(Mi, {
-                                            id: "tooltip-bucket-org-".concat(l.get("foursight.aws_account_number")),
-                                            text: "S3 Bucket Org: ".concat(l.get("foursight.s3.bucket_org")),
+                                            id: "tooltip-bucket-org-".concat(c.get("foursight.aws_account_number")),
+                                            text: "S3 Bucket Org: ".concat(c.get("foursight.s3.bucket_org")),
                                             position: "top"
                                         })]
                                     })]
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
@@ -50458,20 +50499,20 @@
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "Bucket Encryption Key ID:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("foursight.s3.encrypt_key_id") ? (0, Kr.jsxs)(Kr.Fragment, {
+                                children: c.get("foursight.s3.encrypt_key_id") ? (0, Kr.jsxs)(Kr.Fragment, {
                                     children: [(0, Kr.jsx)("span", {
-                                        id: "tooltip-encryption-key-".concat(l.get("foursight.aws_account_number")),
-                                        children: l.get("foursight.s3.encrypt_key_id")
+                                        id: "tooltip-encryption-key-".concat(c.get("foursight.aws_account_number")),
+                                        children: c.get("foursight.s3.encrypt_key_id")
                                     }), (0, Kr.jsx)(Mi, {
-                                        id: "tooltip-encryption-key-".concat(l.get("foursight.aws_account_number")),
+                                        id: "tooltip-encryption-key-".concat(c.get("foursight.aws_account_number")),
                                         text: "S3 Encryption Key ID",
                                         position: "top"
                                     })]
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: " \u2013 "
                                 })
                             })]
@@ -50481,15 +50522,15 @@
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "Stack Name:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("foursight.stack")
+                                children: c.get("foursight.stack")
                             })]
                         }), (0, Kr.jsx)("tr", {
                             children: (0, Kr.jsx)("td", {
                                 style: {
                                     paddingTop: "4pt"
                                 }
                             })
@@ -50512,24 +50553,24 @@
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "AWS Account:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("foursight.aws_account_number") ? (0, Kr.jsxs)(Kr.Fragment, {
+                                children: c.get("foursight.aws_account_number") ? (0, Kr.jsxs)(Kr.Fragment, {
                                     children: [(0, Kr.jsx)("b", {
-                                        children: l.get("foursight.aws_account_number")
-                                    }), l.get("foursight.aws_account_name") && (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: c.get("foursight.aws_account_number")
+                                    }), c.get("foursight.aws_account_name") && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0(", (0, Kr.jsx)("span", {
-                                            id: "tooltip-alias-".concat(l.get("foursight.aws_account_name"), "-").concat(null === l || void 0 === l || null === (s = l.data) || void 0 === s ? void 0 : s.stage),
-                                            children: l.get("foursight.aws_account_name")
+                                            id: "tooltip-alias-".concat(c.get("foursight.aws_account_name"), "-").concat(null === c || void 0 === c || null === (s = c.data) || void 0 === s ? void 0 : s.stage),
+                                            children: c.get("foursight.aws_account_name")
                                         }), ")", (0, Kr.jsx)(Mi, {
-                                            id: "tooltip-alias-".concat(l.get("foursight.aws_account_name"), "-").concat(null === l || void 0 === l || null === (u = l.data) || void 0 === u ? void 0 : u.stage),
-                                            text: "AWS Account Alias: ".concat(l.get("foursight.aws_account_name")),
+                                            id: "tooltip-alias-".concat(c.get("foursight.aws_account_name"), "-").concat(null === c || void 0 === c || null === (u = c.data) || void 0 === u ? void 0 : u.stage),
+                                            text: "AWS Account Alias: ".concat(c.get("foursight.aws_account_name")),
                                             position: "top"
                                         })]
                                     })]
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
@@ -50539,17 +50580,17 @@
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "Default Environment:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("foursight.default_env.name") ? (0, Kr.jsxs)(Kr.Fragment, {
-                                    children: [l.get("foursight.default_env.name"), l.get("foursight.env_count") > 1 && (0, Kr.jsxs)("span", {
-                                        children: ["\xa0(", l.get("foursight.env_count"), " total)"]
+                                children: c.get("foursight.default_env.name") ? (0, Kr.jsxs)(Kr.Fragment, {
+                                    children: [c.get("foursight.default_env.name"), c.get("foursight.env_count") > 1 && (0, Kr.jsxs)("span", {
+                                        children: ["\xa0(", c.get("foursight.env_count"), " total)"]
                                     })]
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
                         }), (0, Kr.jsxs)("tr", {
                             style: {
@@ -50557,17 +50598,17 @@
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "Auth0 Client ID:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("foursight.auth0_client") ? (0, Kr.jsx)(Kr.Fragment, {
-                                    children: l.get("foursight.auth0_client") && (0, Kr.jsx)(Kr.Fragment, {
-                                        children: l.get("foursight.auth0_client")
+                                children: c.get("foursight.auth0_client") ? (0, Kr.jsx)(Kr.Fragment, {
+                                    children: c.get("foursight.auth0_client") && (0, Kr.jsx)(Kr.Fragment, {
+                                        children: c.get("foursight.auth0_client")
                                     })
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
                         }), (0, Kr.jsxs)("tr", {
                             style: {
@@ -50575,22 +50616,34 @@
                             },
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     paddingRight: "10pt"
                                 },
                                 children: "reCAPTCHA Key ID:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("foursight.re_captcha_key") ? (0, Kr.jsx)(Kr.Fragment, {
-                                    children: l.get("foursight.re_captcha_key") && (0, Kr.jsx)(Kr.Fragment, {
-                                        children: l.get("foursight.re_captcha_key")
+                                children: c.get("foursight.re_captcha_key") ? (0, Kr.jsx)(Kr.Fragment, {
+                                    children: c.get("foursight.re_captcha_key") && (0, Kr.jsx)(Kr.Fragment, {
+                                        children: c.get("foursight.re_captcha_key")
                                     })
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: " \u2013 "
                                 })
                             })]
+                        }), ra(l, c) && (0, Kr.jsxs)("tr", {
+                            style: {
+                                fontSize: "small"
+                            },
+                            children: [(0, Kr.jsx)("td", {
+                                style: {
+                                    paddingRight: "10pt"
+                                },
+                                children: " Portal Access Key: "
+                            }), (0, Kr.jsxs)("td", {
+                                children: [" ", p.get("key"), " "]
+                            })]
                         }), (0, Kr.jsx)("tr", {
                             children: (0, Kr.jsx)("td", {
                                 style: {
                                     paddingTop: "4pt"
                                 }
                             })
                         }), (0, Kr.jsx)("tr", {
@@ -50614,18 +50667,18 @@
                                 style: {
                                     whiteSpace: "nowrap",
                                     paddingRight: "4pt",
                                     width: "10%"
                                 },
                                 children: "Foursight Deployed:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("foursight.deployed") ? (0, Kr.jsxs)(Kr.Fragment, {
+                                children: c.get("foursight.deployed") ? (0, Kr.jsxs)(Kr.Fragment, {
                                     children: [(0, Kr.jsx)("b", {
-                                        children: l.get("foursight.deployed")
-                                    }), " \u2013 ", Pr.Ago(l.get("foursight.deployed"))]
+                                        children: c.get("foursight.deployed")
+                                    }), " \u2013 ", Pr.Ago(c.get("foursight.deployed"))]
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
                         }), (0, Kr.jsxs)("tr", {
                             style: {
                                 fontSize: "small"
@@ -50633,27 +50686,27 @@
                             children: [(0, Kr.jsx)("td", {
                                 style: {
                                     whiteSpace: "nowrap",
                                     paddingRight: "4pt"
                                 },
                                 children: "Portal Deployed:"
                             }), (0, Kr.jsx)("td", {
-                                children: l.get("portal.started") ? (0, Kr.jsxs)(Kr.Fragment, {
+                                children: c.get("portal.started") ? (0, Kr.jsxs)(Kr.Fragment, {
                                     children: [(0, Kr.jsx)("b", {
-                                        children: l.get("portal.started")
-                                    }), " \u2013 ", Pr.Ago(l.get("portal.started"))]
+                                        children: c.get("portal.started")
+                                    }), " \u2013 ", Pr.Ago(c.get("portal.started"))]
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
                         })]
                     })
                 })
             },
-            oa = function(e) {
+            ia = function(e) {
                 var t = e.info;
                 return (0, Kr.jsx)("table", {
                     style: {
                         width: "100%",
                         margin: "0",
                         padding: "0"
                     },
@@ -50945,47 +50998,42 @@
                                     children: Fr.EmptySet
                                 })
                             })]
                         })]
                     })
                 })
             },
-            ia = function(e) {
+            aa = function(e) {
                 var n, r, o, i, a, s, u = e.account,
                     l = e.header,
                     c = e.foursightUrl,
                     d = e.all,
                     f = e.decrementAccountCount,
                     p = e.brighten,
                     h = Xi("/accounts_from_s3/".concat(u.id), {
                         onDone: function() {
                             return f()
                         },
                         cache: !0,
                         nofetch: !0
                     });
-
-                function g(e) {
-                    var t, n, r, o, i, a, s, u;
-                    return !st.IsNull(null === l || void 0 === l || null === (t = l.app) || void 0 === t || null === (n = t.credentials) || void 0 === n ? void 0 : n.aws_account_number) && !st.IsNull(null === e || void 0 === e || null === (r = e.data) || void 0 === r || null === (o = r.foursight) || void 0 === o ? void 0 : o.aws_account_number) && (null === l || void 0 === l || null === (i = l.app) || void 0 === i || null === (a = i.credentials) || void 0 === a ? void 0 : a.aws_account_number) === (null === e || void 0 === e || null === (s = e.data) || void 0 === s || null === (u = s.foursight) || void 0 === u ? void 0 : u.aws_account_number)
-                }
                 return (0, t.useEffect)((function() {
                     h.fetch()
-                }), []), d || g(h) ? (0, Kr.jsx)(Kr.Fragment, {
+                }), []), d || ra(l, h) ? (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
-                        className: function(e) {
-                            var t, n;
-                            return g(e) && (null === l || void 0 === l || null === (t = l.app) || void 0 === t ? void 0 : t.stage) === (null === e || void 0 === e || null === (n = e.data) || void 0 === n ? void 0 : n.stage)
-                        }(h) ? "box" : "box lighten",
+                        className: function(e, t) {
+                            var n, r;
+                            return ra(e, t) && (null === e || void 0 === e || null === (n = e.app) || void 0 === n ? void 0 : n.stage) === (null === t || void 0 === t || null === (r = t.data) || void 0 === r ? void 0 : r.stage)
+                        }(l, h) ? "box" : "box lighten",
                         style: {
                             marginTop: "4pt",
                             marginBottom: "8pt",
                             filter: p ? "brightness(1.1)" : ""
                         },
-                        children: [g(h) ? (0, Kr.jsxs)(Kr.Fragment, {
+                        children: [ra(l, h) ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("b", {
                                 id: "tooltip-current-".concat(u.name, "-").concat(null === h || void 0 === h || null === (n = h.data) || void 0 === n ? void 0 : n.stage),
                                 children: (null === (r = h.data) || void 0 === r ? void 0 : r.name) || u.name
                             }), (0, Kr.jsx)(Mi, {
                                 id: "tooltip-current-".concat(u.name, "-").concat(null === h || void 0 === h || null === (o = h.data) || void 0 === o ? void 0 : o.stage),
                                 text: "This is your current account: ".concat(h.get("foursight.aws_account_number")),
                                 position: "top"
@@ -51086,17 +51134,17 @@
                                     style: {
                                         verticalAlign: "top"
                                     },
                                     children: [(0, Kr.jsx)("td", {
                                         style: {
                                             width: "70%"
                                         },
-                                        children: (0, Kr.jsx)(ra, {
-                                            info: h,
+                                        children: (0, Kr.jsx)(oa, {
                                             header: l,
+                                            info: h,
                                             foursightUrl: c
                                         })
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             paddingLeft: "10pt",
                                             width: "12pt"
                                         }
@@ -51108,15 +51156,15 @@
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             width: "30%",
                                             paddingLeft: "12pt",
                                             textAlign: "top",
                                             verticalAlign: "top"
                                         },
-                                        children: (0, Kr.jsx)(oa, {
+                                        children: (0, Kr.jsx)(ia, {
                                             info: h,
                                             header: l
                                         })
                                     })]
                                 })
                             })
                         }), (null === (s = h.data) || void 0 === s ? void 0 : s.__showraw) && (0, Kr.jsxs)(Kr.Fragment, {
@@ -51133,15 +51181,15 @@
                                 },
                                 children: Bi.Format(h.data)
                             })]
                         })]
                     })
                 }) : null
             },
-            aa = function(e) {
+            sa = function(e) {
                 var n, r, o, i, s, u, l, c, d, f = e.header,
                     p = a(Re(), 2),
                     h = p[0],
                     g = p[1],
                     y = h.get("all"),
                     m = a((0, t.useState)("true" === (null === y || void 0 === y ? void 0 : y.toLowerCase()) || "1" === y), 2),
                     v = m[0],
@@ -51251,15 +51299,15 @@
                                     })]
                                 })
                             })]
                         })
                     }), b.length > 0 ? (0, Kr.jsxs)(Kr.Fragment, {
                         children: [null === b || void 0 === b ? void 0 : b.map((function(e, n) {
                             return (0, Kr.jsx)(t.Fragment, {
-                                children: (0, Kr.jsx)(ia, {
+                                children: (0, Kr.jsx)(aa, {
                                     account: e,
                                     header: f,
                                     all: v,
                                     decrementAccountCount: L,
                                     foursightUrl: e.foursight_url
                                 })
                             }, e.id)
@@ -51290,141 +51338,141 @@
                             }) : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "No accounts info found."
                             })
                         })
                     })]
                 })
             },
-            sa = function(e) {
+            ua = function(e) {
                 var t = ta();
                 return (0, Kr.jsx)("div", {
                     className: "container",
-                    children: (0, Kr.jsx)(aa, {
+                    children: (0, Kr.jsx)(sa, {
                         header: t
                     })
                 })
             },
-            ua = function() {
+            la = function() {
                 var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null,
                     t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
                     n = Zi(),
                     r = Vi();
 
                 function o(o, i) {
                     return Ki(e, t, o, i, (function() {}), (function() {}), (function() {}), (function() {}), (function() {}), n, r, !0)
                 }
                 return function(e, t) {
                     return Ji(o(e, t))
                 }
             },
-            la = {
+            ca = {
                 fontSize: "11pt",
                 verticalAlign: "top",
                 paddingBottom: "2pt",
                 paddingRight: "10pt",
                 whiteSpace: "nowrap"
             },
-            ca = Ye(Ye({}, la), {}, {
+            da = Ye(Ye({}, ca), {}, {
                 textAlign: "right"
             }),
-            da = function(e) {
+            fa = function(e) {
                 var t, n = e.cache,
-                    r = ua();
+                    r = la();
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("tr", {
                         children: [(0, Kr.jsx)("td", {
-                            style: la,
+                            style: ca,
                             children: n.name
                         }), (0, Kr.jsx)("td", {
-                            style: ca,
+                            style: da,
                             children: n.hits > 0 ? n.hits : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
-                            style: ca,
+                            style: da,
                             children: n.misses > 0 ? n.misses : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
-                            style: ca,
+                            style: da,
                             children: n.size > 0 ? n.size : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsxs)("td", {
-                            style: la,
+                            style: ca,
                             id: "tooltip-updated-".concat(n.name),
                             children: [(0, Kr.jsx)(Mi, {
                                 id: "tooltip-updated-".concat(n.name),
                                 position: "bottom",
                                 text: "Last time function was actually called."
                             }), n.updated || (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })]
                         }), (0, Kr.jsxs)("td", {
-                            style: ca,
+                            style: da,
                             id: "tooltip-duration-".concat(n.name),
                             children: [(0, Kr.jsx)(Mi, {
                                 id: "tooltip-duration-".concat(n.name),
                                 position: "bottom",
                                 text: "Duration of last actual function call."
                             }), n.duration ? (null === (t = n.duration) || void 0 === t ? void 0 : t.toFixed(1)) + " ms" : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })]
                         }), (0, Kr.jsx)("td", {
-                            style: ca,
+                            style: da,
                             children: n.maxsize >= Number.MAX_SAFE_INTEGER ? (0, Kr.jsx)(Kr.Fragment, {
                                 children: Fr[1 / 0]
                             }) : (0, Kr.jsx)(Kr.Fragment, {
                                 children: n.maxsize
                             })
                         }), (0, Kr.jsx)("td", {
-                            style: ca,
+                            style: da,
                             children: n.ttl || (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
-                            style: ca,
+                            style: da,
                             children: n.ttl_none || (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
-                            style: la,
+                            style: ca,
                             children: n.nocache_none ? (0, Kr.jsx)(Kr.Fragment, {
                                 children: "Yes"
                             }) : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
-                            style: la,
+                            style: ca,
                             children: n.nocache_other ? (0, Kr.jsx)(Kr.Fragment, {
                                 children: "Yes"
                             }) : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
-                            style: la,
+                            style: ca,
                             children: (0, Kr.jsx)("span", {
                                 onClick: function() {
                                     return t = n.name, r("//__functioncacheclear__?name=".concat(t)), void e.refresh();
                                     var t
                                 },
                                 className: "pointer",
                                 children: "Clear"
                             })
                         })]
                     })
                 })
             },
-            fa = function(e) {
+            pa = function(e) {
                 var n = Xi("//__functioncache__"),
-                    r = ua(),
+                    r = la(),
                     o = a((0, t.useState)(!1), 2),
                     i = o[0],
                     s = o[1],
-                    u = Ye(Ye({}, la), {}, {
+                    u = Ye(Ye({}, ca), {}, {
                         verticalAlign: "bottom",
                         fontWeight: "bold",
                         textDecoration: "underline"
                     });
 
                 function l() {
                     n.refresh()
@@ -51506,15 +51554,15 @@
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
                                         children: "Action"
                                     })]
                                 })
                             }), (0, Kr.jsx)("tbody", {
                                 children: n.map((function(e) {
-                                    return (0, Kr.jsx)(da, {
+                                    return (0, Kr.jsx)(fa, {
                                         cache: e,
                                         refresh: l
                                     }, e.name)
                                 }))
                             })]
                         }), i && (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)(ji, {
@@ -51529,15 +51577,15 @@
                                 },
                                 children: Tr.Format(n.data)
                             })]
                         })]
                     })]
                 })
             },
-            pa = function(e) {
+            ha = function(e) {
                 var t = e.columns,
                     n = e.list,
                     r = e.update,
                     o = e.refresh,
                     i = e.sort,
                     a = void 0 === i ? null : i,
                     s = e.state,
@@ -51735,15 +51783,15 @@
                                 },
                                 colSpan: "6"
                             })
                         })]
                     }), M]
                 })
             },
-            ha = function(e) {
+            ga = function(e) {
                 var n = pe().environ,
                     r = Xi(zt.Url("/aws/s3/buckets", n), {
                         initial: []
                     }),
                     o = Xi({
                         initial: []
                     }),
@@ -51951,15 +51999,15 @@
                                         style: {
                                             height: "1px",
                                             background: Ft.GetForegroundColor(),
                                             marginBottom: "1pt"
                                         }
                                     }), (0, Kr.jsxs)("table", {
                                         width: "100%",
-                                        children: [(0, Kr.jsxs)(pa, {
+                                        children: [(0, Kr.jsxs)(ha, {
                                             columns: [{
                                                 label: "Key",
                                                 key: "key"
                                             }, {
                                                 label: "Size",
                                                 key: "size",
                                                 align: "right"
@@ -52223,26 +52271,26 @@
                                     })]
                                 })
                             })
                         })
                     })
                 })
             },
-            ga = Fi((function() {
+            ya = Fi((function() {
                 return bt.IsReadOnlyMode()
             })),
-            ya = function() {
-                var e = a(Yi(ga), 2),
+            ma = function() {
+                var e = a(Yi(ya), 2),
                     t = e[0],
                     n = e[1];
                 return [t, function(e) {
                     n(e), bt.SetReadOnlyMode(e)
                 }]
             },
-            ma = {
+            va = {
                 FormatDateTime: function(e) {
                     var n = e.verbose,
                         r = void 0 !== n && n,
                         o = e.timezone,
                         i = void 0 === o || o,
                         s = a((0, t.useState)(new Date), 2),
                         u = s[0],
@@ -52292,143 +52340,143 @@
                                 id: "tooltip-timestamp-".concat(r || i),
                                 text: Pr.FormatDateTime(r || i)
                             })]
                         })
                     })
                 }
             },
-            va = ma;
-
-        function Ma(e) {
-            e.update()
-        }
+            Ma = va;
 
         function ba(e) {
             e.update()
         }
 
         function ja(e) {
             e.update()
         }
 
-        function wa(e, t) {
-            e.__showingResults = !1, Ma(t)
+        function wa(e) {
+            e.update()
         }
 
-        function xa(e, t, n) {
-            e.__showingResults = !0, Ma(n)
+        function xa(e, t) {
+            e.__showingResults = !1, ba(t)
         }
 
         function Na(e, t, n) {
-            Da(e, n) || (n.prepend(e), Ma(n))
+            e.__showingResults = !0, ba(n)
         }
 
         function Ia(e, t, n) {
+            Sa(e, n) || (n.prepend(e), ba(n))
+        }
+
+        function Da(e, t, n) {
             e.checks.map((function(e) {
-                return ka(e, n)
+                return Ca(e, n)
             }));
             var r = function(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     if (t.get(n).group === e.group) return n
                 }
                 return -1
             }(e, t);
             t.remove(r)
         }
 
-        function Da(e, t) {
+        function Sa(e, t) {
             for (var n = 0; n < t.length; n++) {
                 if (t.get(n).group === e.group) return !0
             }
             return !1
         }
 
-        function Sa(e) {
+        function La(e) {
             return null === e || void 0 === e ? void 0 : e.__showingResults
         }
 
-        function La(e) {
+        function ka(e) {
             Object.keys(e.kwargs).forEach((function(t) {
                 if (!st.IsBoolean(e.kwargs[t]) && !st.IsNonEmptyArray(e.kwargs[t])) {
                     var n = "".concat(e.name, ".").concat(t),
                         r = document.getElementById(n),
                         o = null === r || void 0 === r ? void 0 : r.value;
                     e.kwargs[t] = o
                 }
             }))
         }
 
-        function ka(e, t) {
+        function Ca(e, t) {
             if (e.__showingHistory) {
                 e.__showingHistory = !1;
                 var n = function(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         if (t.get(n).name === e.name) return n
                     }
                     return -1
                 }(e, t);
                 t.remove(n)
             }
         }
 
-        function Ca(e, t, n) {
+        function Ea(e, t, n) {
             ! function(e, t, n) {
-                e.__showingHistory ? ka(e, n) : Ea(e, t, n)
+                e.__showingHistory ? Ca(e, n) : _a(e, t, n)
             }(e, t, n)
         }
 
-        function Ea(e, t, n) {
+        function _a(e, t, n) {
             e.__showingHistory || (e.__showingHistory = !0, n.prepend(e))
         }
 
-        function _a(e, t, n, r, o) {
+        function Ta(e, t, n, r, o) {
             var i = e.kwargs,
                 a = Tr.Str(i),
                 s = btoa(a);
-            Aa(e, n), ja(n), e.__queueingCheckRun = !0, o({
+            Oa(e, n), wa(n), e.__queueingCheckRun = !0, o({
                     url: zt.Url("/checks/".concat(e.name, "/run?args=").concat(s), t),
                     onData: function(t) {
                         return e.__queueingCheckRun = !1, e.__queuedCheckRun = t.uuid, setTimeout((function() {
                             ! function(e) {
                                 e.__resultHistory && e.__resultHistory.refresh()
-                            }(e), ja(n)
+                            }(e), wa(n)
                         }), 4e3), t.uuid
                     }
                 }), e.__queuedCheckRun = null,
                 function(e, t) {
-                    e.showingCheckRunningBox = !0, ja(t)
-                }(e, n), Ea(e, 0, r)
+                    e.showingCheckRunningBox = !0, wa(t)
+                }(e, n), _a(e, 0, r)
         }
 
-        function Ta(e, t, n, r, o) {
+        function Aa(e, t, n, r, o) {
             var i, a = {
                     check_name: e.name,
                     called_by: null === (i = e.__result) || void 0 === i ? void 0 : i.get("uuid")
                 },
                 s = Tr.Str(a),
                 u = btoa(s);
-            Oa(e, r), ja(r), e.__queueingActionRun = !0, o({
+            za(e, r), wa(r), e.__queueingActionRun = !0, o({
                     url: zt.Url("/action/".concat(t, "/run?args=").concat(u), n),
                     onData: function(t) {
                         return e.__queueingActionRun = !1, e.__queuedActionRun = t.uuid, t.uuid
                     }
                 }), e.__queuedActionRun = null,
                 function(e, t) {
-                    e.__showingActionRunningBox = !0, ja(t)
+                    e.__showingActionRunningBox = !0, wa(t)
                 }(e, r)
         }
 
-        function Aa(e, t) {
-            e.showingCheckRunningBox = !1, ja(t)
+        function Oa(e, t) {
+            e.showingCheckRunningBox = !1, wa(t)
         }
 
-        function Oa(e, t) {
-            e.__showingActionRunningBox = !1, ja(t)
+        function za(e, t) {
+            e.__showingActionRunningBox = !1, wa(t)
         }
-        var za = function(e) {
+        var Ua = function(e) {
                 var t = e.groupList,
                     n = e.env,
                     r = e.historyList,
                     o = e.info,
                     i = e.toggleShowingChecksSearch;
                 return t.error ? (0, Kr.jsx)(xi, {
                     error: t.error,
@@ -52454,45 +52502,45 @@
                                 id: "tooltip-search",
                                 position: "right",
                                 shape: "squared",
                                 size: "small",
                                 text: "Click to search for checks."
                             })]
                         }), t.map((function(e, i) {
-                            return (0, Kr.jsx)(Ua, {
+                            return (0, Kr.jsx)(Pa, {
                                 group: e,
                                 env: n,
                                 groupList: t,
                                 historyList: r,
                                 info: o,
                                 style: {
                                     paddingBottom: "6pt"
                                 }
                             }, e.group)
                         }))]
                     }) : (0, Kr.jsx)(Kr.Fragment, {})
                 })
             },
-            Ua = function(e) {
+            Pa = function(e) {
                 var t, n = e.group,
                     r = e.groupList,
                     o = e.historyList,
                     i = e.env,
                     a = e.info,
                     s = e.style,
                     u = void 0 === s ? {} : s;
 
                 function l(e, t) {
                     c(e) ? function(e, t) {
                         e.map((function(e) {
-                            return e.__showingResults && wa(e, t)
+                            return e.__showingResults && xa(e, t)
                         }))
                     }(e, t) : function(e, t, n) {
                         e.map((function(e) {
-                            return !e.__showingResults && xa(e, 0, n)
+                            return !e.__showingResults && Na(e, 0, n)
                         }))
                     }(e, 0, t)
                 }
 
                 function c(e) {
                     for (var t = 0; t < (null === e || void 0 === e ? void 0 : e.length); t++)
                         if (e[t].__showingResults) return !0;
@@ -52526,15 +52574,15 @@
                                 })]
                             }), (0, Kr.jsx)("span", {
                                 style: {
                                     float: "right",
                                     cursor: "pointer"
                                 },
                                 onClick: function() {
-                                    Ia(n, r, o)
+                                    Da(n, r, o)
                                 },
                                 children: (0, Kr.jsx)("b", {
                                     children: Fr.X
                                 })
                             })]
                         }), (0, Kr.jsx)("div", {
                             style: {
@@ -52544,27 +52592,27 @@
                             return e.title > t.title ? 1 : e.title < t.title ? -1 : 0
                         })).map((function(e, t) {
                             return (0, Kr.jsxs)("div", {
                                 children: [t > 0 && (0, Kr.jsx)("div", {
                                     style: {
                                         marginBottom: "12px"
                                     }
-                                }), (0, Kr.jsx)(Pa, {
+                                }), (0, Kr.jsx)(Ra, {
                                     check: e,
                                     env: i,
                                     groupList: r,
                                     historyList: o,
                                     info: a
                                 })]
                             }, t)
                         }))]
                     })
                 })
             },
-            Pa = function(e) {
+            Ra = function(e) {
                 var n, r = e.check,
                     o = e.env,
                     i = e.groupList,
                     s = e.historyList,
                     u = e.info,
                     l = (0, t.useState)(!1);
 
@@ -52637,19 +52685,19 @@
                                         style: {
                                             verticalAlign: "top",
                                             width: "1%",
                                             cursor: "pointer"
                                         },
                                         onClick: function() {
                                             ! function(e, t, n) {
-                                                e.__showingResults ? wa(e, n) : (xa(e, 0, n), g(!0))
+                                                e.__showingResults ? xa(e, n) : (Na(e, 0, n), g(!0))
                                             }(r, 0, i)
                                         },
                                         children: (0, Kr.jsxs)("b", {
-                                            children: [Sa(r) ? (0, Kr.jsx)("small", {
+                                            children: [La(r) ? (0, Kr.jsx)("small", {
                                                 children: Fr.DownArrowHollow
                                             }) : (0, Kr.jsx)("small", {
                                                 children: Fr.RightArrowHollow
                                             }), "\xa0"]
                                         })
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
@@ -52664,15 +52712,15 @@
                                                     id: "tooltip-configure ".concat(r.name),
                                                     className: r.__configuringCheckRun ? "check-config-button" : "check-run-button",
                                                     style: {
                                                         marginTop: "-2pt",
                                                         float: "right"
                                                     },
                                                     onClick: function() {
-                                                        r.__configuringCheckRun ? (La(r), r.__configuringCheckRun = !1) : r.__configuringCheckRun = !0, ja(i), g(!0)
+                                                        r.__configuringCheckRun ? (ka(r), r.__configuringCheckRun = !1) : r.__configuringCheckRun = !0, wa(i), g(!0)
                                                     },
                                                     children: [(0, Kr.jsx)("span", {
                                                         style: {
                                                             fontSize: "small"
                                                         },
                                                         children: Fr.DownArrowFat
                                                     }), "\xa0Configure"]
@@ -52684,15 +52732,15 @@
                                             })
                                         }) : (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("div", {
                                                 style: {
                                                     marginLeft: "10pt",
                                                     float: "right"
                                                 },
-                                                children: (0, Kr.jsx)(Ya, {
+                                                children: (0, Kr.jsx)(Qa, {
                                                     check: r,
                                                     env: o,
                                                     groupList: i,
                                                     historyList: s,
                                                     style: {
                                                         marginTop: "-1pt"
                                                     }
@@ -52702,19 +52750,19 @@
                                             style: {
                                                 whiteSpace: "nowrap"
                                             },
                                             children: [(0, Kr.jsx)("u", {
                                                 id: "tooltip-check-info ".concat(r.name),
                                                 style: {
                                                     cursor: "pointer",
-                                                    fontWeight: Sa(r) ? "bold" : "normal",
+                                                    fontWeight: La(r) ? "bold" : "normal",
                                                     whiteSpace: "break-spaces"
                                                 },
                                                 onClick: function() {
-                                                    Ca(r, o, s)
+                                                    Ea(r, o, s)
                                                 },
                                                 children: (null === (n = r.title) || void 0 === n ? void 0 : n.length) > 70 ? r.title.substring(0, 69) + " ..." : r.title
                                             }), (0, Kr.jsx)(Mi, {
                                                 id: "tooltip-check-info ".concat(r.name),
                                                 text: "Check: ".concat(r.name, ". Module: ").concat(r.module, ".")
                                             }), r.__result.get("action") && (0, Kr.jsx)("u", {
                                                 children: l[0] ? (0, Kr.jsxs)(Kr.Fragment, {
@@ -52772,15 +52820,15 @@
                                                         height: "18"
                                                     })
                                                 }), (0, Kr.jsx)(Mi, {
                                                     id: "tooltip-view-source ".concat(r.name),
                                                     text: "Click to view source code for this check (in new tab)."
                                                 })]
                                             })]
-                                        }), (0, Kr.jsx)(Ra, {
+                                        }), (0, Kr.jsx)(Ba, {
                                             check: r,
                                             env: o,
                                             historyList: s
                                         }), Object.keys(null === r || void 0 === r ? void 0 : r.schedule).map((function(e, t) {
                                             var n, o;
                                             return (0, Kr.jsx)("div", {
                                                 children: it.HasValue(null === (n = r.schedule[e]) || void 0 === n ? void 0 : n.cron_description) ? (0, Kr.jsxs)("div", {
@@ -52802,42 +52850,42 @@
                                                     })]
                                                 }, t) : (0, Kr.jsx)("small", {
                                                     children: (0, Kr.jsx)("i", {
                                                         children: "Not scheduled."
                                                     })
                                                 })
                                             }, e)
-                                        })), (0, Kr.jsx)(Qa, {
+                                        })), (0, Kr.jsx)(Ga, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             historyList: s,
                                             update: function() {
-                                                return ja(i)
+                                                return wa(i)
                                             },
                                             showDependenciesBox: h,
                                             setShowDependenciesBox: g
-                                        }), (0, Kr.jsx)(Ga, {
+                                        }), (0, Kr.jsx)(Wa, {
                                             check: r,
                                             groupList: i,
                                             info: u
-                                        }), (0, Kr.jsx)(Ja, {
+                                        }), (0, Kr.jsx)(Ka, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             update: function() {
                                                 return i.update()
                                             },
                                             fetchResult: c,
                                             runActionAllowedState: l
-                                        }), (0, Kr.jsx)(Wa, {
+                                        }), (0, Kr.jsx)(Ha, {
                                             check: r,
                                             groupList: i,
                                             info: u
-                                        }), (0, Kr.jsx)(Ba, {
+                                        }), (0, Kr.jsx)(Fa, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             fetchResult: c,
                                             runActionAllowedState: l
                                         })]
                                     })]
@@ -52848,25 +52896,25 @@
                                     children: (0, Kr.jsx)("td", {})
                                 })]
                             })
                         })
                     })
                 })
             },
-            Ra = function(e) {
+            Ba = function(e) {
                 var t = e.check,
                     n = e.env,
                     r = e.historyList,
                     o = e.style;
                 return (0, Kr.jsxs)("span", {
                     style: Ye(Ye({}, o), {}, {
                         cursor: "pointer"
                     }),
                     onClick: function() {
-                        return Ca(t, n, r)
+                        return Ea(t, n, r)
                     },
                     children: [(0, Kr.jsx)("span", {
                         id: "tooltip-recent-history ".concat(t.name),
                         children: (0, Kr.jsx)("img", {
                             alt: "history",
                             onClick: function(e) {},
                             src: Ut.History(),
@@ -52880,15 +52928,15 @@
                         id: "tooltip-recent-history ".concat(t.name),
                         text: "Click to " + (t.__showingHistory ? "hide" : "show") + " recent history of check runs."
                     }), t.__showingHistory ? (0, Kr.jsx)("span", {
                         children: Fr.RightArrow
                     }) : (0, Kr.jsx)(Kr.Fragment, {})]
                 })
             },
-            Ba = function(e) {
+            Fa = function(e) {
                 var n, r, o, i = e.check,
                     s = e.env,
                     u = e.groupList,
                     l = e.fetchResult,
                     c = (e.runActionAllowedState, a((0, t.useState)(!1), 2)),
                     d = c[0],
                     f = c[1],
@@ -52905,15 +52953,15 @@
                 }
 
                 function v(e, t) {
                     f(!1), g(!0)
                 }
 
                 function M(e, t) {
-                    e.__showingResultDetails = !e.__showingResultDetails, ba(t)
+                    e.__showingResultDetails = !e.__showingResultDetails, ja(t)
                 }
                 var b = function(e) {
                     var t, n = e.check,
                         r = e.env,
                         o = (e.checkUuid, e.groupList);
                     return t = d ? n.__resultByUuid.loading ? "Fetching latest result: ".concat(n.__result.get("uuid")) : "Click to fetch latest result: ".concat(n.__result.get("uuid")) : n.__result.loading ? "Fetching latest result." : "Click to fetch latest result.", (0, Kr.jsxs)("span", {
                         style: {
@@ -53220,24 +53268,24 @@
                             })]
                         })
                     }), i.__showingResultDetails && (!i.__result.empty || !i.__resultByUuid.empty || !i.__resultByAction.empty) && (0, Kr.jsxs)(Kr.Fragment, {
                         children: [(0, Kr.jsx)("div", {
                             style: {
                                 height: "2pt"
                             }
-                        }), (0, Kr.jsx)(Fa, {
+                        }), (0, Kr.jsx)(Ya, {
                             check: i,
                             groupList: u,
                             showResultByUuid: d,
                             showResultByAction: h
                         })]
                     })]
                 })
             },
-            Fa = function(e) {
+            Ya = function(e) {
                 var t, n = e.check,
                     r = e.groupList,
                     o = e.showResultByUuid,
                     i = e.showResultByAction;
                 e.style;
                 return n.__showingResults ? o ? (0, Kr.jsxs)("pre", {
                     className: "box lighten",
@@ -53278,15 +53326,15 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, ba(r)
+                                n.__showingResultDetails = !1, ja(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {
                             condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                             color: Ft.GetForegroundColor(),
@@ -53334,15 +53382,15 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, ba(r)
+                                n.__showingResultDetails = !1, ja(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {
                             condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                             color: Ft.GetForegroundColor(),
@@ -53391,30 +53439,30 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "x-large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.showingResultDetailsFull = !n.showingResultDetailsFull, ba(r)
+                                n.showingResultDetailsFull = !n.showingResultDetailsFull, ja(r)
                             },
                             children: n.showingResultDetailsFull ? (0, Kr.jsx)("span", {
                                 title: "Show full result output.",
                                 children: Fr.UpArrow
                             }) : (0, Kr.jsx)("span", {
                                 children: Fr.DownArrow
                             })
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, ba(r)
+                                n.__showingResultDetails = !1, ja(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(no, {
                         condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                         color: Ft.GetForegroundColor(),
                         label: "Loading latest result "
@@ -53422,22 +53470,22 @@
                         style: {
                             marginTop: "1pt"
                         },
                         children: "No result."
                     }) : Bi.Format(n.showingResultDetailsFull ? n.__result.get("full_output") : n.__result.get())]
                 }) : (0, Kr.jsx)(Kr.Fragment, {})
             },
-            Ya = function(e) {
+            Qa = function(e) {
                 var t = e.check,
                     n = e.env,
                     r = e.groupList,
                     o = e.historyList,
                     i = e.style,
-                    s = a(ya(), 1)[0],
-                    u = ua();
+                    s = a(ma(), 1)[0],
+                    u = la();
                 if (t.__queueingCheckRun) return t.__queueingCheckRun && (0, Kr.jsxs)("div", {
                     className: "check-run-wait-button",
                     style: i,
                     children: [(0, Kr.jsx)("span", {
                         id: "tooltip-queueing",
                         children: (0, Kr.jsx)("i", {
                             children: "Queueing"
@@ -53458,15 +53506,15 @@
                         className: "check-run-button" + (t.__configuringCheckRun, ""),
                         style: Ye(Ye({}, i), {}, {
                             cursor: s && t.__configuringCheckRun ? "not-allowed" : "",
                             background: s && t.__configuringCheckRun ? "#888888" : "",
                             color: t.__configuringCheckRun ? "yellow" : ""
                         }),
                         onClick: function(e) {
-                            t.__configuringCheckRun ? s || (La(t), _a(t, n, r, o, u)) : (t.__configuringCheckRun = !0, ja(r))
+                            t.__configuringCheckRun ? s || (ka(t), Ta(t, n, r, o, u)) : (t.__configuringCheckRun = !0, wa(r))
                         },
                         children: (0, Kr.jsx)("span", {
                             children: s ? (0, Kr.jsx)(Kr.Fragment, {
                                 children: t.__configuringCheckRun ? (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsxs)("span", {
                                         style: {
                                             fontSize: "",
@@ -53503,15 +53551,15 @@
                                     })
                                 })
                             })
                         })
                     })]
                 })
             },
-            Qa = function(e) {
+            Ga = function(e) {
                 var n = e.check,
                     r = e.env,
                     o = e.groupList,
                     i = e.historyList,
                     a = (e.update, e.showDependenciesBox),
                     s = e.setShowDependenciesBox;
 
@@ -53608,15 +53656,15 @@
                         },
                         children: st.IsNonEmptyObject(n.kwargs) ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     marginTop: "-2pt",
                                     float: "right"
                                 },
-                                children: (0, Kr.jsx)(Ya, {
+                                children: (0, Kr.jsx)(Qa, {
                                     check: n,
                                     env: r,
                                     groupList: o,
                                     historyList: i,
                                     style: {
                                         float: "right"
                                     }
@@ -53647,15 +53695,15 @@
                                                     defaultValue: n.kwargs[e] ? "true" : "false",
                                                     style: {
                                                         background: "lightyellow",
                                                         border: "1px solid lightgray",
                                                         borderRadius: "4pt"
                                                     },
                                                     onChange: function(t) {
-                                                        n.kwargs[e] = "true" === t.target.value, ja(o)
+                                                        n.kwargs[e] = "true" === t.target.value, wa(o)
                                                     },
                                                     children: (n.kwargs[e], (0, Kr.jsxs)(Kr.Fragment, {
                                                         children: [(0, Kr.jsx)("option", {
                                                             children: "true"
                                                         }), (0, Kr.jsx)("option", {
                                                             children: "false"
                                                         })]
@@ -53663,28 +53711,28 @@
                                                 }), st.IsNonEmptyArray(n.kwargs[e]) && (0, Kr.jsx)("select", {
                                                     defaultValue: null === (t = n.kwargs[e]) || void 0 === t ? void 0 : t.__selected,
                                                     style: {
                                                         background: "lightyellow",
                                                         border: "1px solid lightgray"
                                                     },
                                                     onChange: function(t) {
-                                                        n.kwargs[e].__selected = t.target.value, ja(o)
+                                                        n.kwargs[e].__selected = t.target.value, wa(o)
                                                     },
                                                     children: n.kwargs[e].map((function(e) {
                                                         return (0, Kr.jsx)("option", {
                                                             children: e
                                                         }, Dr()())
                                                     }))
                                                 }, Dr()()), !st.IsBoolean(n.kwargs[e]) && !st.IsNonEmptyArray(n.kwargs[e]) && (0, Kr.jsx)(Kr.Fragment, {
                                                     children: (0, Kr.jsx)("input", {
                                                         id: "".concat(n.name, ".").concat(e),
                                                         defaultValue: n.kwargs[e],
                                                         placeholder: "Empty",
                                                         onBlur: function() {
-                                                            La(n)
+                                                            ka(n)
                                                         },
                                                         style: {
                                                             marginLeft: "0pt",
                                                             height: "14pt",
                                                             background: "lightyellow",
                                                             border: "1px solid lightgray",
                                                             borderRadius: "2pt"
@@ -53698,29 +53746,29 @@
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     marginTop: "-3pt",
                                     float: "right"
                                 },
-                                children: (0, Kr.jsx)(Ya, {
+                                children: (0, Kr.jsx)(Qa, {
                                     check: n,
                                     env: r,
                                     groupList: o,
                                     historyList: i,
                                     style: {
                                         float: "right"
                                     }
                                 })
                             }), "No arguments."]
                         })
                     })]
                 })
             },
-            Ga = function(e) {
+            Wa = function(e) {
                 var n = e.check,
                     r = e.groupList,
                     o = e.info,
                     i = a((0, t.useState)(!1), 2),
                     s = i[0],
                     u = i[1];
                 return n.showingCheckRunningBox && n.__configuringCheckRun ? (0, Kr.jsx)("div", {
@@ -53798,15 +53846,15 @@
                                 }), (0, Kr.jsxs)("div", {
                                     style: {
                                         float: "right",
                                         marginTop: "-0pt",
                                         cursor: "pointer"
                                     },
                                     onClick: function() {
-                                        Aa(n, r)
+                                        Oa(n, r)
                                     },
                                     children: ["\xa0", (0, Kr.jsx)("b", {
                                         children: Fr.X
                                     }), "\xa0"]
                                 })]
                             })
                         }), !n.__queuedCheckRun && (0, Kr.jsx)("div", {
@@ -53818,15 +53866,15 @@
                                 label: " Queueing check run",
                                 color: "darkred"
                             })
                         })]
                     })
                 }) : (0, Kr.jsx)("span", {})
             },
-            Wa = function(e) {
+            Ha = function(e) {
                 var n = e.check,
                     r = e.groupList,
                     o = e.info,
                     i = a((0, t.useState)(!1), 2),
                     s = i[0],
                     u = i[1];
                 return n.__showingActionRunningBox && n.__configuringCheckRun ? (0, Kr.jsx)("div", {
@@ -53905,15 +53953,15 @@
                                 }), (0, Kr.jsxs)("div", {
                                     style: {
                                         float: "right",
                                         marginTop: "-0pt",
                                         cursor: "pointer"
                                     },
                                     onClick: function() {
-                                        Oa(n, r)
+                                        za(n, r)
                                     },
                                     children: ["\xa0", Fr.X]
                                 })]
                             })
                         }), !n.__queuedActionRun && (0, Kr.jsx)("div", {
                             style: {
                                 marginTop: "-2pt"
@@ -53923,15 +53971,15 @@
                                 label: " Queueing action run",
                                 color: "darkred"
                             })
                         })]
                     })
                 }) : (0, Kr.jsx)("span", {})
             },
-            Ha = function(e) {
+            Za = function(e) {
                 var t = e.env,
                     n = e.historyList;
                 if (n.error) return (0, Kr.jsx)(xi, {
                     error: n.error,
                     message: "Error loading check history from Foursight API"
                 });
                 var r = n.filter((function(e) {
@@ -53944,24 +53992,24 @@
                         },
                         children: "Recent Results"
                     }), null === r || void 0 === r ? void 0 : r.map((function(e, r) {
                         return (0, Kr.jsx)("div", {
                             style: {
                                 marginTop: "3pt"
                             },
-                            children: (0, Kr.jsx)(Za, {
+                            children: (0, Kr.jsx)(Va, {
                                 check: e,
                                 env: t,
                                 historyList: n
                             })
                         }, e.name)
                     }))]
                 })
             },
-            Za = function(e) {
+            Va = function(e) {
                 var n, r, o, i = e.check,
                     a = (e.env, e.historyList);
 
                 function s(e, t) {
                     e.__resultShowing = !1, e.__result = null, e.__resultLoading = !1, t.update()
                 }
 
@@ -54097,15 +54145,15 @@
                             })]
                         }), (0, Kr.jsxs)("span", {
                             style: {
                                 float: "right",
                                 cursor: "pointer"
                             },
                             onClick: function() {
-                                ka(i, a)
+                                Ca(i, a)
                             },
                             children: ["\xa0\xa0", (0, Kr.jsx)("b", {
                                 children: Fr.X
                             })]
                         })]
                     }), (0, Kr.jsx)("div", {
                         style: {
@@ -54113,15 +54161,15 @@
                         }
                     }), i.__showingHistory && (0, Kr.jsx)(Kr.Fragment, {
                         children: (null === (n = i.__resultHistory) || void 0 === n || null === (r = n.data) || void 0 === r || null === (o = r.list) || void 0 === o ? void 0 : o.length) > 0 ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsxs)("table", {
                                 style: {
                                     width: "100%"
                                 },
-                                children: [(0, Kr.jsx)(pa, {
+                                children: [(0, Kr.jsx)(ha, {
                                     loading: i.__resultHistory.loading,
                                     columns: h,
                                     list: i.__resultHistory.data.list,
                                     refresh: y,
                                     update: function(e) {
                                         return a.update()
                                     },
@@ -54342,15 +54390,15 @@
                                     })
                                 })
                             })
                         })
                     })]
                 })
             },
-            Va = function(e) {
+            qa = function(e) {
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: ["\xa0", (0, Kr.jsxs)("span", {
                         style: {
                             fontWeight: e.showingChecksSearch ? "bold" : "normal"
                         },
                         onClick: e.toggleShowingChecksSearch,
                         children: [(0, Kr.jsx)("span", {
@@ -54368,15 +54416,15 @@
                             },
                             src: Ut.NewIcon(),
                             height: "42"
                         })]
                     }), " ", (0, Kr.jsx)("br", {})]
                 })
             },
-            qa = function(e) {
+            Ja = function(e) {
                 var n = a((0, t.useState)(""), 2),
                     r = n[0],
                     o = n[1],
                     i = a((0, t.useState)([]), 2),
                     s = i[0],
                     l = i[1];
                 (0, t.useEffect)((function() {
@@ -54563,32 +54611,32 @@
                                     children: "No results."
                                 })
                             })]
                         })
                     })]
                 })
             },
-            Ja = function(e) {
+            Ka = function(e) {
                 var n, r = e.check,
                     o = e.env,
                     i = e.groupList,
                     s = e.fetchResult,
                     u = e.runActionAllowedState,
                     l = a((0, t.useState)(!1), 2),
                     c = l[0],
                     d = l[1],
-                    f = a(ya(), 1)[0],
-                    p = ua();
+                    f = a(ma(), 1)[0],
+                    p = la();
 
                 function h() {
                     if (c) {
                         var e;
                         d(!1);
                         var t = null === (e = r.__result) || void 0 === e ? void 0 : e.get("action");
-                        t && (Ta(r, t, o, i, p), u[1](!1))
+                        t && (Aa(r, t, o, i, p), u[1](!1))
                     } else d(!0)
                 }
                 return (0, t.useEffect)((function() {
                     d(!1)
                 }), []), (0, Kr.jsx)(Kr.Fragment, {
                     children: r.__configuringCheckRun && (null === (n = r.__result) || void 0 === n ? void 0 : n.get("action")) && (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsxs)("div", {
@@ -54740,15 +54788,15 @@
                                     })]
                                 })]
                             })]
                         })
                     })
                 })
             },
-            Ka = function(e) {
+            Xa = function(e) {
                 var n = pe().environ,
                     r = Xi({
                         initial: []
                     }),
                     o = Xi({
                         initial: []
                     }),
@@ -54759,15 +54807,15 @@
                 var c = Xi({
                         url: zt.Url("/checks/grouped/schedule", n),
                         nofetch: !0,
                         cache: !0,
                         onData: function(e) {
                             return e.sort((function(e, t) {
                                 return e.group > t.group ? 1 : e.group < t.group ? -1 : 0
-                            })), e.length > 0 && Na(function(e) {
+                            })), e.length > 0 && Ia(function(e) {
                                 for (var t = null, n = 0; n < (null === e || void 0 === e ? void 0 : e.length); n++) {
                                     var r, o;
                                     (!t || (null === (r = e[n]) || void 0 === r || null === (o = r.checks) || void 0 === o ? void 0 : o.length) < t.checks.length) && (t = e[n])
                                 }
                                 return t
                             }(e), 0, o), e
                         }
@@ -54787,15 +54835,15 @@
                 var f = Xi();
 
                 function p() {
                     f.refresh(zt.Url("/checks_status", n))
                 }
 
                 function h(e, t, n, r) {
-                    Da(e, n) ? Ia(e, n, r) : Na(e, 0, n)
+                    Sa(e, n) ? Da(e, n, r) : Ia(e, 0, n)
                 }
 
                 function g() {
                     l(!u), o.update([])
                 }
                 var y = function(e) {
                         e.props;
@@ -54912,15 +54960,15 @@
                                 },
                                 children: c.map((function(e, t) {
                                     var n;
                                     return (0, Kr.jsxs)("div", {
                                         children: [(0, Kr.jsxs)("span", {
                                             id: "tooltip-group-count-".concat(t),
                                             style: {
-                                                fontWeight: Da(e, o) ? "bold" : "normal",
+                                                fontWeight: Sa(e, o) ? "bold" : "normal",
                                                 cursor: "pointer"
                                             },
                                             onClick: function() {
                                                 return h(e, 0, o, r)
                                             },
                                             children: [e.group.replace(/ checks$/i, ""), " \xa0", (0, Kr.jsxs)("small", {
                                                 children: ["(", e.checks.length, ")"]
@@ -55150,15 +55198,15 @@
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Most Recent"
                                             }), ":\xa0"]
                                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Top"
                                             }), ":\xa0"]
-                                        }), (0, Kr.jsx)(va.FormatDuration, {
+                                        }), (0, Kr.jsx)(Ma.FormatDuration, {
                                             start: null === C || void 0 === C || null === (u = C.data[0]) || void 0 === u ? void 0 : u.timestamp,
                                             verbose: !0,
                                             fallback: "just now",
                                             suffix: "ago",
                                             tooltip: !0
                                         })]
                                     }), (0, Kr.jsx)("b", {
@@ -55170,15 +55218,15 @@
                                         onClick: O,
                                         children: Fr.X
                                     }), (0, Kr.jsxs)("table", {
                                         style: {
                                             width: "100%"
                                         },
                                         border: "0",
-                                        children: [(0, Kr.jsx)(pa, {
+                                        children: [(0, Kr.jsx)(ha, {
                                             columns: [{
                                                 label: "__refresh"
                                             }, {
                                                 label: "Timestamp",
                                                 key: "timestamp"
                                             }, {
                                                 label: "Check",
@@ -55270,15 +55318,15 @@
                                                                 width: "45%"
                                                             },
                                                             children: [(0, Kr.jsx)("b", {
                                                                 style: {
                                                                     cursor: "pointer"
                                                                 },
                                                                 onClick: function() {
-                                                                    return Ca(P(e.check, e.group), n, r)
+                                                                    return Ea(P(e.check, e.group), n, r)
                                                                 },
                                                                 children: e.title
                                                             }), "\xa0\xa0", (0, Kr.jsxs)(Oe, {
                                                                 to: kr.Path("/checks/".concat(e.check, "/history")),
                                                                 rel: "noreferrer",
                                                                 target: "_blank",
                                                                 children: [(0, Kr.jsx)("small", {
@@ -55744,15 +55792,15 @@
                                                                             children: [(0, Kr.jsx)("b", {
                                                                                 id: "tooltip-lambda-check-".concat(e.check_name),
                                                                                 style: {
                                                                                     color: Ft.GetForegroundColor(),
                                                                                     cursor: "pointer"
                                                                                 },
                                                                                 onClick: function() {
-                                                                                    return Ca(P(e.check_name, e.check_group), n, r)
+                                                                                    return Ea(P(e.check_name, e.check_group), n, r)
                                                                                 },
                                                                                 children: e.check_title
                                                                             }), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("i", {
                                                                                 id: "tooltip-lambda-check-group-".concat(e.check_name),
                                                                                 style: {
                                                                                     color: Ft.GetForegroundColor(),
                                                                                     cursor: "pointer"
@@ -55835,60 +55883,60 @@
                                             }), (0, Kr.jsx)(N, {}), (0, Kr.jsx)("div", {
                                                 style: {
                                                     marginTop: "3pt",
                                                     marginBottom: "3pt",
                                                     height: "1px",
                                                     backgroundColor: "var(--box-fg)"
                                                 }
-                                            }), (0, Kr.jsx)(Va, {
+                                            }), (0, Kr.jsx)(qa, {
                                                 showingChecksSearch: D,
                                                 toggleShowingChecksSearch: L
                                             })]
                                         }), (0, Kr.jsx)(F, {}), (0, Kr.jsx)(H, {})]
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
                                             paddingLeft: "8pt",
                                             verticalAlign: "top"
                                         },
                                         children: [(0, Kr.jsx)(k, {
                                             info: i
-                                        }), (0, Kr.jsx)(za, {
+                                        }), (0, Kr.jsx)(Ua, {
                                             env: n,
                                             groupList: o,
                                             historyList: r,
                                             info: i,
                                             toggleShowingChecksSearch: L
                                         })]
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
                                             paddingLeft: (null === o || void 0 === o ? void 0 : o.length) > 0 || o.error || j() ? "8pt" : "0",
                                             verticalAlign: "top"
                                         },
-                                        children: [(0, Kr.jsx)(qa, {
+                                        children: [(0, Kr.jsx)(Ja, {
                                             checks: c,
                                             groupList: o,
                                             environ: n,
                                             findGroup: U,
                                             toggleShowGroup: h,
                                             showingChecksSearch: D,
                                             toggleShowingChecksSearch: L
-                                        }), (0, Kr.jsx)(Z, {}), (0, Kr.jsx)(B, {}), (0, Kr.jsx)(Ha, {
+                                        }), (0, Kr.jsx)(Z, {}), (0, Kr.jsx)(B, {}), (0, Kr.jsx)(Za, {
                                             env: n,
                                             historyList: r
                                         })]
                                     })]
                                 })
                             })
                         })
                     })
                 })
             },
-            Xa = __webpack_require__(8145),
-            $a = __webpack_require__.n(Xa),
-            es = function(e) {
+            $a = __webpack_require__(8145),
+            es = __webpack_require__.n($a),
+            ts = function(e) {
                 var t = e.pages,
                     n = e.page,
                     r = e.onChange,
                     o = e.refresh,
                     i = e.loading,
                     a = e.spinner;
                 return (0, Kr.jsx)("table", {
@@ -55903,15 +55951,15 @@
                                         style: {
                                             pointerEvents: i ? "none" : "",
                                             opacity: i ? "0.4" : "",
                                             fontSize: "8pt",
                                             fontWeight: "bold"
                                         },
                                         className: "pagination-control",
-                                        children: (0, Kr.jsx)($a(), {
+                                        children: (0, Kr.jsx)(es(), {
                                             nextLabel: "NEXT",
                                             onPageChange: r,
                                             pageRangeDisplayed: 2,
                                             initialPage: n,
                                             disableInitialCallback: !0,
                                             marginPagesDisplayed: 2,
                                             pageCount: t,
@@ -55966,23 +56014,23 @@
                                 })
                             })]
                         })
                     })
                 })
             };
 
-        function ts(e) {
+        function ns(e) {
             var t;
             return null === e || void 0 === e || null === (t = e.split("/")) || void 0 === t ? void 0 : t.reverse()[0]
         }
 
-        function ns(e) {
+        function rs(e) {
             return null === e || void 0 === e ? void 0 : e.substring(0, null === e || void 0 === e ? void 0 : e.lastIndexOf("/"))
         }
-        var rs = function(e) {
+        var os = function(e) {
                 var t = e.check,
                     n = e.checkInfo;
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "box",
                         children: (0, Kr.jsx)("table", {
                             children: (0, Kr.jsxs)("tbody", {
@@ -56097,16 +56145,16 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsxs)("td", {
                                         children: [(0, Kr.jsx)("b", {
                                             children: "Code"
                                         }), ":"]
                                     }), (0, Kr.jsxs)("td", {
-                                        children: [ts(n.get("file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                            children: ns(n.get("file"))
+                                        children: [ns(n.get("file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                            children: rs(n.get("file"))
                                         })]
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             paddingTop: "2px"
                                         }
@@ -56199,15 +56247,15 @@
                                     })]
                                 })]
                             })
                         })
                     })
                 })
             },
-            os = function(e) {
+            is = function(e) {
                 var n, r = e.check,
                     o = e.checkInfo;
 
                 function i(e) {
                     var t = e.get("schedule");
                     if (t) {
                         var n = Object.values(t);
@@ -56471,16 +56519,16 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsxs)("td", {
                                         children: [(0, Kr.jsx)("b", {
                                             children: "Code"
                                         }), ":"]
                                     }), (0, Kr.jsxs)("td", {
-                                        children: [ts(o.get("registered_file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                            children: ns(o.get("registered_file"))
+                                        children: [ns(o.get("registered_file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                            children: rs(o.get("registered_file"))
                                         })]
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             paddingTop: "3px"
                                         }
@@ -56687,16 +56735,16 @@
                                             style: {
                                                 paddingRight: "8pt"
                                             },
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Code"
                                             }), ":"]
                                         }), (0, Kr.jsxs)("td", {
-                                            children: [ts(o.get("registered_action.file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                                children: ns(o.get("registered_action.file"))
+                                            children: [ns(o.get("registered_action.file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                                children: rs(o.get("registered_action.file"))
                                             })]
                                         })]
                                     }), (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "3px"
                                             }
@@ -56796,15 +56844,15 @@
                                     })]
                                 })
                             })
                         })]
                     })]
                 })
             },
-            is = function(e) {
+            as = function(e) {
                 var n, r = pe(),
                     o = r.environ,
                     i = r.check,
                     s = a(Re(), 2),
                     u = s[0],
                     l = s[1],
                     c = a((0, t.useState)(parseInt(u.get("limit")) || 25), 2),
@@ -56961,15 +57009,15 @@
                             }
                         }), (null === (r = o.get("list")) || void 0 === r ? void 0 : r.length) > 0 ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsxs)("table", {
                                 style: {
                                     width: "100%"
                                 },
                                 className: "fg",
-                                children: [(0, Kr.jsx)(pa, {
+                                children: [(0, Kr.jsx)(ha, {
                                     columns: f,
                                     list: o.get("list"),
                                     state: {
                                         key: u,
                                         order: m.endsWith(".desc") ? -1 : 1
                                     },
                                     update: function(e, t) {
@@ -57217,15 +57265,15 @@
                                         },
                                         children: (0, Kr.jsx)("tbody", {
                                             children: (0, Kr.jsxs)("tr", {
                                                 children: [(0, Kr.jsx)("td", {
                                                     style: {
                                                         width: "90%"
                                                     },
-                                                    children: (0, Kr.jsx)(es, {
+                                                    children: (0, Kr.jsx)(ts, {
                                                         pages: x,
                                                         onChange: function(e) {
                                                             var t = e.selected * d % I.get("paging.total");
                                                             S(d, t, m)
                                                         },
                                                         refresh: function() {
                                                             return L(d, h, m)
@@ -57341,43 +57389,43 @@
                                     children: (0, Kr.jsx)(_, {
                                         history: I
                                     })
                                 }), (0, Kr.jsx)("td", {
                                     style: {
                                         verticalAlign: "top"
                                     },
-                                    children: "action" === D.get("type") ? (0, Kr.jsx)(rs, {
+                                    children: "action" === D.get("type") ? (0, Kr.jsx)(os, {
                                         check: i,
                                         checkInfo: D
-                                    }) : (0, Kr.jsx)(os, {
+                                    }) : (0, Kr.jsx)(is, {
                                         check: i,
                                         checkInfo: D
                                     })
                                 })]
                             })]
                         })
                     })
                 })
             },
-            as = function() {
+            ss = function() {
                 var e = a((0, t.useContext)(ea), 2),
                     n = (e[0], e[1]),
                     r = $i();
                 return function(e) {
                     return r.refresh(zt.Url("/header", e), {
                         onData: function(e) {
                             return n(e)
                         },
                         cache: !0
                     })
                 }
             },
-            ss = function(e) {
+            us = function(e) {
                 var t, n, r = ta(),
-                    o = as(),
+                    o = ss(),
                     i = Xi(Br.IsLoggedIn() ? zt.Url("/info") : null);
                 Ui.NoteLastUrl(r);
                 var a = fe();
 
                 function s() {
                     return At.IsKnown(At.Current(), r)
                 }
@@ -57712,15 +57760,15 @@
                             style: {
                                 marginTop: "8pt"
                             }
                         })]
                     })
                 })
             },
-            us = function(e) {
+            ls = function(e) {
                 var t = ta();
                 return t.loading ? null : (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("br", {}), (0, Kr.jsx)("table", {
                         width: "100%",
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
                                 style: {
@@ -57753,15 +57801,15 @@
                                 },
                                 children: (0, Kr.jsx)("td", {})
                             })]
                         })
                     })]
                 })
             },
-            ls = function(e) {
+            cs = function(e) {
                 var t = ta();
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "container",
                         id: "login_container",
                         children: (0, Kr.jsxs)("div", {
                             className: "boxstyle check-error",
@@ -57800,16 +57848,16 @@
                                     })
                                 }), " page."]
                             })]
                         })
                     })
                 })
             },
-            cs = function() {
-                var e = a(ya(), 2),
+            ds = function() {
+                var e = a(ma(), 2),
                     t = e[0],
                     n = e[1];
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("img", {
                         id: "tooltip-readonly",
                         alt: "lock",
                         src: t ? Ut.Lock() : Ut.Unlock(),
@@ -57823,74 +57871,74 @@
                     }), (0, Kr.jsx)(Mi, {
                         id: "tooltip-readonly",
                         position: "bottom",
                         text: "You are in ".concat(t ? "readonly" : "read/write", " mode. Click to enter ").concat(t ? "read/write" : "readonly", " mode.")
                     })]
                 })
             },
-            ds = function(e) {
+            fs = function(e) {
                 var t = e.header;
                 return (0, Kr.jsxs)(Kr.Fragment, {
-                    children: [(0, Kr.jsx)(fs, {
+                    children: [(0, Kr.jsx)(ps, {
                         header: t
-                    }), (0, Kr.jsx)(ps, {
+                    }), (0, Kr.jsx)(hs, {
                         header: t
                     })]
                 })
             },
-            fs = function() {
+            ps = function() {
                 a(Re(), 1)[0];
                 var e = Xi("/certificates");
                 if (e.loading) return (0, Kr.jsx)(Kr.Fragment, {});
                 var t = e.find((function(e) {
                     return "Portal" === e.name
                 }));
-                return t && t.expires_soon ? (0, Kr.jsxs)(hs, {
+                return t && t.expires_soon ? (0, Kr.jsxs)(gs, {
                     children: [(0, Kr.jsx)("b", {
                         children: "Warning: SSL certificate for associated Portal will expire soon"
                     }), "\xa0", Fr.RightArrow, "\xa0 ", t.expires_at, " \xa0", Fr.RightArrow, "\xa0", Pr.FromNow(t.expires_at, !0, !1), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                         to: kr.Path("/certificates"),
                         style: {
                             color: "inherit"
                         },
                         children: "View"
                     })]
                 }) : void 0
             },
-            ps = function(e) {
+            hs = function(e) {
                 e.header;
                 var t = Xi("/portal_access_key");
                 if (t.loading) return (0, Kr.jsx)(Kr.Fragment, {});
                 if (t) {
                     var n, r;
-                    if (null !== t && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.expires_soon) return (0, Kr.jsxs)(hs, {
+                    if (null !== t && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.expires_soon) return (0, Kr.jsxs)(gs, {
                         children: [(0, Kr.jsx)("b", {
                             children: "Warning: Access key for associated Portal will expire soon"
                         }), "\xa0", Fr.RightArrow, "\xa0 ", t.data.expires_at, " \xa0", Fr.RightArrow, "\xa0", Pr.FromNow(t.data.expires_at, !0, !1), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                             to: kr.Path("/portal_access_key"),
                             style: {
                                 color: "inherit"
                             },
                             children: "View"
                         })]
                     });
-                    if (null !== (r = t.data) && void 0 !== r && r.invalid) return (0, Kr.jsxs)(hs, {
+                    if (null !== (r = t.data) && void 0 !== r && r.invalid) return (0, Kr.jsxs)(gs, {
                         children: [(0, Kr.jsxs)("b", {
                             children: ["Warning: Access key for associated Portal ", t.data.expired ? "has expired" : "is invalid"]
                         }), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                             to: kr.Path("/portal_access_key"),
                             style: {
                                 color: "inherit"
                             },
                             children: "View"
                         })]
                     })
                 }
             },
-            hs = function(e) {
+            gs = function(e) {
                 var t = e.children;
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("tr", {
                         children: (0, Kr.jsx)("td", {
                             style: {
                                 background: "black",
                                 height: "2px"
@@ -57915,15 +57963,15 @@
                                 height: "1px"
                             },
                             colSpan: "3"
                         })
                     })]
                 })
             },
-            gs = function(e) {
+            ys = function(e) {
                 var t = e.header,
                     n = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10),
                     r = function(e) {
                         var t = e.path,
                             n = e.label;
                         return (0, Kr.jsx)(Kr.Fragment, {
                             children: kr.CurrentLogicalPath() === t ? (0, Kr.jsxs)("span", {
@@ -57997,15 +58045,15 @@
                                 path: "/login",
                                 label: Br.IsLoggedIn(t) ? "Session" : "Login"
                             })]
                         })]
                     })
                 })
             },
-            ys = function(e) {
+            ms = function(e) {
                 var t, n, r, o, i = e.header;
 
                 function a(e) {
                     return e ? {
                         textDecoration: "none",
                         color: "black",
                         fontWeight: "bold"
@@ -58081,29 +58129,29 @@
                     }), (0, Kr.jsx)(Mi, {
                         id: "tooltip-header-aws",
                         position: "bottom",
                         text: "Open AWS console for (".concat(null !== (n = i.app) && void 0 !== n && n.credentials.aws_account_name ? (null === (r = i.app) || void 0 === r ? void 0 : r.credentials.aws_account_name) + "/" : "").concat(null === (o = i.app) || void 0 === o ? void 0 : o.credentials.aws_account_number, ") account (in new tab).")
                     })]
                 })
             },
-            ms = function(e) {
+            vs = function(e) {
                 var t = e.header;
                 return (0, Kr.jsxs)("span", {
-                    children: [(0, Kr.jsx)(gs, {
+                    children: [(0, Kr.jsx)(ys, {
                         header: t
                     }), (0, Kr.jsx)(Kr.Fragment, {
                         children: "\xa0|\xa0"
-                    }), (0, Kr.jsx)(ys, {
+                    }), (0, Kr.jsx)(ms, {
                         header: t
                     })]
                 })
             },
-            vs = function(e) {
+            Ms = function(e) {
                 var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I, D, S, L, k = ta(),
-                    C = as(),
+                    C = ss(),
                     E = fe(),
                     _ = a(na(), 1)[0],
                     T = At.IsFoursightFourfront(k) ? "#14533C" : "#143C53",
                     A = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10);
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: k.loading ? (0, Kr.jsxs)("div", {
                         style: {
@@ -58384,15 +58432,15 @@
                                             style: {
                                                 paddingRight: "10pt",
                                                 whiteSpace: "nowrap",
                                                 color: "#D6EAF8"
                                             },
                                             align: "right",
                                             children: [(0, Kr.jsx)("small", {
-                                                children: (0, Kr.jsx)(va.FormatDateTime, {
+                                                children: (0, Kr.jsx)(Ma.FormatDateTime, {
                                                     verbose: !0,
                                                     timezone: !1
                                                 })
                                             }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, Kr.jsxs)(Kr.Fragment, {
                                                 children: ["\xa0|\xa0", (0, Kr.jsx)(Oe, {
                                                     id: "tooltip-header-account",
                                                     to: kr.Path("/login"),
@@ -58450,15 +58498,15 @@
                                             width: "49%",
                                             style: {
                                                 paddingLeft: "10pt",
                                                 paddingTop: "3pt",
                                                 paddingBottom: "3pt",
                                                 whiteSpace: "nowrap"
                                             },
-                                            children: (0, Kr.jsx)(ms, {
+                                            children: (0, Kr.jsx)(vs, {
                                                 header: k
                                             })
                                         }), (0, Kr.jsx)("td", {
                                             width: "2%",
                                             align: "center",
                                             style: {
                                                 whiteSpace: "nowrap",
@@ -58780,15 +58828,15 @@
                                                                 })]
                                                             })
                                                         })]
                                                     })
                                                 })
                                             })
                                         })]
-                                    }), (0, Kr.jsx)(ds, {
+                                    }), (0, Kr.jsx)(fs, {
                                         header: k
                                     }), (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 height: "1px",
                                                 background: "darkblue"
                                             }
@@ -58806,25 +58854,25 @@
                                 children: (0, Kr.jsx)("table", {
                                     children: (0, Kr.jsx)("tbody", {
                                         children: (0, Kr.jsx)("tr", {
                                             children: (0, Kr.jsx)("td", {
                                                 style: {
                                                     paddingLeft: "10pt"
                                                 },
-                                                children: (0, Kr.jsx)(cs, {})
+                                                children: (0, Kr.jsx)(ds, {})
                                             })
                                         })
                                     })
                                 })
                             })]
                         })]
                     })
                 })
             },
-            Ms = function(e) {
+            bs = function(e) {
                 var n = e.children,
                     r = a((0, t.useState)({
                         loading: !0
                     }), 2),
                     o = r[0],
                     i = r[1];
                 return Xi("/header", {
@@ -58840,15 +58888,15 @@
                     },
                     cache: !0
                 }), (0, Kr.jsx)(ea.Provider, {
                     value: [o, i],
                     children: n
                 })
             },
-            bs = function(e) {
+            js = function(e) {
                 var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w = ta(),
                     x = (At.IsFoursightFourfront(w) ? "foursight" : "foursight-cgap") + ": " + (null === w || void 0 === w || null === (n = w.versions) || void 0 === n ? void 0 : n.foursight_core) + " | foursight-core: " + (null === w || void 0 === w || null === (r = w.versions) || void 0 === r ? void 0 : r.foursight) + " | dcicutils: " + (null === w || void 0 === w || null === (o = w.versions) || void 0 === o ? void 0 : o.dcicutils),
                     N = {
                         id: "".concat(null === (i = w.app) || void 0 === i || null === (s = i.credentials) || void 0 === s ? void 0 : s.aws_account_name, ":").concat(null === w || void 0 === w || null === (u = w.app) || void 0 === u ? void 0 : u.stage),
                         name: null === (l = w.app) || void 0 === l || null === (c = l.credentials) || void 0 === c ? void 0 : c.aws_account_name,
                         stage: null === (d = w.app) || void 0 === d ? void 0 : d.stage
                     },
@@ -58955,15 +59003,15 @@
                                 top: "4pt",
                                 bottom: "10pt"
                             }), D && (0, Kr.jsx)(Kr.Fragment, {
                                 children: (0, Kr.jsx)("div", {
                                     style: {
                                         marginBottom: "12pt"
                                     },
-                                    children: (0, Kr.jsx)(ia, {
+                                    children: (0, Kr.jsx)(aa, {
                                         account: N,
                                         header: w,
                                         decrementAccountCount: function() {},
                                         all: !0,
                                         brighten: !0
                                     })
                                 })
@@ -59123,15 +59171,15 @@
                                     }
                                 })]
                             })
                         })]
                     })
                 })
             },
-            js = function(e) {
+            ws = function(e) {
                 var n = e.title,
                     r = e.show,
                     o = void 0 === r || r,
                     i = e.info,
                     s = e.children,
                     u = a((0, t.useState)(o), 2),
                     l = u[0],
@@ -59220,15 +59268,15 @@
                                     children: "show"
                                 }), "."]
                             })]
                         })
                     })
                 })
             },
-            ws = function(e) {
+            xs = function(e) {
                 var t = e.name,
                     n = e.value,
                     r = e.monospace,
                     o = void 0 !== r && r,
                     i = e.copy,
                     a = void 0 === i || i,
                     s = e.size,
@@ -59385,257 +59433,257 @@
                                     })]
                                 }), E]
                             }))]
                         }) : (0, Kr.jsx)("span", {})
                     })
                 })
             },
-            xs = function() {
+            Ns = function() {
                 var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R = ta(),
                     B = Xi("/info"),
                     F = a((0, t.useState)(!1), 2),
                     Y = F[0],
                     Q = F[1],
                     G = a((0, t.useState)(!1), 2),
                     W = G[0],
                     H = G[1],
                     Z = a((0, t.useState)(!1), 2),
                     V = Z[0],
                     q = Z[1],
                     J = Xi("/portal_access_key"),
-                    K = ua();
+                    K = la();
                 return B.error ? (0, Kr.jsx)(xi, {
                     error: B.error,
                     message: "Error loading info from Foursight API"
                 }) : (0, Kr.jsxs)("div", {
                     className: "container",
-                    children: [(0, Kr.jsxs)(js, {
+                    children: [(0, Kr.jsxs)(ws, {
                         info: B,
                         title: "Versions",
-                        children: [(0, Kr.jsx)(ws, {
+                        children: [(0, Kr.jsx)(xs, {
                             name: null === (e = R.app) || void 0 === e ? void 0 : e.package,
                             value: null === (n = R.versions) || void 0 === n ? void 0 : n.foursight,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: At.IsFoursightFourfront(R) ? "4dn-dcic" : "dbmi-bgm",
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "foursight-core",
                             value: null === (r = R.versions) || void 0 === r ? void 0 : r.foursight_core,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "dcicutils",
                             value: null === (o = R.versions) || void 0 === o ? void 0 : o.dcicutils,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "tibanna",
                             value: null === (i = R.versions) || void 0 === i ? void 0 : i.tibanna,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "tibanna-ff",
                             value: null === (s = R.versions) || void 0 === s ? void 0 : s.tibanna_ff,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "chalice",
                             value: null === (u = R.versions) || void 0 === u ? void 0 : u.chalice,
                             monospace: !0,
                             copy: !0,
                             chalice: !0,
                             size: "2",
                             pypi: !0,
                             github: "aws"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "python",
                             value: null === (l = R.versions) || void 0 === l ? void 0 : l.python,
                             monospace: !0,
                             copy: !0,
                             python: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "elasticsearch-server",
                             value: (null === (c = R.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = B.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             elasticsearch: !0
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "elasticsearch",
                             value: null === (p = R.versions) || void 0 === p ? void 0 : p.elasticsearch,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "elasticsearch-dsl",
                             value: null === (h = R.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         })]
-                    }), (0, Kr.jsxs)(js, {
+                    }), (0, Kr.jsxs)(ws, {
                         info: B,
                         title: "Credentials Info",
-                        children: [(0, Kr.jsx)(ws, {
+                        children: [(0, Kr.jsx)(xs, {
                             name: "AWS Account Number",
                             value: B.get("app.credentials.aws_account_number"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "AWS Region Name",
                             value: B.get("app.credentials.aws_region"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "AWS User ARN",
                             value: B.get("app.credentials.aws_user_arn"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "AWS Access Key ID",
                             value: B.get("app.credentials.aws_access_key_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), B.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(ws, {
+                        }), B.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(xs, {
                             name: "AWS S3 Access Key ID",
                             value: B.get("environ.S3_AWS_ACCESS_KEY_ID"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Portal Access Key",
                             value: J.get("key"),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             portalAccessKey: !0
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Auth0 Client ID",
                             value: B.get("app.credentials.auth0_client_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(js, {
+                    }), (0, Kr.jsxs)(ws, {
                         info: B,
                         title: "Resources",
-                        children: [(0, Kr.jsx)(ws, {
+                        children: [(0, Kr.jsx)(xs, {
                             name: "Foursight Server",
                             value: B.get("server.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Portal Server",
                             value: B.get("server.portal"),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             portalCertificate: !0
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "ElasticSearch Server",
                             value: B.get("server.es"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "RDS Server",
                             value: B.get("server.rds"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "SQS Server",
                             value: B.get("server.sqs"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(js, {
+                    }), (0, Kr.jsxs)(ws, {
                         info: B,
                         title: "Environment Names",
-                        children: [(0, Kr.jsx)(ws, {
+                        children: [(0, Kr.jsx)(xs, {
                             name: "Environment Name",
                             value: At.RegularName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Environment Name (Full)",
                             value: At.FullName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Environment Name (Short)",
                             value: At.ShortName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Environment Name (Public)",
                             value: At.PublicName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Environment Name (Foursight)",
                             value: At.FoursightName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Environment Name (Preferred)",
                             value: At.PreferredName(At.Current(R), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         })]
-                    }), (0, Kr.jsxs)(js, {
+                    }), (0, Kr.jsxs)(ws, {
                         info: B,
                         title: "Bucket Names",
-                        children: [(0, Kr.jsx)(ws, {
+                        children: [(0, Kr.jsx)(xs, {
                             name: "Global Environment Bucket",
                             value: B.get("buckets.env"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Foursight Bucket Name",
                             value: B.get("buckets.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Foursight Bucket Prefix",
                             value: B.get("buckets.foursight_prefix"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         })]
-                    }), (0, Kr.jsx)(js, {
+                    }), (0, Kr.jsx)(ws, {
                         info: B,
                         title: "Environment & Bucket Names",
                         children: (0, Kr.jsx)("pre", {
                             className: "box",
                             style: {
                                 border: "0",
                                 margin: "0",
@@ -59650,84 +59698,84 @@
                                         marginTop: "6px",
                                         marginBottom: "6px",
                                         background: "black"
                                     }
                                 }) : (0, Kr.jsx)("span", {})]
                             }, Dr()())
                         })
-                    }), (0, Kr.jsx)(js, {
+                    }), (0, Kr.jsx)(ws, {
                         info: B,
                         title: "Ecosystem",
                         show: !1,
                         children: (0, Kr.jsx)("pre", {
                             className: "box",
                             style: {
                                 border: "0",
                                 margin: "0",
                                 paddingTop: "8",
                                 paddingBottom: "8",
                                 marginTop: "0"
                             },
                             children: Bi.Format(B.get("buckets.ecosystem"))
                         })
-                    }), (0, Kr.jsxs)(js, {
+                    }), (0, Kr.jsxs)(ws, {
                         info: B,
                         title: "Authentication/Authorization Info",
                         show: !1,
-                        children: [(0, Kr.jsx)(ws, {
+                        children: [(0, Kr.jsx)(xs, {
                             name: "Email",
                             value: null === (y = Br.Token()) || void 0 === y ? void 0 : y.user,
                             monospace: !0,
                             copy: !0,
                             check: null === (m = Br.Token()) || void 0 === m ? void 0 : m.user_verified,
                             link: kr.Path("/users/" + Br.LoggedInUser(R), !0),
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "First Name",
                             value: null === (v = Br.Token()) || void 0 === v ? void 0 : v.first_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Last Name",
                             value: null === (M = Br.Token()) || void 0 === M ? void 0 : M.last_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Environments",
                             value: null === (b = Br.Token()) || void 0 === b ? void 0 : b.allowed_envs.join(", "),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Audience",
                             value: null === (j = Br.Token()) || void 0 === j ? void 0 : j.aud,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Issued At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
-                            value: (0, Kr.jsx)(va.FormatDuration, {
+                            value: (0, Kr.jsx)(Ma.FormatDuration, {
                                 start: null === (w = Br.Token()) || void 0 === w ? void 0 : w.authenticated_at,
                                 verbose: !0,
                                 fallback: "just now",
                                 suffix: "ago",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Expires At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
-                            value: (0, Kr.jsx)(va.FormatDuration, {
+                            value: (0, Kr.jsx)(Ma.FormatDuration, {
                                 end: null === (x = Br.Token()) || void 0 === x ? void 0 : x.authenticated_until,
                                 verbose: !0,
                                 fallback: "now",
                                 suffix: "from now",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
@@ -59792,70 +59840,70 @@
                                     children: [(0, Kr.jsx)("u", {
                                         children: "AuthToken"
                                     }), "\xa0", Fr.UpArrow]
                                 })
                             }), (0, Kr.jsx)("br", {})]
                         })]
                     }), B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Kr.jsx)(Kr.Fragment, {
-                        children: (0, Kr.jsxs)(js, {
+                        children: (0, Kr.jsxs)(ws, {
                             info: B,
                             title: "Logs",
-                            children: [(0, Kr.jsx)(ws, {
+                            children: [(0, Kr.jsx)(xs, {
                                 name: "Log Group",
                                 value: B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, Kr.jsx)(ws, {
+                            }), (0, Kr.jsx)(xs, {
                                 name: "Log Stream",
                                 value: B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
                                 monospace: !0,
                                 size: "2"
                             })]
                         })
-                    }), B.get("app.lambda") && (0, Kr.jsxs)(js, {
+                    }), B.get("app.lambda") && (0, Kr.jsxs)(ws, {
                         info: B,
                         title: "Lambda",
                         show: !1,
-                        children: [(0, Kr.jsx)(ws, {
+                        children: [(0, Kr.jsx)(xs, {
                             name: "Name",
                             value: B.get("app.lambda.lambda_name"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Function",
                             value: B.get("app.lambda.lambda_function_name"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "ARN",
                             value: B.get("app.lambda.lambda_function_arn"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "S3 Location",
                             value: B.get("app.lambda.lambda_code_s3_bucket") + "/" + B.get("app.lambda.lambda_code_s3_bucket_key"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Size",
                             value: B.get("app.lambda.lambda_code_size"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Modified",
                             value: Pr.FormatDateTime(B.get("app.lambda.lambda_modified")),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Role",
                             value: B.get("app.lambda.lambda_role"),
                             monospace: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(js, {
+                    }), (0, Kr.jsxs)(ws, {
                         info: B,
                         title: "Miscellany",
                         children: [V ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 id: "tooltip-info-reloading",
                                 style: {
                                     float: "right"
@@ -59909,128 +59957,128 @@
                                 }
                             })]
                         }), (0, Kr.jsx)(Mi, {
                             id: "tooltip-info-clear",
                             position: "bottom",
                             size: "small",
                             text: "Click to clear any server-side caches."
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "App Deployed At",
                             value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (N = R.app) || void 0 === N ? void 0 : N.deployed) + Pr.FormatDuration(null === (I = R.app) || void 0 === I ? void 0 : I.deployed, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             copy: !0,
                             optional: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "App Launched At",
                             value: (null === (D = R.app) || void 0 === D ? void 0 : D.launched) + Pr.FormatDuration(null === (S = R.app) || void 0 === S ? void 0 : S.launched, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Page Loaded At",
                             value: B.get("page.loaded") + Pr.FormatDuration(B.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Package",
                             value: null === (L = R.app) || void 0 === L ? void 0 : L.package,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Stage",
                             value: null === (k = R.app) || void 0 === k ? void 0 : k.stage,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Environment",
                             value: At.Current(),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Domain",
                             value: null === (C = R.app) || void 0 === C ? void 0 : C.domain,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Context",
                             value: null === (E = R.app) || void 0 === E ? void 0 : E.context,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Path",
                             value: B.get("page.path"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Endpoint",
                             value: B.get("page.endpoint"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Client (React UI)",
                             value: kr.BaseUrl(),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Server (React API)",
                             value: zt.BaseUrl(),
                             monospace: !0,
                             size: "2",
                             apiCache: !0
-                        }), (0, Kr.jsx)(ws, {
+                        }), (0, Kr.jsx)(xs, {
                             name: "Checks File",
                             value: null === (_ = B.data) || void 0 === _ || null === (T = _.checks) || void 0 === T ? void 0 : T.file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Kr.jsx)(ws, {
+                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Kr.jsx)(xs, {
                             name: "Accounts File",
                             value: null === (O = R.app) || void 0 === O ? void 0 : O.accounts_file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Kr.jsx)(ws, {
+                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Kr.jsx)(xs, {
                             name: "Accounts File (S3)",
                             value: null === (U = R.app) || void 0 === U ? void 0 : U.accounts_file_from_s3,
                             monospace: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsx)(js, {
+                    }), (0, Kr.jsx)(ws, {
                         info: B,
                         title: "GAC: ".concat(B.get("gac.name")),
                         show: !1,
                         children: B.get("gac.values") ? (0, Kr.jsx)("span", {
                             children: Object.keys(B.get("gac.values")).map((function(e) {
-                                return (0, Kr.jsx)(ws, {
+                                return (0, Kr.jsx)(xs, {
                                     name: e,
                                     value: B.get("gac.values")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
-                    }), (0, Kr.jsx)(js, {
+                    }), (0, Kr.jsx)(ws, {
                         info: B,
                         title: "Environment Variables",
                         show: !1,
                         children: B.get("environ") ? (0, Kr.jsx)("span", {
                             children: Object.keys(B.get("environ")).map((function(e) {
-                                return (0, Kr.jsx)(ws, {
+                                return (0, Kr.jsx)(xs, {
                                     name: e,
                                     value: B.get("environ")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
                     }), (null === (P = R.app) || void 0 === P ? void 0 : P.accounts) && (0, Kr.jsx)("div", {
                         className: "container",
                         style: {
                             marginTop: "4pt"
                         },
                         children: W ? (0, Kr.jsx)(Kr.Fragment, {
-                            children: (0, Kr.jsx)(aa, {})
+                            children: (0, Kr.jsx)(sa, {})
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("b", {
                                 onClick: function() {
                                     return H(!0)
                                 },
                                 style: {
                                     cursor: "pointer"
@@ -60056,40 +60104,40 @@
                                     children: "show"
                                 }), "."]
                             })]
                         })
                     })]
                 })
             },
-            Ns = function(e, t) {
-                return Ns = Object.setPrototypeOf || {
+            Is = function(e, t) {
+                return Is = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, Ns(e, t)
+                }, Is(e, t)
             };
 
-        function Is(e, t) {
+        function Ds(e, t) {
             function n() {
                 this.constructor = e
             }
-            Ns(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            Is(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         }
-        var Ds, Ss, Ls, ks = function() {
-            return ks = Object.assign || function(e) {
+        var Ss, Ls, ks, Cs = function() {
+            return Cs = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, ks.apply(this, arguments)
+            }, Cs.apply(this, arguments)
         };
 
-        function Cs(e, t, n, r) {
+        function Es(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60109,15 +60157,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Es(e, t) {
+        function _s(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60185,15 +60233,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function _s(e, t) {
+        function Ts(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60207,50 +60255,50 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Ts(e) {
+        function As(e) {
             return e && !!["provider"].find((function(t) {
                 return e.hasOwnProperty(t)
             }))
         }
 
-        function As(e) {
+        function Os(e) {
             return void 0 !== e.redirectSignIn
         }! function(e) {
             e.Cognito = "COGNITO", e.Google = "Google", e.Facebook = "Facebook", e.Amazon = "LoginWithAmazon", e.Apple = "SignInWithApple"
-        }(Ds || (Ds = {})),
+        }(Ss || (Ss = {})),
         function(e) {
             e.NoConfig = "noConfig", e.MissingAuthConfig = "missingAuthConfig", e.EmptyUsername = "emptyUsername", e.InvalidUsername = "invalidUsername", e.EmptyPassword = "emptyPassword", e.EmptyCode = "emptyCode", e.SignUpError = "signUpError", e.NoMFA = "noMFA", e.InvalidMFA = "invalidMFA", e.EmptyChallengeResponse = "emptyChallengeResponse", e.NoUserSession = "noUserSession", e.Default = "default", e.DeviceConfig = "deviceConfig", e.NetworkError = "networkError", e.AutoSignInError = "autoSignInError"
-        }(Ss || (Ss = {})),
+        }(Ls || (Ls = {})),
         function(e) {
             e.API_KEY = "API_KEY", e.AWS_IAM = "AWS_IAM", e.OPENID_CONNECT = "OPENID_CONNECT", e.AMAZON_COGNITO_USER_POOLS = "AMAZON_COGNITO_USER_POOLS", e.AWS_LAMBDA = "AWS_LAMBDA"
-        }(Ls || (Ls = {}));
-        var Os = function(e, t) {
-            return Os = Object.setPrototypeOf || {
+        }(ks || (ks = {}));
+        var zs = function(e, t) {
+            return zs = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-            }, Os(e, t)
+            }, zs(e, t)
         };
-        var zs = function() {
-            return zs = Object.assign || function(e) {
+        var Us = function() {
+            return Us = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, zs.apply(this, arguments)
+            }, Us.apply(this, arguments)
         };
 
-        function Us(e, t, n, r) {
+        function Ps(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60270,15 +60318,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Ps(e, t) {
+        function Rs(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60346,15 +60394,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Rs(e) {
+        function Bs(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -60362,15 +60410,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Bs(e, t) {
+        function Fs(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60384,58 +60432,58 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Fs() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Bs(arguments[t]));
+        function Ys() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Fs(arguments[t]));
             return e
         }
-        var Ys, Qs = {
+        var Qs, Gs = {
             VERBOSE: 1,
             DEBUG: 2,
             INFO: 3,
             WARN: 4,
             ERROR: 5
         };
         ! function(e) {
             e.DEBUG = "DEBUG", e.ERROR = "ERROR", e.INFO = "INFO", e.WARN = "WARN", e.VERBOSE = "VERBOSE"
-        }(Ys || (Ys = {}));
-        var Gs = function() {
+        }(Qs || (Qs = {}));
+        var Ws = function() {
                 function e(e, t) {
-                    void 0 === t && (t = Ys.WARN), this.name = e, this.level = t, this._pluggables = []
+                    void 0 === t && (t = Qs.WARN), this.name = e, this.level = t, this._pluggables = []
                 }
                 return e.prototype._padding = function(e) {
                     return e < 10 ? "0" + e : "" + e
                 }, e.prototype._ts = function() {
                     var e = new Date;
                     return [this._padding(e.getMinutes()), this._padding(e.getSeconds())].join(":") + "." + e.getMilliseconds()
                 }, e.prototype.configure = function(e) {
                     return e ? (this._config = e, this._config) : this._config
                 }, e.prototype._log = function(t) {
                     for (var n, r, o = [], i = 1; i < arguments.length; i++) o[i - 1] = arguments[i];
                     var a = this.level;
                     e.LOG_LEVEL && (a = e.LOG_LEVEL), "undefined" !== typeof window && window.LOG_LEVEL && (a = window.LOG_LEVEL);
-                    var s = Qs[a],
-                        u = Qs[t];
+                    var s = Gs[a],
+                        u = Gs[t];
                     if (u >= s) {
                         var l = console.log.bind(console);
-                        t === Ys.ERROR && console.error && (l = console.error.bind(console)), t === Ys.WARN && console.warn && (l = console.warn.bind(console));
+                        t === Qs.ERROR && console.error && (l = console.error.bind(console)), t === Qs.WARN && console.warn && (l = console.warn.bind(console));
                         var c = "[" + t + "] " + this._ts() + " " + this.name,
                             d = "";
                         if (1 === o.length && "string" === typeof o[0]) l(d = c + " - " + o[0]);
                         else if (1 === o.length) d = c + " " + o[0], l(c, o[0]);
                         else if ("string" === typeof o[0]) {
                             var f = o.slice(1);
                             1 === f.length && (f = f[0]), d = c + " - " + o[0] + " " + f, l(c + " - " + o[0], f)
                         } else d = c + " " + o, l(c, o);
                         try {
-                            for (var p = Rs(this._pluggables), h = p.next(); !h.done; h = p.next()) {
+                            for (var p = Bs(this._pluggables), h = p.next(); !h.done; h = p.next()) {
                                 var g = h.value,
                                     y = {
                                         message: d,
                                         timestamp: Date.now()
                                     };
                                 g.pushLogs([y])
                             }
@@ -60449,78 +60497,78 @@
                             } finally {
                                 if (n) throw n.error
                             }
                         }
                     }
                 }, e.prototype.log = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Fs([Ys.INFO], e))
+                    this._log.apply(this, Ys([Qs.INFO], e))
                 }, e.prototype.info = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Fs([Ys.INFO], e))
+                    this._log.apply(this, Ys([Qs.INFO], e))
                 }, e.prototype.warn = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Fs([Ys.WARN], e))
+                    this._log.apply(this, Ys([Qs.WARN], e))
                 }, e.prototype.error = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Fs([Ys.ERROR], e))
+                    this._log.apply(this, Ys([Qs.ERROR], e))
                 }, e.prototype.debug = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Fs([Ys.DEBUG], e))
+                    this._log.apply(this, Ys([Qs.DEBUG], e))
                 }, e.prototype.verbose = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Fs([Ys.VERBOSE], e))
+                    this._log.apply(this, Ys([Qs.VERBOSE], e))
                 }, e.prototype.addPluggable = function(e) {
                     e && "Logging" === e.getCategoryName() && (this._pluggables.push(e), e.configure(this._config))
                 }, e.prototype.listPluggables = function() {
                     return this._pluggables
                 }, e.LOG_LEVEL = null, e
             }(),
-            Ws = new Gs("Hub"),
-            Hs = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
-        var Zs = function() {
+            Hs = new Ws("Hub"),
+            Zs = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
+        var Vs = function() {
                 function e(e) {
                     this.listeners = [], this.patterns = [], this.protectedChannels = ["core", "auth", "api", "analytics", "interactions", "pubsub", "storage", "ui", "xr"], this.name = e
                 }
                 return e.prototype._remove = function(e, t) {
                     if (e instanceof RegExp) {
                         var n = this.patterns.find((function(t) {
                             return t.pattern.source === e.source
                         }));
-                        if (!n) return void Ws.warn("No listeners for " + e);
-                        this.patterns = Fs(this.patterns.filter((function(e) {
+                        if (!n) return void Hs.warn("No listeners for " + e);
+                        this.patterns = Ys(this.patterns.filter((function(e) {
                             return e !== n
                         })))
                     } else {
                         var r = this.listeners[e];
-                        if (!r) return void Ws.warn("No listeners for " + e);
-                        this.listeners[e] = Fs(r.filter((function(e) {
+                        if (!r) return void Hs.warn("No listeners for " + e);
+                        this.listeners[e] = Ys(r.filter((function(e) {
                             return e.callback !== t
                         })))
                     }
                 }, e.prototype.remove = function(e, t) {
                     this._remove(e, t)
                 }, e.prototype.dispatch = function(e, t, n, r) {
-                    (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === Hs || Ws.warn("WARNING: " + e + " is protected and dispatching on it can have unintended consequences"));
+                    (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === Zs || Hs.warn("WARNING: " + e + " is protected and dispatching on it can have unintended consequences"));
                     var o = {
                         channel: e,
-                        payload: zs({}, t),
+                        payload: Us({}, t),
                         source: n,
                         patternInfo: []
                     };
                     try {
                         this._toListeners(o)
                     } catch (i) {
-                        Ws.error(i)
+                        Hs.error(i)
                     }
                 }, e.prototype.listen = function(e, t, n) {
                     var r, o = this;
                     if (void 0 === n && (n = "noname"), function(e) {
                             return void 0 !== e.onHubCapsule
-                        }(t)) Ws.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
+                        }(t)) Hs.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
                     else {
                         if ("function" !== typeof t) throw new Error("No callback supplied to Hub");
                         r = t
                     }
                     if (e instanceof RegExp) this.patterns.push({
                         pattern: e,
                         callback: r
@@ -60536,115 +60584,115 @@
                         o._remove(e, r)
                     }
                 }, e.prototype._toListeners = function(e) {
                     var t = e.channel,
                         n = e.payload,
                         r = this.listeners[t];
                     if (r && r.forEach((function(r) {
-                            Ws.debug("Dispatching to " + t + " with ", n);
+                            Hs.debug("Dispatching to " + t + " with ", n);
                             try {
                                 r.callback(e)
                             } catch (o) {
-                                Ws.error(o)
+                                Hs.error(o)
                             }
                         })), this.patterns.length > 0) {
-                        if (!n.message) return void Ws.warn("Cannot perform pattern matching without a message key");
+                        if (!n.message) return void Hs.warn("Cannot perform pattern matching without a message key");
                         var o = n.message;
                         this.patterns.forEach((function(t) {
                             var n = o.match(t.pattern);
                             if (n) {
-                                var r = Bs(n).slice(1),
-                                    i = zs(zs({}, e), {
+                                var r = Fs(n).slice(1),
+                                    i = Us(Us({}, e), {
                                         patternInfo: r
                                     });
                                 try {
                                     t.callback(i)
                                 } catch (a) {
-                                    Ws.error(a)
+                                    Hs.error(a)
                                 }
                             }
                         }))
                     }
                 }, e
             }(),
-            Vs = new Zs("__default__"),
-            qs = {},
-            Js = function() {
+            qs = new Vs("__default__"),
+            Js = {},
+            Ks = function() {
                 function e() {}
                 return e.setItem = function(e, t) {
-                    return qs[e] = t, qs[e]
+                    return Js[e] = t, Js[e]
                 }, e.getItem = function(e) {
-                    return Object.prototype.hasOwnProperty.call(qs, e) ? qs[e] : void 0
+                    return Object.prototype.hasOwnProperty.call(Js, e) ? Js[e] : void 0
                 }, e.removeItem = function(e) {
-                    return delete qs[e]
+                    return delete Js[e]
                 }, e.clear = function() {
-                    return qs = {}
+                    return Js = {}
                 }, e
             }(),
-            Ks = function() {
+            Xs = function() {
                 function e() {
                     try {
                         this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.amplify.test-ls", 1), this.storageWindow.removeItem("aws.amplify.test-ls")
                     } catch (e) {
-                        this.storageWindow = Js
+                        this.storageWindow = Ks
                     }
                 }
                 return e.prototype.getStorage = function() {
                     return this.storageWindow
                 }, e
             }(),
-            Xs = function() {
+            $s = function() {
                 return {
                     isBrowser: "undefined" !== typeof window && "undefined" !== typeof window.document,
                     isNode: "undefined" !== typeof process && null != process.versions && null != process.versions.node
                 }
             },
-            $s = new Gs("Util"),
-            eu = function(e) {
+            eu = new Ws("Util"),
+            tu = function(e) {
                 function t(t) {
                     var n = e.call(this, t) || this;
                     return n.nonRetryable = !0, n
                 }
                 return function(e, t) {
                     function n() {
                         this.constructor = e
                     }
-                    Os(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                    zs(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
                 }(t, e), t
             }(Error);
-        var tu = 3e5;
-        var nu = function(e, t, n, r) {
-                return void 0 === n && (n = tu),
+        var nu = 3e5;
+        var ru = function(e, t, n, r) {
+                return void 0 === n && (n = nu),
                     function(e, t, n, r) {
-                        return Us(this, void 0, void 0, (function() {
+                        return Ps(this, void 0, void 0, (function() {
                             var o = this;
-                            return Ps(this, (function(i) {
+                            return Rs(this, (function(i) {
                                 if ("function" !== typeof e) throw Error("functionToRetry must be a function");
                                 return [2, new Promise((function(i, a) {
-                                    return Us(o, void 0, void 0, (function() {
+                                    return Ps(o, void 0, void 0, (function() {
                                         var o, s, u, l, c, d, f;
-                                        return Ps(this, (function(p) {
+                                        return Rs(this, (function(p) {
                                             switch (p.label) {
                                                 case 0:
                                                     o = 0, s = !1, l = function() {}, r && r.then((function() {
                                                         s = !0, clearTimeout(u), l()
                                                     })), d = function() {
                                                         var r, d, f, p;
-                                                        return Ps(this, (function(h) {
+                                                        return Rs(this, (function(h) {
                                                             switch (h.label) {
                                                                 case 0:
-                                                                    o++, $s.debug(e.name + " attempt #" + o + " with this vars: " + JSON.stringify(t)), h.label = 1;
+                                                                    o++, eu.debug(e.name + " attempt #" + o + " with this vars: " + JSON.stringify(t)), h.label = 1;
                                                                 case 1:
-                                                                    return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, Fs(t))];
+                                                                    return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, Ys(t))];
                                                                 case 2:
                                                                     return [2, (r.value = d.apply(void 0, [h.sent()]), r)];
                                                                 case 3:
-                                                                    return f = h.sent(), c = f, $s.debug("error on " + e.name, f), (g = f) && g.nonRetryable ? ($s.debug(e.name + " non retryable error", f), [2, {
+                                                                    return f = h.sent(), c = f, eu.debug("error on " + e.name, f), (g = f) && g.nonRetryable ? (eu.debug(e.name + " non retryable error", f), [2, {
                                                                         value: a(f)
-                                                                    }]) : (p = n(o, t, f), $s.debug(e.name + " retrying in " + p + " ms"), !1 === p || s ? [2, {
+                                                                    }]) : (p = n(o, t, f), eu.debug(e.name + " retrying in " + p + " ms"), !1 === p || s ? [2, {
                                                                         value: a(f)
                                                                     }] : [3, 4]);
                                                                 case 4:
                                                                     return [4, new Promise((function(e) {
                                                                         l = e, u = setTimeout(l, p)
                                                                     }))];
                                                                 case 5:
@@ -60666,147 +60714,147 @@
                                             }
                                         }))
                                     }))
                                 }))]
                             }))
                         }))
                     }(e, t, function(e) {
-                        return void 0 === e && (e = tu),
+                        return void 0 === e && (e = nu),
                             function(t) {
                                 var n = 100 * Math.pow(2, t) + 100 * Math.random();
                                 return !(n > e) && n
                             }
                     }(n), r)
             },
-            ru = new Gs("CognitoCredentials"),
-            ou = new Promise((function(e, t) {
-                return Xs().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (ru.debug("google api already loaded"), e()) : void setTimeout((function() {
+            ou = new Ws("CognitoCredentials"),
+            iu = new Promise((function(e, t) {
+                return $s().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (ou.debug("google api already loaded"), e()) : void setTimeout((function() {
                     return e()
-                }), 2e3) : (ru.debug("not in the browser, directly resolved"), e())
+                }), 2e3) : (ou.debug("not in the browser, directly resolved"), e())
             })),
-            iu = function() {
+            au = function() {
                 function e() {
                     this.initialized = !1, this.refreshGoogleToken = this.refreshGoogleToken.bind(this), this._refreshGoogleTokenImpl = this._refreshGoogleTokenImpl.bind(this)
                 }
                 return e.prototype.refreshGoogleToken = function() {
-                    return Us(this, void 0, void 0, (function() {
-                        return Ps(this, (function(e) {
+                    return Ps(this, void 0, void 0, (function() {
+                        return Rs(this, (function(e) {
                             switch (e.label) {
                                 case 0:
-                                    return this.initialized ? [3, 2] : (ru.debug("need to wait for the Google SDK loaded"), [4, ou]);
+                                    return this.initialized ? [3, 2] : (ou.debug("need to wait for the Google SDK loaded"), [4, iu]);
                                 case 1:
-                                    e.sent(), this.initialized = !0, ru.debug("finish waiting"), e.label = 2;
+                                    e.sent(), this.initialized = !0, ou.debug("finish waiting"), e.label = 2;
                                 case 2:
                                     return [2, this._refreshGoogleTokenImpl()]
                             }
                         }))
                     }))
                 }, e.prototype._refreshGoogleTokenImpl = function() {
                     var e = null;
-                    return Xs().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
+                    return $s().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
                         e.getAuthInstance().then((function(e) {
-                            e || (ru.debug("google Auth undefined"), n(new eu("google Auth undefined")));
+                            e || (ou.debug("google Auth undefined"), n(new tu("google Auth undefined")));
                             var r = e.currentUser.get();
-                            r.isSignedIn() ? (ru.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
+                            r.isSignedIn() ? (ou.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
                                 var n = e.id_token,
                                     r = e.expires_at;
                                 t({
                                     token: n,
                                     expires_at: r
                                 })
                             })).catch((function(e) {
-                                e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new eu("Failed to reload google auth response"))
-                            }))) : n(new eu("User is not signed in with Google"))
+                                e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new tu("Failed to reload google auth response"))
+                            }))) : n(new tu("User is not signed in with Google"))
                         })).catch((function(e) {
-                            ru.debug("Failed to refresh google token", e), n(new eu("Failed to refresh google token"))
+                            ou.debug("Failed to refresh google token", e), n(new tu("Failed to refresh google token"))
                         }))
-                    })) : (ru.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
+                    })) : (ou.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
                 }, e
             }(),
-            au = new Gs("CognitoCredentials"),
-            su = new Promise((function(e, t) {
-                return Xs().isBrowser ? window.FB ? (au.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
+            su = new Ws("CognitoCredentials"),
+            uu = new Promise((function(e, t) {
+                return $s().isBrowser ? window.FB ? (su.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
                     return e()
-                }), 2e3) : (au.debug("not in the browser, directly resolved"), e())
+                }), 2e3) : (su.debug("not in the browser, directly resolved"), e())
             })),
-            uu = function() {
+            lu = function() {
                 function e() {
                     this.initialized = !1, this.refreshFacebookToken = this.refreshFacebookToken.bind(this), this._refreshFacebookTokenImpl = this._refreshFacebookTokenImpl.bind(this)
                 }
                 return e.prototype.refreshFacebookToken = function() {
-                    return Us(this, void 0, void 0, (function() {
-                        return Ps(this, (function(e) {
+                    return Ps(this, void 0, void 0, (function() {
+                        return Rs(this, (function(e) {
                             switch (e.label) {
                                 case 0:
-                                    return this.initialized ? [3, 2] : (au.debug("need to wait for the Facebook SDK loaded"), [4, su]);
+                                    return this.initialized ? [3, 2] : (su.debug("need to wait for the Facebook SDK loaded"), [4, uu]);
                                 case 1:
-                                    e.sent(), this.initialized = !0, au.debug("finish waiting"), e.label = 2;
+                                    e.sent(), this.initialized = !0, su.debug("finish waiting"), e.label = 2;
                                 case 2:
                                     return [2, this._refreshFacebookTokenImpl()]
                             }
                         }))
                     }))
                 }, e.prototype._refreshFacebookTokenImpl = function() {
                     var e = null;
-                    if (Xs().isBrowser && (e = window.FB), !e) {
+                    if ($s().isBrowser && (e = window.FB), !e) {
                         var t = "no fb sdk available";
-                        return au.debug(t), Promise.reject(new eu(t))
+                        return su.debug(t), Promise.reject(new tu(t))
                     }
                     return new Promise((function(t, n) {
                         e.getLoginStatus((function(e) {
                             if (e && e.authResponse) {
                                 var r = e.authResponse,
                                     o = r.accessToken,
                                     i = 1e3 * r.expiresIn + (new Date).getTime();
                                 if (!o) {
                                     a = "the jwtToken is undefined";
-                                    au.debug(a), n(new eu(a))
+                                    su.debug(a), n(new tu(a))
                                 }
                                 t({
                                     token: o,
                                     expires_at: i
                                 })
                             } else {
                                 var a = "no response from facebook when refreshing the jwt token";
-                                au.debug(a), n(new eu(a))
+                                su.debug(a), n(new tu(a))
                             }
                         }), {
                             scope: "public_profile,email"
                         })
                     }))
                 }, e
             }(),
-            lu = new iu,
-            cu = new uu,
-            du = new Gs("Amplify"),
-            fu = new(function() {
+            cu = new au,
+            du = new lu,
+            fu = new Ws("Amplify"),
+            pu = new(function() {
                 function e() {
-                    this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = Gs, this.ServiceWorker = null
+                    this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = Ws, this.ServiceWorker = null
                 }
                 return e.prototype.register = function(e) {
-                    du.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : du.debug("no getModuleName method for component", e), e.configure(this._config)
+                    fu.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : fu.debug("no getModuleName method for component", e), e.configure(this._config)
                 }, e.prototype.configure = function(e) {
                     var t = this;
-                    return e ? (this._config = Object.assign(this._config, e), du.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
-                        var n = Bs(e, 2),
+                    return e ? (this._config = Object.assign(this._config, e), fu.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
+                        var n = Fs(e, 2),
                             r = (n[0], n[1]);
                         Object.keys(r).forEach((function(e) {
                             t._modules[e] && (r[e] = t._modules[e])
                         }))
                     })), this._components.map((function(e) {
                         e.configure(t._config)
                     })), this._config) : this._config
                 }, e.prototype.addPluggable = function(e) {
                     e && e.getCategory && "function" === typeof e.getCategory && this._components.map((function(t) {
                         t.addPluggable && "function" === typeof t.addPluggable && t.addPluggable(e)
                     }))
                 }, e
             }());
 
-        function pu(e, t, n, r) {
+        function hu(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60826,15 +60874,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function hu(e, t) {
+        function gu(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60902,15 +60950,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function gu(e, t) {
+        function yu(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60923,42 +60971,42 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var yu = function(e, t) {
-            return yu = Object.setPrototypeOf || {
+        var mu = function(e, t) {
+            return mu = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
-            }, yu(e, t)
+            }, mu(e, t)
         };
 
-        function mu(e, t) {
+        function vu(e, t) {
             if ("function" !== typeof t && null !== t) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
 
             function n() {
                 this.constructor = e
             }
-            yu(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            mu(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         }
-        var vu = function() {
-            return vu = Object.assign || function(e) {
+        var Mu = function() {
+            return Mu = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, vu.apply(this, arguments)
+            }, Mu.apply(this, arguments)
         };
 
-        function Mu(e, t, n, r) {
+        function bu(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60978,15 +61026,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function bu(e, t) {
+        function ju(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -61055,15 +61103,15 @@
                         }
                     }([i, s])
                 }
             }
         }
         Object.create;
 
-        function ju(e, t) {
+        function wu(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -61076,312 +61124,312 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var wu, xu, Nu, Iu, Du, Su, Lu, ku, Cu, Eu, _u, Tu, Au, Ou, zu, Uu, Pu, Ru, Bu, Fu, Yu, Qu, Gu, Wu, Hu, Zu, Vu, qu, Ju, Ku, Xu, $u, el, tl, nl, rl, ol, il, al, sl, ul, ll, cl, dl, fl, pl, hl, gl, yl, ml, vl, Ml, bl, jl, wl, xl, Nl;
+        var xu, Nu, Iu, Du, Su, Lu, ku, Cu, Eu, _u, Tu, Au, Ou, zu, Uu, Pu, Ru, Bu, Fu, Yu, Qu, Gu, Wu, Hu, Zu, Vu, qu, Ju, Ku, Xu, $u, el, tl, nl, rl, ol, il, al, sl, ul, ll, cl, dl, fl, pl, hl, gl, yl, ml, vl, Ml, bl, jl, wl, xl, Nl, Il;
         Object.create;
         ! function(e) {
             e.AUTHENTICATED_ROLE = "AuthenticatedRole", e.DENY = "Deny"
-        }(wu || (wu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return vu({}, e)
-            }
         }(xu || (xu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Nu || (Nu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Iu || (Iu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Du || (Du = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Su || (Su = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Lu || (Lu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(ku || (ku = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Cu || (Cu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Eu || (Eu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(_u || (_u = {})),
         function(e) {
-            e.ACCESS_DENIED = "AccessDenied", e.INTERNAL_SERVER_ERROR = "InternalServerError"
-        }(Tu || (Tu = {})),
-        function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
+        }(Tu || (Tu = {})),
+        function(e) {
+            e.ACCESS_DENIED = "AccessDenied", e.INTERNAL_SERVER_ERROR = "InternalServerError"
         }(Au || (Au = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Ou || (Ou = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(zu || (zu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Uu || (Uu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Pu || (Pu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Ru || (Ru = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Bu || (Bu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Fu || (Fu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Yu || (Yu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Qu || (Qu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Gu || (Gu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Wu || (Wu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Hu || (Hu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Zu || (Zu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Vu || (Vu = {})),
         function(e) {
-            e.CONTAINS = "Contains", e.EQUALS = "Equals", e.NOT_EQUAL = "NotEqual", e.STARTS_WITH = "StartsWith"
-        }(qu || (qu = {})),
-        function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
+        }(qu || (qu = {})),
+        function(e) {
+            e.CONTAINS = "Contains", e.EQUALS = "Equals", e.NOT_EQUAL = "NotEqual", e.STARTS_WITH = "StartsWith"
         }(Ju || (Ju = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Ku || (Ku = {})),
         function(e) {
-            e.RULES = "Rules", e.TOKEN = "Token"
-        }(Xu || (Xu = {})),
-        function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
+        }(Xu || (Xu = {})),
+        function(e) {
+            e.RULES = "Rules", e.TOKEN = "Token"
         }($u || ($u = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(el || (el = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(tl || (tl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(nl || (nl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(rl || (rl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(ol || (ol = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(il || (il = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(al || (al = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(sl || (sl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(ul || (ul = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(ll || (ll = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(cl || (cl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(dl || (dl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(fl || (fl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(pl || (pl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(hl || (hl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(gl || (gl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(yl || (yl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(ml || (ml = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(vl || (vl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(Ml || (Ml = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(bl || (bl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(jl || (jl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(wl || (wl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
             }
         }(xl || (xl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return vu({}, e)
+                return Mu({}, e)
+            }
+        }(Nl || (Nl = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Mu({}, e)
             }
-        }(Nl || (Nl = {}));
-        var Il = function() {
+        }(Il || (Il = {}));
+        var Dl = function() {
             function e(e) {
                 this.statusCode = e.statusCode, this.headers = e.headers || {}, this.body = e.body
             }
             return e.isInstance = function(e) {
                 if (!e) return !1;
                 var t = e;
                 return "number" === typeof t.statusCode && "object" === typeof t.headers
             }, e
         }();
-        var Dl = function() {
-            return Dl = Object.assign || function(e) {
+        var Sl = function() {
+            return Sl = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Dl.apply(this, arguments)
+            }, Sl.apply(this, arguments)
         };
 
-        function Sl(e, t) {
+        function Ll(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -61394,44 +61442,44 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var Ll = function() {
+        var kl = function() {
             function e(e) {
                 this.method = e.method || "GET", this.hostname = e.hostname || "localhost", this.port = e.port, this.query = e.query || {}, this.headers = e.headers || {}, this.body = e.body, this.protocol = e.protocol ? ":" !== e.protocol.substr(-1) ? e.protocol + ":" : e.protocol : "https:", this.path = e.path ? "/" !== e.path.charAt(0) ? "/" + e.path : e.path : "/"
             }
             return e.isInstance = function(e) {
                 if (!e) return !1;
                 var t = e;
                 return "method" in t && "protocol" in t && "hostname" in t && "path" in t && "object" === typeof t.query && "object" === typeof t.headers
             }, e.prototype.clone = function() {
-                var t, n = new e(Dl(Dl({}, this), {
-                    headers: Dl({}, this.headers)
+                var t, n = new e(Sl(Sl({}, this), {
+                    headers: Sl({}, this.headers)
                 }));
                 return n.query && (n.query = (t = n.query, Object.keys(t).reduce((function(e, n) {
                     var r, o = t[n];
-                    return Dl(Dl({}, e), ((r = {})[n] = Array.isArray(o) ? function() {
-                        for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Sl(arguments[t]));
+                    return Sl(Sl({}, e), ((r = {})[n] = Array.isArray(o) ? function() {
+                        for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Ll(arguments[t]));
                         return e
                     }(o) : o, r))
                 }), {}))), n
             }, e
         }();
-        var kl = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+        var Cl = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y;
-                    return bu(this, (function(m) {
+                    return ju(this, (function(m) {
                         switch (m.label) {
                             case 0:
-                                return r = [vu({}, e)], y = {}, [4, oc(e.body, t)];
+                                return r = [Mu({}, e)], y = {}, [4, ic(e.body, t)];
                             case 1:
-                                switch (n = vu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = ic(e, n.body), i) {
+                                switch (n = Mu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = ac(e, n.body), i) {
                                     case "ExternalServiceException":
                                     case "com.amazonaws.cognitoidentity#ExternalServiceException":
                                         return [3, 2];
                                     case "InternalErrorException":
                                     case "com.amazonaws.cognitoidentity#InternalErrorException":
                                         return [3, 4];
                                     case "InvalidIdentityPoolConfigurationException":
@@ -61451,91 +61499,91 @@
                                         return [3, 14];
                                     case "TooManyRequestsException":
                                     case "com.amazonaws.cognitoidentity#TooManyRequestsException":
                                         return [3, 16]
                                 }
                                 return [3, 18];
                             case 2:
-                                return a = [{}], [4, El(n, t)];
+                                return a = [{}], [4, _l(n, t)];
                             case 3:
-                                return o = vu.apply(void 0, [vu.apply(void 0, a.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, a.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 4:
-                                return s = [{}], [4, _l(n, t)];
+                                return s = [{}], [4, Tl(n, t)];
                             case 5:
-                                return o = vu.apply(void 0, [vu.apply(void 0, s.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, s.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 6:
-                                return u = [{}], [4, Tl(n, t)];
+                                return u = [{}], [4, Al(n, t)];
                             case 7:
-                                return o = vu.apply(void 0, [vu.apply(void 0, u.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, u.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 8:
-                                return l = [{}], [4, Al(n, t)];
+                                return l = [{}], [4, Ol(n, t)];
                             case 9:
-                                return o = vu.apply(void 0, [vu.apply(void 0, l.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, l.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 10:
-                                return c = [{}], [4, zl(n, t)];
+                                return c = [{}], [4, Ul(n, t)];
                             case 11:
-                                return o = vu.apply(void 0, [vu.apply(void 0, c.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, c.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 12:
-                                return d = [{}], [4, Ul(n, t)];
+                                return d = [{}], [4, Pl(n, t)];
                             case 13:
-                                return o = vu.apply(void 0, [vu.apply(void 0, d.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, d.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 14:
-                                return f = [{}], [4, Pl(n, t)];
+                                return f = [{}], [4, Rl(n, t)];
                             case 15:
-                                return o = vu.apply(void 0, [vu.apply(void 0, f.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, f.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 16:
-                                return p = [{}], [4, Rl(n, t)];
+                                return p = [{}], [4, Bl(n, t)];
                             case 17:
-                                return o = vu.apply(void 0, [vu.apply(void 0, p.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, p.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 18:
-                                h = n.body, i = h.code || h.Code || i, o = vu(vu({}, h), {
+                                h = n.body, i = h.code || h.Code || i, o = Mu(Mu({}, h), {
                                     name: "" + i,
                                     message: h.message || h.Message || i,
                                     $fault: "client",
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }), m.label = 19;
                             case 19:
                                 return g = o.message || o.Message || i, o.message = g, delete o.Message, [2, Promise.reject(Object.assign(new Error(g), o))]
                         }
                     }))
                 }))
             },
-            Cl = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            El = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y;
-                    return bu(this, (function(m) {
+                    return ju(this, (function(m) {
                         switch (m.label) {
                             case 0:
-                                return r = [vu({}, e)], y = {}, [4, oc(e.body, t)];
+                                return r = [Mu({}, e)], y = {}, [4, ic(e.body, t)];
                             case 1:
-                                switch (n = vu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = ic(e, n.body), i) {
+                                switch (n = Mu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = ac(e, n.body), i) {
                                     case "ExternalServiceException":
                                     case "com.amazonaws.cognitoidentity#ExternalServiceException":
                                         return [3, 2];
                                     case "InternalErrorException":
                                     case "com.amazonaws.cognitoidentity#InternalErrorException":
                                         return [3, 4];
                                     case "InvalidParameterException":
@@ -61555,243 +61603,238 @@
                                         return [3, 14];
                                     case "TooManyRequestsException":
                                     case "com.amazonaws.cognitoidentity#TooManyRequestsException":
                                         return [3, 16]
                                 }
                                 return [3, 18];
                             case 2:
-                                return a = [{}], [4, El(n, t)];
+                                return a = [{}], [4, _l(n, t)];
                             case 3:
-                                return o = vu.apply(void 0, [vu.apply(void 0, a.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, a.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 4:
-                                return s = [{}], [4, _l(n, t)];
+                                return s = [{}], [4, Tl(n, t)];
                             case 5:
-                                return o = vu.apply(void 0, [vu.apply(void 0, s.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, s.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 6:
-                                return u = [{}], [4, Al(n, t)];
+                                return u = [{}], [4, Ol(n, t)];
                             case 7:
-                                return o = vu.apply(void 0, [vu.apply(void 0, u.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, u.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 8:
-                                return l = [{}], [4, Ol(n, t)];
+                                return l = [{}], [4, zl(n, t)];
                             case 9:
-                                return o = vu.apply(void 0, [vu.apply(void 0, l.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, l.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 10:
-                                return c = [{}], [4, zl(n, t)];
+                                return c = [{}], [4, Ul(n, t)];
                             case 11:
-                                return o = vu.apply(void 0, [vu.apply(void 0, c.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, c.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 12:
-                                return d = [{}], [4, Ul(n, t)];
+                                return d = [{}], [4, Pl(n, t)];
                             case 13:
-                                return o = vu.apply(void 0, [vu.apply(void 0, d.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, d.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 14:
-                                return f = [{}], [4, Pl(n, t)];
+                                return f = [{}], [4, Rl(n, t)];
                             case 15:
-                                return o = vu.apply(void 0, [vu.apply(void 0, f.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, f.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 16:
-                                return p = [{}], [4, Rl(n, t)];
+                                return p = [{}], [4, Bl(n, t)];
                             case 17:
-                                return o = vu.apply(void 0, [vu.apply(void 0, p.concat([m.sent()])), {
+                                return o = Mu.apply(void 0, [Mu.apply(void 0, p.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }]), [3, 19];
                             case 18:
-                                h = n.body, i = h.code || h.Code || i, o = vu(vu({}, h), {
+                                h = n.body, i = h.code || h.Code || i, o = Mu(Mu({}, h), {
                                     name: "" + i,
                                     message: h.message || h.Message || i,
                                     $fault: "client",
-                                    $metadata: tc(e)
+                                    $metadata: nc(e)
                                 }), m.label = 19;
                             case 19:
                                 return g = o.message || o.Message || i, o.message = g, delete o.Message, [2, Promise.reject(Object.assign(new Error(g), o))]
                         }
                     }))
                 }))
             },
-            El = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            _l = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = Gl(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = Wl(n, t), [2, Mu({
                             name: "ExternalServiceException",
                             $fault: "client",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            _l = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            Tl = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = Zl(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = Vl(n, t), [2, Mu({
                             name: "InternalErrorException",
                             $fault: "server",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            Tl = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            Al = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = Vl(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = ql(n, t), [2, Mu({
                             name: "InvalidIdentityPoolConfigurationException",
                             $fault: "client",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            Al = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            Ol = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = ql(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = Jl(n, t), [2, Mu({
                             name: "InvalidParameterException",
                             $fault: "client",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            Ol = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            zl = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = Jl(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = Kl(n, t), [2, Mu({
                             name: "LimitExceededException",
                             $fault: "client",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            zl = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            Ul = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = Kl(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = Xl(n, t), [2, Mu({
                             name: "NotAuthorizedException",
                             $fault: "client",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            Ul = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            Pl = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = Xl(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = $l(n, t), [2, Mu({
                             name: "ResourceConflictException",
                             $fault: "client",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            Pl = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            Rl = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = $l(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = ec(n, t), [2, Mu({
                             name: "ResourceNotFoundException",
                             $fault: "client",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            Rl = function(e, t) {
-                return Mu(void 0, void 0, void 0, (function() {
+            Bl = function(e, t) {
+                return bu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return bu(this, (function(o) {
-                        return n = e.body, r = ec(n, t), [2, vu({
+                    return ju(this, (function(o) {
+                        return n = e.body, r = tc(n, t), [2, Mu({
                             name: "TooManyRequestsException",
                             $fault: "client",
-                            $metadata: tc(e)
+                            $metadata: nc(e)
                         }, r)]
                     }))
                 }))
             },
-            Bl = function(e, t) {
-                return vu(vu(vu({}, void 0 !== e.CustomRoleArn && null !== e.CustomRoleArn && {
+            Fl = function(e, t) {
+                return Mu(Mu(Mu({}, void 0 !== e.CustomRoleArn && null !== e.CustomRoleArn && {
                     CustomRoleArn: e.CustomRoleArn
                 }), void 0 !== e.IdentityId && null !== e.IdentityId && {
                     IdentityId: e.IdentityId
                 }), void 0 !== e.Logins && null !== e.Logins && {
-                    Logins: Yl(e.Logins, t)
+                    Logins: Ql(e.Logins, t)
                 })
             },
-            Fl = function(e, t) {
-                return vu(vu(vu({}, void 0 !== e.AccountId && null !== e.AccountId && {
+            Yl = function(e, t) {
+                return Mu(Mu(Mu({}, void 0 !== e.AccountId && null !== e.AccountId && {
                     AccountId: e.AccountId
                 }), void 0 !== e.IdentityPoolId && null !== e.IdentityPoolId && {
                     IdentityPoolId: e.IdentityPoolId
                 }), void 0 !== e.Logins && null !== e.Logins && {
-                    Logins: Yl(e.Logins, t)
+                    Logins: Ql(e.Logins, t)
                 })
             },
-            Yl = function(e, t) {
+            Ql = function(e, t) {
                 return Object.entries(e).reduce((function(e, t) {
-                    var n, r = ju(t, 2),
+                    var n, r = wu(t, 2),
                         o = r[0],
                         i = r[1];
-                    return null === i ? e : vu(vu({}, e), ((n = {})[o] = i, n))
+                    return null === i ? e : Mu(Mu({}, e), ((n = {})[o] = i, n))
                 }), {})
             },
-            Ql = function(e, t) {
+            Gl = function(e, t) {
                 return {
                     AccessKeyId: void 0 !== e.AccessKeyId && null !== e.AccessKeyId ? e.AccessKeyId : void 0,
                     Expiration: void 0 !== e.Expiration && null !== e.Expiration ? new Date(Math.round(1e3 * e.Expiration)) : void 0,
                     SecretKey: void 0 !== e.SecretKey && null !== e.SecretKey ? e.SecretKey : void 0,
                     SessionToken: void 0 !== e.SessionToken && null !== e.SessionToken ? e.SessionToken : void 0
                 }
             },
-            Gl = function(e, t) {
-                return {
-                    message: void 0 !== e.message && null !== e.message ? e.message : void 0
-                }
-            },
             Wl = function(e, t) {
                 return {
-                    Credentials: void 0 !== e.Credentials && null !== e.Credentials ? Ql(e.Credentials) : void 0,
-                    IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
+                    message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
             Hl = function(e, t) {
                 return {
+                    Credentials: void 0 !== e.Credentials && null !== e.Credentials ? Gl(e.Credentials) : void 0,
                     IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
                 }
             },
             Zl = function(e, t) {
                 return {
-                    message: void 0 !== e.message && null !== e.message ? e.message : void 0
+                    IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
                 }
             },
             Vl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
@@ -61821,74 +61864,79 @@
                 }
             },
             ec = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            tc = function(e) {
+            tc = function(e, t) {
+                return {
+                    message: void 0 !== e.message && null !== e.message ? e.message : void 0
+                }
+            },
+            nc = function(e) {
                 var t;
                 return {
                     httpStatusCode: e.statusCode,
                     requestId: null !== (t = e.headers["x-amzn-requestid"]) && void 0 !== t ? t : e.headers["x-amzn-request-id"],
                     extendedRequestId: e.headers["x-amz-id-2"],
                     cfId: e.headers["x-amz-cf-id"]
                 }
             },
-            nc = function(e, t) {
+            rc = function(e, t) {
                 return void 0 === e && (e = new Uint8Array), e instanceof Uint8Array ? Promise.resolve(e) : t.streamCollector(e) || Promise.resolve(new Uint8Array)
             },
-            rc = function(e, t, n, r, o) {
-                return Mu(void 0, void 0, void 0, (function() {
+            oc = function(e, t, n, r, o) {
+                return bu(void 0, void 0, void 0, (function() {
                     var i, a, s, u, l, c;
-                    return bu(this, (function(d) {
+                    return ju(this, (function(d) {
                         switch (d.label) {
                             case 0:
                                 return [4, e.endpoint()];
                             case 1:
                                 return i = d.sent(), a = i.hostname, s = i.protocol, u = void 0 === s ? "https" : s, l = i.port, c = {
                                     protocol: u,
                                     hostname: a,
                                     port: l,
                                     method: "POST",
                                     path: n,
                                     headers: t
-                                }, void 0 !== r && (c.hostname = r), void 0 !== o && (c.body = o), [2, new Ll(c)]
+                                }, void 0 !== r && (c.hostname = r), void 0 !== o && (c.body = o), [2, new kl(c)]
                         }
                     }))
                 }))
             },
-            oc = function(e, t) {
+            ic = function(e, t) {
                 return function(e, t) {
-                    return nc(e, t).then((function(e) {
+                    return rc(e, t).then((function(e) {
                         return t.utf8Encoder(e)
                     }))
                 }(e, t).then((function(e) {
                     return e.length ? JSON.parse(e) : {}
                 }))
             },
-            ic = function(e, t) {
+            ac = function(e, t) {
                 var n, r, o = function(e) {
                         var t = e;
                         return t.indexOf(":") >= 0 && (t = t.split(":")[0]), t.indexOf("#") >= 0 && (t = t.split("#")[1]), t
                     },
                     i = (n = e.headers, r = "x-amzn-errortype", Object.keys(n).find((function(e) {
                         return e.toLowerCase() === r.toLowerCase()
                     })));
                 return void 0 !== i ? o(e.headers[i]) : void 0 !== t.code ? o(t.code) : void 0 !== t.__type ? o(t.__type) : ""
             };
-        var ac = function() {
-            return ac = Object.assign || function(e) {
+        var sc = function() {
+            return sc = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, ac.apply(this, arguments)
+            }, sc.apply(this, arguments)
         };
 
-        function sc(e, t, n, r) {
+        function uc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -61908,15 +61956,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function uc(e, t) {
+        function lc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -61983,36 +62031,36 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var lc = {
+        var cc = {
                 name: "deserializerMiddleware",
                 step: "deserialize",
                 tags: ["DESERIALIZER"],
                 override: !0
             },
-            cc = {
+            dc = {
                 name: "serializerMiddleware",
                 step: "serialize",
                 tags: ["SERIALIZER"],
                 override: !0
             };
 
-        function dc(e, t, n) {
+        function fc(e, t, n) {
             return {
                 applyToStack: function(r) {
                     r.add(function(e, t) {
                         return function(n, r) {
                             return function(r) {
-                                return sc(void 0, void 0, void 0, (function() {
+                                return uc(void 0, void 0, void 0, (function() {
                                     var o, i;
-                                    return uc(this, (function(a) {
+                                    return lc(this, (function(a) {
                                         switch (a.label) {
                                             case 0:
                                                 return [4, n(r)];
                                             case 1:
                                                 return o = a.sent().response, [4, t(o, e)];
                                             case 2:
                                                 return i = a.sent(), [2, {
@@ -62020,45 +62068,45 @@
                                                     output: i
                                                 }]
                                         }
                                     }))
                                 }))
                             }
                         }
-                    }(e, n), lc), r.add(function(e, t) {
+                    }(e, n), cc), r.add(function(e, t) {
                         return function(n, r) {
                             return function(r) {
-                                return sc(void 0, void 0, void 0, (function() {
+                                return uc(void 0, void 0, void 0, (function() {
                                     var o;
-                                    return uc(this, (function(i) {
+                                    return lc(this, (function(i) {
                                         switch (i.label) {
                                             case 0:
                                                 return [4, t(r.input, e)];
                                             case 1:
-                                                return o = i.sent(), [2, n(ac(ac({}, r), {
+                                                return o = i.sent(), [2, n(sc(sc({}, r), {
                                                     request: o
                                                 }))]
                                         }
                                     }))
                                 }))
                             }
                         }
-                    }(e, t), cc)
+                    }(e, t), dc)
                 }
             }
         }
-        var fc = function() {
-            return fc = Object.assign || function(e) {
+        var pc = function() {
+            return pc = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, fc.apply(this, arguments)
+            }, pc.apply(this, arguments)
         };
 
-        function pc(e) {
+        function hc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -62066,15 +62114,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function hc(e, t) {
+        function gc(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -62088,75 +62136,75 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function gc() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(hc(arguments[t]));
+        function yc() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(gc(arguments[t]));
             return e
         }
-        var yc = function e() {
+        var mc = function e() {
                 var t = [],
                     n = [],
                     r = new Set,
                     o = function(e) {
                         return t.forEach((function(t) {
-                            e.add(t.middleware, fc({}, t))
+                            e.add(t.middleware, pc({}, t))
                         })), n.forEach((function(t) {
-                            e.addRelativeTo(t.middleware, fc({}, t))
+                            e.addRelativeTo(t.middleware, pc({}, t))
                         })), e
                     },
                     i = function e(t) {
                         var n = [];
                         return t.before.forEach((function(t) {
-                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, gc(e(t)))
+                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, yc(e(t)))
                         })), n.push(t), t.after.reverse().forEach((function(t) {
-                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, gc(e(t)))
+                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, yc(e(t)))
                         })), n
                     },
                     a = function() {
                         var e = [],
                             r = [],
                             o = {};
                         t.forEach((function(t) {
-                            var n = fc(fc({}, t), {
+                            var n = pc(pc({}, t), {
                                 before: [],
                                 after: []
                             });
                             n.name && (o[n.name] = n), e.push(n)
                         })), n.forEach((function(e) {
-                            var t = fc(fc({}, e), {
+                            var t = pc(pc({}, e), {
                                 before: [],
                                 after: []
                             });
                             t.name && (o[t.name] = t), r.push(t)
                         })), r.forEach((function(e) {
                             if (e.toMiddleware) {
                                 var t = o[e.toMiddleware];
                                 if (void 0 === t) throw new Error(e.toMiddleware + " is not found when adding " + (e.name || "anonymous") + " middleware " + e.relation + " " + e.toMiddleware);
                                 "after" === e.relation && t.after.push(e), "before" === e.relation && t.before.push(e)
                             }
                         }));
                         var a, s = (a = e, a.sort((function(e, t) {
-                            return mc[t.step] - mc[e.step] || vc[t.priority || "normal"] - vc[e.priority || "normal"]
+                            return vc[t.step] - vc[e.step] || Mc[t.priority || "normal"] - Mc[e.priority || "normal"]
                         }))).map(i).reduce((function(e, t) {
-                            return e.push.apply(e, gc(t)), e
+                            return e.push.apply(e, yc(t)), e
                         }), []);
                         return s.map((function(e) {
                             return e.middleware
                         }))
                     },
                     s = {
                         add: function(e, n) {
                             void 0 === n && (n = {});
                             var o = n.name,
                                 i = n.override,
-                                a = fc({
+                                a = pc({
                                     step: "initialize",
                                     priority: "normal",
                                     middleware: e
                                 }, n);
                             if (o) {
                                 if (r.has(o)) {
                                     if (!i) throw new Error("Duplicate middleware name '" + o + "'");
@@ -62170,15 +62218,15 @@
                                 r.add(o)
                             }
                             t.push(a)
                         },
                         addRelativeTo: function(e, t) {
                             var o = t.name,
                                 i = t.override,
-                                a = fc({
+                                a = pc({
                                     middleware: e
                                 }, t);
                             if (o) {
                                 if (r.has(o)) {
                                     if (!i) throw new Error("Duplicate middleware name '" + o + "'");
                                     var s = n.findIndex((function(e) {
                                             return e.name === o
@@ -62225,15 +62273,15 @@
                             var n = o(e());
                             return n.use(t), n
                         },
                         applyToStack: o,
                         resolve: function(e, t) {
                             var n, r;
                             try {
-                                for (var o = pc(a().reverse()), i = o.next(); !i.done; i = o.next()) {
+                                for (var o = hc(a().reverse()), i = o.next(); !i.done; i = o.next()) {
                                     e = (0, i.value)(e, t)
                                 }
                             } catch (s) {
                                 n = {
                                     error: s
                                 }
                             } finally {
@@ -62244,29 +62292,29 @@
                                 }
                             }
                             return e
                         }
                     };
                 return s
             },
-            mc = {
+            vc = {
                 initialize: 5,
                 serialize: 4,
                 build: 3,
                 finalizeRequest: 2,
                 deserialize: 1
             },
-            vc = {
+            Mc = {
                 high: 3,
                 normal: 2,
                 low: 1
             },
-            Mc = function() {
+            bc = function() {
                 function e(e) {
-                    this.middlewareStack = yc(), this.config = e
+                    this.middlewareStack = mc(), this.config = e
                 }
                 return e.prototype.send = function(e, t, n) {
                     var r = "function" !== typeof t ? t : void 0,
                         o = "function" === typeof t ? t : n,
                         i = e.resolveMiddleware(this.middlewareStack, this.config, r);
                     if (!o) return i(e).then((function(e) {
                         return e.output
@@ -62276,29 +62324,29 @@
                     }), (function(e) {
                         return o(e)
                     })).catch((function() {}))
                 }, e.prototype.destroy = function() {
                     this.config.requestHandler.destroy && this.config.requestHandler.destroy()
                 }, e
             }(),
-            bc = function() {
-                this.middlewareStack = yc()
+            jc = function() {
+                this.middlewareStack = mc()
             },
-            jc = function(e, t) {
-                return jc = Object.setPrototypeOf || {
+            wc = function(e, t) {
+                return wc = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, jc(e, t)
+                }, wc(e, t)
             };
 
-        function wc(e, t) {
+        function xc(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -62312,225 +62360,225 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function xc() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(wc(arguments[t]));
+        function Nc() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(xc(arguments[t]));
             return e
         }
-        var Nc = function() {
+        var Ic = function() {
             var e = Object.getPrototypeOf(this).constructor,
-                t = Function.bind.apply(String, xc([null], arguments)),
+                t = Function.bind.apply(String, Nc([null], arguments)),
                 n = new t;
             return Object.setPrototypeOf(n, e.prototype), n
         };
-        Nc.prototype = Object.create(String.prototype, {
+        Ic.prototype = Object.create(String.prototype, {
             constructor: {
-                value: Nc,
+                value: Ic,
                 enumerable: !1,
                 writable: !0,
                 configurable: !0
             }
-        }), Object.setPrototypeOf(Nc, String);
+        }), Object.setPrototypeOf(Ic, String);
         ! function(e) {
             function t() {
                 return null !== e && e.apply(this, arguments) || this
             }(function(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                jc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                wc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             })(t, e), t.prototype.deserializeJSON = function() {
                 return JSON.parse(e.prototype.toString.call(this))
             }, t.prototype.toJSON = function() {
                 return e.prototype.toString.call(this)
             }, t.fromObject = function(e) {
                 return e instanceof t ? e : new t(e instanceof String || "string" === typeof e ? e : JSON.stringify(e))
             }
-        }(Nc);
-        var Ic = function(e) {
+        }(Ic);
+        var Dc = function(e) {
                 function t(t) {
                     var n = e.call(this) || this;
                     return n.input = t, n
                 }
-                return mu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
-                    this.middlewareStack.use(dc(t, this.serialize, this.deserialize));
+                return vu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
+                    this.middlewareStack.use(fc(t, this.serialize, this.deserialize));
                     var r = e.concat(this.middlewareStack),
                         o = {
                             logger: t.logger,
                             clientName: "CognitoIdentityClient",
                             commandName: "GetCredentialsForIdentityCommand",
-                            inputFilterSensitiveLog: Yu.filterSensitiveLog,
-                            outputFilterSensitiveLog: Gu.filterSensitiveLog
+                            inputFilterSensitiveLog: Qu.filterSensitiveLog,
+                            outputFilterSensitiveLog: Wu.filterSensitiveLog
                         },
                         i = t.requestHandler;
                     return r.resolve((function(e) {
                         return i.handle(e.request, n || {})
                     }), o)
                 }, t.prototype.serialize = function(e, t) {
                     return function(e, t) {
-                        return Mu(void 0, void 0, void 0, (function() {
+                        return bu(void 0, void 0, void 0, (function() {
                             var n, r;
-                            return bu(this, (function(o) {
+                            return ju(this, (function(o) {
                                 return n = {
                                     "content-type": "application/x-amz-json-1.1",
                                     "x-amz-target": "AWSCognitoIdentityService.GetCredentialsForIdentity"
-                                }, r = JSON.stringify(Bl(e, t)), [2, rc(t, n, "/", void 0, r)]
+                                }, r = JSON.stringify(Fl(e, t)), [2, oc(t, n, "/", void 0, r)]
                             }))
                         }))
                     }(e, t)
                 }, t.prototype.deserialize = function(e, t) {
                     return function(e, t) {
-                        return Mu(void 0, void 0, void 0, (function() {
+                        return bu(void 0, void 0, void 0, (function() {
                             var n, r, o;
-                            return bu(this, (function(i) {
+                            return ju(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
-                                        return e.statusCode >= 300 ? [2, kl(e, t)] : [4, oc(e.body, t)];
+                                        return e.statusCode >= 300 ? [2, Cl(e, t)] : [4, ic(e.body, t)];
                                     case 1:
-                                        return n = i.sent(), r = Wl(n, t), o = vu({
-                                            $metadata: tc(e)
+                                        return n = i.sent(), r = Hl(n, t), o = Mu({
+                                            $metadata: nc(e)
                                         }, r), [2, Promise.resolve(o)]
                                 }
                             }))
                         }))
                     }(e, t)
                 }, t
-            }(bc),
-            Dc = function(e, t) {
-                return Dc = Object.setPrototypeOf || {
+            }(jc),
+            Sc = function(e, t) {
+                return Sc = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, Dc(e, t)
+                }, Sc(e, t)
             };
-        var Sc = function(e) {
+        var Lc = function(e) {
             function t(t, n) {
                 void 0 === n && (n = !0);
                 var r = e.call(this, t) || this;
                 return r.tryNextLink = n, r
             }
             return function(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                Dc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                Sc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             }(t, e), t
         }(Error);
 
-        function Lc(e) {
+        function kc(e) {
             return Promise.all(Object.keys(e).reduce((function(t, n) {
                 var r = e[n];
                 return "string" === typeof r ? t.push([n, r]) : t.push(r().then((function(e) {
                     return [n, e]
                 }))), t
             }), [])).then((function(e) {
                 return e.reduce((function(e, t) {
-                    var n = gu(t, 2),
+                    var n = yu(t, 2),
                         r = n[0],
                         o = n[1];
                     return e[r] = o, e
                 }), {})
             }))
         }
 
-        function kc(e) {
+        function Cc(e) {
             var t = this;
             return function() {
-                return pu(t, void 0, void 0, (function() {
+                return hu(t, void 0, void 0, (function() {
                     var t, n, r, o, i, a, s, u, l, c, d, f, p;
-                    return hu(this, (function(h) {
+                    return gu(this, (function(h) {
                         switch (h.label) {
                             case 0:
-                                return c = (l = e.client).send, d = Ic.bind, p = {
+                                return c = (l = e.client).send, d = Dc.bind, p = {
                                     CustomRoleArn: e.customRoleArn,
                                     IdentityId: e.identityId
-                                }, e.logins ? [4, Lc(e.logins)] : [3, 2];
+                                }, e.logins ? [4, kc(e.logins)] : [3, 2];
                             case 1:
                                 return f = h.sent(), [3, 3];
                             case 2:
                                 f = void 0, h.label = 3;
                             case 3:
-                                return [4, c.apply(l, [new(d.apply(Ic, [void 0, (p.Logins = f, p)]))])];
+                                return [4, c.apply(l, [new(d.apply(Dc, [void 0, (p.Logins = f, p)]))])];
                             case 4:
                                 return t = h.sent().Credentials, n = void 0 === t ? function() {
-                                    throw new Sc("Response from Amazon Cognito contained no credentials")
+                                    throw new Lc("Response from Amazon Cognito contained no credentials")
                                 }() : t, r = n.AccessKeyId, o = void 0 === r ? function() {
-                                    throw new Sc("Response from Amazon Cognito contained no access key ID")
+                                    throw new Lc("Response from Amazon Cognito contained no access key ID")
                                 }() : r, i = n.Expiration, a = n.SecretKey, s = void 0 === a ? function() {
-                                    throw new Sc("Response from Amazon Cognito contained no secret key")
+                                    throw new Lc("Response from Amazon Cognito contained no secret key")
                                 }() : a, u = n.SessionToken, [2, {
                                     identityId: e.identityId,
                                     accessKeyId: o,
                                     secretAccessKey: s,
                                     sessionToken: u,
                                     expiration: i
                                 }]
                         }
                     }))
                 }))
             }
         }
-        var Cc = function(e) {
+        var Ec = function(e) {
                 function t(t) {
                     var n = e.call(this) || this;
                     return n.input = t, n
                 }
-                return mu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
-                    this.middlewareStack.use(dc(t, this.serialize, this.deserialize));
+                return vu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
+                    this.middlewareStack.use(fc(t, this.serialize, this.deserialize));
                     var r = e.concat(this.middlewareStack),
                         o = {
                             logger: t.logger,
                             clientName: "CognitoIdentityClient",
                             commandName: "GetIdCommand",
-                            inputFilterSensitiveLog: Hu.filterSensitiveLog,
-                            outputFilterSensitiveLog: Zu.filterSensitiveLog
+                            inputFilterSensitiveLog: Zu.filterSensitiveLog,
+                            outputFilterSensitiveLog: Vu.filterSensitiveLog
                         },
                         i = t.requestHandler;
                     return r.resolve((function(e) {
                         return i.handle(e.request, n || {})
                     }), o)
                 }, t.prototype.serialize = function(e, t) {
                     return function(e, t) {
-                        return Mu(void 0, void 0, void 0, (function() {
+                        return bu(void 0, void 0, void 0, (function() {
                             var n, r;
-                            return bu(this, (function(o) {
+                            return ju(this, (function(o) {
                                 return n = {
                                     "content-type": "application/x-amz-json-1.1",
                                     "x-amz-target": "AWSCognitoIdentityService.GetId"
-                                }, r = JSON.stringify(Fl(e, t)), [2, rc(t, n, "/", void 0, r)]
+                                }, r = JSON.stringify(Yl(e, t)), [2, oc(t, n, "/", void 0, r)]
                             }))
                         }))
                     }(e, t)
                 }, t.prototype.deserialize = function(e, t) {
                     return function(e, t) {
-                        return Mu(void 0, void 0, void 0, (function() {
+                        return bu(void 0, void 0, void 0, (function() {
                             var n, r, o;
-                            return bu(this, (function(i) {
+                            return ju(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
-                                        return e.statusCode >= 300 ? [2, Cl(e, t)] : [4, oc(e.body, t)];
+                                        return e.statusCode >= 300 ? [2, El(e, t)] : [4, ic(e.body, t)];
                                     case 1:
-                                        return n = i.sent(), r = Hl(n, t), o = vu({
-                                            $metadata: tc(e)
+                                        return n = i.sent(), r = Zl(n, t), o = Mu({
+                                            $metadata: nc(e)
                                         }, r), [2, Promise.resolve(o)]
                                 }
                             }))
                         }))
                     }(e, t)
                 }, t
-            }(bc),
-            Ec = "IdentityIds",
-            _c = function() {
+            }(jc),
+            _c = "IdentityIds",
+            Tc = function() {
                 function e(e) {
                     void 0 === e && (e = "aws:cognito-identity-ids"), this.dbName = e
                 }
                 return e.prototype.getItem = function(e) {
                     return this.withObjectStore("readonly", (function(t) {
                         var n = t.get(e);
                         return new Promise((function(e) {
@@ -62577,106 +62625,106 @@
                             n(e.error)
                         }, e.onblocked = function() {
                             n(new Error("Unable to access DB"))
                         }, e.onupgradeneeded = function() {
                             var t = e.result;
                             t.onerror = function() {
                                 n(new Error("Failed to create object store"))
-                            }, t.createObjectStore(Ec, {
+                            }, t.createObjectStore(_c, {
                                 keyPath: "id"
                             })
                         }
                     }))
                 }, e.prototype.withObjectStore = function(e, t) {
                     return this.getDb().then((function(n) {
-                        var r = n.transaction(Ec, e);
+                        var r = n.transaction(_c, e);
                         return r.oncomplete = function() {
                             return n.close()
                         }, new Promise((function(e, n) {
                             r.onerror = function() {
                                 return n(r.error)
-                            }, e(t(r.objectStore(Ec)))
+                            }, e(t(r.objectStore(_c)))
                         })).catch((function(e) {
                             throw n.close(), e
                         }))
                     }))
                 }, e
             }(),
-            Tc = new(function() {
+            Ac = new(function() {
                 function e(e) {
                     void 0 === e && (e = {}), this.store = e
                 }
                 return e.prototype.getItem = function(e) {
                     return e in this.store ? this.store[e] : null
                 }, e.prototype.removeItem = function(e) {
                     delete this.store[e]
                 }, e.prototype.setItem = function(e, t) {
                     this.store[e] = t
                 }, e
             }());
 
-        function Ac(e) {
+        function Oc(e) {
             var t = this,
                 n = e.accountId,
                 r = e.cache,
-                o = void 0 === r ? "object" === typeof self && self.indexedDB ? new _c : "object" === typeof window && window.localStorage ? window.localStorage : Tc : r,
+                o = void 0 === r ? "object" === typeof self && self.indexedDB ? new Tc : "object" === typeof window && window.localStorage ? window.localStorage : Ac : r,
                 i = e.client,
                 a = e.customRoleArn,
                 s = e.identityPoolId,
                 u = e.logins,
                 l = e.userIdentifier,
                 c = void 0 === l ? u && 0 !== Object.keys(u).length ? void 0 : "ANONYMOUS" : l,
                 d = c ? "aws:cognito-identity-credentials:" + s + ":" + c : void 0,
                 f = function() {
-                    return pu(t, void 0, void 0, (function() {
+                    return hu(t, void 0, void 0, (function() {
                         var e, t, r, l, c, p, h, g, y;
-                        return hu(this, (function(m) {
+                        return gu(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return (t = d) ? [4, o.getItem(d)] : [3, 2];
                                 case 1:
                                     t = m.sent(), m.label = 2;
                                 case 2:
-                                    return (e = t) ? [3, 7] : (p = (c = i).send, h = Cc.bind, y = {
+                                    return (e = t) ? [3, 7] : (p = (c = i).send, h = Ec.bind, y = {
                                         AccountId: n,
                                         IdentityPoolId: s
-                                    }, u ? [4, Lc(u)] : [3, 4]);
+                                    }, u ? [4, kc(u)] : [3, 4]);
                                 case 3:
                                     return g = m.sent(), [3, 5];
                                 case 4:
                                     g = void 0, m.label = 5;
                                 case 5:
-                                    return [4, p.apply(c, [new(h.apply(Cc, [void 0, (y.Logins = g, y)]))])];
+                                    return [4, p.apply(c, [new(h.apply(Ec, [void 0, (y.Logins = g, y)]))])];
                                 case 6:
                                     r = m.sent().IdentityId, l = void 0 === r ? function() {
-                                        throw new Sc("Response from Amazon Cognito contained no identity ID")
+                                        throw new Lc("Response from Amazon Cognito contained no identity ID")
                                     }() : r, e = l, d && Promise.resolve(o.setItem(d, e)).catch((function() {})), m.label = 7;
                                 case 7:
-                                    return [2, (f = kc({
+                                    return [2, (f = Cc({
                                         client: i,
                                         customRoleArn: a,
                                         logins: u,
                                         identityId: e
                                     }))()]
                             }
                         }))
                     }))
                 };
             return function() {
                 return f().catch((function(e) {
-                    return pu(t, void 0, void 0, (function() {
-                        return hu(this, (function(t) {
+                    return hu(t, void 0, void 0, (function() {
+                        return gu(this, (function(t) {
                             throw d && Promise.resolve(o.removeItem(d)).catch((function() {})), e
                         }))
                     }))
                 }))
             }
         }
-        var Oc = new Gs("Parser"),
-            zc = function(e) {
+        var zc = new Ws("Parser"),
+            Uc = function(e) {
                 var t, n = {};
                 if (e.aws_mobile_analytics_app_id) {
                     var r = {
                         AWSPinpoint: {
                             appId: e.aws_mobile_analytics_app_id,
                             region: e.aws_mobile_analytics_app_region
                         }
@@ -62693,23 +62741,23 @@
                     signUpVerificationMethod: e.aws_cognito_sign_up_verification_method || "code"
                 }), t = e.aws_user_files_s3_bucket ? {
                     AWSS3: {
                         bucket: e.aws_user_files_s3_bucket,
                         region: e.aws_user_files_s3_bucket_region,
                         dangerouslyConnectToHttpEndpointForTesting: e.aws_user_files_s3_dangerously_connect_to_http_endpoint_for_testing
                     }
-                } : e ? e.Storage || e : {}, e.Logging && (n.Logging = zs(zs({}, e.Logging), {
+                } : e ? e.Storage || e : {}, e.Logging && (n.Logging = Us(Us({}, e.Logging), {
                     region: e.aws_project_region
                 })), e.geo && (n.Geo = Object.assign({}, e.geo), e.geo.amazon_location_service && (n.Geo = {
                     AmazonLocationService: e.geo.amazon_location_service
-                })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), Oc.debug("parse config", e, "to amplifyconfig", n), n
+                })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), zc.debug("parse config", e, "to amplifyconfig", n), n
             },
-            Uc = __webpack_require__(3219);
+            Pc = __webpack_require__(3219);
 
-        function Pc(e, t, n, r) {
+        function Rc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62729,15 +62777,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Rc(e, t) {
+        function Bc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62805,15 +62853,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Bc(e) {
+        function Fc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -62821,36 +62869,36 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Fc(e) {
+        function Yc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
                         value: e && e[r++],
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
-        var Yc = function(e) {
-                return encodeURIComponent(e).replace(/[!'()*]/g, Qc)
+        var Qc = function(e) {
+                return encodeURIComponent(e).replace(/[!'()*]/g, Gc)
             },
-            Qc = function(e) {
+            Gc = function(e) {
                 return "%" + e.charCodeAt(0).toString(16).toUpperCase()
             };
-        for (var Gc = function() {
+        for (var Wc = function() {
                 function e(e) {
                     var t = (void 0 === e ? {} : e).requestTimeout;
                     this.requestTimeout = t
                 }
                 return e.prototype.destroy = function() {}, e.prototype.handle = function(e, t) {
                     var n = (void 0 === t ? {} : t).abortSignal,
                         r = this.requestTimeout;
@@ -62859,22 +62907,22 @@
                         return o.name = "AbortError", Promise.reject(o)
                     }
                     var i = e.path;
                     if (e.query) {
                         var a = function(e) {
                             var t, n, r = [];
                             try {
-                                for (var o = Fc(Object.keys(e).sort()), i = o.next(); !i.done; i = o.next()) {
+                                for (var o = Yc(Object.keys(e).sort()), i = o.next(); !i.done; i = o.next()) {
                                     var a = i.value,
                                         s = e[a];
-                                    if (a = Yc(a), Array.isArray(s))
-                                        for (var u = 0, l = s.length; u < l; u++) r.push(a + "=" + Yc(s[u]));
+                                    if (a = Qc(a), Array.isArray(s))
+                                        for (var u = 0, l = s.length; u < l; u++) r.push(a + "=" + Qc(s[u]));
                                     else {
                                         var c = a;
-                                        (s || "string" === typeof s) && (c += "=" + Yc(s)), r.push(c)
+                                        (s || "string" === typeof s) && (c += "=" + Qc(s)), r.push(c)
                                     }
                                 }
                             } catch (d) {
                                 t = {
                                     error: d
                                 }
                             } finally {
@@ -62898,15 +62946,15 @@
                         };
                     "undefined" !== typeof AbortController && (c.signal = n);
                     var d, f = new Request(l, c),
                         p = [fetch(f).then((function(e) {
                             var t, n, r = e.headers,
                                 o = {};
                             try {
-                                for (var i = Bc(r.entries()), a = i.next(); !a.done; a = i.next()) {
+                                for (var i = Fc(r.entries()), a = i.next(); !a.done; a = i.next()) {
                                     var s = a.value;
                                     o[s[0]] = s[1]
                                 }
                             } catch (u) {
                                 t = {
                                     error: u
                                 }
@@ -62914,22 +62962,22 @@
                                 try {
                                     a && !a.done && (n = i.return) && n.call(i)
                                 } finally {
                                     if (t) throw t.error
                                 }
                             }
                             return void 0 !== e.body ? {
-                                response: new Il({
+                                response: new Dl({
                                     headers: o,
                                     statusCode: e.status,
                                     body: e.body
                                 })
                             } : e.blob().then((function(t) {
                                 return {
-                                    response: new Il({
+                                    response: new Dl({
                                         headers: o,
                                         statusCode: e.status,
                                         body: t
                                     })
                                 }
                             }))
                         })), (d = r, void 0 === d && (d = 0), new Promise((function(e, t) {
@@ -62941,46 +62989,46 @@
                     return n && p.push(new Promise((function(e, t) {
                         n.onabort = function() {
                             var e = new Error("Request aborted");
                             e.name = "AbortError", t(e)
                         }
                     }))), Promise.race(p)
                 }, e
-            }(), Wc = {}, Hc = new Array(64), Zc = 0, Vc = "A".charCodeAt(0), qc = "Z".charCodeAt(0); Zc + Vc <= qc; Zc++) {
-            var Jc = String.fromCharCode(Zc + Vc);
-            Wc[Jc] = Zc, Hc[Zc] = Jc
-        }
-        for (Zc = 0, Vc = "a".charCodeAt(0), qc = "z".charCodeAt(0); Zc + Vc <= qc; Zc++) {
-            Jc = String.fromCharCode(Zc + Vc);
-            var Kc = Zc + 26;
-            Wc[Jc] = Kc, Hc[Kc] = Jc
-        }
-        for (Zc = 0; Zc < 10; Zc++) {
-            Wc[Zc.toString(10)] = Zc + 52;
-            Jc = Zc.toString(10), Kc = Zc + 52;
-            Wc[Jc] = Kc, Hc[Kc] = Jc
+            }(), Hc = {}, Zc = new Array(64), Vc = 0, qc = "A".charCodeAt(0), Jc = "Z".charCodeAt(0); Vc + qc <= Jc; Vc++) {
+            var Kc = String.fromCharCode(Vc + qc);
+            Hc[Kc] = Vc, Zc[Vc] = Kc
+        }
+        for (Vc = 0, qc = "a".charCodeAt(0), Jc = "z".charCodeAt(0); Vc + qc <= Jc; Vc++) {
+            Kc = String.fromCharCode(Vc + qc);
+            var Xc = Vc + 26;
+            Hc[Kc] = Xc, Zc[Xc] = Kc
+        }
+        for (Vc = 0; Vc < 10; Vc++) {
+            Hc[Vc.toString(10)] = Vc + 52;
+            Kc = Vc.toString(10), Xc = Vc + 52;
+            Hc[Kc] = Xc, Zc[Xc] = Kc
         }
-        Wc["+"] = 62, Hc[62] = "+", Wc["/"] = 63, Hc[63] = "/";
+        Hc["+"] = 62, Zc[62] = "+", Hc["/"] = 63, Zc[63] = "/";
 
-        function Xc(e) {
+        function $c(e) {
             var t = e.length / 4 * 3;
             "==" === e.substr(-2) ? t -= 2 : "=" === e.substr(-1) && t--;
             for (var n = new ArrayBuffer(t), r = new DataView(n), o = 0; o < e.length; o += 4) {
-                for (var i = 0, a = 0, s = o, u = o + 3; s <= u; s++) "=" !== e[s] ? (i |= Wc[e[s]] << 6 * (u - s), a += 6) : i >>= 6;
+                for (var i = 0, a = 0, s = o, u = o + 3; s <= u; s++) "=" !== e[s] ? (i |= Hc[e[s]] << 6 * (u - s), a += 6) : i >>= 6;
                 var l = o / 4 * 3;
                 i >>= a % 8;
                 for (var c = Math.floor(a / 8), d = 0; d < c; d++) {
                     var f = 8 * (c - d - 1);
                     r.setUint8(l + d, (i & 255 << f) >> f)
                 }
             }
             return new Uint8Array(n)
         }
 
-        function $c(e) {
+        function ed(e) {
             return new Promise((function(t, n) {
                 var r = new FileReader;
                 r.onloadend = function() {
                     var e;
                     if (2 !== r.readyState) return n(new Error("Reader aborted too early"));
                     var o = null !== (e = r.result) && void 0 !== e ? e : "",
                         i = o.indexOf(","),
@@ -62989,23 +63037,23 @@
                 }, r.onabort = function() {
                     return n(new Error("Read aborted"))
                 }, r.onerror = function() {
                     return n(r.error)
                 }, r.readAsDataURL(e)
             }))
         }
-        var ed = function() {
-            return ed = Object.assign || function(e) {
+        var td = function() {
+            return td = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, ed.apply(this, arguments)
+            }, td.apply(this, arguments)
         };
 
-        function td(e, t, n, r) {
+        function nd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63025,15 +63073,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function nd(e, t) {
+        function rd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63101,15 +63149,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function rd(e, t) {
+        function od(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -63122,65 +63170,65 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var od = function(e) {
+        var id = function(e) {
                 return function(t, n) {
                     return function(r) {
-                        return td(void 0, void 0, void 0, (function() {
+                        return nd(void 0, void 0, void 0, (function() {
                             var o;
-                            return nd(this, (function(i) {
+                            return rd(this, (function(i) {
                                 return (null === (o = null === e || void 0 === e ? void 0 : e.retryStrategy) || void 0 === o ? void 0 : o.mode) && (n.userAgent = function() {
-                                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(rd(arguments[t]));
+                                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(od(arguments[t]));
                                     return e
                                 }(n.userAgent || [], [
                                     ["cfg/retry-mode", e.retryStrategy.mode]
                                 ])), [2, e.retryStrategy.retry(t, r)]
                             }))
                         }))
                     }
                 }
             },
-            id = {
+            ad = {
                 name: "retryMiddleware",
                 tags: ["RETRY"],
                 step: "finalizeRequest",
                 priority: "high",
                 override: !0
             },
-            ad = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch"],
-            sd = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException", "TransactionInProgressException"],
-            ud = ["AbortError", "TimeoutError", "RequestTimeout", "RequestTimeoutException"],
-            ld = [500, 502, 503, 504],
-            cd = function(e) {
+            sd = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch"],
+            ud = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException", "TransactionInProgressException"],
+            ld = ["AbortError", "TimeoutError", "RequestTimeout", "RequestTimeoutException"],
+            cd = [500, 502, 503, 504],
+            dd = function(e) {
                 var t, n;
-                return 429 === (null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || sd.includes(e.name) || 1 == (null === (n = e.$retryable) || void 0 === n ? void 0 : n.throttling)
+                return 429 === (null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || ud.includes(e.name) || 1 == (null === (n = e.$retryable) || void 0 === n ? void 0 : n.throttling)
             },
-            dd = __webpack_require__(6231),
-            fd = function(e, t) {
+            fd = __webpack_require__(6231),
+            pd = function(e, t) {
                 return Math.floor(Math.min(2e4, Math.random() * Math.pow(2, t) * e))
             },
-            pd = function(e) {
+            hd = function(e) {
                 return !!e && (function(e) {
                     return void 0 !== e.$retryable
                 }(e) || function(e) {
-                    return ad.includes(e.name)
-                }(e) || cd(e) || function(e) {
+                    return sd.includes(e.name)
+                }(e) || dd(e) || function(e) {
                     var t;
-                    return ud.includes(e.name) || ld.includes((null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || 0)
+                    return ld.includes(e.name) || cd.includes((null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || 0)
                 }(e))
             },
-            hd = "standard",
-            gd = function() {
+            gd = "standard",
+            yd = function() {
                 function e(e, t) {
                     var n, r, o;
-                    this.maxAttemptsProvider = e, this.mode = hd, this.retryDecider = null !== (n = null === t || void 0 === t ? void 0 : t.retryDecider) && void 0 !== n ? n : pd, this.delayDecider = null !== (r = null === t || void 0 === t ? void 0 : t.delayDecider) && void 0 !== r ? r : fd, this.retryQuota = null !== (o = null === t || void 0 === t ? void 0 : t.retryQuota) && void 0 !== o ? o : function(e) {
+                    this.maxAttemptsProvider = e, this.mode = gd, this.retryDecider = null !== (n = null === t || void 0 === t ? void 0 : t.retryDecider) && void 0 !== n ? n : hd, this.delayDecider = null !== (r = null === t || void 0 === t ? void 0 : t.delayDecider) && void 0 !== r ? r : pd, this.retryQuota = null !== (o = null === t || void 0 === t ? void 0 : t.retryQuota) && void 0 !== o ? o : function(e) {
                         var t = e,
                             n = e,
                             r = function(e) {
                                 return "TimeoutError" === e.name ? 10 : 5
                             },
                             o = function(e) {
                                 return r(e) <= n
@@ -63197,52 +63245,52 @@
                             }
                         })
                     }(500)
                 }
                 return e.prototype.shouldRetry = function(e, t, n) {
                     return t < n && this.retryDecider(e) && this.retryQuota.hasRetryTokens(e)
                 }, e.prototype.getMaxAttempts = function() {
-                    return td(this, void 0, void 0, (function() {
+                    return nd(this, void 0, void 0, (function() {
                         var e;
-                        return nd(this, (function(t) {
+                        return rd(this, (function(t) {
                             switch (t.label) {
                                 case 0:
                                     return t.trys.push([0, 2, , 3]), [4, this.maxAttemptsProvider()];
                                 case 1:
                                     return e = t.sent(), [3, 3];
                                 case 2:
                                     return t.sent(), e = 3, [3, 3];
                                 case 3:
                                     return [2, e]
                             }
                         }))
                     }))
                 }, e.prototype.retry = function(e, t) {
-                    return td(this, void 0, void 0, (function() {
+                    return nd(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u, l;
-                        return nd(this, (function(c) {
+                        return rd(this, (function(c) {
                             switch (c.label) {
                                 case 0:
                                     return r = 0, o = 0, [4, this.getMaxAttempts()];
                                 case 1:
-                                    i = c.sent(), a = t.request, Ll.isInstance(a) && (a.headers["amz-sdk-invocation-id"] = (0, dd.v4)()), s = function() {
+                                    i = c.sent(), a = t.request, kl.isInstance(a) && (a.headers["amz-sdk-invocation-id"] = (0, fd.v4)()), s = function() {
                                         var s, l, c, d, f;
-                                        return nd(this, (function(p) {
+                                        return rd(this, (function(p) {
                                             switch (p.label) {
                                                 case 0:
-                                                    return p.trys.push([0, 2, , 5]), Ll.isInstance(a) && (a.headers["amz-sdk-request"] = "attempt=" + (r + 1) + "; max=" + i), [4, e(t)];
+                                                    return p.trys.push([0, 2, , 5]), kl.isInstance(a) && (a.headers["amz-sdk-request"] = "attempt=" + (r + 1) + "; max=" + i), [4, e(t)];
                                                 case 1:
                                                     return s = p.sent(), l = s.response, c = s.output, u.retryQuota.releaseRetryTokens(n), c.$metadata.attempts = r + 1, c.$metadata.totalRetryDelay = o, [2, {
                                                         value: {
                                                             response: l,
                                                             output: c
                                                         }
                                                     }];
                                                 case 2:
-                                                    return d = p.sent(), r++, u.shouldRetry(d, r, i) ? (n = u.retryQuota.retrieveRetryTokens(d), f = u.delayDecider(cd(d) ? 500 : 100, r), o += f, [4, new Promise((function(e) {
+                                                    return d = p.sent(), r++, u.shouldRetry(d, r, i) ? (n = u.retryQuota.retrieveRetryTokens(d), f = u.delayDecider(dd(d) ? 500 : 100, r), o += f, [4, new Promise((function(e) {
                                                         return setTimeout(e, f)
                                                     }))]) : [3, 4];
                                                 case 3:
                                                     return p.sent(), [2, "continue"];
                                                 case 4:
                                                     throw d.$metadata || (d.$metadata = {}), d.$metadata.attempts = r, d.$metadata.totalRetryDelay = o, d;
                                                 case 5:
@@ -63257,25 +63305,25 @@
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e
             }(),
-            yd = function(e) {
+            md = function(e) {
                 if (void 0 === e && (e = 3), "number" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
 
-        function md(e, t, n, r) {
+        function vd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63295,15 +63343,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function vd(e, t) {
+        function Md(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63370,25 +63418,25 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Md = __webpack_require__(984),
-            bd = __webpack_require__.n(Md),
-            jd = __webpack_require__(5863),
-            wd = "cognito-identity.{region}.amazonaws.com",
-            xd = new Set(["af-south-1", "ap-east-1", "ap-northeast-1", "ap-northeast-2", "ap-south-1", "ap-southeast-1", "ap-southeast-2", "ca-central-1", "eu-central-1", "eu-north-1", "eu-south-1", "eu-west-1", "eu-west-2", "eu-west-3", "me-south-1", "sa-east-1", "us-east-1", "us-east-2", "us-west-1", "us-west-2"]),
-            Nd = new Set(["cn-north-1", "cn-northwest-1"]),
-            Id = new Set(["us-iso-east-1"]),
-            Dd = new Set(["us-isob-east-1"]),
-            Sd = new Set(["us-gov-east-1", "us-gov-west-1"]);
+        var bd = __webpack_require__(984),
+            jd = __webpack_require__.n(bd),
+            wd = __webpack_require__(5863),
+            xd = "cognito-identity.{region}.amazonaws.com",
+            Nd = new Set(["af-south-1", "ap-east-1", "ap-northeast-1", "ap-northeast-2", "ap-south-1", "ap-southeast-1", "ap-southeast-2", "ca-central-1", "eu-central-1", "eu-north-1", "eu-south-1", "eu-west-1", "eu-west-2", "eu-west-3", "me-south-1", "sa-east-1", "us-east-1", "us-east-2", "us-west-1", "us-west-2"]),
+            Id = new Set(["cn-north-1", "cn-northwest-1"]),
+            Dd = new Set(["us-iso-east-1"]),
+            Sd = new Set(["us-isob-east-1"]),
+            Ld = new Set(["us-gov-east-1", "us-gov-west-1"]);
 
-        function Ld(e) {
+        function kd(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -63396,15 +63444,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function kd(e, t) {
+        function Cd(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -63417,15 +63465,15 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var Cd, Ed = {
+        var Ed, _d = {
                 apiVersion: "2014-06-30",
                 disableHostPrefix: !1,
                 logger: {},
                 regionInfoProvider: function(e, t) {
                     var n = void 0;
                     switch (e) {
                         case "ap-northeast-1":
@@ -63561,51 +63609,51 @@
                         case "us-west-2":
                             n = {
                                 hostname: "cognito-identity.us-west-2.amazonaws.com",
                                 partition: "aws"
                             };
                             break;
                         default:
-                            xd.has(e) && (n = {
-                                hostname: wd.replace("{region}", e),
+                            Nd.has(e) && (n = {
+                                hostname: xd.replace("{region}", e),
                                 partition: "aws"
-                            }), Nd.has(e) && (n = {
+                            }), Id.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.amazonaws.com.cn".replace("{region}", e),
                                 partition: "aws-cn"
-                            }), Id.has(e) && (n = {
+                            }), Dd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.c2s.ic.gov".replace("{region}", e),
                                 partition: "aws-iso"
-                            }), Dd.has(e) && (n = {
+                            }), Sd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.sc2s.sgov.gov".replace("{region}", e),
                                 partition: "aws-iso-b"
-                            }), Sd.has(e) && (n = {
+                            }), Ld.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.amazonaws.com".replace("{region}", e),
                                 partition: "aws-us-gov"
                             }), void 0 === n && (n = {
-                                hostname: wd.replace("{region}", e),
+                                hostname: xd.replace("{region}", e),
                                 partition: "aws"
                             })
                     }
-                    return Promise.resolve(vu({
+                    return Promise.resolve(Mu({
                         signingService: "cognito-identity"
                     }, n))
                 },
                 serviceId: "Cognito Identity",
                 urlParser: function(e) {
                     var t, n = new URL(e),
                         r = n.hostname,
                         o = n.pathname,
                         i = n.port,
                         a = n.protocol,
                         s = n.search;
                     return s && (t = function(e) {
                         var t, n, r = {};
                         if (e = e.replace(/^\?/, "")) try {
-                            for (var o = Ld(e.split("&")), i = o.next(); !i.done; i = o.next()) {
-                                var a = kd(i.value.split("="), 2),
+                            for (var o = kd(e.split("&")), i = o.next(); !i.done; i = o.next()) {
+                                var a = Cd(i.value.split("="), 2),
                                     s = a[0],
                                     u = a[1],
                                     l = void 0 === u ? null : u;
                                 s = decodeURIComponent(s), l && (l = decodeURIComponent(l)), s in r ? Array.isArray(r[s]) ? r[s].push(l) : r[s] = [r[s], l] : r[s] = l
                             }
                         } catch (c) {
                             t = {
@@ -63624,25 +63672,25 @@
                         port: i ? parseInt(i) : void 0,
                         protocol: a,
                         path: o,
                         query: t
                     }
                 }
             },
-            _d = vu(vu({}, Ed), {
+            Td = Mu(Mu({}, _d), {
                 runtime: "browser",
-                base64Decoder: Xc,
+                base64Decoder: $c,
                 base64Encoder: function(e) {
                     for (var t = "", n = 0; n < e.length; n += 3) {
                         for (var r = 0, o = 0, i = n, a = Math.min(n + 3, e.length); i < a; i++) r |= e[i] << 8 * (a - i - 1), o += 8;
                         var s = Math.ceil(o / 6);
                         r <<= 6 * s - o;
                         for (var u = 1; u <= s; u++) {
                             var l = 6 * (s - u);
-                            t += Hc[(r & 63 << l) >> l]
+                            t += Zc[(r & 63 << l) >> l]
                         }
                         t += "==".slice(0, 4 - s)
                     }
                     return t
                 },
                 bodyLengthChecker: function(e) {
                     if ("string" === typeof e) {
@@ -63659,79 +63707,79 @@
                         return Promise.reject(new Error("Credential is missing"))
                     }
                 },
                 defaultUserAgentProvider: function(e) {
                     var t = e.serviceId,
                         n = e.clientVersion;
                     return function() {
-                        return md(void 0, void 0, void 0, (function() {
+                        return vd(void 0, void 0, void 0, (function() {
                             var e, r, o, i, a, s, u, l, c;
-                            return vd(this, (function(d) {
-                                return e = (null === (o = null === window || void 0 === window ? void 0 : window.navigator) || void 0 === o ? void 0 : o.userAgent) ? bd().parse(window.navigator.userAgent) : void 0, r = [
+                            return Md(this, (function(d) {
+                                return e = (null === (o = null === window || void 0 === window ? void 0 : window.navigator) || void 0 === o ? void 0 : o.userAgent) ? jd().parse(window.navigator.userAgent) : void 0, r = [
                                     ["aws-sdk-js", n],
                                     ["os/" + ((null === (i = null === e || void 0 === e ? void 0 : e.os) || void 0 === i ? void 0 : i.name) || "other"), null === (a = null === e || void 0 === e ? void 0 : e.os) || void 0 === a ? void 0 : a.version],
                                     ["lang/js"],
                                     ["md/browser", (null !== (u = null === (s = null === e || void 0 === e ? void 0 : e.browser) || void 0 === s ? void 0 : s.name) && void 0 !== u ? u : "unknown") + "_" + (null !== (c = null === (l = null === e || void 0 === e ? void 0 : e.browser) || void 0 === l ? void 0 : l.version) && void 0 !== c ? c : "unknown")]
                                 ], t && r.push(["api/" + t, n]), [2, r]
                             }))
                         }))
                     }
                 }({
-                    serviceId: Ed.serviceId,
+                    serviceId: _d.serviceId,
                     clientVersion: "3.6.1"
                 }),
                 maxAttempts: 3,
-                region: (Cd = "Region is missing", function() {
-                    return Promise.reject(Cd)
+                region: (Ed = "Region is missing", function() {
+                    return Promise.reject(Ed)
                 }),
-                requestHandler: new Gc,
-                sha256: Uc.Sha256,
+                requestHandler: new Wc,
+                sha256: Pc.Sha256,
                 streamCollector: function(e) {
                     return "function" === typeof Blob && e instanceof Blob ? function(e) {
-                        return Pc(this, void 0, void 0, (function() {
+                        return Rc(this, void 0, void 0, (function() {
                             var t, n;
-                            return Rc(this, (function(r) {
+                            return Bc(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
-                                        return [4, $c(e)];
+                                        return [4, ed(e)];
                                     case 1:
-                                        return t = r.sent(), n = Xc(t), [2, new Uint8Array(n)]
+                                        return t = r.sent(), n = $c(t), [2, new Uint8Array(n)]
                                 }
                             }))
                         }))
                     }(e) : function(e) {
-                        return Pc(this, void 0, void 0, (function() {
+                        return Rc(this, void 0, void 0, (function() {
                             var t, n, r, o, i, a, s;
-                            return Rc(this, (function(u) {
+                            return Bc(this, (function(u) {
                                 switch (u.label) {
                                     case 0:
                                         t = new Uint8Array(0), n = e.getReader(), r = !1, u.label = 1;
                                     case 1:
                                         return r ? [3, 3] : [4, n.read()];
                                     case 2:
                                         return o = u.sent(), i = o.done, (a = o.value) && (s = t, (t = new Uint8Array(s.length + a.length)).set(s), t.set(a, s.length)), r = i, [3, 1];
                                     case 3:
                                         return [2, t]
                                 }
                             }))
                         }))
                     }(e)
                 },
-                utf8Decoder: jd.fromUtf8,
-                utf8Encoder: jd.toUtf8
+                utf8Decoder: wd.fromUtf8,
+                utf8Encoder: wd.toUtf8
             });
-        var Td = function() {
-            return Td = Object.assign || function(e) {
+        var Ad = function() {
+            return Ad = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Td.apply(this, arguments)
+            }, Ad.apply(this, arguments)
         };
 
-        function Ad(e, t, n, r) {
+        function Od(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63751,15 +63799,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Od(e, t) {
+        function zd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63826,15 +63874,15 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var zd = function(e) {
+        var Ud = function(e) {
                 var t = e.endpoint,
                     n = e.urlParser;
                 if ("string" === typeof t) {
                     var r = Promise.resolve(n(t));
                     return function() {
                         return r
                     }
@@ -63843,49 +63891,49 @@
                     var o = Promise.resolve(t);
                     return function() {
                         return o
                     }
                 }
                 return t
             },
-            Ud = function(e) {
-                return Ad(void 0, void 0, void 0, (function() {
+            Pd = function(e) {
+                return Od(void 0, void 0, void 0, (function() {
                     var t, n, r, o, i;
-                    return Od(this, (function(a) {
+                    return zd(this, (function(a) {
                         switch (a.label) {
                             case 0:
                                 return t = e.tls, n = void 0 === t || t, [4, e.region()];
                             case 1:
                                 if (r = a.sent(), !new RegExp(/^([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9-]{0,61}[a-zA-Z0-9])$/).test(r)) throw new Error("Invalid region in client config");
                                 return [4, e.regionInfoProvider(r)];
                             case 2:
                                 if (!(o = (null !== (i = a.sent()) && void 0 !== i ? i : {}).hostname)) throw new Error("Cannot resolve hostname from client config");
                                 return [2, e.urlParser((n ? "https:" : "http:") + "//" + o)]
                         }
                     }))
                 }))
             },
-            Pd = function(e) {
+            Rd = function(e) {
                 if ("string" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
-        var Rd = function() {
-            return Rd = Object.assign || function(e) {
+        var Bd = function() {
+            return Bd = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Rd.apply(this, arguments)
+            }, Bd.apply(this, arguments)
         };
 
-        function Bd(e, t, n, r) {
+        function Fd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63905,15 +63953,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Fd(e, t) {
+        function Yd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63980,46 +64028,46 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Yd = "content-length";
-        var Qd = {
+        var Qd = "content-length";
+        var Gd = {
                 step: "build",
                 tags: ["SET_CONTENT_LENGTH", "CONTENT_LENGTH"],
                 name: "contentLengthMiddleware",
                 override: !0
             },
-            Gd = function(e) {
+            Wd = function(e) {
                 return {
                     applyToStack: function(t) {
                         t.add(function(e) {
                             var t = this;
                             return function(n) {
                                 return function(r) {
-                                    return Bd(t, void 0, void 0, (function() {
+                                    return Fd(t, void 0, void 0, (function() {
                                         var t, o, i, a, s;
-                                        return Fd(this, (function(u) {
-                                            return t = r.request, Ll.isInstance(t) && (o = t.body, i = t.headers, o && -1 === Object.keys(i).map((function(e) {
+                                        return Yd(this, (function(u) {
+                                            return t = r.request, kl.isInstance(t) && (o = t.body, i = t.headers, o && -1 === Object.keys(i).map((function(e) {
                                                 return e.toLowerCase()
-                                            })).indexOf(Yd) && void 0 !== (a = e(o)) && (t.headers = Rd(Rd({}, t.headers), ((s = {})["content-length"] = String(a), s)))), [2, n(Rd(Rd({}, r), {
+                                            })).indexOf(Qd) && void 0 !== (a = e(o)) && (t.headers = Bd(Bd({}, t.headers), ((s = {})["content-length"] = String(a), s)))), [2, n(Bd(Bd({}, r), {
                                                 request: t
                                             }))]
                                         }))
                                     }))
                                 }
                             }
-                        }(e.bodyLengthChecker), Qd)
+                        }(e.bodyLengthChecker), Gd)
                     }
                 }
             };
 
-        function Wd(e, t, n, r) {
+        function Hd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64039,15 +64087,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Hd(e, t) {
+        function Zd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64114,41 +64162,41 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Zd = {
+        var Vd = {
                 name: "hostHeaderMiddleware",
                 step: "build",
                 priority: "low",
                 tags: ["HOST"],
                 override: !0
             },
-            Vd = function(e) {
+            qd = function(e) {
                 return {
                     applyToStack: function(t) {
                         t.add(function(e) {
                             return function(t) {
                                 return function(n) {
-                                    return Wd(void 0, void 0, void 0, (function() {
+                                    return Hd(void 0, void 0, void 0, (function() {
                                         var r, o;
-                                        return Hd(this, (function(i) {
-                                            return Ll.isInstance(n.request) ? (r = n.request, (void 0 === (o = (e.requestHandler.metadata || {}).handlerProtocol) ? "" : o).indexOf("h2") >= 0 && !r.headers[":authority"] ? (delete r.headers.host, r.headers[":authority"] = "") : r.headers.host || (r.headers.host = r.hostname), [2, t(n)]) : [2, t(n)]
+                                        return Zd(this, (function(i) {
+                                            return kl.isInstance(n.request) ? (r = n.request, (void 0 === (o = (e.requestHandler.metadata || {}).handlerProtocol) ? "" : o).indexOf("h2") >= 0 && !r.headers[":authority"] ? (delete r.headers.host, r.headers[":authority"] = "") : r.headers.host || (r.headers.host = r.hostname), [2, t(n)]) : [2, t(n)]
                                         }))
                                     }))
                                 }
                             }
-                        }(e), Zd)
+                        }(e), Vd)
                     }
                 }
             };
 
-        function qd(e, t, n, r) {
+        function Jd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64168,15 +64216,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Jd(e, t) {
+        function Kd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64243,20 +64291,20 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Kd = function() {
+        var Xd = function() {
                 return function(e, t) {
                     return function(n) {
-                        return qd(void 0, void 0, void 0, (function() {
+                        return Jd(void 0, void 0, void 0, (function() {
                             var r, o, i, a, s, u, l, c, d;
-                            return Jd(this, (function(f) {
+                            return Kd(this, (function(f) {
                                 switch (f.label) {
                                     case 0:
                                         return r = t.clientName, o = t.commandName, i = t.inputFilterSensitiveLog, a = t.logger, s = t.outputFilterSensitiveLog, [4, e(n)];
                                     case 1:
                                         return u = f.sent(), a ? ("function" === typeof a.info && (l = u.output, c = l.$metadata, d = function(e, t) {
                                             var n = {};
                                             for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
@@ -64274,29 +64322,29 @@
                                         })), [2, u]) : [2, u]
                                 }
                             }))
                         }))
                     }
                 }
             },
-            Xd = {
+            $d = {
                 name: "loggerMiddleware",
                 tags: ["LOGGER"],
                 step: "initialize",
                 override: !0
             };
-        var $d = function() {
-            return $d = Object.assign || function(e) {
+        var ef = function() {
+            return ef = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, $d.apply(this, arguments)
+            }, ef.apply(this, arguments)
         };
 
-        function ef(e, t, n, r) {
+        function tf(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64316,15 +64364,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function tf(e, t) {
+        function nf(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64392,15 +64440,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function nf(e, t) {
+        function rf(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -64413,23 +64461,23 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var rf = function() {
-            return rf = Object.assign || function(e) {
+        var of = function() {
+            return of = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, rf.apply(this, arguments)
+            }, of.apply(this, arguments)
         };
 
-        function of(e, t, n, r) {
+        function af(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64449,15 +64497,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function af(e, t) {
+        function sf(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64525,15 +64573,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function sf(e) {
+        function uf(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -64541,15 +64589,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function uf(e, t) {
+        function lf(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -64562,33 +64610,33 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        for (var lf = {}, cf = {}, df = 0; df < 256; df++) {
-            var ff = df.toString(16).toLowerCase();
-            1 === ff.length && (ff = "0" + ff), lf[df] = ff, cf[ff] = df
+        for (var cf = {}, df = {}, ff = 0; ff < 256; ff++) {
+            var pf = ff.toString(16).toLowerCase();
+            1 === pf.length && (pf = "0" + pf), cf[ff] = pf, df[pf] = ff
         }
 
-        function pf(e) {
-            for (var t = "", n = 0; n < e.byteLength; n++) t += lf[e[n]];
+        function hf(e) {
+            for (var t = "", n = 0; n < e.byteLength; n++) t += cf[e[n]];
             return t
         }
-        var hf = "X-Amz-Date",
-            gf = "X-Amz-Signature",
-            yf = "X-Amz-Security-Token",
-            mf = "authorization",
-            vf = hf.toLowerCase(),
-            Mf = [mf, vf, "date"],
-            bf = gf.toLowerCase(),
-            jf = "x-amz-content-sha256",
-            wf = yf.toLowerCase(),
-            xf = {
+        var gf = "X-Amz-Date",
+            yf = "X-Amz-Signature",
+            mf = "X-Amz-Security-Token",
+            vf = "authorization",
+            Mf = gf.toLowerCase(),
+            bf = [vf, Mf, "date"],
+            jf = yf.toLowerCase(),
+            wf = "x-amz-content-sha256",
+            xf = mf.toLowerCase(),
+            Nf = {
                 authorization: !0,
                 "cache-control": !0,
                 connection: !0,
                 expect: !0,
                 from: !0,
                 "keep-alive": !0,
                 "max-forwards": !0,
@@ -64597,39 +64645,39 @@
                 te: !0,
                 trailer: !0,
                 "transfer-encoding": !0,
                 upgrade: !0,
                 "user-agent": !0,
                 "x-amzn-trace-id": !0
             },
-            Nf = /^proxy-/,
-            If = /^sec-/,
-            Df = "AWS4-HMAC-SHA256",
-            Sf = "AWS4-HMAC-SHA256-PAYLOAD",
-            Lf = "aws4_request",
-            kf = {},
-            Cf = [];
+            If = /^proxy-/,
+            Df = /^sec-/,
+            Sf = "AWS4-HMAC-SHA256",
+            Lf = "AWS4-HMAC-SHA256-PAYLOAD",
+            kf = "aws4_request",
+            Cf = {},
+            Ef = [];
 
-        function Ef(e, t, n) {
-            return e + "/" + t + "/" + n + "/" + Lf
+        function _f(e, t, n) {
+            return e + "/" + t + "/" + n + "/" + kf
         }
 
-        function _f(e, t, n) {
+        function Tf(e, t, n) {
             var r = new e(t);
             return r.update(n), r.digest()
         }
 
-        function Tf(e, t, n) {
+        function Af(e, t, n) {
             var r, o, i = e.headers,
                 a = {};
             try {
-                for (var s = sf(Object.keys(i).sort()), u = s.next(); !u.done; u = s.next()) {
+                for (var s = uf(Object.keys(i).sort()), u = s.next(); !u.done; u = s.next()) {
                     var l = u.value,
                         c = l.toLowerCase();
-                    (c in xf || (null === t || void 0 === t ? void 0 : t.has(c)) || Nf.test(c) || If.test(c)) && (!n || n && !n.has(c)) || (a[c] = i[l].trim().replace(/\s+/g, " "))
+                    (c in Nf || (null === t || void 0 === t ? void 0 : t.has(c)) || If.test(c) || Df.test(c)) && (!n || n && !n.has(c)) || (a[c] = i[l].trim().replace(/\s+/g, " "))
                 }
             } catch (d) {
                 r = {
                     error: d
                 }
             } finally {
                 try {
@@ -64637,84 +64685,84 @@
                 } finally {
                     if (r) throw r.error
                 }
             }
             return a
         }
 
-        function Af(e, t) {
+        function Of(e, t) {
             var n = e.headers,
                 r = e.body;
-            return of(this, void 0, void 0, (function() {
+            return af(this, void 0, void 0, (function() {
                 var e, o, i, a, s, u, l;
-                return af(this, (function(c) {
+                return sf(this, (function(c) {
                     switch (c.label) {
                         case 0:
                             try {
-                                for (e = sf(Object.keys(n)), o = e.next(); !o.done; o = e.next())
-                                    if ((i = o.value).toLowerCase() === jf) return [2, n[i]]
+                                for (e = uf(Object.keys(n)), o = e.next(); !o.done; o = e.next())
+                                    if ((i = o.value).toLowerCase() === wf) return [2, n[i]]
                             } catch (f) {
                                 u = {
                                     error: f
                                 }
                             } finally {
                                 try {
                                     o && !o.done && (l = e.return) && l.call(e)
                                 } finally {
                                     if (u) throw u.error
                                 }
                             }
                             return void 0 != r ? [3, 1] : [2, "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"];
                         case 1:
-                            return "string" === typeof r || ArrayBuffer.isView(r) || (d = r, "function" === typeof ArrayBuffer && d instanceof ArrayBuffer || "[object ArrayBuffer]" === Object.prototype.toString.call(d)) ? ((a = new t).update(r), s = pf, [4, a.digest()]) : [3, 3];
+                            return "string" === typeof r || ArrayBuffer.isView(r) || (d = r, "function" === typeof ArrayBuffer && d instanceof ArrayBuffer || "[object ArrayBuffer]" === Object.prototype.toString.call(d)) ? ((a = new t).update(r), s = hf, [4, a.digest()]) : [3, 3];
                         case 2:
                             return [2, s.apply(void 0, [c.sent()])];
                         case 3:
                             return [2, "UNSIGNED-PAYLOAD"]
                     }
                     var d
                 }))
             }))
         }
 
-        function Of(e) {
+        function zf(e) {
             var t = e.headers,
                 n = e.query,
                 r = function(e, t) {
                     var n = {};
                     for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
                     if (null != e && "function" === typeof Object.getOwnPropertySymbols) {
                         var o = 0;
                         for (r = Object.getOwnPropertySymbols(e); o < r.length; o++) t.indexOf(r[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[o]) && (n[r[o]] = e[r[o]])
                     }
                     return n
                 }(e, ["headers", "query"]);
-            return rf(rf({}, r), {
-                headers: rf({}, t),
-                query: n ? zf(n) : void 0
+            return of(of({}, r), {
+                headers: of({}, t),
+                query: n ? Uf(n) : void 0
             })
         }
 
-        function zf(e) {
+        function Uf(e) {
             return Object.keys(e).reduce((function(t, n) {
                 var r, o = e[n];
-                return rf(rf({}, t), ((r = {})[n] = Array.isArray(o) ? function() {
-                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(uf(arguments[t]));
+                return of(of({}, t), ((r = {})[n] = Array.isArray(o) ? function() {
+                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(lf(arguments[t]));
                     return e
                 }(o) : o, r))
             }), {})
         }
 
-        function Uf(e) {
+        function Pf(e) {
             var t, n;
-            e = "function" === typeof e.clone ? e.clone() : Of(e);
+            e = "function" === typeof e.clone ? e.clone() : zf(e);
             try {
-                for (var r = sf(Object.keys(e.headers)), o = r.next(); !o.done; o = r.next()) {
+                for (var r = uf(Object.keys(e.headers)), o = r.next(); !o.done; o = r.next()) {
                     var i = o.value;
-                    Mf.indexOf(i.toLowerCase()) > -1 && delete e.headers[i]
+                    bf.indexOf(i.toLowerCase()) > -1 && delete e.headers[i]
                 }
             } catch (a) {
                 t = {
                     error: a
                 }
             } finally {
                 try {
@@ -64722,55 +64770,55 @@
                 } finally {
                     if (t) throw t.error
                 }
             }
             return e
         }
 
-        function Pf(e) {
+        function Rf(e) {
             return function(e) {
                 if ("number" === typeof e) return new Date(1e3 * e);
                 if ("string" === typeof e) return Number(e) ? new Date(1e3 * Number(e)) : new Date(e);
                 return e
             }(e).toISOString().replace(/\.\d{3}Z$/, "Z")
         }
-        var Rf = function() {
+        var Bf = function() {
                 function e(e) {
                     var t = e.applyChecksum,
                         n = e.credentials,
                         r = e.region,
                         o = e.service,
                         i = e.sha256,
                         a = e.uriEscapePath,
                         s = void 0 === a || a;
-                    this.service = o, this.sha256 = i, this.uriEscapePath = s, this.applyChecksum = "boolean" !== typeof t || t, this.regionProvider = Yf(r), this.credentialProvider = Qf(n)
+                    this.service = o, this.sha256 = i, this.uriEscapePath = s, this.applyChecksum = "boolean" !== typeof t || t, this.regionProvider = Qf(r), this.credentialProvider = Gf(n)
                 }
                 return e.prototype.presign = function(e, t) {
-                    return void 0 === t && (t = {}), of(this, void 0, void 0, (function() {
+                    return void 0 === t && (t = {}), af(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I;
-                        return af(this, (function(D) {
+                        return sf(this, (function(D) {
                             switch (D.label) {
                                 case 0:
                                     return n = t.signingDate, r = void 0 === n ? new Date : n, o = t.expiresIn, i = void 0 === o ? 3600 : o, a = t.unsignableHeaders, s = t.unhoistableHeaders, u = t.signableHeaders, l = t.signingRegion, c = t.signingService, [4, this.credentialProvider()];
                                 case 1:
                                     return d = D.sent(), null === l || void 0 === l ? [3, 2] : (p = l, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     p = D.sent(), D.label = 4;
                                 case 4:
-                                    return f = p, h = Bf(r), g = h.longDate, y = h.shortDate, i > 604800 ? [2, Promise.reject("Signature version 4 presigned URLs must have an expiration date less than one week in the future")] : (m = Ef(y, f, null !== c && void 0 !== c ? c : this.service), v = function(e, t) {
+                                    return f = p, h = Ff(r), g = h.longDate, y = h.shortDate, i > 604800 ? [2, Promise.reject("Signature version 4 presigned URLs must have an expiration date less than one week in the future")] : (m = _f(y, f, null !== c && void 0 !== c ? c : this.service), v = function(e, t) {
                                         var n, r, o;
                                         void 0 === t && (t = {});
-                                        var i = "function" === typeof e.clone ? e.clone() : Of(e),
+                                        var i = "function" === typeof e.clone ? e.clone() : zf(e),
                                             a = i.headers,
                                             s = i.query,
                                             u = void 0 === s ? {} : s;
                                         try {
-                                            for (var l = sf(Object.keys(a)), c = l.next(); !c.done; c = l.next()) {
+                                            for (var l = uf(Object.keys(a)), c = l.next(); !c.done; c = l.next()) {
                                                 var d = c.value,
                                                     f = d.toLowerCase();
                                                 "x-amz-" !== f.substr(0, 6) || (null === (o = t.unhoistableHeaders) || void 0 === o ? void 0 : o.has(f)) || (u[d] = a[d], delete a[d])
                                             }
                                         } catch (p) {
                                             n = {
                                                 error: p
@@ -64778,159 +64826,159 @@
                                         } finally {
                                             try {
                                                 c && !c.done && (r = l.return) && r.call(l)
                                             } finally {
                                                 if (n) throw n.error
                                             }
                                         }
-                                        return rf(rf({}, e), {
+                                        return of(of({}, e), {
                                             headers: a,
                                             query: u
                                         })
-                                    }(Uf(e), {
+                                    }(Pf(e), {
                                         unhoistableHeaders: s
-                                    }), d.sessionToken && (v.query[yf] = d.sessionToken), v.query["X-Amz-Algorithm"] = Df, v.query["X-Amz-Credential"] = d.accessKeyId + "/" + m, v.query["X-Amz-Date"] = g, v.query["X-Amz-Expires"] = i.toString(10), M = Tf(v, a, u), v.query["X-Amz-SignedHeaders"] = Ff(M), b = v.query, j = gf, w = this.getSignature, x = [g, m, this.getSigningKey(d, f, y, c)], N = this.createCanonicalRequest, I = [v, M], [4, Af(e, this.sha256)]);
+                                    }), d.sessionToken && (v.query[mf] = d.sessionToken), v.query["X-Amz-Algorithm"] = Sf, v.query["X-Amz-Credential"] = d.accessKeyId + "/" + m, v.query["X-Amz-Date"] = g, v.query["X-Amz-Expires"] = i.toString(10), M = Af(v, a, u), v.query["X-Amz-SignedHeaders"] = Yf(M), b = v.query, j = yf, w = this.getSignature, x = [g, m, this.getSigningKey(d, f, y, c)], N = this.createCanonicalRequest, I = [v, M], [4, Of(e, this.sha256)]);
                                 case 5:
                                     return [4, w.apply(this, x.concat([N.apply(this, I.concat([D.sent()]))]))];
                                 case 6:
                                     return b[j] = D.sent(), [2, v]
                             }
                         }))
                     }))
                 }, e.prototype.sign = function(e, t) {
-                    return of(this, void 0, void 0, (function() {
-                        return af(this, (function(n) {
+                    return af(this, void 0, void 0, (function() {
+                        return sf(this, (function(n) {
                             return "string" === typeof e ? [2, this.signString(e, t)] : e.headers && e.payload ? [2, this.signEvent(e, t)] : [2, this.signRequest(e, t)]
                         }))
                     }))
                 }, e.prototype.signEvent = function(e, t) {
                     var n = e.headers,
                         r = e.payload,
                         o = t.signingDate,
                         i = void 0 === o ? new Date : o,
                         a = t.priorSignature,
                         s = t.signingRegion,
                         u = t.signingService;
-                    return of(this, void 0, void 0, (function() {
+                    return af(this, void 0, void 0, (function() {
                         var e, t, o, l, c, d, f, p, h, g, y;
-                        return af(this, (function(m) {
+                        return sf(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return null === s || void 0 === s ? [3, 1] : (t = s, [3, 3]);
                                 case 1:
                                     return [4, this.regionProvider()];
                                 case 2:
                                     t = m.sent(), m.label = 3;
                                 case 3:
-                                    return e = t, o = Bf(i), l = o.shortDate, c = o.longDate, d = Ef(l, e, null !== u && void 0 !== u ? u : this.service), [4, Af({
+                                    return e = t, o = Ff(i), l = o.shortDate, c = o.longDate, d = _f(l, e, null !== u && void 0 !== u ? u : this.service), [4, Of({
                                         headers: {},
                                         body: r
                                     }, this.sha256)];
                                 case 4:
-                                    return f = m.sent(), (p = new this.sha256).update(n), g = pf, [4, p.digest()];
+                                    return f = m.sent(), (p = new this.sha256).update(n), g = hf, [4, p.digest()];
                                 case 5:
-                                    return h = g.apply(void 0, [m.sent()]), y = [Sf, c, d, a, h, f].join("\n"), [2, this.signString(y, {
+                                    return h = g.apply(void 0, [m.sent()]), y = [Lf, c, d, a, h, f].join("\n"), [2, this.signString(y, {
                                         signingDate: i,
                                         signingRegion: e,
                                         signingService: u
                                     })]
                             }
                         }))
                     }))
                 }, e.prototype.signString = function(e, t) {
                     var n = void 0 === t ? {} : t,
                         r = n.signingDate,
                         o = void 0 === r ? new Date : r,
                         i = n.signingRegion,
                         a = n.signingService;
-                    return of(this, void 0, void 0, (function() {
+                    return af(this, void 0, void 0, (function() {
                         var t, n, r, s, u, l, c, d;
-                        return af(this, (function(f) {
+                        return sf(this, (function(f) {
                             switch (f.label) {
                                 case 0:
                                     return [4, this.credentialProvider()];
                                 case 1:
                                     return t = f.sent(), null === i || void 0 === i ? [3, 2] : (r = i, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     r = f.sent(), f.label = 4;
                                 case 4:
-                                    return n = r, s = Bf(o).shortDate, c = (l = this.sha256).bind, [4, this.getSigningKey(t, n, s, a)];
+                                    return n = r, s = Ff(o).shortDate, c = (l = this.sha256).bind, [4, this.getSigningKey(t, n, s, a)];
                                 case 5:
-                                    return (u = new(c.apply(l, [void 0, f.sent()]))).update(e), d = pf, [4, u.digest()];
+                                    return (u = new(c.apply(l, [void 0, f.sent()]))).update(e), d = hf, [4, u.digest()];
                                 case 6:
                                     return [2, d.apply(void 0, [f.sent()])]
                             }
                         }))
                     }))
                 }, e.prototype.signRequest = function(e, t) {
                     var n = void 0 === t ? {} : t,
                         r = n.signingDate,
                         o = void 0 === r ? new Date : r,
                         i = n.signableHeaders,
                         a = n.unsignableHeaders,
                         s = n.signingRegion,
                         u = n.signingService;
-                    return of(this, void 0, void 0, (function() {
+                    return af(this, void 0, void 0, (function() {
                         var t, n, r, l, c, d, f, p, h, g, y;
-                        return af(this, (function(m) {
+                        return sf(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return [4, this.credentialProvider()];
                                 case 1:
                                     return t = m.sent(), null === s || void 0 === s ? [3, 2] : (r = s, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     r = m.sent(), m.label = 4;
                                 case 4:
-                                    return n = r, l = Uf(e), c = Bf(o), d = c.longDate, f = c.shortDate, p = Ef(f, n, null !== u && void 0 !== u ? u : this.service), l.headers[vf] = d, t.sessionToken && (l.headers[wf] = t.sessionToken), [4, Af(l, this.sha256)];
+                                    return n = r, l = Pf(e), c = Ff(o), d = c.longDate, f = c.shortDate, p = _f(f, n, null !== u && void 0 !== u ? u : this.service), l.headers[Mf] = d, t.sessionToken && (l.headers[xf] = t.sessionToken), [4, Of(l, this.sha256)];
                                 case 5:
                                     return h = m.sent(), ! function(e, t) {
                                         var n, r;
                                         e = e.toLowerCase();
                                         try {
-                                            for (var o = sf(Object.keys(t)), i = o.next(); !i.done; i = o.next())
+                                            for (var o = uf(Object.keys(t)), i = o.next(); !i.done; i = o.next())
                                                 if (e === i.value.toLowerCase()) return !0
                                         } catch (a) {
                                             n = {
                                                 error: a
                                             }
                                         } finally {
                                             try {
                                                 i && !i.done && (r = o.return) && r.call(o)
                                             } finally {
                                                 if (n) throw n.error
                                             }
                                         }
                                         return !1
-                                    }(jf, l.headers) && this.applyChecksum && (l.headers[jf] = h), g = Tf(l, a, i), [4, this.getSignature(d, p, this.getSigningKey(t, n, f, u), this.createCanonicalRequest(l, g, h))];
+                                    }(wf, l.headers) && this.applyChecksum && (l.headers[wf] = h), g = Af(l, a, i), [4, this.getSignature(d, p, this.getSigningKey(t, n, f, u), this.createCanonicalRequest(l, g, h))];
                                 case 6:
-                                    return y = m.sent(), l.headers[mf] = "AWS4-HMAC-SHA256 Credential=" + t.accessKeyId + "/" + p + ", SignedHeaders=" + Ff(g) + ", Signature=" + y, [2, l]
+                                    return y = m.sent(), l.headers[vf] = "AWS4-HMAC-SHA256 Credential=" + t.accessKeyId + "/" + p + ", SignedHeaders=" + Yf(g) + ", Signature=" + y, [2, l]
                             }
                         }))
                     }))
                 }, e.prototype.createCanonicalRequest = function(e, t, n) {
                     var r = Object.keys(t).sort();
                     return e.method + "\n" + this.getCanonicalPath(e) + "\n" + function(e) {
                         var t, n, r = e.query,
                             o = void 0 === r ? {} : r,
                             i = [],
                             a = {},
                             s = function(e) {
-                                if (e.toLowerCase() === bf) return "continue";
+                                if (e.toLowerCase() === jf) return "continue";
                                 i.push(e);
                                 var t = o[e];
-                                "string" === typeof t ? a[e] = Yc(e) + "=" + Yc(t) : Array.isArray(t) && (a[e] = t.slice(0).sort().reduce((function(t, n) {
-                                    return t.concat([Yc(e) + "=" + Yc(n)])
+                                "string" === typeof t ? a[e] = Qc(e) + "=" + Qc(t) : Array.isArray(t) && (a[e] = t.slice(0).sort().reduce((function(t, n) {
+                                    return t.concat([Qc(e) + "=" + Qc(n)])
                                 }), []).join("&"))
                             };
                         try {
-                            for (var u = sf(Object.keys(o).sort()), l = u.next(); !l.done; l = u.next()) s(l.value)
+                            for (var u = uf(Object.keys(o).sort()), l = u.next(); !l.done; l = u.next()) s(l.value)
                         } catch (c) {
                             t = {
                                 error: c
                             }
                         } finally {
                             try {
                                 l && !l.done && (n = u.return) && n.call(u)
@@ -64943,60 +64991,60 @@
                         })).filter((function(e) {
                             return e
                         })).join("&")
                     }(e) + "\n" + r.map((function(e) {
                         return e + ":" + t[e]
                     })).join("\n") + "\n\n" + r.join(";") + "\n" + n
                 }, e.prototype.createStringToSign = function(e, t, n) {
-                    return of(this, void 0, void 0, (function() {
+                    return af(this, void 0, void 0, (function() {
                         var r, o;
-                        return af(this, (function(i) {
+                        return sf(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return (r = new this.sha256).update(n), [4, r.digest()];
                                 case 1:
-                                    return o = i.sent(), [2, "AWS4-HMAC-SHA256\n" + e + "\n" + t + "\n" + pf(o)]
+                                    return o = i.sent(), [2, "AWS4-HMAC-SHA256\n" + e + "\n" + t + "\n" + hf(o)]
                             }
                         }))
                     }))
                 }, e.prototype.getCanonicalPath = function(e) {
                     var t = e.path;
                     return this.uriEscapePath ? "/" + encodeURIComponent(t.replace(/^\//, "")).replace(/%2F/g, "/") : t
                 }, e.prototype.getSignature = function(e, t, n, r) {
-                    return of(this, void 0, void 0, (function() {
+                    return af(this, void 0, void 0, (function() {
                         var o, i, a, s, u;
-                        return af(this, (function(l) {
+                        return sf(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return [4, this.createStringToSign(e, t, r)];
                                 case 1:
                                     return o = l.sent(), s = (a = this.sha256).bind, [4, n];
                                 case 2:
-                                    return (i = new(s.apply(a, [void 0, l.sent()]))).update(o), u = pf, [4, i.digest()];
+                                    return (i = new(s.apply(a, [void 0, l.sent()]))).update(o), u = hf, [4, i.digest()];
                                 case 3:
                                     return [2, u.apply(void 0, [l.sent()])]
                             }
                         }))
                     }))
                 }, e.prototype.getSigningKey = function(e, t, n, r) {
                     return function(e, t, n, r, o) {
-                        return of(void 0, void 0, void 0, (function() {
+                        return af(void 0, void 0, void 0, (function() {
                             var i, a, s, u, l, c, d, f, p;
-                            return af(this, (function(h) {
+                            return sf(this, (function(h) {
                                 switch (h.label) {
                                     case 0:
-                                        return [4, _f(e, t.secretAccessKey, t.accessKeyId)];
+                                        return [4, Tf(e, t.secretAccessKey, t.accessKeyId)];
                                     case 1:
-                                        if (i = h.sent(), (a = n + ":" + r + ":" + o + ":" + pf(i) + ":" + t.sessionToken) in kf) return [2, kf[a]];
-                                        for (Cf.push(a); Cf.length > 50;) delete kf[Cf.shift()];
+                                        if (i = h.sent(), (a = n + ":" + r + ":" + o + ":" + hf(i) + ":" + t.sessionToken) in Cf) return [2, Cf[a]];
+                                        for (Ef.push(a); Ef.length > 50;) delete Cf[Ef.shift()];
                                         s = "AWS4" + t.secretAccessKey, h.label = 2;
                                     case 2:
-                                        h.trys.push([2, 7, 8, 9]), u = sf([n, r, o, Lf]), l = u.next(), h.label = 3;
+                                        h.trys.push([2, 7, 8, 9]), u = uf([n, r, o, kf]), l = u.next(), h.label = 3;
                                     case 3:
-                                        return l.done ? [3, 6] : (c = l.value, [4, _f(e, s, c)]);
+                                        return l.done ? [3, 6] : (c = l.value, [4, Tf(e, s, c)]);
                                     case 4:
                                         s = h.sent(), h.label = 5;
                                     case 5:
                                         return l = u.next(), [3, 3];
                                     case 6:
                                         return [3, 9];
                                     case 7:
@@ -65007,68 +65055,68 @@
                                         try {
                                             l && !l.done && (p = u.return) && p.call(u)
                                         } finally {
                                             if (f) throw f.error
                                         }
                                         return [7];
                                     case 9:
-                                        return [2, kf[a] = s]
+                                        return [2, Cf[a] = s]
                                 }
                             }))
                         }))
                     }(this.sha256, e, n, t, r || this.service)
                 }, e
             }(),
-            Bf = function(e) {
-                var t = Pf(e).replace(/[\-:]/g, "");
+            Ff = function(e) {
+                var t = Rf(e).replace(/[\-:]/g, "");
                 return {
                     longDate: t,
                     shortDate: t.substr(0, 8)
                 }
             },
-            Ff = function(e) {
+            Yf = function(e) {
                 return Object.keys(e).sort().join(";")
             },
-            Yf = function(e) {
+            Qf = function(e) {
                 if ("string" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             },
-            Qf = function(e) {
+            Gf = function(e) {
                 if ("object" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
 
-        function Gf(e) {
+        function Wf(e) {
             if ("object" === typeof e) {
                 var t = Promise.resolve(e);
                 return function() {
                     return t
                 }
             }
             return e
         }
-        var Wf = function() {
-            return Wf = Object.assign || function(e) {
+        var Hf = function() {
+            return Hf = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Wf.apply(this, arguments)
+            }, Hf.apply(this, arguments)
         };
 
-        function Hf(e, t, n, r) {
+        function Zf(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -65088,15 +65136,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Zf(e, t) {
+        function Vf(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -65164,15 +65212,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Vf(e, t) {
+        function qf(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -65186,213 +65234,213 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function qf() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Vf(arguments[t]));
+        function Jf() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(qf(arguments[t]));
             return e
         }
-        var Jf = "user-agent",
-            Kf = /[^\!\#\$\%\&\'\*\+\-\.\^\_\`\|\~\d\w]/g,
-            Xf = function(e) {
-                var t = Vf(e, 2),
+        var Kf = "user-agent",
+            Xf = /[^\!\#\$\%\&\'\*\+\-\.\^\_\`\|\~\d\w]/g,
+            $f = function(e) {
+                var t = qf(e, 2),
                     n = t[0],
                     r = t[1],
                     o = n.indexOf("/"),
                     i = n.substring(0, o),
                     a = n.substring(o + 1);
                 return "api" === i && (a = a.toLowerCase()), [i, a, r].filter((function(e) {
                     return e && e.length > 0
                 })).map((function(e) {
-                    return null === e || void 0 === e ? void 0 : e.replace(Kf, "_")
+                    return null === e || void 0 === e ? void 0 : e.replace(Xf, "_")
                 })).join("/")
             },
-            $f = {
+            ep = {
                 name: "getUserAgentMiddleware",
                 step: "build",
                 priority: "low",
                 tags: ["SET_USER_AGENT", "USER_AGENT"],
                 override: !0
             },
-            ep = function(e) {
+            tp = function(e) {
                 return {
                     applyToStack: function(t) {
                         var n;
                         t.add((n = e, function(e, t) {
                             return function(r) {
-                                return Hf(void 0, void 0, void 0, (function() {
+                                return Zf(void 0, void 0, void 0, (function() {
                                     var o, i, a, s, u, l, c, d;
-                                    return Zf(this, (function(f) {
+                                    return Vf(this, (function(f) {
                                         switch (f.label) {
                                             case 0:
-                                                return o = r.request, Ll.isInstance(o) ? (i = o.headers, a = (null === (c = null === t || void 0 === t ? void 0 : t.userAgent) || void 0 === c ? void 0 : c.map(Xf)) || [], [4, n.defaultUserAgentProvider()]) : [2, e(r)];
+                                                return o = r.request, kl.isInstance(o) ? (i = o.headers, a = (null === (c = null === t || void 0 === t ? void 0 : t.userAgent) || void 0 === c ? void 0 : c.map($f)) || [], [4, n.defaultUserAgentProvider()]) : [2, e(r)];
                                             case 1:
-                                                return s = f.sent().map(Xf), u = (null === (d = null === n || void 0 === n ? void 0 : n.customUserAgent) || void 0 === d ? void 0 : d.map(Xf)) || [], i["x-amz-user-agent"] = qf(s, a, u).join(" "), l = qf(s.filter((function(e) {
+                                                return s = f.sent().map($f), u = (null === (d = null === n || void 0 === n ? void 0 : n.customUserAgent) || void 0 === d ? void 0 : d.map($f)) || [], i["x-amz-user-agent"] = Jf(s, a, u).join(" "), l = Jf(s.filter((function(e) {
                                                     return e.startsWith("aws-sdk-")
-                                                })), u).join(" "), "browser" !== n.runtime && l && (i[Jf] = i[Jf] ? i[Jf] + " " + l : l), [2, e(Wf(Wf({}, r), {
+                                                })), u).join(" "), "browser" !== n.runtime && l && (i[Kf] = i[Kf] ? i[Kf] + " " + l : l), [2, e(Hf(Hf({}, r), {
                                                     request: o
                                                 }))]
                                         }
                                     }))
                                 }))
                             }
-                        }), $f)
+                        }), ep)
                     }
                 }
             },
-            tp = function(e) {
+            np = function(e) {
                 function t(t) {
                     var n, r, o = this,
                         i = function(e) {
                             if (!e.region) throw new Error("Region is missing");
-                            return Td(Td({}, e), {
-                                region: Pd(e.region)
+                            return Ad(Ad({}, e), {
+                                region: Rd(e.region)
                             })
-                        }(vu(vu({}, _d), t)),
+                        }(Mu(Mu({}, Td), t)),
                         a = function(e) {
                             var t;
-                            return Td(Td({}, e), {
+                            return Ad(Ad({}, e), {
                                 tls: null === (t = e.tls) || void 0 === t || t,
-                                endpoint: e.endpoint ? zd(e) : function() {
-                                    return Ud(e)
+                                endpoint: e.endpoint ? Ud(e) : function() {
+                                    return Pd(e)
                                 },
                                 isCustomEndpoint: !!e.endpoint
                             })
                         }(i),
                         s = function(e) {
                             var t, n = this,
-                                r = Gf(e.credentials || e.credentialDefaultProvider(e)),
+                                r = Wf(e.credentials || e.credentialDefaultProvider(e)),
                                 o = e.signingEscapePath,
                                 i = void 0 === o || o,
                                 a = e.systemClockOffset,
                                 s = void 0 === a ? e.systemClockOffset || 0 : a,
                                 u = e.sha256;
-                            return t = e.signer ? Gf(e.signer) : function() {
-                                return Gf(e.region)().then((function(t) {
-                                    return ef(n, void 0, void 0, (function() {
-                                        return tf(this, (function(n) {
+                            return t = e.signer ? Wf(e.signer) : function() {
+                                return Wf(e.region)().then((function(t) {
+                                    return tf(n, void 0, void 0, (function() {
+                                        return nf(this, (function(n) {
                                             switch (n.label) {
                                                 case 0:
                                                     return [4, e.regionInfoProvider(t)];
                                                 case 1:
                                                     return [2, [n.sent() || {}, t]]
                                             }
                                         }))
                                     }))
                                 })).then((function(t) {
-                                    var n = nf(t, 2),
+                                    var n = rf(t, 2),
                                         o = n[0],
                                         a = n[1],
                                         s = o.signingRegion,
                                         l = o.signingService;
-                                    return e.signingRegion = e.signingRegion || s || a, e.signingName = e.signingName || l || e.serviceId, new Rf({
+                                    return e.signingRegion = e.signingRegion || s || a, e.signingName = e.signingName || l || e.serviceId, new Bf({
                                         credentials: r,
                                         region: e.signingRegion,
                                         service: e.signingName,
                                         sha256: u,
                                         uriEscapePath: i
                                     })
                                 }))
-                            }, $d($d({}, e), {
+                            }, ef(ef({}, e), {
                                 systemClockOffset: s,
                                 signingEscapePath: i,
                                 credentials: r,
                                 signer: t
                             })
                         }(a),
                         u = function(e) {
-                            var t = yd(e.maxAttempts);
-                            return ed(ed({}, e), {
+                            var t = md(e.maxAttempts);
+                            return td(td({}, e), {
                                 maxAttempts: t,
-                                retryStrategy: e.retryStrategy || new gd(t)
+                                retryStrategy: e.retryStrategy || new yd(t)
                             })
                         }(s),
-                        l = Wf(Wf({}, n = u), {
+                        l = Hf(Hf({}, n = u), {
                             customUserAgent: "string" === typeof n.customUserAgent ? [
                                 [n.customUserAgent]
                             ] : n.customUserAgent
                         });
                     return (o = e.call(this, l) || this).config = l, o.middlewareStack.use((r = o.config, {
                         applyToStack: function(e) {
-                            e.add(od(r), id)
+                            e.add(id(r), ad)
                         }
-                    })), o.middlewareStack.use(Gd(o.config)), o.middlewareStack.use(Vd(o.config)), o.middlewareStack.use((o.config, {
+                    })), o.middlewareStack.use(Wd(o.config)), o.middlewareStack.use(qd(o.config)), o.middlewareStack.use((o.config, {
                         applyToStack: function(e) {
-                            e.add(Kd(), Xd)
+                            e.add(Xd(), $d)
                         }
-                    })), o.middlewareStack.use(ep(o.config)), o
+                    })), o.middlewareStack.use(tp(o.config)), o
                 }
-                return mu(t, e), t.prototype.destroy = function() {
+                return vu(t, e), t.prototype.destroy = function() {
                     e.prototype.destroy.call(this)
                 }, t
-            }(Mc),
-            np = "aws-amplify/5.0.10",
-            rp = {
-                userAgent: np + " js",
+            }(bc),
+            rp = "aws-amplify/5.0.10",
+            op = {
+                userAgent: rp + " js",
                 product: "",
                 navigator: null,
                 isReactNative: !1
             };
         if ("undefined" !== typeof navigator && navigator.product)
-            if (rp.product = navigator.product || "", rp.navigator = navigator || null, "ReactNative" === navigator.product) rp.userAgent = np + " react-native", rp.isReactNative = !0;
-            else rp.userAgent = np + " js", rp.isReactNative = !1;
+            if (op.product = navigator.product || "", op.navigator = navigator || null, "ReactNative" === navigator.product) op.userAgent = rp + " react-native", op.isReactNative = !0;
+            else op.userAgent = rp + " js", op.isReactNative = !1;
 
-        function op(e) {
-            var t, n = new tp({
+        function ip(e) {
+            var t, n = new np({
                 region: e.region,
-                customUserAgent: "" + rp.userAgent + (t || "")
+                customUserAgent: "" + op.userAgent + (t || "")
             });
             return n.middlewareStack.add((function(e, t) {
                 return function(t) {
                     return e(function(e) {
-                        return zs(zs({}, e), {
-                            request: zs(zs({}, e.request), {
-                                headers: zs(zs({}, e.request.headers), {
+                        return Us(Us({}, e), {
+                            request: Us(Us({}, e.request), {
+                                headers: Us(Us({}, e.request.headers), {
                                     "cache-control": "no-store"
                                 })
                             })
                         })
                     }(t))
                 }
             }), {
                 step: "build",
                 name: "cacheControlMiddleWare"
             }), n
         }
-        var ip = new Gs("Credentials"),
-            ap = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            sp = function() {
+        var ap = new Ws("Credentials"),
+            sp = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            up = function() {
                 function e(e) {
-                    this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = lu.refreshGoogleToken, this._refreshHandlers.facebook = cu.refreshFacebookToken
+                    this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = cu.refreshGoogleToken, this._refreshHandlers.facebook = du.refreshFacebookToken
                 }
                 return e.prototype.getModuleName = function() {
                     return "Credentials"
                 }, e.prototype.getCredSource = function() {
                     return this._credentials_source
                 }, e.prototype.configure = function(e) {
                     if (!e) return this._config || {};
                     this._config = Object.assign({}, this._config, e);
                     var t = this._config.refreshHandlers;
-                    return t && (this._refreshHandlers = zs(zs({}, this._refreshHandlers), t)), this._storage = this._config.storage, this._storage || (this._storage = (new Ks).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()),
+                    return t && (this._refreshHandlers = Us(Us({}, this._refreshHandlers), t)), this._storage = this._config.storage, this._storage || (this._storage = (new Xs).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()),
                         function(e, t, n) {
-                            Vs.dispatch("core", {
+                            qs.dispatch("core", {
                                 event: e,
                                 data: t,
                                 message: n
-                            }, "Credentials", ap)
+                            }, "Credentials", sp)
                         }("credentials_configured", null, "Credentials has been configured successfully"), this._config
                 }, e.prototype.get = function() {
-                    return ip.debug("getting credentials"), this._pickupCredentials()
+                    return ap.debug("getting credentials"), this._pickupCredentials()
                 }, e.prototype._getCognitoIdentityIdStorageKey = function(e) {
                     return "CognitoIdentityId-" + e
                 }, e.prototype._pickupCredentials = function() {
-                    return ip.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? ip.debug("getting old cred promise") : (ip.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
+                    return ap.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? ap.debug("getting old cred promise") : (ap.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
                         if (e.isResolved) return e;
                         var t = !0,
                             n = !1,
                             r = !1,
                             o = e.then((function(e) {
                                 return r = !0, t = !1, e
                             }), (function(e) {
@@ -65403,152 +65451,152 @@
                         }, o.isPending = function() {
                             return t
                         }, o.isRejected = function() {
                             return n
                         }, o
                     }(this._keepAlive())), this._gettingCredPromise
                 }, e.prototype._keepAlive = function() {
-                    return Us(this, void 0, void 0, (function() {
+                    return Ps(this, void 0, void 0, (function() {
                         var e, t, n, r, o, i, a;
-                        return Ps(this, (function(s) {
+                        return Rs(this, (function(s) {
                             switch (s.label) {
                                 case 0:
-                                    if (ip.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return ip.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
-                                    if (ip.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? fu.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
+                                    if (ap.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return ap.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
+                                    if (ap.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? pu.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
                                     if (this._isExpired(e) || !this._isPastTTL()) return [3, 6];
-                                    ip.debug("ttl has passed but token is not yet expired"), s.label = 1;
+                                    ap.debug("ttl has passed but token is not yet expired"), s.label = 1;
                                 case 1:
                                     return s.trys.push([1, 5, , 6]), [4, n.currentUserPoolUser()];
                                 case 2:
                                     return r = s.sent(), [4, n.currentSession()];
                                 case 3:
                                     return o = s.sent(), i = o.refreshToken, [4, new Promise((function(e, t) {
                                         r.refreshSession(i, (function(n, r) {
                                             return n ? t(n) : e(r)
                                         }))
                                     }))];
                                 case 4:
                                     return s.sent(), [3, 6];
                                 case 5:
-                                    return a = s.sent(), ip.debug("Error attempting to refreshing the session", a), [3, 6];
+                                    return a = s.sent(), ap.debug("Error attempting to refreshing the session", a), [3, 6];
                                 case 6:
                                     return [2, n.currentUserCredentials()]
                             }
                         }))
                     }))
                 }, e.prototype.refreshFederatedToken = function(e) {
-                    ip.debug("Getting federated credentials");
+                    ap.debug("Getting federated credentials");
                     var t = e.provider,
                         n = e.user,
                         r = e.token,
                         o = e.identity_id,
                         i = e.expires_at;
                     i = 1970 === new Date(i).getFullYear() ? 1e3 * i : i;
                     var a = this;
-                    return ip.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (ip.debug("token not expired"), this._setCredentialsFromFederation({
+                    return ap.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (ap.debug("token not expired"), this._setCredentialsFromFederation({
                         provider: t,
                         token: r,
                         user: n,
                         identity_id: o,
                         expires_at: i
-                    })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (ip.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
+                    })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (ap.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
                         refreshHandler: a._refreshHandlers[t],
                         provider: t,
                         user: n
-                    })) : (ip.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
+                    })) : (ap.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
                 }, e.prototype._providerRefreshWithRetry = function(e) {
                     var t = this,
                         n = e.refreshHandler,
                         r = e.provider,
                         o = e.user;
-                    return nu(n, [], 1e4).then((function(e) {
-                        return ip.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
+                    return ru(n, [], 1e4).then((function(e) {
+                        return ap.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
                             provider: r,
                             token: e.token,
                             user: o,
                             identity_id: e.identity_id,
                             expires_at: e.expires_at
                         })
                     })).catch((function(e) {
-                        return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), ip.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
+                        return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), ap.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
                     }))
                 }, e.prototype._isExpired = function(e) {
-                    if (!e) return ip.debug("no credentials for expiration check"), !0;
-                    ip.debug("are these credentials expired?", e);
+                    if (!e) return ap.debug("no credentials for expiration check"), !0;
+                    ap.debug("are these credentials expired?", e);
                     var t = Date.now();
                     return e.expiration.getTime() <= t
                 }, e.prototype._isPastTTL = function() {
                     return this._nextCredentialsRefresh <= Date.now()
                 }, e.prototype._setCredentialsForGuest = function() {
                     var e;
-                    return Us(this, void 0, void 0, (function() {
+                    return Ps(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d = this;
-                        return Ps(this, (function(f) {
+                        return Rs(this, (function(f) {
                             switch (f.label) {
                                 case 0:
-                                    return ip.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, zc(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (ip.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (ip.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
+                                    return ap.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, Uc(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (ap.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (ap.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
                                 case 1:
-                                    return a = s._identityId = f.sent(), u = op({
+                                    return a = s._identityId = f.sent(), u = ip({
                                         region: i || r
-                                    }), l = void 0, a ? l = kc({
+                                    }), l = void 0, a ? l = Cc({
                                         identityId: a,
                                         client: u
                                     })() : (c = function() {
-                                        return Us(d, void 0, void 0, (function() {
+                                        return Ps(d, void 0, void 0, (function() {
                                             var e;
-                                            return Ps(this, (function(t) {
+                                            return Rs(this, (function(t) {
                                                 switch (t.label) {
                                                     case 0:
-                                                        return [4, u.send(new Cc({
+                                                        return [4, u.send(new Ec({
                                                             IdentityPoolId: n
                                                         }))];
                                                     case 1:
-                                                        return e = t.sent().IdentityId, this._identityId = e, [2, kc({
+                                                        return e = t.sent().IdentityId, this._identityId = e, [2, Cc({
                                                             client: u,
                                                             identityId: e
                                                         })()]
                                                 }
                                             }))
                                         }))
                                     }, l = c().catch((function(e) {
-                                        return Us(d, void 0, void 0, (function() {
-                                            return Ps(this, (function(t) {
+                                        return Ps(d, void 0, void 0, (function() {
+                                            return Rs(this, (function(t) {
                                                 throw e
                                             }))
                                         }))
                                     }))), [2, this._loadCredentials(l, "guest", !1, null).then((function(e) {
                                         return e
                                     })).catch((function(e) {
-                                        return Us(d, void 0, void 0, (function() {
+                                        return Ps(d, void 0, void 0, (function() {
                                             var t, r = this;
-                                            return Ps(this, (function(o) {
+                                            return Rs(this, (function(o) {
                                                 switch (o.label) {
                                                     case 0:
-                                                        return "ResourceNotFoundException" !== e.name || e.message !== "Identity '" + a + "' not found." ? [3, 2] : (ip.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
+                                                        return "ResourceNotFoundException" !== e.name || e.message !== "Identity '" + a + "' not found." ? [3, 2] : (ap.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
                                                     case 1:
                                                         return o.sent(), t = function() {
-                                                            return Us(r, void 0, void 0, (function() {
+                                                            return Ps(r, void 0, void 0, (function() {
                                                                 var e;
-                                                                return Ps(this, (function(t) {
+                                                                return Rs(this, (function(t) {
                                                                     switch (t.label) {
                                                                         case 0:
-                                                                            return [4, u.send(new Cc({
+                                                                            return [4, u.send(new Ec({
                                                                                 IdentityPoolId: n
                                                                             }))];
                                                                         case 1:
-                                                                            return e = t.sent().IdentityId, this._identityId = e, [2, kc({
+                                                                            return e = t.sent().IdentityId, this._identityId = e, [2, Cc({
                                                                                 client: u,
                                                                                 identityId: e
                                                                             })()]
                                                                     }
                                                                 }))
                                                             }))
                                                         }, l = t().catch((function(e) {
-                                                            return Us(r, void 0, void 0, (function() {
-                                                                return Ps(this, (function(t) {
+                                                            return Ps(r, void 0, void 0, (function() {
+                                                                return Rs(this, (function(t) {
                                                                     throw e
                                                                 }))
                                                             }))
                                                         })), [2, this._loadCredentials(l, "guest", !1, null)];
                                                     case 2:
                                                         return [2, e]
                                                 }
@@ -65571,191 +65619,191 @@
                     if (!o) return Promise.reject("You must specify a federated provider");
                     var i = {};
                     i[o] = n;
                     var a = this._config,
                         s = a.identityPoolId,
                         u = a.region,
                         l = a.identityPoolRegion;
-                    if (!s) return ip.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                    if (!l && !u) return ip.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
-                    var c = op({
+                    if (!s) return ap.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                    if (!l && !u) return ap.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                    var c = ip({
                             region: l || u
                         }),
                         d = void 0;
-                    r ? d = kc({
+                    r ? d = Cc({
                         identityId: r,
                         logins: i,
                         client: c
-                    })() : d = Ac({
+                    })() : d = Oc({
                         logins: i,
                         identityPoolId: s,
                         client: c
                     })();
                     return this._loadCredentials(d, "federated", !0, e)
                 }, e.prototype._setCredentialsFromSession = function(e) {
                     var t = this;
-                    ip.debug("set credentials from session");
+                    ap.debug("set credentials from session");
                     var n = e.getIdToken().getJwtToken(),
                         r = this._config,
                         o = r.region,
                         i = r.userPoolId,
                         a = r.identityPoolId,
                         s = r.identityPoolRegion;
-                    if (!a) return ip.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                    if (!s && !o) return ip.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                    if (!a) return ap.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                    if (!s && !o) return ap.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
                     var u = {};
                     u["cognito-idp." + o + ".amazonaws.com/" + i] = n;
-                    var l = op({
+                    var l = ip({
                             region: s || o
                         }),
-                        c = Us(t, void 0, void 0, (function() {
+                        c = Ps(t, void 0, void 0, (function() {
                             var e, t, n, r, o, i, s, c, d, f;
-                            return Ps(this, (function(p) {
+                            return Rs(this, (function(p) {
                                 switch (p.label) {
                                     case 0:
                                         return [4, this._getGuestIdentityId()];
                                     case 1:
-                                        return (e = p.sent()) ? [3, 3] : [4, l.send(new Cc({
+                                        return (e = p.sent()) ? [3, 3] : [4, l.send(new Ec({
                                             IdentityPoolId: a,
                                             Logins: u
                                         }))];
                                     case 2:
                                         n = p.sent().IdentityId, t = n, p.label = 3;
                                     case 3:
-                                        return [4, l.send(new Ic({
+                                        return [4, l.send(new Dc({
                                             IdentityId: e || t,
                                             Logins: u
                                         }))];
                                     case 4:
-                                        return r = p.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, f = r.IdentityId, this._identityId = f, e ? (ip.debug("The guest identity " + e + " has been successfully linked to the logins"), e === f && ip.debug("The guest identity " + e + " has become the primary identity"), [4, this._removeGuestIdentityId()]) : [3, 6];
+                                        return r = p.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, f = r.IdentityId, this._identityId = f, e ? (ap.debug("The guest identity " + e + " has been successfully linked to the logins"), e === f && ap.debug("The guest identity " + e + " has become the primary identity"), [4, this._removeGuestIdentityId()]) : [3, 6];
                                     case 5:
                                         p.sent(), p.label = 6;
                                     case 6:
                                         return [2, {
                                             accessKeyId: i,
                                             secretAccessKey: c,
                                             sessionToken: d,
                                             expiration: s,
                                             identityId: f
                                         }]
                                 }
                             }))
                         })).catch((function(e) {
-                            return Us(t, void 0, void 0, (function() {
-                                return Ps(this, (function(t) {
+                            return Ps(t, void 0, void 0, (function() {
+                                return Rs(this, (function(t) {
                                     throw e
                                 }))
                             }))
                         }));
                     return this._loadCredentials(c, "userPool", !0, null)
                 }, e.prototype._loadCredentials = function(e, t, n, r) {
                     var o = this,
                         i = this;
                     return new Promise((function(a, s) {
                         e.then((function(e) {
-                            return Us(o, void 0, void 0, (function() {
+                            return Ps(o, void 0, void 0, (function() {
                                 var o, s, u, l, c;
-                                return Ps(this, (function(d) {
+                                return Rs(this, (function(d) {
                                     switch (d.label) {
                                         case 0:
-                                            if (ip.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
+                                            if (ap.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
                                                 o = Object.assign({
                                                     id: this._credentials.identityId
                                                 }, r.user), s = r.provider, u = r.token, l = r.expires_at, c = r.identity_id;
                                                 try {
                                                     this._storage.setItem("aws-amplify-federatedInfo", JSON.stringify({
                                                         provider: s,
                                                         token: u,
                                                         user: o,
                                                         expires_at: l,
                                                         identity_id: c
                                                     }))
                                                 } catch (f) {
-                                                    ip.debug("Failed to put federated info into auth storage", f)
+                                                    ap.debug("Failed to put federated info into auth storage", f)
                                                 }
                                             }
                                             return "guest" !== t ? [3, 2] : [4, this._setGuestIdentityId(e.identityId)];
                                         case 1:
                                             d.sent(), d.label = 2;
                                         case 2:
                                             return a(i._credentials), [2]
                                     }
                                 }))
                             }))
                         })).catch((function(t) {
-                            if (t) return ip.debug("Failed to load credentials", e), ip.debug("Error loading credentials", t), void s(t)
+                            if (t) return ap.debug("Failed to load credentials", e), ap.debug("Error loading credentials", t), void s(t)
                         }))
                     }))
                 }, e.prototype.set = function(e, t) {
-                    return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (ip.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
+                    return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (ap.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
                 }, e.prototype.clear = function() {
-                    return Us(this, void 0, void 0, (function() {
-                        return Ps(this, (function(e) {
-                            return this._credentials = null, this._credentials_source = null, ip.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
+                    return Ps(this, void 0, void 0, (function() {
+                        return Rs(this, (function(e) {
+                            return this._credentials = null, this._credentials_source = null, ap.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
                         }))
                     }))
                 }, e.prototype._getGuestIdentityId = function() {
-                    return Us(this, void 0, void 0, (function() {
+                    return Ps(this, void 0, void 0, (function() {
                         var e, t;
-                        return Ps(this, (function(n) {
+                        return Rs(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     e = this._config.identityPoolId, n.label = 1;
                                 case 1:
                                     return n.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return n.sent(), [2, this._storage.getItem(this._getCognitoIdentityIdStorageKey(e))];
                                 case 3:
-                                    return t = n.sent(), ip.debug("Failed to get the cached guest identityId", t), [3, 4];
+                                    return t = n.sent(), ap.debug("Failed to get the cached guest identityId", t), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._setGuestIdentityId = function(e) {
-                    return Us(this, void 0, void 0, (function() {
+                    return Ps(this, void 0, void 0, (function() {
                         var t, n;
-                        return Ps(this, (function(r) {
+                        return Rs(this, (function(r) {
                             switch (r.label) {
                                 case 0:
                                     t = this._config.identityPoolId, r.label = 1;
                                 case 1:
                                     return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return r.sent(), this._storage.setItem(this._getCognitoIdentityIdStorageKey(t), e), [3, 4];
                                 case 3:
-                                    return n = r.sent(), ip.debug("Failed to cache guest identityId", n), [3, 4];
+                                    return n = r.sent(), ap.debug("Failed to cache guest identityId", n), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._removeGuestIdentityId = function() {
-                    return Us(this, void 0, void 0, (function() {
+                    return Ps(this, void 0, void 0, (function() {
                         var e;
-                        return Ps(this, (function(t) {
-                            return e = this._config.identityPoolId, ip.debug("removing " + this._getCognitoIdentityIdStorageKey(e) + " from storage"), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
+                        return Rs(this, (function(t) {
+                            return e = this._config.identityPoolId, ap.debug("removing " + this._getCognitoIdentityIdStorageKey(e) + " from storage"), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
                         }))
                     }))
                 }, e.prototype.shear = function(e) {
                     return {
                         accessKeyId: e.accessKeyId,
                         sessionToken: e.sessionToken,
                         secretAccessKey: e.secretAccessKey,
                         identityId: e.identityId,
                         authenticated: e.authenticated
                     }
                 }, e
             }(),
-            up = new sp(null);
-        fu.register(up);
-        var lp = Xs().isBrowser,
-            cp = function() {
+            lp = new up(null);
+        pu.register(lp);
+        var cp = $s().isBrowser,
+            dp = function() {
                 function e(e) {
-                    void 0 === e && (e = {}), this.cookies = new tt, this.store = lp ? window.localStorage : Object.create(null), this.cookies = e.req ? new tt(e.req.headers.cookie) : new tt, Object.assign(this.store, this.cookies.getAll())
+                    void 0 === e && (e = {}), this.cookies = new tt, this.store = cp ? window.localStorage : Object.create(null), this.cookies = e.req ? new tt(e.req.headers.cookie) : new tt, Object.assign(this.store, this.cookies.getAll())
                 }
                 return Object.defineProperty(e.prototype, "length", {
                     get: function() {
                         return Object.entries(this.store).length
                     },
                     enumerable: !0,
                     configurable: !0
@@ -65787,22 +65835,22 @@
                     var n = e.split(".").pop();
                     ["LastAuthUser", "accessToken", "refreshToken", "idToken"].includes(null !== n && void 0 !== n ? n : "") && this.setUniversalItem(e, t, {
                         expires: new Date(Date.now() + 31536e6)
                     })
                 }, e.prototype.setLocalItem = function(e, t) {
                     this.store[e] = t
                 }, e.prototype.setUniversalItem = function(e, t, n) {
-                    void 0 === n && (n = {}), this.cookies.set(e, t, zs(zs({}, n), {
+                    void 0 === n && (n = {}), this.cookies.set(e, t, Us(Us({}, n), {
                         path: "/",
                         sameSite: !0,
-                        secure: !lp || "localhost" !== window.location.hostname
+                        secure: !cp || "localhost" !== window.location.hostname
                     }))
                 }, e
             }();
-        var dp, fp = function() {
+        var fp, pp = function() {
                 function e(e) {
                     var t = e || {},
                         n = t.ValidationData,
                         r = t.Username,
                         o = t.Password,
                         i = t.AuthParameters,
                         a = t.ClientMetadata;
@@ -65817,253 +65865,253 @@
                     return this.validationData
                 }, t.getAuthParameters = function() {
                     return this.authParameters
                 }, t.getClientMetadata = function() {
                     return this.clientMetadata
                 }, e
             }(),
-            pp = __webpack_require__(2890);
+            hp = __webpack_require__(2890);
 
-        function hp() {
-            if (dp) {
-                if ("function" === typeof dp.getRandomValues) try {
-                    return dp.getRandomValues(new Uint32Array(1))[0]
+        function gp() {
+            if (fp) {
+                if ("function" === typeof fp.getRandomValues) try {
+                    return fp.getRandomValues(new Uint32Array(1))[0]
                 } catch (e) {}
-                if ("function" === typeof dp.randomBytes) try {
-                    return dp.randomBytes(4).readInt32LE()
+                if ("function" === typeof fp.randomBytes) try {
+                    return fp.randomBytes(4).readInt32LE()
                 } catch (e) {}
             }
             throw new Error("Native crypto module could not be used to get secure random number.")
         }
-        "undefined" !== typeof window && window.crypto && (dp = window.crypto), !dp && "undefined" !== typeof window && window.msCrypto && (dp = window.msCrypto);
-        var gp, yp = function() {
+        "undefined" !== typeof window && window.crypto && (fp = window.crypto), !fp && "undefined" !== typeof window && window.msCrypto && (fp = window.msCrypto);
+        var yp, mp = function() {
                 function e(e, t) {
                     e = this.words = e || [], this.sigBytes = void 0 != t ? t : 4 * e.length
                 }
                 var t = e.prototype;
                 return t.random = function(t) {
-                    for (var n = [], r = 0; r < t; r += 4) n.push(hp());
+                    for (var n = [], r = 0; r < t; r += 4) n.push(gp());
                     return new e(n, t)
                 }, t.toString = function() {
                     return function(e) {
                         for (var t = e.words, n = e.sigBytes, r = [], o = 0; o < n; o++) {
                             var i = t[o >>> 2] >>> 24 - o % 4 * 8 & 255;
                             r.push((i >>> 4).toString(16)), r.push((15 & i).toString(16))
                         }
                         return r.join("")
                     }(this)
                 }, e
             }(),
-            mp = __webpack_require__(6915),
-            vp = Mp;
+            vp = __webpack_require__(6915),
+            Mp = bp;
 
-        function Mp(e, t) {
+        function bp(e, t) {
             null != e && this.fromString(e, t)
         }
 
-        function bp() {
-            return new Mp(null)
+        function jp() {
+            return new bp(null)
         }
-        var jp = "undefined" !== typeof navigator;
-        jp && "Microsoft Internet Explorer" == navigator.appName ? (Mp.prototype.am = function(e, t, n, r, o, i) {
+        var wp = "undefined" !== typeof navigator;
+        wp && "Microsoft Internet Explorer" == navigator.appName ? (bp.prototype.am = function(e, t, n, r, o, i) {
             for (var a = 32767 & t, s = t >> 15; --i >= 0;) {
                 var u = 32767 & this[e],
                     l = this[e++] >> 15,
                     c = s * u + l * a;
                 o = ((u = a * u + ((32767 & c) << 15) + n[r] + (1073741823 & o)) >>> 30) + (c >>> 15) + s * l + (o >>> 30), n[r++] = 1073741823 & u
             }
             return o
-        }, gp = 30) : jp && "Netscape" != navigator.appName ? (Mp.prototype.am = function(e, t, n, r, o, i) {
+        }, yp = 30) : wp && "Netscape" != navigator.appName ? (bp.prototype.am = function(e, t, n, r, o, i) {
             for (; --i >= 0;) {
                 var a = t * this[e++] + n[r] + o;
                 o = Math.floor(a / 67108864), n[r++] = 67108863 & a
             }
             return o
-        }, gp = 26) : (Mp.prototype.am = function(e, t, n, r, o, i) {
+        }, yp = 26) : (bp.prototype.am = function(e, t, n, r, o, i) {
             for (var a = 16383 & t, s = t >> 14; --i >= 0;) {
                 var u = 16383 & this[e],
                     l = this[e++] >> 14,
                     c = s * u + l * a;
                 o = ((u = a * u + ((16383 & c) << 14) + n[r] + o) >> 28) + (c >> 14) + s * l, n[r++] = 268435455 & u
             }
             return o
-        }, gp = 28), Mp.prototype.DB = gp, Mp.prototype.DM = (1 << gp) - 1, Mp.prototype.DV = 1 << gp;
-        Mp.prototype.FV = Math.pow(2, 52), Mp.prototype.F1 = 52 - gp, Mp.prototype.F2 = 2 * gp - 52;
-        var wp, xp, Np = new Array;
-        for (wp = "0".charCodeAt(0), xp = 0; xp <= 9; ++xp) Np[wp++] = xp;
-        for (wp = "a".charCodeAt(0), xp = 10; xp < 36; ++xp) Np[wp++] = xp;
-        for (wp = "A".charCodeAt(0), xp = 10; xp < 36; ++xp) Np[wp++] = xp;
+        }, yp = 28), bp.prototype.DB = yp, bp.prototype.DM = (1 << yp) - 1, bp.prototype.DV = 1 << yp;
+        bp.prototype.FV = Math.pow(2, 52), bp.prototype.F1 = 52 - yp, bp.prototype.F2 = 2 * yp - 52;
+        var xp, Np, Ip = new Array;
+        for (xp = "0".charCodeAt(0), Np = 0; Np <= 9; ++Np) Ip[xp++] = Np;
+        for (xp = "a".charCodeAt(0), Np = 10; Np < 36; ++Np) Ip[xp++] = Np;
+        for (xp = "A".charCodeAt(0), Np = 10; Np < 36; ++Np) Ip[xp++] = Np;
 
-        function Ip(e) {
+        function Dp(e) {
             return "0123456789abcdefghijklmnopqrstuvwxyz".charAt(e)
         }
 
-        function Dp(e, t) {
-            var n = Np[e.charCodeAt(t)];
+        function Sp(e, t) {
+            var n = Ip[e.charCodeAt(t)];
             return null == n ? -1 : n
         }
 
-        function Sp(e) {
-            var t = bp();
+        function Lp(e) {
+            var t = jp();
             return t.fromInt(e), t
         }
 
-        function Lp(e) {
+        function kp(e) {
             var t, n = 1;
             return 0 != (t = e >>> 16) && (e = t, n += 16), 0 != (t = e >> 8) && (e = t, n += 8), 0 != (t = e >> 4) && (e = t, n += 4), 0 != (t = e >> 2) && (e = t, n += 2), 0 != (t = e >> 1) && (e = t, n += 1), n
         }
 
-        function kp(e) {
+        function Cp(e) {
             this.m = e, this.mp = e.invDigit(), this.mpl = 32767 & this.mp, this.mph = this.mp >> 15, this.um = (1 << e.DB - 15) - 1, this.mt2 = 2 * e.t
         }
 
-        function Cp(e) {
-            return pp.lW.from((new yp).random(e).toString(), "hex")
+        function Ep(e) {
+            return hp.lW.from((new mp).random(e).toString(), "hex")
         }
-        kp.prototype.convert = function(e) {
-            var t = bp();
-            return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(Mp.ZERO) > 0 && this.m.subTo(t, t), t
-        }, kp.prototype.revert = function(e) {
-            var t = bp();
+        Cp.prototype.convert = function(e) {
+            var t = jp();
+            return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(bp.ZERO) > 0 && this.m.subTo(t, t), t
+        }, Cp.prototype.revert = function(e) {
+            var t = jp();
             return e.copyTo(t), this.reduce(t), t
-        }, kp.prototype.reduce = function(e) {
+        }, Cp.prototype.reduce = function(e) {
             for (; e.t <= this.mt2;) e[e.t++] = 0;
             for (var t = 0; t < this.m.t; ++t) {
                 var n = 32767 & e[t],
                     r = n * this.mpl + ((n * this.mph + (e[t] >> 15) * this.mpl & this.um) << 15) & e.DM;
                 for (e[n = t + this.m.t] += this.m.am(0, r, e, t, 0, this.m.t); e[n] >= e.DV;) e[n] -= e.DV, e[++n]++
             }
             e.clamp(), e.drShiftTo(this.m.t, e), e.compareTo(this.m) >= 0 && e.subTo(this.m, e)
-        }, kp.prototype.mulTo = function(e, t, n) {
+        }, Cp.prototype.mulTo = function(e, t, n) {
             e.multiplyTo(t, n), this.reduce(n)
-        }, kp.prototype.sqrTo = function(e, t) {
+        }, Cp.prototype.sqrTo = function(e, t) {
             e.squareTo(t), this.reduce(t)
-        }, Mp.prototype.copyTo = function(e) {
+        }, bp.prototype.copyTo = function(e) {
             for (var t = this.t - 1; t >= 0; --t) e[t] = this[t];
             e.t = this.t, e.s = this.s
-        }, Mp.prototype.fromInt = function(e) {
+        }, bp.prototype.fromInt = function(e) {
             this.t = 1, this.s = e < 0 ? -1 : 0, e > 0 ? this[0] = e : e < -1 ? this[0] = e + this.DV : this.t = 0
-        }, Mp.prototype.fromString = function(e, t) {
+        }, bp.prototype.fromString = function(e, t) {
             var n;
             if (16 == t) n = 4;
             else if (8 == t) n = 3;
             else if (2 == t) n = 1;
             else if (32 == t) n = 5;
             else {
                 if (4 != t) throw new Error("Only radix 2, 4, 8, 16, 32 are supported");
                 n = 2
             }
             this.t = 0, this.s = 0;
             for (var r = e.length, o = !1, i = 0; --r >= 0;) {
-                var a = Dp(e, r);
+                var a = Sp(e, r);
                 a < 0 ? "-" == e.charAt(r) && (o = !0) : (o = !1, 0 == i ? this[this.t++] = a : i + n > this.DB ? (this[this.t - 1] |= (a & (1 << this.DB - i) - 1) << i, this[this.t++] = a >> this.DB - i) : this[this.t - 1] |= a << i, (i += n) >= this.DB && (i -= this.DB))
             }
-            this.clamp(), o && Mp.ZERO.subTo(this, this)
-        }, Mp.prototype.clamp = function() {
+            this.clamp(), o && bp.ZERO.subTo(this, this)
+        }, bp.prototype.clamp = function() {
             for (var e = this.s & this.DM; this.t > 0 && this[this.t - 1] == e;) --this.t
-        }, Mp.prototype.dlShiftTo = function(e, t) {
+        }, bp.prototype.dlShiftTo = function(e, t) {
             var n;
             for (n = this.t - 1; n >= 0; --n) t[n + e] = this[n];
             for (n = e - 1; n >= 0; --n) t[n] = 0;
             t.t = this.t + e, t.s = this.s
-        }, Mp.prototype.drShiftTo = function(e, t) {
+        }, bp.prototype.drShiftTo = function(e, t) {
             for (var n = e; n < this.t; ++n) t[n - e] = this[n];
             t.t = Math.max(this.t - e, 0), t.s = this.s
-        }, Mp.prototype.lShiftTo = function(e, t) {
+        }, bp.prototype.lShiftTo = function(e, t) {
             var n, r = e % this.DB,
                 o = this.DB - r,
                 i = (1 << o) - 1,
                 a = Math.floor(e / this.DB),
                 s = this.s << r & this.DM;
             for (n = this.t - 1; n >= 0; --n) t[n + a + 1] = this[n] >> o | s, s = (this[n] & i) << r;
             for (n = a - 1; n >= 0; --n) t[n] = 0;
             t[a] = s, t.t = this.t + a + 1, t.s = this.s, t.clamp()
-        }, Mp.prototype.rShiftTo = function(e, t) {
+        }, bp.prototype.rShiftTo = function(e, t) {
             t.s = this.s;
             var n = Math.floor(e / this.DB);
             if (n >= this.t) t.t = 0;
             else {
                 var r = e % this.DB,
                     o = this.DB - r,
                     i = (1 << r) - 1;
                 t[0] = this[n] >> r;
                 for (var a = n + 1; a < this.t; ++a) t[a - n - 1] |= (this[a] & i) << o, t[a - n] = this[a] >> r;
                 r > 0 && (t[this.t - n - 1] |= (this.s & i) << o), t.t = this.t - n, t.clamp()
             }
-        }, Mp.prototype.subTo = function(e, t) {
+        }, bp.prototype.subTo = function(e, t) {
             for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] - e[n], t[n++] = r & this.DM, r >>= this.DB;
             if (e.t < this.t) {
                 for (r -= e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += this.s
             } else {
                 for (r += this.s; n < e.t;) r -= e[n], t[n++] = r & this.DM, r >>= this.DB;
                 r -= e.s
             }
             t.s = r < 0 ? -1 : 0, r < -1 ? t[n++] = this.DV + r : r > 0 && (t[n++] = r), t.t = n, t.clamp()
-        }, Mp.prototype.multiplyTo = function(e, t) {
+        }, bp.prototype.multiplyTo = function(e, t) {
             var n = this.abs(),
                 r = e.abs(),
                 o = n.t;
             for (t.t = o + r.t; --o >= 0;) t[o] = 0;
             for (o = 0; o < r.t; ++o) t[o + n.t] = n.am(0, r[o], t, o, 0, n.t);
-            t.s = 0, t.clamp(), this.s != e.s && Mp.ZERO.subTo(t, t)
-        }, Mp.prototype.squareTo = function(e) {
+            t.s = 0, t.clamp(), this.s != e.s && bp.ZERO.subTo(t, t)
+        }, bp.prototype.squareTo = function(e) {
             for (var t = this.abs(), n = e.t = 2 * t.t; --n >= 0;) e[n] = 0;
             for (n = 0; n < t.t - 1; ++n) {
                 var r = t.am(n, t[n], e, 2 * n, 0, 1);
                 (e[n + t.t] += t.am(n + 1, 2 * t[n], e, 2 * n + 1, r, t.t - n - 1)) >= t.DV && (e[n + t.t] -= t.DV, e[n + t.t + 1] = 1)
             }
             e.t > 0 && (e[e.t - 1] += t.am(n, t[n], e, 2 * n, 0, 1)), e.s = 0, e.clamp()
-        }, Mp.prototype.divRemTo = function(e, t, n) {
+        }, bp.prototype.divRemTo = function(e, t, n) {
             var r = e.abs();
             if (!(r.t <= 0)) {
                 var o = this.abs();
                 if (o.t < r.t) return null != t && t.fromInt(0), void(null != n && this.copyTo(n));
-                null == n && (n = bp());
-                var i = bp(),
+                null == n && (n = jp());
+                var i = jp(),
                     a = this.s,
                     s = e.s,
-                    u = this.DB - Lp(r[r.t - 1]);
+                    u = this.DB - kp(r[r.t - 1]);
                 u > 0 ? (r.lShiftTo(u, i), o.lShiftTo(u, n)) : (r.copyTo(i), o.copyTo(n));
                 var l = i.t,
                     c = i[l - 1];
                 if (0 != c) {
                     var d = c * (1 << this.F1) + (l > 1 ? i[l - 2] >> this.F2 : 0),
                         f = this.FV / d,
                         p = (1 << this.F1) / d,
                         h = 1 << this.F2,
                         g = n.t,
                         y = g - l,
-                        m = null == t ? bp() : t;
-                    for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), Mp.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
+                        m = null == t ? jp() : t;
+                    for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), bp.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
                     for (; --y >= 0;) {
                         var v = n[--g] == c ? this.DM : Math.floor(n[g] * f + (n[g - 1] + h) * p);
                         if ((n[g] += i.am(0, v, n, y, 0, l)) < v)
                             for (i.dlShiftTo(y, m), n.subTo(m, n); n[g] < --v;) n.subTo(m, n)
                     }
-                    null != t && (n.drShiftTo(l, t), a != s && Mp.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && Mp.ZERO.subTo(n, n)
+                    null != t && (n.drShiftTo(l, t), a != s && bp.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && bp.ZERO.subTo(n, n)
                 }
             }
-        }, Mp.prototype.invDigit = function() {
+        }, bp.prototype.invDigit = function() {
             if (this.t < 1) return 0;
             var e = this[0];
             if (0 == (1 & e)) return 0;
             var t = 3 & e;
             return (t = (t = (t = (t = t * (2 - (15 & e) * t) & 15) * (2 - (255 & e) * t) & 255) * (2 - ((65535 & e) * t & 65535)) & 65535) * (2 - e * t % this.DV) % this.DV) > 0 ? this.DV - t : -t
-        }, Mp.prototype.addTo = function(e, t) {
+        }, bp.prototype.addTo = function(e, t) {
             for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] + e[n], t[n++] = r & this.DM, r >>= this.DB;
             if (e.t < this.t) {
                 for (r += e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += this.s
             } else {
                 for (r += this.s; n < e.t;) r += e[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += e.s
             }
             t.s = r < 0 ? -1 : 0, r > 0 ? t[n++] = r : r < -1 && (t[n++] = this.DV + r), t.t = n, t.clamp()
-        }, Mp.prototype.toString = function(e) {
+        }, bp.prototype.toString = function(e) {
             if (this.s < 0) return "-" + this.negate().toString(e);
             var t;
             if (16 == e) t = 4;
             else if (8 == e) t = 3;
             else if (2 == e) t = 1;
             else if (32 == e) t = 5;
             else {
@@ -66072,236 +66120,236 @@
             }
             var n, r = (1 << t) - 1,
                 o = !1,
                 i = "",
                 a = this.t,
                 s = this.DB - a * this.DB % t;
             if (a-- > 0)
-                for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = Ip(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += Ip(n));
+                for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = Dp(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += Dp(n));
             return o ? i : "0"
-        }, Mp.prototype.negate = function() {
-            var e = bp();
-            return Mp.ZERO.subTo(this, e), e
-        }, Mp.prototype.abs = function() {
+        }, bp.prototype.negate = function() {
+            var e = jp();
+            return bp.ZERO.subTo(this, e), e
+        }, bp.prototype.abs = function() {
             return this.s < 0 ? this.negate() : this
-        }, Mp.prototype.compareTo = function(e) {
+        }, bp.prototype.compareTo = function(e) {
             var t = this.s - e.s;
             if (0 != t) return t;
             var n = this.t;
             if (0 != (t = n - e.t)) return this.s < 0 ? -t : t;
             for (; --n >= 0;)
                 if (0 != (t = this[n] - e[n])) return t;
             return 0
-        }, Mp.prototype.bitLength = function() {
-            return this.t <= 0 ? 0 : this.DB * (this.t - 1) + Lp(this[this.t - 1] ^ this.s & this.DM)
-        }, Mp.prototype.mod = function(e) {
-            var t = bp();
-            return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(Mp.ZERO) > 0 && e.subTo(t, t), t
-        }, Mp.prototype.equals = function(e) {
+        }, bp.prototype.bitLength = function() {
+            return this.t <= 0 ? 0 : this.DB * (this.t - 1) + kp(this[this.t - 1] ^ this.s & this.DM)
+        }, bp.prototype.mod = function(e) {
+            var t = jp();
+            return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(bp.ZERO) > 0 && e.subTo(t, t), t
+        }, bp.prototype.equals = function(e) {
             return 0 == this.compareTo(e)
-        }, Mp.prototype.add = function(e) {
-            var t = bp();
+        }, bp.prototype.add = function(e) {
+            var t = jp();
             return this.addTo(e, t), t
-        }, Mp.prototype.subtract = function(e) {
-            var t = bp();
+        }, bp.prototype.subtract = function(e) {
+            var t = jp();
             return this.subTo(e, t), t
-        }, Mp.prototype.multiply = function(e) {
-            var t = bp();
+        }, bp.prototype.multiply = function(e) {
+            var t = jp();
             return this.multiplyTo(e, t), t
-        }, Mp.prototype.divide = function(e) {
-            var t = bp();
+        }, bp.prototype.divide = function(e) {
+            var t = jp();
             return this.divRemTo(e, t, null), t
-        }, Mp.prototype.modPow = function(e, t, n) {
+        }, bp.prototype.modPow = function(e, t, n) {
             var r, o = e.bitLength(),
-                i = Sp(1),
-                a = new kp(t);
+                i = Lp(1),
+                a = new Cp(t);
             if (o <= 0) return i;
             r = o < 18 ? 1 : o < 48 ? 3 : o < 144 ? 4 : o < 768 ? 5 : 6;
             var s = new Array,
                 u = 3,
                 l = r - 1,
                 c = (1 << r) - 1;
             if (s[1] = a.convert(this), r > 1) {
-                var d = bp();
-                for (a.sqrTo(s[1], d); u <= c;) s[u] = bp(), a.mulTo(d, s[u - 2], s[u]), u += 2
+                var d = jp();
+                for (a.sqrTo(s[1], d); u <= c;) s[u] = jp(), a.mulTo(d, s[u - 2], s[u]), u += 2
             }
             var f, p, h = e.t - 1,
                 g = !0,
-                y = bp();
-            for (o = Lp(e[h]) - 1; h >= 0;) {
+                y = jp();
+            for (o = kp(e[h]) - 1; h >= 0;) {
                 for (o >= l ? f = e[h] >> o - l & c : (f = (e[h] & (1 << o + 1) - 1) << l - o, h > 0 && (f |= e[h - 1] >> this.DB + o - l)), u = r; 0 == (1 & f);) f >>= 1, --u;
                 if ((o -= u) < 0 && (o += this.DB, --h), g) s[f].copyTo(i), g = !1;
                 else {
                     for (; u > 1;) a.sqrTo(i, y), a.sqrTo(y, i), u -= 2;
                     u > 0 ? a.sqrTo(i, y) : (p = i, i = y, y = p), a.mulTo(y, s[f], i)
                 }
                 for (; h >= 0 && 0 == (e[h] & 1 << o);) a.sqrTo(i, y), p = i, i = y, y = p, --o < 0 && (o = this.DB - 1, --h)
             }
             var m = a.revert(i);
             return n(null, m), m
-        }, Mp.ZERO = Sp(0), Mp.ONE = Sp(1);
-        var Ep = /^[89a-f]/i,
-            _p = function() {
+        }, bp.ZERO = Lp(0), bp.ONE = Lp(1);
+        var _p = /^[89a-f]/i,
+            Tp = function() {
                 function e(e) {
-                    this.N = new vp("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new vp("2", 16), this.k = new vp(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = pp.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
+                    this.N = new Mp("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new Mp("2", 16), this.k = new Mp(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = hp.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
                 }
                 var t = e.prototype;
                 return t.getSmallAValue = function() {
                     return this.smallAValue
                 }, t.getLargeAValue = function(e) {
                     var t = this;
                     this.largeAValue ? e(null, this.largeAValue) : this.calculateA(this.smallAValue, (function(n, r) {
                         n && e(n, null), t.largeAValue = r, e(null, t.largeAValue)
                     }))
                 }, t.generateRandomSmallA = function() {
-                    var e = Cp(128).toString("hex");
-                    return new vp(e, 16)
+                    var e = Ep(128).toString("hex");
+                    return new Mp(e, 16)
                 }, t.generateRandomString = function() {
-                    return Cp(40).toString("base64")
+                    return Ep(40).toString("base64")
                 }, t.getRandomPassword = function() {
                     return this.randomPassword
                 }, t.getSaltDevices = function() {
                     return this.SaltToHashDevices
                 }, t.getVerifierDevices = function() {
                     return this.verifierDevices
                 }, t.generateHashDevice = function(e, t, n) {
                     var r = this;
                     this.randomPassword = this.generateRandomString();
                     var o = "" + e + t + ":" + this.randomPassword,
                         i = this.hash(o),
-                        a = Cp(16).toString("hex");
-                    this.SaltToHashDevices = this.padHex(new vp(a, 16)), this.g.modPow(new vp(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
+                        a = Ep(16).toString("hex");
+                    this.SaltToHashDevices = this.padHex(new Mp(a, 16)), this.g.modPow(new Mp(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
                         e && n(e, null), r.verifierDevices = r.padHex(t), n(null, null)
                     }))
                 }, t.calculateA = function(e, t) {
                     var n = this;
                     this.g.modPow(e, this.N, (function(e, r) {
-                        e && t(e, null), r.mod(n.N).equals(vp.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
+                        e && t(e, null), r.mod(n.N).equals(Mp.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
                     }))
                 }, t.calculateU = function(e, t) {
-                    return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new vp(this.UHexHash, 16)
+                    return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new Mp(this.UHexHash, 16)
                 }, t.hash = function(e) {
-                    var t = new mp.Sha256;
+                    var t = new vp.Sha256;
                     t.update(e);
                     var n = t.digestSync(),
-                        r = pp.lW.from(n).toString("hex");
+                        r = hp.lW.from(n).toString("hex");
                     return new Array(64 - r.length).join("0") + r
                 }, t.hexHash = function(e) {
-                    return this.hash(pp.lW.from(e, "hex"))
+                    return this.hash(hp.lW.from(e, "hex"))
                 }, t.computehkdf = function(e, t) {
-                    var n = pp.lW.concat([this.infoBits, pp.lW.from(String.fromCharCode(1), "utf8")]),
-                        r = new mp.Sha256(t);
+                    var n = hp.lW.concat([this.infoBits, hp.lW.from(String.fromCharCode(1), "utf8")]),
+                        r = new vp.Sha256(t);
                     r.update(e);
                     var o = r.digestSync(),
-                        i = new mp.Sha256(o);
+                        i = new vp.Sha256(o);
                     return i.update(n), i.digestSync().slice(0, 16)
                 }, t.getPasswordAuthenticationKey = function(e, t, n, r, o) {
                     var i = this;
-                    if (n.mod(this.N).equals(vp.ZERO)) throw new Error("B cannot be zero.");
-                    if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(vp.ZERO)) throw new Error("U cannot be zero.");
+                    if (n.mod(this.N).equals(Mp.ZERO)) throw new Error("B cannot be zero.");
+                    if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(Mp.ZERO)) throw new Error("U cannot be zero.");
                     var a = "" + this.poolName + e + ":" + t,
                         s = this.hash(a),
-                        u = new vp(this.hexHash(this.padHex(r) + s), 16);
+                        u = new Mp(this.hexHash(this.padHex(r) + s), 16);
                     this.calculateS(u, n, (function(e, t) {
                         e && o(e, null);
-                        var n = i.computehkdf(pp.lW.from(i.padHex(t), "hex"), pp.lW.from(i.padHex(i.UValue), "hex"));
+                        var n = i.computehkdf(hp.lW.from(i.padHex(t), "hex"), hp.lW.from(i.padHex(i.UValue), "hex"));
                         o(null, n)
                     }))
                 }, t.calculateS = function(e, t, n) {
                     var r = this;
                     this.g.modPow(e, this.N, (function(o, i) {
                         o && n(o, null), t.subtract(r.k.multiply(i)).modPow(r.smallAValue.add(r.UValue.multiply(e)), r.N, (function(e, t) {
                             e && n(e, null), n(null, t.mod(r.N))
                         }))
                     }))
                 }, t.getNewPasswordRequiredChallengeUserAttributePrefix = function() {
                     return "userAttributes."
                 }, t.padHex = function(e) {
-                    if (!(e instanceof vp)) throw new Error("Not a BigInteger");
-                    var t = e.compareTo(vp.ZERO) < 0,
+                    if (!(e instanceof Mp)) throw new Error("Not a BigInteger");
+                    var t = e.compareTo(Mp.ZERO) < 0,
                         n = e.abs().toString(16);
-                    if (n = n.length % 2 !== 0 ? "0" + n : n, n = Ep.test(n) ? "00" + n : n, t) {
+                    if (n = n.length % 2 !== 0 ? "0" + n : n, n = _p.test(n) ? "00" + n : n, t) {
                         var r = n.split("").map((function(e) {
                             var t = 15 & ~parseInt(e, 16);
                             return "0123456789ABCDEF".charAt(t)
                         })).join("");
-                        (n = new vp(r, 16).add(vp.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
+                        (n = new Mp(r, 16).add(Mp.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
                     }
                     return n
                 }, e
             }(),
-            Tp = function() {
+            Ap = function() {
                 function e(e) {
                     this.jwtToken = e || "", this.payload = this.decodePayload()
                 }
                 var t = e.prototype;
                 return t.getJwtToken = function() {
                     return this.jwtToken
                 }, t.getExpiration = function() {
                     return this.payload.exp
                 }, t.getIssuedAt = function() {
                     return this.payload.iat
                 }, t.decodePayload = function() {
                     var e = this.jwtToken.split(".")[1];
                     try {
-                        return JSON.parse(pp.lW.from(e, "base64").toString("utf8"))
+                        return JSON.parse(hp.lW.from(e, "base64").toString("utf8"))
                     } catch (t) {
                         return {}
                     }
                 }, e
             }();
 
-        function Ap(e, t) {
-            return Ap = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function Op(e, t) {
+            return Op = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, Ap(e, t)
+            }, Op(e, t)
         }
-        var Op = function(e) {
+        var zp = function(e) {
             var t, n;
 
             function r(t) {
                 var n = (void 0 === t ? {} : t).AccessToken;
                 return e.call(this, n || "") || this
             }
-            return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Ap(t, n), r
-        }(Tp);
+            return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Op(t, n), r
+        }(Ap);
 
-        function zp(e, t) {
-            return zp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function Up(e, t) {
+            return Up = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, zp(e, t)
+            }, Up(e, t)
         }
-        var Up = function(e) {
+        var Pp = function(e) {
                 var t, n;
 
                 function r(t) {
                     var n = (void 0 === t ? {} : t).IdToken;
                     return e.call(this, n || "") || this
                 }
-                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, zp(t, n), r
-            }(Tp),
-            Pp = function() {
+                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Up(t, n), r
+            }(Ap),
+            Rp = function() {
                 function e(e) {
                     var t = (void 0 === e ? {} : e).RefreshToken;
                     this.token = t || ""
                 }
                 return e.prototype.getToken = function() {
                     return this.token
                 }, e
             }(),
-            Rp = {
+            Bp = {
                 userAgent: "aws-amplify/5.0.4 js",
                 product: "",
                 navigator: null,
                 isReactNative: !1
             };
         if ("undefined" !== typeof navigator && navigator.product)
-            if (Rp.product = navigator.product || "", Rp.navigator = navigator || null, "ReactNative" === navigator.product) Rp.userAgent = "aws-amplify/5.0.4 react-native", Rp.isReactNative = !0;
-            else Rp.userAgent = "aws-amplify/5.0.4 js", Rp.isReactNative = !1;
-        var Bp = function() {
+            if (Bp.product = navigator.product || "", Bp.navigator = navigator || null, "ReactNative" === navigator.product) Bp.userAgent = "aws-amplify/5.0.4 react-native", Bp.isReactNative = !0;
+            else Bp.userAgent = "aws-amplify/5.0.4 js", Bp.isReactNative = !1;
+        var Fp = function() {
                 function e(e) {
                     var t = void 0 === e ? {} : e,
                         n = t.IdToken,
                         r = t.RefreshToken,
                         o = t.AccessToken,
                         i = t.ClockDrift;
                     if (null == o || null == n) throw new Error("Id token and Access Token must be present.");
@@ -66319,32 +66367,32 @@
                 }, t.calculateClockDrift = function() {
                     return Math.floor(new Date / 1e3) - Math.min(this.accessToken.getIssuedAt(), this.idToken.getIssuedAt())
                 }, t.isValid = function() {
                     var e = Math.floor(new Date / 1e3) - this.clockDrift;
                     return e < this.accessToken.getExpiration() && e < this.idToken.getExpiration()
                 }, e
             }(),
-            Fp = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
-            Yp = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
-            Qp = function() {
+            Yp = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
+            Qp = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
+            Gp = function() {
                 function e() {}
                 return e.prototype.getNowString = function() {
                     var e = new Date,
-                        t = Yp[e.getUTCDay()],
-                        n = Fp[e.getUTCMonth()],
+                        t = Qp[e.getUTCDay()],
+                        n = Yp[e.getUTCMonth()],
                         r = e.getUTCDate(),
                         o = e.getUTCHours();
                     o < 10 && (o = "0" + o);
                     var i = e.getUTCMinutes();
                     i < 10 && (i = "0" + i);
                     var a = e.getUTCSeconds();
                     return a < 10 && (a = "0" + a), t + " " + n + " " + r + " " + o + ":" + i + ":" + a + " UTC " + e.getUTCFullYear()
                 }, e
             }(),
-            Gp = function() {
+            Wp = function() {
                 function e(e) {
                     var t = void 0 === e ? {} : e,
                         n = t.Name,
                         r = t.Value;
                     this.Name = n || "", this.Value = r || ""
                 }
                 var t = e.prototype;
@@ -66361,44 +66409,44 @@
                 }, t.toJSON = function() {
                     return {
                         Name: this.Name,
                         Value: this.Value
                     }
                 }, e
             }(),
-            Wp = {},
-            Hp = function() {
+            Hp = {},
+            Zp = function() {
                 function e() {}
                 return e.setItem = function(e, t) {
-                    return Wp[e] = t, Wp[e]
+                    return Hp[e] = t, Hp[e]
                 }, e.getItem = function(e) {
-                    return Object.prototype.hasOwnProperty.call(Wp, e) ? Wp[e] : void 0
+                    return Object.prototype.hasOwnProperty.call(Hp, e) ? Hp[e] : void 0
                 }, e.removeItem = function(e) {
-                    return delete Wp[e]
+                    return delete Hp[e]
                 }, e.clear = function() {
-                    return Wp = {}
+                    return Hp = {}
                 }, e
             }(),
-            Zp = function() {
+            Vp = function() {
                 function e() {
                     try {
                         this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.cognito.test-ls", 1), this.storageWindow.removeItem("aws.cognito.test-ls")
                     } catch (e) {
-                        this.storageWindow = Hp
+                        this.storageWindow = Zp
                     }
                 }
                 return e.prototype.getStorage = function() {
                     return this.storageWindow
                 }, e
             }(),
-            Vp = "undefined" !== typeof navigator ? Rp.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
-            qp = function() {
+            qp = "undefined" !== typeof navigator ? Bp.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
+            Jp = function() {
                 function e(e) {
                     if (null == e || null == e.Username || null == e.Pool) throw new Error("Username and Pool information are required.");
-                    this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new Zp).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
+                    this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new Vp).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
                 }
                 var t = e.prototype;
                 return t.setSignInUserSession = function(e) {
                     this.clearCachedUserData(), this.signInUserSession = e, this.cacheTokens()
                 }, t.getSignInUserSession = function() {
                     return this.signInUserSession
                 }, t.getUsername = function() {
@@ -66424,37 +66472,37 @@
                             i = r.ChallengeParameters;
                         return "CUSTOM_CHALLENGE" === o ? (n.Session = r.Session, t.customChallenge(i)) : (n.signInUserSession = n.getCognitoUserSession(r.AuthenticationResult), n.cacheTokens(), t.onSuccess(n.signInUserSession))
                     }))
                 }, t.authenticateUser = function(e, t) {
                     return "USER_PASSWORD_AUTH" === this.authenticationFlowType ? this.authenticateUserPlainUsernamePassword(e, t) : "USER_SRP_AUTH" === this.authenticationFlowType || "CUSTOM_AUTH" === this.authenticationFlowType ? this.authenticateUserDefaultAuth(e, t) : t.onFailure(new Error("Authentication flow type is invalid."))
                 }, t.authenticateUserDefaultAuth = function(e, t) {
                     var n, r, o = this,
-                        i = new _p(this.pool.getUserPoolName()),
-                        a = new Qp,
+                        i = new Tp(this.pool.getUserPoolName()),
+                        a = new Gp,
                         s = {};
                     null != this.deviceKey && (s.DEVICE_KEY = this.deviceKey), s.USERNAME = this.username, i.getLargeAValue((function(u, l) {
                         u && t.onFailure(u), s.SRP_A = l.toString(16), "CUSTOM_AUTH" === o.authenticationFlowType && (s.CHALLENGE_NAME = "SRP_A");
                         var c = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                             d = {
                                 AuthFlow: o.authenticationFlowType,
                                 ClientId: o.pool.getClientId(),
                                 AuthParameters: s,
                                 ClientMetadata: c
                             };
                         o.getUserContextData(o.username) && (d.UserContextData = o.getUserContextData(o.username)), o.client.request("InitiateAuth", d, (function(s, u) {
                             if (s) return t.onFailure(s);
                             var l = u.ChallengeParameters;
-                            o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new vp(l.SRP_B, 16), r = new vp(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
+                            o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new Mp(l.SRP_B, 16), r = new Mp(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
                                 e && t.onFailure(e);
                                 var r = a.getNowString(),
-                                    s = pp.lW.concat([pp.lW.from(o.pool.getUserPoolName(), "utf8"), pp.lW.from(o.username, "utf8"), pp.lW.from(l.SECRET_BLOCK, "base64"), pp.lW.from(r, "utf8")]),
-                                    d = new mp.Sha256(n);
+                                    s = hp.lW.concat([hp.lW.from(o.pool.getUserPoolName(), "utf8"), hp.lW.from(o.username, "utf8"), hp.lW.from(l.SECRET_BLOCK, "base64"), hp.lW.from(r, "utf8")]),
+                                    d = new vp.Sha256(n);
                                 d.update(s);
                                 var f = d.digestSync(),
-                                    p = pp.lW.from(f).toString("base64"),
+                                    p = hp.lW.from(f).toString("base64"),
                                     h = {};
                                 h.USERNAME = o.username, h.PASSWORD_CLAIM_SECRET_BLOCK = l.SECRET_BLOCK, h.TIMESTAMP = r, h.PASSWORD_CLAIM_SIGNATURE = p, null != o.deviceKey && (h.DEVICE_KEY = o.deviceKey);
                                 var g = {
                                     ChallengeName: "PASSWORD_VERIFIER",
                                     ClientId: o.pool.getClientId(),
                                     ChallengeResponses: h,
                                     Session: u.Session,
@@ -66471,15 +66519,15 @@
                             }))
                         }))
                     }))
                 }, t.authenticateUserPlainUsernamePassword = function(e, t) {
                     var n = this,
                         r = {};
                     if (r.USERNAME = this.username, r.PASSWORD = e.getPassword(), r.PASSWORD) {
-                        var o = new _p(this.pool.getUserPoolName());
+                        var o = new Tp(this.pool.getUserPoolName());
                         this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (r.DEVICE_KEY = this.deviceKey);
                         var i = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                             a = {
                                 AuthFlow: "USER_PASSWORD_AUTH",
                                 ClientId: this.pool.getClientId(),
                                 AuthParameters: r,
                                 ClientMetadata: i
@@ -66510,30 +66558,30 @@
                     if ("DEVICE_SRP_AUTH" === o) return this.Session = e.Session, void this.getDeviceResponse(n);
                     this.signInUserSession = this.getCognitoUserSession(e.AuthenticationResult), this.challengeName = o, this.cacheTokens();
                     var d = e.AuthenticationResult.NewDeviceMetadata;
                     if (null == d) return n.onSuccess(this.signInUserSession);
                     t.generateHashDevice(e.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, e.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(o) {
                         if (o) return n.onFailure(o);
                         var i = {
-                            Salt: pp.lW.from(t.getSaltDevices(), "hex").toString("base64"),
-                            PasswordVerifier: pp.lW.from(t.getVerifierDevices(), "hex").toString("base64")
+                            Salt: hp.lW.from(t.getSaltDevices(), "hex").toString("base64"),
+                            PasswordVerifier: hp.lW.from(t.getVerifierDevices(), "hex").toString("base64")
                         };
                         r.verifierDevices = i.PasswordVerifier, r.deviceGroupKey = d.DeviceGroupKey, r.randomPassword = t.getRandomPassword(), r.client.request("ConfirmDevice", {
                             DeviceKey: d.DeviceKey,
                             AccessToken: r.signInUserSession.getAccessToken().getJwtToken(),
                             DeviceSecretVerifierConfig: i,
-                            DeviceName: Vp
+                            DeviceName: qp
                         }, (function(t, o) {
                             return t ? n.onFailure(t) : (r.deviceKey = e.AuthenticationResult.NewDeviceMetadata.DeviceKey, r.cacheDeviceKeyAndPassword(), !0 === o.UserConfirmationNecessary ? n.onSuccess(r.signInUserSession, o.UserConfirmationNecessary) : n.onSuccess(r.signInUserSession))
                         }))
                     }))
                 }, t.completeNewPasswordChallenge = function(e, t, n, r) {
                     var o = this;
                     if (!e) return n.onFailure(new Error("New password is required."));
-                    var i = new _p(this.pool.getUserPoolName()),
+                    var i = new Tp(this.pool.getUserPoolName()),
                         a = i.getNewPasswordRequiredChallengeUserAttributePrefix(),
                         s = {};
                     t && Object.keys(t).forEach((function(e) {
                         s[a + e] = t[e]
                     })), s.NEW_PASSWORD = e, s.USERNAME = this.username;
                     var u = {
                         ChallengeName: "NEW_PASSWORD_REQUIRED",
@@ -66543,39 +66591,39 @@
                         ClientMetadata: r
                     };
                     this.getUserContextData() && (u.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", u, (function(e, t) {
                         return e ? n.onFailure(e) : o.authenticateUserInternal(t, i, n)
                     }))
                 }, t.getDeviceResponse = function(e, t) {
                     var n = this,
-                        r = new _p(this.deviceGroupKey),
-                        o = new Qp,
+                        r = new Tp(this.deviceGroupKey),
+                        o = new Gp,
                         i = {};
                     i.USERNAME = this.username, i.DEVICE_KEY = this.deviceKey, r.getLargeAValue((function(a, s) {
                         a && e.onFailure(a), i.SRP_A = s.toString(16);
                         var u = {
                             ChallengeName: "DEVICE_SRP_AUTH",
                             ClientId: n.pool.getClientId(),
                             ChallengeResponses: i,
                             ClientMetadata: t,
                             Session: n.Session
                         };
                         n.getUserContextData() && (u.UserContextData = n.getUserContextData()), n.client.request("RespondToAuthChallenge", u, (function(t, i) {
                             if (t) return e.onFailure(t);
                             var a = i.ChallengeParameters,
-                                s = new vp(a.SRP_B, 16),
-                                u = new vp(a.SALT, 16);
+                                s = new Mp(a.SRP_B, 16),
+                                u = new Mp(a.SALT, 16);
                             r.getPasswordAuthenticationKey(n.deviceKey, n.randomPassword, s, u, (function(t, r) {
                                 if (t) return e.onFailure(t);
                                 var s = o.getNowString(),
-                                    u = pp.lW.concat([pp.lW.from(n.deviceGroupKey, "utf8"), pp.lW.from(n.deviceKey, "utf8"), pp.lW.from(a.SECRET_BLOCK, "base64"), pp.lW.from(s, "utf8")]),
-                                    l = new mp.Sha256(r);
+                                    u = hp.lW.concat([hp.lW.from(n.deviceGroupKey, "utf8"), hp.lW.from(n.deviceKey, "utf8"), hp.lW.from(a.SECRET_BLOCK, "base64"), hp.lW.from(s, "utf8")]),
+                                    l = new vp.Sha256(r);
                                 l.update(u);
                                 var c = l.digestSync(),
-                                    d = pp.lW.from(c).toString("base64"),
+                                    d = hp.lW.from(c).toString("base64"),
                                     f = {};
                                 f.USERNAME = n.username, f.PASSWORD_CLAIM_SECRET_BLOCK = a.SECRET_BLOCK, f.TIMESTAMP = s, f.PASSWORD_CLAIM_SIGNATURE = d, f.DEVICE_KEY = n.deviceKey;
                                 var p = {
                                     ChallengeName: "DEVICE_PASSWORD_VERIFIER",
                                     ClientId: n.pool.getClientId(),
                                     ChallengeResponses: f,
                                     Session: i.Session
@@ -66597,15 +66645,15 @@
                     this.getUserContextData() && (o.UserContextData = this.getUserContextData()), this.client.request("ConfirmSignUp", o, (function(e) {
                         return e ? n(e, null) : n(null, "SUCCESS")
                     }))
                 }, t.sendCustomChallengeAnswer = function(e, t, n) {
                     var r = this,
                         o = {};
                     o.USERNAME = this.username, o.ANSWER = e;
-                    var i = new _p(this.pool.getUserPoolName());
+                    var i = new Tp(this.pool.getUserPoolName());
                     this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (o.DEVICE_KEY = this.deviceKey);
                     var a = {
                         ChallengeName: "CUSTOM_CHALLENGE",
                         ChallengeResponses: o,
                         ClientId: this.pool.getClientId(),
                         Session: this.Session,
                         ClientMetadata: n
@@ -66626,26 +66674,26 @@
                         Session: this.Session,
                         ClientMetadata: r
                     };
                     this.getUserContextData() && (s.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", s, (function(e, n) {
                         if (e) return t.onFailure(e);
                         if ("DEVICE_SRP_AUTH" !== n.ChallengeName) {
                             if (o.signInUserSession = o.getCognitoUserSession(n.AuthenticationResult), o.cacheTokens(), null == n.AuthenticationResult.NewDeviceMetadata) return t.onSuccess(o.signInUserSession);
-                            var r = new _p(o.pool.getUserPoolName());
+                            var r = new Tp(o.pool.getUserPoolName());
                             r.generateHashDevice(n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, n.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(e) {
                                 if (e) return t.onFailure(e);
                                 var i = {
-                                    Salt: pp.lW.from(r.getSaltDevices(), "hex").toString("base64"),
-                                    PasswordVerifier: pp.lW.from(r.getVerifierDevices(), "hex").toString("base64")
+                                    Salt: hp.lW.from(r.getSaltDevices(), "hex").toString("base64"),
+                                    PasswordVerifier: hp.lW.from(r.getVerifierDevices(), "hex").toString("base64")
                                 };
                                 o.verifierDevices = i.PasswordVerifier, o.deviceGroupKey = n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, o.randomPassword = r.getRandomPassword(), o.client.request("ConfirmDevice", {
                                     DeviceKey: n.AuthenticationResult.NewDeviceMetadata.DeviceKey,
                                     AccessToken: o.signInUserSession.getAccessToken().getJwtToken(),
                                     DeviceSecretVerifierConfig: i,
-                                    DeviceName: Vp
+                                    DeviceName: qp
                                 }, (function(e, r) {
                                     return e ? t.onFailure(e) : (o.deviceKey = n.AuthenticationResult.NewDeviceMetadata.DeviceKey, o.cacheDeviceKeyAndPassword(), !0 === r.UserConfirmationNecessary ? t.onSuccess(o.signInUserSession, r.UserConfirmationNecessary) : t.onSuccess(o.signInUserSession))
                                 }))
                             }))
                         } else o.getDeviceResponse(t)
                     }))
                 }, t.changePassword = function(e, t, n, r) {
@@ -66717,15 +66765,15 @@
                     }, (function(t, n) {
                         if (t) return e(t, null);
                         for (var r = [], o = 0; o < n.UserAttributes.length; o++) {
                             var i = {
                                     Name: n.UserAttributes[o].Name,
                                     Value: n.UserAttributes[o].Value
                                 },
-                                a = new Gp(i);
+                                a = new Wp(i);
                             r.push(a)
                         }
                         return e(null, r)
                     }))
                 }, t.getMFAOptions = function(e) {
                     if (null == this.signInUserSession || !this.signInUserSession.isValid()) return e(new Error("User is not authenticated"), null);
                     this.client.request("GetUser", {
@@ -66799,25 +66847,25 @@
                     if (null != this.signInUserSession && this.signInUserSession.isValid()) return e(null, this.signInUserSession);
                     var n = "CognitoIdentityServiceProvider." + this.pool.getClientId() + "." + this.username,
                         r = n + ".idToken",
                         o = n + ".accessToken",
                         i = n + ".refreshToken",
                         a = n + ".clockDrift";
                     if (this.storage.getItem(r)) {
-                        var s = new Up({
+                        var s = new Pp({
                                 IdToken: this.storage.getItem(r)
                             }),
-                            u = new Op({
+                            u = new zp({
                                 AccessToken: this.storage.getItem(o)
                             }),
-                            l = new Pp({
+                            l = new Rp({
                                 RefreshToken: this.storage.getItem(i)
                             }),
                             c = parseInt(this.storage.getItem(a), 0) || 0,
-                            d = new Bp({
+                            d = new Fp({
                                 IdToken: s,
                                 AccessToken: u,
                                 RefreshToken: l,
                                 ClockDrift: c
                             });
                         if (d.isValid()) return this.signInUserSession = d, e(null, this.signInUserSession);
                         if (!l.getToken()) return e(new Error("Cannot retrieve a new session. Please authenticate."), null);
@@ -66885,18 +66933,18 @@
                         t = e + "." + this.username + ".idToken",
                         n = e + "." + this.username + ".accessToken",
                         r = e + "." + this.username + ".refreshToken",
                         o = e + ".LastAuthUser",
                         i = e + "." + this.username + ".clockDrift";
                     this.storage.removeItem(t), this.storage.removeItem(n), this.storage.removeItem(r), this.storage.removeItem(o), this.storage.removeItem(i)
                 }, t.getCognitoUserSession = function(e) {
-                    var t = new Up(e),
-                        n = new Op(e),
-                        r = new Pp(e);
-                    return new Bp({
+                    var t = new Pp(e),
+                        n = new zp(e),
+                        r = new Rp(e);
+                    return new Fp({
                         IdToken: t,
                         AccessToken: n,
                         RefreshToken: r
                     })
                 }, t.forgotPassword = function(e, t) {
                     var n = {
                         ClientId: this.pool.getClientId(),
@@ -67083,106 +67131,106 @@
                             return e ? n.onFailure(e) : (r.signInUserSession = r.getCognitoUserSession(t.AuthenticationResult), r.cacheTokens(), n.onSuccess(r.signInUserSession))
                         }))
                     }))
                 }, e
             }();
         __webpack_require__(8117);
 
-        function Jp() {}
-        Jp.prototype.userAgent = Rp.userAgent;
-        var Kp = Jp;
+        function Kp() {}
+        Kp.prototype.userAgent = Bp.userAgent;
+        var Xp = Kp;
 
-        function Xp(e, t) {
-            e.prototype = Object.create(t.prototype), e.prototype.constructor = e, nh(e, t)
+        function $p(e, t) {
+            e.prototype = Object.create(t.prototype), e.prototype.constructor = e, rh(e, t)
         }
 
-        function $p(e) {
+        function eh(e) {
             var t = "function" === typeof Map ? new Map : void 0;
-            return $p = function(e) {
+            return eh = function(e) {
                 if (null === e || (n = e, -1 === Function.toString.call(n).indexOf("[native code]"))) return e;
                 var n;
                 if ("function" !== typeof e) throw new TypeError("Super expression must either be null or a function");
                 if ("undefined" !== typeof t) {
                     if (t.has(e)) return t.get(e);
                     t.set(e, r)
                 }
 
                 function r() {
-                    return eh(e, arguments, rh(this).constructor)
+                    return th(e, arguments, oh(this).constructor)
                 }
                 return r.prototype = Object.create(e.prototype, {
                     constructor: {
                         value: r,
                         enumerable: !1,
                         writable: !0,
                         configurable: !0
                     }
-                }), nh(r, e)
-            }, $p(e)
+                }), rh(r, e)
+            }, eh(e)
         }
 
-        function eh(e, t, n) {
-            return eh = th() ? Reflect.construct.bind() : function(e, t, n) {
+        function th(e, t, n) {
+            return th = nh() ? Reflect.construct.bind() : function(e, t, n) {
                 var r = [null];
                 r.push.apply(r, t);
                 var o = new(Function.bind.apply(e, r));
-                return n && nh(o, n.prototype), o
-            }, eh.apply(null, arguments)
+                return n && rh(o, n.prototype), o
+            }, th.apply(null, arguments)
         }
 
-        function th() {
+        function nh() {
             if ("undefined" === typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" === typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }
 
-        function nh(e, t) {
-            return nh = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function rh(e, t) {
+            return rh = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, nh(e, t)
+            }, rh(e, t)
         }
 
-        function rh(e) {
-            return rh = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+        function oh(e) {
+            return oh = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                 return e.__proto__ || Object.getPrototypeOf(e)
-            }, rh(e)
+            }, oh(e)
         }
-        var oh = function(e) {
+        var ih = function(e) {
                 function t(t, n, r, o) {
                     var i;
                     return (i = e.call(this, t) || this).code = n, i.name = r, i.statusCode = o, i
                 }
-                return Xp(t, e), t
-            }($p(Error)),
-            ih = function() {
+                return $p(t, e), t
+            }(eh(Error)),
+            ah = function() {
                 function e(e, t, n) {
                     this.endpoint = t || "https://cognito-idp." + e + ".amazonaws.com/";
                     var r = (n || {}).credentials;
                     this.fetchOptions = r ? {
                         credentials: r
                     } : {}
                 }
                 var t = e.prototype;
                 return t.promisifyRequest = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         n.request(e, t, (function(e, t) {
-                            e ? o(new oh(e.message, e.code, e.name, e.statusCode)) : r(t)
+                            e ? o(new ih(e.message, e.code, e.name, e.statusCode)) : r(t)
                         }))
                     }))
                 }, t.requestWithRetry = function(e, t, n) {
                     var r = this;
                     (function(e, t, n) {
-                        void 0 === n && (n = uh);
-                        return sh(e, t, function(e) {
+                        void 0 === n && (n = lh);
+                        return uh(e, t, function(e) {
                             var t = 100,
                                 n = 100;
                             return function(r) {
                                 var o = Math.pow(2, r) * t + n * Math.random();
                                 return !(o > e) && o
                             }
                         }(n))
@@ -67197,15 +67245,15 @@
                     })).catch((function(e) {
                         return n(e)
                     }))
                 }, t.request = function(e, t, n) {
                     var r, o = {
                             "Content-Type": "application/x-amz-json-1.1",
                             "X-Amz-Target": "AWSCognitoIdentityProviderService." + e,
-                            "X-Amz-User-Agent": Kp.prototype.userAgent,
+                            "X-Amz-User-Agent": Xp.prototype.userAgent,
                             "Cache-Control": "no-store"
                         },
                         i = Object.assign({}, this.fetchOptions, {
                             headers: o,
                             method: "POST",
                             mode: "cors",
                             body: JSON.stringify(t)
@@ -67233,43 +67281,43 @@
                         } catch (i) {
                             return n(e)
                         } else e instanceof Error && "Network error" === e.message && (e.code = "NetworkError");
                         return n(e)
                     }))
                 }, e
             }(),
-            ah = function() {};
+            sh = function() {};
         Error;
 
-        function sh(e, t, n, r) {
+        function uh(e, t, n, r) {
             if (void 0 === r && (r = 1), "function" !== typeof e) throw Error("functionToRetry must be a function");
-            return ah(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
-                if (ah("error on " + e.name, o), (i = o) && i.nonRetryable) throw ah(e.name + " non retryable error", o), o;
+            return sh(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
+                if (sh("error on " + e.name, o), (i = o) && i.nonRetryable) throw sh(e.name + " non retryable error", o), o;
                 var i, a = n(r, t, o);
-                if (ah(e.name + " retrying in " + a + " ms"), !1 !== a) return new Promise((function(e) {
+                if (sh(e.name + " retrying in " + a + " ms"), !1 !== a) return new Promise((function(e) {
                     return setTimeout(e, a)
                 })).then((function() {
-                    return sh(e, t, n, r + 1)
+                    return uh(e, t, n, r + 1)
                 }));
                 throw o
             }))
         }
-        var uh = 3e5;
-        var lh, ch = function() {
+        var lh = 3e5;
+        var ch, dh = function() {
                 function e(e, t) {
                     var n = e || {},
                         r = n.UserPoolId,
                         o = n.ClientId,
                         i = n.endpoint,
                         a = n.fetchOptions,
                         s = n.AdvancedSecurityDataCollectionFlag;
                     if (!r || !o) throw new Error("Both UserPoolId and ClientId are required.");
                     if (r.length > 55 || !/^[\w-]+_[0-9a-zA-Z]+$/.test(r)) throw new Error("Invalid UserPoolId format.");
                     var u = r.split("_")[0];
-                    this.userPoolId = r, this.clientId = o, this.client = new ih(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new Zp).getStorage(), t && (this.wrapRefreshSessionCallback = t)
+                    this.userPoolId = r, this.clientId = o, this.client = new ah(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new Vp).getStorage(), t && (this.wrapRefreshSessionCallback = t)
                 }
                 var t = e.prototype;
                 return t.getUserPoolId = function() {
                     return this.userPoolId
                 }, t.getUserPoolName = function() {
                     return this.getUserPoolId().split("_")[1]
                 }, t.getClientId = function() {
@@ -67288,15 +67336,15 @@
                         if (t) return o(t, null);
                         var r = {
                                 Username: e,
                                 Pool: a,
                                 Storage: a.storage
                             },
                             i = {
-                                user: new qp(r),
+                                user: new Jp(r),
                                 userConfirmed: n.UserConfirmed,
                                 userSub: n.UserSub,
                                 codeDeliveryDetails: n.CodeDeliveryDetails
                             };
                         return o(null, i)
                     }))
                 }, t.getCurrentUser = function() {
@@ -67304,15 +67352,15 @@
                         t = this.storage.getItem(e);
                     if (t) {
                         var n = {
                             Username: t,
                             Pool: this,
                             Storage: this.storage
                         };
-                        return new qp(n)
+                        return new Jp(n)
                     }
                     return null
                 }, t.getUserContextData = function(e) {
                     if ("undefined" !== typeof AmazonCognitoAdvancedSecurityData) {
                         var t = AmazonCognitoAdvancedSecurityData;
                         if (this.advancedSecurityDataCollectionFlag) {
                             var n = t.getData(e, this.userPoolId, this.clientId);
@@ -67320,16 +67368,16 @@
                                 EncodedData: n
                             }
                         }
                         return {}
                     }
                 }, e
             }(),
-            dh = __webpack_require__(5943),
-            fh = function() {
+            fh = __webpack_require__(5943),
+            ph = function() {
                 function e(e) {
                     if (!e.domain) throw new Error("The domain of cookieStorage can not be undefined.");
                     if (this.domain = e.domain, e.path ? this.path = e.path : this.path = "/", Object.prototype.hasOwnProperty.call(e, "expires") ? this.expires = e.expires : this.expires = 365, Object.prototype.hasOwnProperty.call(e, "secure") ? this.secure = e.secure : this.secure = !0, Object.prototype.hasOwnProperty.call(e, "sameSite")) {
                         if (!["strict", "lax", "none"].includes(e.sameSite)) throw new Error('The sameSite value of cookieStorage must be "lax", "strict" or "none".');
                         if ("none" === e.sameSite && !this.secure) throw new Error("sameSite = None requires the Secure attribute in latest browser versions.");
                         this.sameSite = e.sameSite
                     } else this.sameSite = null
@@ -67338,116 +67386,116 @@
                 return t.setItem = function(e, t) {
                     var n = {
                         path: this.path,
                         expires: this.expires,
                         domain: this.domain,
                         secure: this.secure
                     };
-                    return this.sameSite && (n.sameSite = this.sameSite), dh.set(e, t, n), dh.get(e)
+                    return this.sameSite && (n.sameSite = this.sameSite), fh.set(e, t, n), fh.get(e)
                 }, t.getItem = function(e) {
-                    return dh.get(e)
+                    return fh.get(e)
                 }, t.removeItem = function(e) {
                     var t = {
                         path: this.path,
                         expires: this.expires,
                         domain: this.domain,
                         secure: this.secure
                     };
-                    return this.sameSite && (t.sameSite = this.sameSite), dh.remove(e, t)
+                    return this.sameSite && (t.sameSite = this.sameSite), fh.remove(e, t)
                 }, t.clear = function() {
-                    for (var e = dh.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
+                    for (var e = fh.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
                     return {}
                 }, e
             }(),
-            ph = __webpack_require__(2770),
-            hh = function(e) {
+            hh = __webpack_require__(2770),
+            gh = function(e) {
                 var t = window.open(e, "_self");
                 return t ? Promise.resolve(t) : Promise.reject()
             },
-            gh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            yh = function(e, t, n) {
-                Vs.dispatch("auth", {
+            yh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            mh = function(e, t, n) {
+                qs.dispatch("auth", {
                     event: e,
                     data: t,
                     message: n
-                }, "Auth", gh)
+                }, "Auth", yh)
             },
-            mh = new Gs("OAuth"),
-            vh = function() {
+            vh = new Ws("OAuth"),
+            Mh = function() {
                 function e(e) {
                     var t = e.config,
                         n = e.cognitoClientId,
                         r = e.scopes,
                         o = void 0 === r ? [] : r;
-                    if (this._urlOpener = t.urlOpener || hh, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
+                    if (this._urlOpener = t.urlOpener || gh, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
                     this._scopes = o
                 }
                 return e.prototype.isValidScopes = function(e) {
                     return Array.isArray(e) && e.every((function(e) {
                         return "string" === typeof e
                     }))
                 }, e.prototype.oauthSignIn = function(e, t, n, r, o, i) {
-                    void 0 === e && (e = "code"), void 0 === o && (o = Ds.Cognito);
+                    void 0 === e && (e = "code"), void 0 === o && (o = Ss.Cognito);
                     var a = this._generateState(32),
                         s = i ? a + "-" + i.split("").map((function(e) {
                             return e.charCodeAt(0).toString(16).padStart(2, "0")
                         })).join("") : a;
                     ! function(e) {
                         window.sessionStorage.setItem("oauth_state", e)
                     }(s);
                     var u, l = this._generateRandom(128);
                     u = l, window.sessionStorage.setItem("ouath_pkce_key", u);
                     var c = this._generateChallenge(l),
                         d = this._scopes.join(" "),
-                        f = Object.entries(ks(ks({
+                        f = Object.entries(Cs(Cs({
                             redirect_uri: n,
                             response_type: e,
                             client_id: r,
                             identity_provider: o,
                             scope: d,
                             state: s
                         }, "code" === e ? {
                             code_challenge: c
                         } : {}), "code" === e ? {
                             code_challenge_method: "S256"
                         } : {})).map((function(e) {
-                            var t = _s(e, 2),
+                            var t = Ts(e, 2),
                                 n = t[0],
                                 r = t[1];
                             return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                         })).join("&"),
                         p = "https://" + t + "/oauth2/authorize?" + f;
-                    mh.debug("Redirecting to " + p), this._urlOpener(p, n)
+                    vh.debug("Redirecting to " + p), this._urlOpener(p, n)
                 }, e.prototype._handleCodeFlow = function(e) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d, f, p, h;
-                        return Es(this, (function(g) {
+                        return _s(this, (function(g) {
                             switch (g.label) {
                                 case 0:
-                                    return t = ((0, ph.Qc)(e).query || "").split("&").map((function(e) {
+                                    return t = ((0, hh.Qc)(e).query || "").split("&").map((function(e) {
                                         return e.split("=")
                                     })).reduce((function(e, t) {
-                                        var n, r = _s(t, 2),
+                                        var n, r = Ts(t, 2),
                                             o = r[0],
                                             i = r[1];
-                                        return ks(ks({}, e), ((n = {})[o] = i, n))
+                                        return Cs(Cs({}, e), ((n = {})[o] = i, n))
                                     }), {
                                         code: void 0
-                                    }).code, n = (0, ph.Qc)(e).pathname || "/", r = (0, ph.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", yh("codeFlow", {}, "Retrieving tokens from " + o), i = As(this._config) ? this._cognitoClientId : this._config.clientID, a = As(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
+                                    }).code, n = (0, hh.Qc)(e).pathname || "/", r = (0, hh.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", mh("codeFlow", {}, "Retrieving tokens from " + o), i = Os(this._config) ? this._cognitoClientId : this._config.clientID, a = Os(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
                                         var e = window.sessionStorage.getItem("ouath_pkce_key");
                                         return window.sessionStorage.removeItem("ouath_pkce_key"), e
-                                    }(), u = ks({
+                                    }(), u = Cs({
                                         grant_type: "authorization_code",
                                         code: t,
                                         client_id: i,
                                         redirect_uri: a
                                     }, s ? {
                                         code_verifier: s
-                                    } : {}), mh.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
-                                        var t = _s(e, 2),
+                                    } : {}), vh.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
+                                        var t = Ts(e, 2),
                                             n = t[0],
                                             r = t[1];
                                         return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                                     })).join("&"), [4, fetch(o, {
                                         method: "POST",
                                         headers: {
                                             "Content-Type": "application/x-www-form-urlencoded"
@@ -67463,70 +67511,70 @@
                                         refreshToken: f,
                                         idToken: p
                                     }]
                             }
                         }))
                     }))
                 }, e.prototype._handleImplicitFlow = function(e) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var t, n, r;
-                        return Es(this, (function(o) {
-                            return t = ((0, ph.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                        return _s(this, (function(o) {
+                            return t = ((0, hh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                 return e.split("=")
                             })).reduce((function(e, t) {
-                                var n, r = _s(t, 2),
+                                var n, r = Ts(t, 2),
                                     o = r[0],
                                     i = r[1];
-                                return ks(ks({}, e), ((n = {})[o] = i, n))
+                                return Cs(Cs({}, e), ((n = {})[o] = i, n))
                             }), {
                                 id_token: void 0,
                                 access_token: void 0
-                            }), n = t.id_token, r = t.access_token, yh("implicitFlow", {}, "Got tokens from " + e), mh.debug("Retrieving implicit tokens from " + e + " with"), [2, {
+                            }), n = t.id_token, r = t.access_token, mh("implicitFlow", {}, "Got tokens from " + e), vh.debug("Retrieving implicit tokens from " + e + " with"), [2, {
                                 accessToken: r,
                                 idToken: n,
                                 refreshToken: null
                             }]
                         }))
                     }))
                 }, e.prototype.handleAuthResponse = function(e) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s;
-                        return Es(this, (function(u) {
+                        return _s(this, (function(u) {
                             switch (u.label) {
                                 case 0:
-                                    if (u.trys.push([0, 5, , 6]), t = e ? ks(ks({}, ((0, ph.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                                    if (u.trys.push([0, 5, , 6]), t = e ? Cs(Cs({}, ((0, hh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n = _s(t, 2),
+                                            var n = Ts(t, 2),
                                                 r = n[0],
                                                 o = n[1];
                                             return e[r] = o, e
-                                        }), {})), ((0, ph.Qc)(e).query || "").split("&").map((function(e) {
+                                        }), {})), ((0, hh.Qc)(e).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n = _s(t, 2),
+                                            var n = Ts(t, 2),
                                                 r = n[0],
                                                 o = n[1];
                                             return e[r] = o, e
                                         }), {})) : {}, n = t.error, r = t.error_description, n) throw new Error(r);
-                                    return o = this._validateState(t), mh.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
+                                    return o = this._validateState(t), vh.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
                                 case 1:
-                                    return [2, ks.apply(void 0, [ks.apply(void 0, i.concat([u.sent()])), {
+                                    return [2, Cs.apply(void 0, [Cs.apply(void 0, i.concat([u.sent()])), {
                                         state: o
                                     }])];
                                 case 2:
                                     return a = [{}], [4, this._handleImplicitFlow(e)];
                                 case 3:
-                                    return [2, ks.apply(void 0, [ks.apply(void 0, a.concat([u.sent()])), {
+                                    return [2, Cs.apply(void 0, [Cs.apply(void 0, a.concat([u.sent()])), {
                                         state: o
                                     }])];
                                 case 4:
                                     return [3, 6];
                                 case 5:
-                                    throw s = u.sent(), mh.error("Error handling auth response.", s), s;
+                                    throw s = u.sent(), vh.error("Error handling auth response.", s), s;
                                 case 6:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._validateState = function(e) {
                     if (e) {
@@ -67535,33 +67583,33 @@
                                 return window.sessionStorage.removeItem("oauth_state"), e
                             }(),
                             n = e.state;
                         if (t && t !== n) throw new Error("Invalid state in OAuth flow");
                         return n
                     }
                 }, e.prototype.signOut = function() {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var e, t, n;
-                        return Es(this, (function(r) {
-                            return e = "https://" + this._config.domain + "/logout?", t = As(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = As(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
+                        return _s(this, (function(r) {
+                            return e = "https://" + this._config.domain + "/logout?", t = Os(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = Os(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
                                 client_id: t,
                                 logout_uri: encodeURIComponent(n)
                             }).map((function(e) {
-                                var t = _s(e, 2);
+                                var t = Ts(e, 2);
                                 return t[0] + "=" + t[1]
-                            })).join("&"), yh("oAuthSignOut", {
+                            })).join("&"), mh("oAuthSignOut", {
                                 oAuth: "signOut"
-                            }, "Signing out from " + e), mh.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
+                            }, "Signing out from " + e), vh.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
                         }))
                     }))
                 }, e.prototype._generateState = function(e) {
                     for (var t = "", n = e, r = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"; n > 0; --n) t += r[Math.round(Math.random() * (r.length - 1))];
                     return t
                 }, e.prototype._generateChallenge = function(e) {
-                    var t = new mp.Sha256;
+                    var t = new vp.Sha256;
                     t.update(e);
                     var n = t.digestSync(),
                         r = nt.lW.from(n).toString("base64");
                     return this._base64URL(r)
                 }, e.prototype._base64URL = function(e) {
                     return e.replace(/=/g, "").replace(/\+/g, "-").replace(/\//g, "_")
                 }, e.prototype._generateRandom = function(e) {
@@ -67574,104 +67622,104 @@
                     for (var t = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789", n = [], r = 0; r < e.byteLength; r += 1) {
                         var o = e[r] % t.length;
                         n.push(t[o])
                     }
                     return n.join("")
                 }, e
             }(),
-            Mh = vh;
+            bh = Mh;
         ! function(e) {
             e.DEFAULT_MSG = "Authentication Error", e.EMPTY_EMAIL = "Email cannot be empty", e.EMPTY_PHONE = "Phone number cannot be empty", e.EMPTY_USERNAME = "Username cannot be empty", e.INVALID_USERNAME = "The username should either be a string or one of the sign in types", e.EMPTY_PASSWORD = "Password cannot be empty", e.EMPTY_CODE = "Confirmation code cannot be empty", e.SIGN_UP_ERROR = "Error creating account", e.NO_MFA = "No valid MFA method provided", e.INVALID_MFA = "Invalid MFA type", e.EMPTY_CHALLENGE = "Challenge response cannot be empty", e.NO_USER_SESSION = "Failed to get the session because the user is empty", e.NETWORK_ERROR = "Network Error", e.DEVICE_CONFIG = "Device tracking has not been configured in this User Pool", e.AUTOSIGNIN_ERROR = "Please use your credentials to sign in"
-        }(lh || (lh = {}));
-        var bh = new Gs("AuthError"),
-            jh = function(e) {
+        }(ch || (ch = {}));
+        var jh = new Ws("AuthError"),
+            wh = function(e) {
                 function t(n) {
                     var r = this,
-                        o = xh[n],
+                        o = Nh[n],
                         i = o.message,
                         a = o.log;
-                    return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, bh.error(r.log), r
+                    return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, jh.error(r.log), r
                 }
-                return Is(t, e), t
+                return Ds(t, e), t
             }(Error),
-            wh = function(e) {
+            xh = function(e) {
                 function t(n) {
                     var r = e.call(this, n) || this;
                     return r.constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "NoUserPoolError", r
                 }
-                return Is(t, e), t
-            }(jh),
-            xh = {
+                return Ds(t, e), t
+            }(wh),
+            Nh = {
                 noConfig: {
-                    message: lh.DEFAULT_MSG,
+                    message: ch.DEFAULT_MSG,
                     log: "\n            Error: Amplify has not been configured correctly.\n            This error is typically caused by one of the following scenarios:\n\n            1. Make sure you're passing the awsconfig object to Amplify.configure() in your app's entry point\n                See https://aws-amplify.github.io/docs/js/authentication#configure-your-app for more information\n            \n            2. There might be multiple conflicting versions of amplify packages in your node_modules.\n\t\t\t\tRefer to our docs site for help upgrading Amplify packages (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js)\n        "
                 },
                 missingAuthConfig: {
-                    message: lh.DEFAULT_MSG,
+                    message: ch.DEFAULT_MSG,
                     log: "\n            Error: Amplify has not been configured correctly. \n            The configuration object is missing required auth properties.\n            This error is typically caused by one of the following scenarios:\n\n            1. Did you run `amplify push` after adding auth via `amplify add auth`?\n                See https://aws-amplify.github.io/docs/js/authentication#amplify-project-setup for more information\n\n            2. This could also be caused by multiple conflicting versions of amplify packages, see (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js) for help upgrading Amplify packages.\n        "
                 },
                 emptyUsername: {
-                    message: lh.EMPTY_USERNAME
+                    message: ch.EMPTY_USERNAME
                 },
                 invalidUsername: {
-                    message: lh.INVALID_USERNAME
+                    message: ch.INVALID_USERNAME
                 },
                 emptyPassword: {
-                    message: lh.EMPTY_PASSWORD
+                    message: ch.EMPTY_PASSWORD
                 },
                 emptyCode: {
-                    message: lh.EMPTY_CODE
+                    message: ch.EMPTY_CODE
                 },
                 signUpError: {
-                    message: lh.SIGN_UP_ERROR,
+                    message: ch.SIGN_UP_ERROR,
                     log: "The first parameter should either be non-null string or object"
                 },
                 noMFA: {
-                    message: lh.NO_MFA
+                    message: ch.NO_MFA
                 },
                 invalidMFA: {
-                    message: lh.INVALID_MFA
+                    message: ch.INVALID_MFA
                 },
                 emptyChallengeResponse: {
-                    message: lh.EMPTY_CHALLENGE
+                    message: ch.EMPTY_CHALLENGE
                 },
                 noUserSession: {
-                    message: lh.NO_USER_SESSION
+                    message: ch.NO_USER_SESSION
                 },
                 deviceConfig: {
-                    message: lh.DEVICE_CONFIG
+                    message: ch.DEVICE_CONFIG
                 },
                 networkError: {
-                    message: lh.NETWORK_ERROR
+                    message: ch.NETWORK_ERROR
                 },
                 autoSignInError: {
-                    message: lh.AUTOSIGNIN_ERROR
+                    message: ch.AUTOSIGNIN_ERROR
                 },
                 default: {
-                    message: lh.DEFAULT_MSG
+                    message: ch.DEFAULT_MSG
                 }
             },
-            Nh = new Gs("AuthClass"),
-            Ih = "aws.cognito.signin.user.admin",
-            Dh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            Sh = function(e, t, n) {
-                Vs.dispatch("auth", {
+            Ih = new Ws("AuthClass"),
+            Dh = "aws.cognito.signin.user.admin",
+            Sh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            Lh = function(e, t, n) {
+                qs.dispatch("auth", {
                     event: e,
                     data: t,
                     message: n
-                }, "Auth", Dh)
+                }, "Auth", Sh)
             },
-            Lh = function() {
+            kh = function() {
                 function e(e) {
                     var t = this;
-                    this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = up, this.wrapRefreshSessionCallback = function(e) {
+                    this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = lp, this.wrapRefreshSessionCallback = function(e) {
                         return function(t, n) {
-                            return n ? Sh("tokenRefresh", void 0, "New token retrieved") : Sh("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
+                            return n ? Lh("tokenRefresh", void 0, "New token retrieved") : Lh("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
                         }
-                    }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), Vs.listen("auth", (function(e) {
+                    }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), qs.listen("auth", (function(e) {
                         switch (e.payload.event) {
                             case "verify":
                             case "signIn":
                                 t._storage.setItem("amplify-signin-with-hostedUI", "false");
                                 break;
                             case "signOut":
                                 t._storage.removeItem("amplify-signin-with-hostedUI");
@@ -67682,80 +67730,80 @@
                     }))
                 }
                 return e.prototype.getModuleName = function() {
                     return "Auth"
                 }, e.prototype.configure = function(e) {
                     var t = this;
                     if (!e) return this._config || {};
-                    Nh.debug("configure Auth");
-                    var n = Object.assign({}, this._config, zc(e).Auth, e);
+                    Ih.debug("configure Auth");
+                    var n = Object.assign({}, this._config, Uc(e).Auth, e);
                     this._config = n;
                     var r = this._config,
                         o = r.userPoolId,
                         i = r.userPoolWebClientId,
                         a = r.cookieStorage,
                         s = r.oauth,
                         u = r.region,
                         l = r.identityPoolId,
                         c = r.mandatorySignIn,
                         d = r.refreshHandlers,
                         f = r.identityPoolRegion,
                         p = r.clientMetadata,
                         h = r.endpoint;
                     if (this._config.storage) {
-                        if (!this._isValidAuthStorage(this._config.storage)) throw Nh.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
+                        if (!this._isValidAuthStorage(this._config.storage)) throw Ih.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
                         this._storage = this._config.storage
-                    } else this._storage = a ? new fh(a) : e.ssr ? new cp : (new Ks).getStorage();
+                    } else this._storage = a ? new ph(a) : e.ssr ? new dp : (new Xs).getStorage();
                     if (this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()), o) {
                         var g = {
                             UserPoolId: o,
                             ClientId: i,
                             endpoint: h
                         };
-                        g.Storage = this._storage, this.userPool = new ch(g, this.wrapRefreshSessionCallback)
+                        g.Storage = this._storage, this.userPool = new dh(g, this.wrapRefreshSessionCallback)
                     }
                     this.Credentials.configure({
                         mandatorySignIn: c,
                         region: u,
                         userPoolId: o,
                         identityPoolId: l,
                         refreshHandlers: d,
                         storage: this._storage,
                         identityPoolRegion: f
                     });
-                    var y = s ? As(this._config.oauth) ? s : s.awsCognito : void 0;
+                    var y = s ? Os(this._config.oauth) ? s : s.awsCognito : void 0;
                     if (y) {
                         var m = Object.assign({
                             cognitoClientId: i,
                             UserPoolId: o,
                             domain: y.domain,
                             scopes: y.scope,
                             redirectSignIn: y.redirectSignIn,
                             redirectSignOut: y.redirectSignOut,
                             responseType: y.responseType,
                             Storage: this._storage,
                             urlOpener: y.urlOpener,
                             clientMetadata: p
                         }, y.options);
-                        this._oAuthHandler = new Mh({
+                        this._oAuthHandler = new bh({
                             scopes: m.scopes,
                             config: m,
                             cognitoClientId: m.cognitoClientId
                         });
                         var v = {};
                         ! function(e) {
-                            if (Xs().isBrowser && window.location) e({
+                            if ($s().isBrowser && window.location) e({
                                 url: window.location.href
                             });
-                            else if (!Xs().isNode) throw new Error("Not supported")
+                            else if (!$s().isNode) throw new Error("Not supported")
                         }((function(e) {
                             var n = e.url;
                             v[n] || (v[n] = !0, t._handleAuthResponse(n))
                         }))
-                    }(Sh("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (Sh("autoSignIn_failure", null, Ss.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
+                    }(Lh("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (Lh("autoSignIn_failure", null, Ls.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
                     return this._config
                 }, e.prototype.signUp = function(e) {
                     for (var t, n, r, o = this, i = [], a = 1; a < arguments.length; a++) i[a - 1] = arguments[a];
                     if (!this.userPool) return this.rejectNoUserPool();
                     var s, u = null,
                         l = null,
                         c = [],
@@ -67765,187 +67813,187 @@
                         },
                         p = {},
                         h = {};
                     if (e && "string" === typeof e) {
                         u = e, l = i ? i[0] : null;
                         var g = i ? i[1] : null,
                             y = i ? i[2] : null;
-                        g && c.push(new Gp({
+                        g && c.push(new Wp({
                             Name: "email",
                             Value: g
-                        })), y && c.push(new Gp({
+                        })), y && c.push(new Wp({
                             Name: "phone_number",
                             Value: y
                         }))
                     } else {
-                        if (!e || "object" !== typeof e) return this.rejectAuthError(Ss.SignUpError);
+                        if (!e || "object" !== typeof e) return this.rejectAuthError(Ls.SignUpError);
                         u = e.username, l = e.password, e && e.clientMetadata ? s = e.clientMetadata : this._config.clientMetadata && (s = this._config.clientMetadata);
                         var m = e.attributes;
                         m && Object.keys(m).map((function(e) {
-                            c.push(new Gp({
+                            c.push(new Wp({
                                 Name: e,
                                 Value: m[e]
                             }))
                         }));
                         var v = e.validationData;
                         v && (d = [], Object.keys(v).map((function(e) {
-                            d.push(new Gp({
+                            d.push(new Wp({
                                 Name: e,
                                 Value: v[e]
                             }))
                         }))), (f = null !== (t = e.autoSignIn) && void 0 !== t ? t : {
                             enabled: !1
                         }).enabled && (this._storage.setItem("amplify-auto-sign-in", "true"), p = null !== (n = f.validationData) && void 0 !== n ? n : {}, h = null !== (r = f.clientMetaData) && void 0 !== r ? r : {})
                     }
-                    return u ? l ? (Nh.debug("signUp attrs:", c), Nh.debug("signUp validation data:", d), new Promise((function(e, t) {
+                    return u ? l ? (Ih.debug("signUp attrs:", c), Ih.debug("signUp validation data:", d), new Promise((function(e, t) {
                         o.userPool.signUp(u, l, c, d, (function(n, r) {
-                            n ? (Sh("signUp_failure", n, u + " failed to signup"), t(n)) : (Sh("signUp", r, u + " has signed up successfully"), f.enabled && o.handleAutoSignIn(u, l, p, h, r), e(r))
+                            n ? (Lh("signUp_failure", n, u + " failed to signup"), t(n)) : (Lh("signUp", r, u + " has signed up successfully"), f.enabled && o.handleAutoSignIn(u, l, p, h, r), e(r))
                         }), s)
-                    }))) : this.rejectAuthError(Ss.EmptyPassword) : this.rejectAuthError(Ss.EmptyUsername)
+                    }))) : this.rejectAuthError(Ls.EmptyPassword) : this.rejectAuthError(Ls.EmptyUsername)
                 }, e.prototype.handleAutoSignIn = function(e, t, n, r, o) {
                     this.autoSignInInitiated = !0;
-                    var i = new fp({
+                    var i = new pp({
                         Username: e,
                         Password: t,
                         ValidationData: n,
                         ClientMetadata: r
                     });
                     o.userConfirmed ? this.signInAfterUserConfirmed(i) : "link" === this._config.signUpVerificationMethod ? this.handleLinkAutoSignIn(i) : this.handleCodeAutoSignIn(i)
                 }, e.prototype.handleCodeAutoSignIn = function(e) {
                     var t = this;
-                    Vs.listen("auth", (function n(r) {
+                    qs.listen("auth", (function n(r) {
                         "confirmSignUp" === r.payload.event && t.signInAfterUserConfirmed(e, n)
                     }))
                 }, e.prototype.handleLinkAutoSignIn = function(e) {
                     var t = this;
                     this._storage.setItem("amplify-polling-started", "true");
                     var n = Date.now(),
                         r = setInterval((function() {
-                            Date.now() - n > 18e4 ? (clearInterval(r), Sh("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
+                            Date.now() - n > 18e4 ? (clearInterval(r), Lh("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
                         }), 5e3)
                 }, e.prototype.signInAfterUserConfirmed = function(e, t, n) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var r, o, i = this;
-                        return Es(this, (function(a) {
+                        return _s(this, (function(a) {
                             switch (a.label) {
                                 case 0:
                                     r = this.createCognitoUser(e.getUsername()), a.label = 1;
                                 case 1:
                                     return a.trys.push([1, 3, , 4]), [4, r.authenticateUser(e, this.authCallbacks(r, (function(r) {
-                                        Sh("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && Vs.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
+                                        Lh("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && qs.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
                                     }), (function(e) {
-                                        Nh.error(e), i._storage.removeItem("amplify-auto-sign-in")
+                                        Ih.error(e), i._storage.removeItem("amplify-auto-sign-in")
                                     })))];
                                 case 2:
                                     return a.sent(), [3, 4];
                                 case 3:
-                                    return o = a.sent(), Nh.error(o), [3, 4];
+                                    return o = a.sent(), Ih.error(o), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype.confirmSignUp = function(e, t, n) {
                     var r = this;
                     if (!this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(Ss.EmptyUsername);
-                    if (!t) return this.rejectAuthError(Ss.EmptyCode);
+                    if (!e) return this.rejectAuthError(Ls.EmptyUsername);
+                    if (!t) return this.rejectAuthError(Ls.EmptyCode);
                     var o, i = this.createCognitoUser(e),
                         a = !n || "boolean" !== typeof n.forceAliasCreation || n.forceAliasCreation;
                     return n && n.clientMetadata ? o = n.clientMetadata : this._config.clientMetadata && (o = this._config.clientMetadata), new Promise((function(n, s) {
                         i.confirmRegistration(t, a, (function(t, o) {
-                            t ? s(t) : (Sh("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (Sh("autoSignIn_failure", null, Ss.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
+                            t ? s(t) : (Lh("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (Lh("autoSignIn_failure", null, Ls.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
                         }), o)
                     }))
                 }, e.prototype.isTrueStorageValue = function(e) {
                     var t = this._storage.getItem(e);
                     return !!t && "true" === t
                 }, e.prototype.resendSignUp = function(e, t) {
                     if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(Ss.EmptyUsername);
+                    if (!e) return this.rejectAuthError(Ls.EmptyUsername);
                     var n = this.createCognitoUser(e);
                     return new Promise((function(e, r) {
                         n.resendConfirmationCode((function(t, n) {
                             t ? r(t) : e(n)
                         }), t)
                     }))
                 }, e.prototype.signIn = function(e, t, n) {
                     if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
                     var r = null,
                         o = null,
                         i = {};
                     if ("string" === typeof e) r = e, o = t;
                     else {
-                        if (!e.username) return this.rejectAuthError(Ss.InvalidUsername);
-                        "undefined" !== typeof t && Nh.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
+                        if (!e.username) return this.rejectAuthError(Ls.InvalidUsername);
+                        "undefined" !== typeof t && Ih.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
                     }
-                    if (!r) return this.rejectAuthError(Ss.EmptyUsername);
-                    var a = new fp({
+                    if (!r) return this.rejectAuthError(Ls.EmptyUsername);
+                    var a = new pp({
                         Username: r,
                         Password: o,
                         ValidationData: i,
                         ClientMetadata: n
                     });
                     return o ? this.signInWithPassword(a) : this.signInWithoutPassword(a)
                 }, e.prototype.authCallbacks = function(e, t, n) {
                     var r = this,
                         o = this;
                     return {
                         onSuccess: function(i) {
-                            return Cs(r, void 0, void 0, (function() {
+                            return Es(r, void 0, void 0, (function() {
                                 var r, a, s, u;
-                                return Es(this, (function(l) {
+                                return _s(this, (function(l) {
                                     switch (l.label) {
                                         case 0:
-                                            Nh.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
+                                            Ih.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
                                         case 1:
                                             return l.trys.push([1, 4, 5, 9]), [4, this.Credentials.clear()];
                                         case 2:
                                             return l.sent(), [4, this.Credentials.set(i, "session")];
                                         case 3:
-                                            return r = l.sent(), Nh.debug("succeed to get cognito credentials", r), [3, 9];
+                                            return r = l.sent(), Ih.debug("succeed to get cognito credentials", r), [3, 9];
                                         case 4:
-                                            return a = l.sent(), Nh.debug("cannot get cognito credentials", a), [3, 9];
+                                            return a = l.sent(), Ih.debug("cannot get cognito credentials", a), [3, 9];
                                         case 5:
                                             return l.trys.push([5, 7, , 8]), [4, this.currentUserPoolUser()];
                                         case 6:
-                                            return s = l.sent(), o.user = s, Sh("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
+                                            return s = l.sent(), o.user = s, Lh("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
                                         case 7:
-                                            return u = l.sent(), Nh.error("Failed to get the signed in user", u), n(u), [3, 8];
+                                            return u = l.sent(), Ih.error("Failed to get the signed in user", u), n(u), [3, 8];
                                         case 8:
                                             return [7];
                                         case 9:
                                             return [2]
                                     }
                                 }))
                             }))
                         },
                         onFailure: function(t) {
-                            Nh.debug("signIn failure", t), Sh("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
+                            Ih.debug("signIn failure", t), Lh("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
                         },
                         customChallenge: function(n) {
-                            Nh.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
+                            Ih.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
                         },
                         mfaRequired: function(n, r) {
-                            Nh.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
+                            Ih.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         mfaSetup: function(n, r) {
-                            Nh.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
+                            Ih.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         newPasswordRequired: function(n, r) {
-                            Nh.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
+                            Ih.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
                                 userAttributes: n,
                                 requiredAttributes: r
                             }, t(e)
                         },
                         totpRequired: function(n, r) {
-                            Nh.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
+                            Ih.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         selectMFAType: function(n, r) {
-                            Nh.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
+                            Ih.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
                         }
                     }
                 }, e.prototype.signInWithPassword = function(e) {
                     var t = this;
                     if (this.pendingSignIn) throw new Error("Pending sign-in attempt already in progress");
                     var n = this.createCognitoUser(e.getUsername());
                     return this.pendingSignIn = new Promise((function(r, o) {
@@ -67960,32 +68008,32 @@
                         n = this.createCognitoUser(e.getUsername());
                     return n.setAuthenticationFlowType("CUSTOM_AUTH"), new Promise((function(r, o) {
                         n.initiateAuth(e, t.authCallbacks(n, r, o))
                     }))
                 }, e.prototype.getMFAOptions = function(e) {
                     return new Promise((function(t, n) {
                         e.getMFAOptions((function(e, r) {
-                            if (e) return Nh.debug("get MFA Options failed", e), void n(e);
-                            Nh.debug("get MFA options success", r), t(r)
+                            if (e) return Ih.debug("get MFA Options failed", e), void n(e);
+                            Ih.debug("get MFA options success", r), t(r)
                         }))
                     }))
                 }, e.prototype.getPreferredMFA = function(e, t) {
                     var n = this,
                         r = this;
                     return new Promise((function(o, i) {
                         var a = n._config.clientMetadata,
                             s = !!t && t.bypassCache;
                         e.getUserData((function(t, a) {
-                            return Cs(n, void 0, void 0, (function() {
+                            return Es(n, void 0, void 0, (function() {
                                 var n, s;
-                                return Es(this, (function(u) {
+                                return _s(this, (function(u) {
                                     switch (u.label) {
                                         case 0:
                                             if (!t) return [3, 5];
-                                            if (Nh.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                            if (Ih.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                             u.label = 1;
                                         case 1:
                                             return u.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                         case 2:
                                             return u.sent(), [3, 4];
                                         case 3:
                                             return n = u.sent(), i(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -68003,29 +68051,29 @@
                     }))
                 }, e.prototype._getMfaTypeFromUserData = function(e) {
                     var t = null,
                         n = e.PreferredMfaSetting;
                     if (n) t = n;
                     else {
                         var r = e.UserMFASettingList;
-                        if (r) 0 === r.length ? t = "NOMFA" : Nh.debug("invalid case for getPreferredMFA", e);
+                        if (r) 0 === r.length ? t = "NOMFA" : Ih.debug("invalid case for getPreferredMFA", e);
                         else t = e.MFAOptions ? "SMS_MFA" : "NOMFA"
                     }
                     return t
                 }, e.prototype._getUserData = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         e.getUserData((function(t, i) {
-                            return Cs(n, void 0, void 0, (function() {
+                            return Es(n, void 0, void 0, (function() {
                                 var n;
-                                return Es(this, (function(a) {
+                                return _s(this, (function(a) {
                                     switch (a.label) {
                                         case 0:
                                             if (!t) return [3, 5];
-                                            if (Nh.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                            if (Ih.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                             a.label = 1;
                                         case 1:
                                             return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                         case 2:
                                             return a.sent(), [3, 4];
                                         case 3:
                                             return n = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -68037,17 +68085,17 @@
                                             return [2]
                                     }
                                 }))
                             }))
                         }), t)
                     }))
                 }, e.prototype.setPreferredMFA = function(e, t) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u = this;
-                        return Es(this, (function(l) {
+                        return _s(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return n = this._config.clientMetadata, [4, this._getUserData(e, {
                                         bypassCache: !0,
                                         clientMetadata: n
                                     })];
                                 case 1:
@@ -68077,15 +68125,15 @@
                                 case 5:
                                     if ("NOMFA" === (s = l.sent())) return [2, Promise.resolve("No change for mfa type")];
                                     if ("SMS_MFA" === s) o = {
                                         PreferredMfa: !1,
                                         Enabled: !1
                                     };
                                     else {
-                                        if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(Ss.InvalidMFA)];
+                                        if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(Ls.InvalidMFA)];
                                         i = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         }
                                     }
                                     return a && 0 !== a.length && a.forEach((function(e) {
                                         "SMS_MFA" === e ? o = {
@@ -68093,27 +68141,27 @@
                                             Enabled: !1
                                         } : "SOFTWARE_TOKEN_MFA" === e && (i = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         })
                                     })), [3, 7];
                                 case 6:
-                                    return Nh.debug("no validmfa method provided"), [2, this.rejectAuthError(Ss.NoMFA)];
+                                    return Ih.debug("no validmfa method provided"), [2, this.rejectAuthError(Ls.NoMFA)];
                                 case 7:
                                     return this, [2, new Promise((function(t, r) {
                                         e.setUserMfaPreference(o, i, (function(o, i) {
-                                            if (o) return Nh.debug("Set user mfa preference error", o), r(o);
-                                            Nh.debug("Set user mfa success", i), Nh.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
-                                                return Cs(u, void 0, void 0, (function() {
+                                            if (o) return Ih.debug("Set user mfa preference error", o), r(o);
+                                            Ih.debug("Set user mfa success", i), Ih.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
+                                                return Es(u, void 0, void 0, (function() {
                                                     var o;
-                                                    return Es(this, (function(a) {
+                                                    return _s(this, (function(a) {
                                                         switch (a.label) {
                                                             case 0:
                                                                 if (!n) return [3, 5];
-                                                                if (Nh.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
+                                                                if (Ih.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
                                                                 a.label = 1;
                                                             case 1:
                                                                 return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                             case 2:
                                                                 return a.sent(), [3, 4];
                                                             case 3:
                                                                 return o = a.sent(), r(new Error("Session is invalid due to: " + n.message + " and failed to clean up invalid session: " + o.message)), [2];
@@ -68132,195 +68180,195 @@
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.disableSMS = function(e) {
                     return new Promise((function(t, n) {
                         e.disableMFA((function(e, r) {
-                            if (e) return Nh.debug("disable mfa failed", e), void n(e);
-                            Nh.debug("disable mfa succeed", r), t(r)
+                            if (e) return Ih.debug("disable mfa failed", e), void n(e);
+                            Ih.debug("disable mfa succeed", r), t(r)
                         }))
                     }))
                 }, e.prototype.enableSMS = function(e) {
                     return new Promise((function(t, n) {
                         e.enableMFA((function(e, r) {
-                            if (e) return Nh.debug("enable mfa failed", e), void n(e);
-                            Nh.debug("enable mfa succeed", r), t(r)
+                            if (e) return Ih.debug("enable mfa failed", e), void n(e);
+                            Ih.debug("enable mfa succeed", r), t(r)
                         }))
                     }))
                 }, e.prototype.setupTOTP = function(e) {
                     return new Promise((function(t, n) {
                         e.associateSoftwareToken({
                             onFailure: function(e) {
-                                Nh.debug("associateSoftwareToken failed", e), n(e)
+                                Ih.debug("associateSoftwareToken failed", e), n(e)
                             },
                             associateSecretCode: function(e) {
-                                Nh.debug("associateSoftwareToken sucess", e), t(e)
+                                Ih.debug("associateSoftwareToken sucess", e), t(e)
                             }
                         })
                     }))
                 }, e.prototype.verifyTotpToken = function(e, t) {
-                    return Nh.debug("verification totp token", e, t), new Promise((function(n, r) {
+                    return Ih.debug("verification totp token", e, t), new Promise((function(n, r) {
                         e.verifySoftwareToken(t, "My TOTP device", {
                             onFailure: function(e) {
-                                Nh.debug("verifyTotpToken failed", e), r(e)
+                                Ih.debug("verifyTotpToken failed", e), r(e)
                             },
                             onSuccess: function(t) {
-                                Sh("signIn", e, "A user " + e.getUsername() + " has been signed in"), Sh("verify", e, "A user " + e.getUsername() + " has been verified"), Nh.debug("verifyTotpToken success", t), n(t)
+                                Lh("signIn", e, "A user " + e.getUsername() + " has been signed in"), Lh("verify", e, "A user " + e.getUsername() + " has been verified"), Ih.debug("verifyTotpToken success", t), n(t)
                             }
                         })
                     }))
                 }, e.prototype.confirmSignIn = function(e, t, n, r) {
                     var o = this;
-                    if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Ss.EmptyCode);
+                    if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Ls.EmptyCode);
                     var i = this;
                     return new Promise((function(a, s) {
                         e.sendMFACode(t, {
                             onSuccess: function(t) {
-                                return Cs(o, void 0, void 0, (function() {
+                                return Es(o, void 0, void 0, (function() {
                                     var n, r;
-                                    return Es(this, (function(o) {
+                                    return _s(this, (function(o) {
                                         switch (o.label) {
                                             case 0:
-                                                Nh.debug(t), o.label = 1;
+                                                Ih.debug(t), o.label = 1;
                                             case 1:
                                                 return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return o.sent(), [4, this.Credentials.set(t, "session")];
                                             case 3:
-                                                return n = o.sent(), Nh.debug("succeed to get cognito credentials", n), [3, 6];
+                                                return n = o.sent(), Ih.debug("succeed to get cognito credentials", n), [3, 6];
                                             case 4:
-                                                return r = o.sent(), Nh.debug("cannot get cognito credentials", r), [3, 6];
+                                                return r = o.sent(), Ih.debug("cannot get cognito credentials", r), [3, 6];
                                             case 5:
-                                                return i.user = e, Sh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                return i.user = e, Lh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                             case 6:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(e) {
-                                Nh.debug("confirm signIn failure", e), s(e)
+                                Ih.debug("confirm signIn failure", e), s(e)
                             }
                         }, n, r)
                     }))
                 }, e.prototype.completeNewPassword = function(e, t, n, r) {
                     var o = this;
-                    if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Ss.EmptyPassword);
+                    if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Ls.EmptyPassword);
                     var i = this;
                     return new Promise((function(a, s) {
                         e.completeNewPasswordChallenge(t, n, {
                             onSuccess: function(t) {
-                                return Cs(o, void 0, void 0, (function() {
+                                return Es(o, void 0, void 0, (function() {
                                     var n, r;
-                                    return Es(this, (function(o) {
+                                    return _s(this, (function(o) {
                                         switch (o.label) {
                                             case 0:
-                                                Nh.debug(t), o.label = 1;
+                                                Ih.debug(t), o.label = 1;
                                             case 1:
                                                 return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return o.sent(), [4, this.Credentials.set(t, "session")];
                                             case 3:
-                                                return n = o.sent(), Nh.debug("succeed to get cognito credentials", n), [3, 6];
+                                                return n = o.sent(), Ih.debug("succeed to get cognito credentials", n), [3, 6];
                                             case 4:
-                                                return r = o.sent(), Nh.debug("cannot get cognito credentials", r), [3, 6];
+                                                return r = o.sent(), Ih.debug("cannot get cognito credentials", r), [3, 6];
                                             case 5:
-                                                return i.user = e, Sh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                return i.user = e, Lh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                             case 6:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(e) {
-                                Nh.debug("completeNewPassword failure", e), Sh("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
+                                Ih.debug("completeNewPassword failure", e), Lh("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
                             },
                             mfaRequired: function(t, n) {
-                                Nh.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
+                                Ih.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
                             },
                             mfaSetup: function(t, n) {
-                                Nh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                Ih.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                             },
                             totpRequired: function(t, n) {
-                                Nh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                Ih.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                             }
                         }, r)
                     }))
                 }, e.prototype.sendCustomChallengeAnswer = function(e, t, n) {
                     var r = this;
                     if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!t) return this.rejectAuthError(Ss.EmptyChallengeResponse);
+                    if (!t) return this.rejectAuthError(Ls.EmptyChallengeResponse);
                     return new Promise((function(o, i) {
                         e.sendCustomChallengeAnswer(t, r.authCallbacks(e, o, i), n)
                     }))
                 }, e.prototype.deleteUserAttributes = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         n.userSession(e).then((function(n) {
                             e.deleteAttributes(t, (function(e, t) {
                                 return e ? o(e) : r(t)
                             }))
                         }))
                     }))
                 }, e.prototype.deleteUser = function() {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var e, t, n = this;
-                        return Es(this, (function(r) {
+                        return _s(this, (function(r) {
                             switch (r.label) {
                                 case 0:
                                     return r.trys.push([0, 2, , 3]), [4, this._storageSync];
                                 case 1:
                                     return r.sent(), [3, 3];
                                 case 2:
-                                    throw e = r.sent(), Nh.debug("Failed to sync cache info into memory", e), new Error(e);
+                                    throw e = r.sent(), Ih.debug("Failed to sync cache info into memory", e), new Error(e);
                                 case 3:
                                     return t = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(e, r) {
-                                        return Cs(n, void 0, void 0, (function() {
+                                        return Es(n, void 0, void 0, (function() {
                                             var n, o = this;
-                                            return Es(this, (function(i) {
+                                            return _s(this, (function(i) {
                                                 if (this.userPool) {
-                                                    if (!(n = this.userPool.getCurrentUser())) return Nh.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
+                                                    if (!(n = this.userPool.getCurrentUser())) return Ih.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
                                                     n.getSession((function(i, a) {
-                                                        return Cs(o, void 0, void 0, (function() {
+                                                        return Es(o, void 0, void 0, (function() {
                                                             var o, a = this;
-                                                            return Es(this, (function(s) {
+                                                            return _s(this, (function(s) {
                                                                 switch (s.label) {
                                                                     case 0:
                                                                         if (!i) return [3, 5];
-                                                                        if (Nh.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
+                                                                        if (Ih.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
                                                                         s.label = 1;
                                                                     case 1:
                                                                         return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(n)];
                                                                     case 2:
                                                                         return s.sent(), [3, 4];
                                                                     case 3:
                                                                         return o = s.sent(), r(new Error("Session is invalid due to: " + i.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                                     case 4:
                                                                         return [2, r(i)];
                                                                     case 5:
                                                                         n.deleteUser((function(o, i) {
                                                                             if (o) r(o);
                                                                             else {
-                                                                                Sh("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
+                                                                                Lh("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
                                                                                 try {
                                                                                     a.cleanCachedItems()
                                                                                 } catch (s) {
-                                                                                    Nh.debug("failed to clear cached items")
+                                                                                    Ih.debug("failed to clear cached items")
                                                                                 }
-                                                                                t ? a.oAuthSignOutRedirect(e, r) : (Sh("signOut", a.user, "A user has been signed out"), e(i))
+                                                                                t ? a.oAuthSignOutRedirect(e, r) : (Lh("signOut", a.user, "A user has been signed out"), e(i))
                                                                             }
                                                                         })), s.label = 6;
                                                                     case 6:
                                                                         return [2]
                                                                 }
                                                             }))
                                                         }))
                                                     }))
-                                                } else Nh.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
+                                                } else Ih.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
                                                 return [2]
                                             }))
                                         }))
                                     }))]
                             }
                         }))
                     }))
@@ -68335,17 +68383,17 @@
                                 if ("sub" !== u && u.indexOf("_verified") < 0) {
                                     var l = {
                                         Name: u,
                                         Value: t[u]
                                     };
                                     o.push(l)
                                 } e.updateAttributes(o, (function(e, n, o) {
-                                if (e) return Sh("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
+                                if (e) return Lh("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
                                 var i = r.createUpdateAttributesResultList(t, null === o || void 0 === o ? void 0 : o.CodeDeliveryDetailsList);
-                                return Sh("updateUserAttributes", i, "Attributes successfully updated"), a(n)
+                                return Lh("updateUserAttributes", i, "Attributes successfully updated"), a(n)
                             }), n)
                         }))
                     }))
                 }, e.prototype.createUpdateAttributesResultList = function(e, t) {
                     var n = {};
                     return Object.keys(e).forEach((function(e) {
                         n[e] = {
@@ -68389,73 +68437,73 @@
                 }, e.prototype.isRefreshTokenExpiredError = function(e) {
                     return this.isErrorWithMessage(e) && "Refresh Token has expired" === e.message
                 }, e.prototype.isSignedInHostedUI = function() {
                     return this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI")
                 }, e.prototype.isSessionInvalid = function(e) {
                     return this.isUserDisabledError(e) || this.isUserDoesNotExistError(e) || this.isTokenRevokedError(e) || this.isRefreshTokenRevokedError(e) || this.isRefreshTokenExpiredError(e)
                 }, e.prototype.cleanUpInvalidSession = function(e) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var t = this;
-                        return Es(this, (function(n) {
+                        return _s(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     e.signOut(), this.user = null, n.label = 1;
                                 case 1:
                                     return n.trys.push([1, 3, , 4]), [4, this.cleanCachedItems()];
                                 case 2:
                                     return n.sent(), [3, 4];
                                 case 3:
-                                    return n.sent(), Nh.debug("failed to clear cached items"), [3, 4];
+                                    return n.sent(), Ih.debug("failed to clear cached items"), [3, 4];
                                 case 4:
                                     return this.isSignedInHostedUI() ? [2, new Promise((function(e, n) {
                                         t.oAuthSignOutRedirect(e, n)
-                                    }))] : (Sh("signOut", this.user, "A user has been signed out"), [2])
+                                    }))] : (Lh("signOut", this.user, "A user has been signed out"), [2])
                             }
                         }))
                     }))
                 }, e.prototype.currentUserPoolUser = function(e) {
                     var t = this;
                     return this.userPool ? new Promise((function(n, r) {
                         t._storageSync.then((function() {
-                            return Cs(t, void 0, void 0, (function() {
+                            return Es(t, void 0, void 0, (function() {
                                 var t, o, i, a, s, u, l = this;
-                                return Es(this, (function(c) {
+                                return _s(this, (function(c) {
                                     switch (c.label) {
                                         case 0:
-                                            return this.isOAuthInProgress() ? (Nh.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
+                                            return this.isOAuthInProgress() ? (Ih.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
                                                 var t = setTimeout((function() {
-                                                    Nh.debug("OAuth signIn in progress timeout"), Vs.remove("auth", n), e()
+                                                    Ih.debug("OAuth signIn in progress timeout"), qs.remove("auth", n), e()
                                                 }), 1e4);
 
                                                 function n(r) {
                                                     var o = r.payload.event;
-                                                    "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (Nh.debug("OAuth signIn resolved: " + o), clearTimeout(t), Vs.remove("auth", n), e())
+                                                    "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (Ih.debug("OAuth signIn resolved: " + o), clearTimeout(t), qs.remove("auth", n), e())
                                                 }
-                                                Vs.listen("auth", n)
+                                                qs.listen("auth", n)
                                             }))]) : [3, 2];
                                         case 1:
                                             c.sent(), c.label = 2;
                                         case 2:
-                                            if (!(t = this.userPool.getCurrentUser())) return Nh.debug("Failed to get user from user pool"), r("No current user"), [2];
+                                            if (!(t = this.userPool.getCurrentUser())) return Ih.debug("Failed to get user from user pool"), r("No current user"), [2];
                                             c.label = 3;
                                         case 3:
                                             return c.trys.push([3, 7, , 8]), [4, this._userSession(t)];
                                         case 4:
                                             return o = c.sent(), (i = !!e && e.bypassCache) ? [4, this.Credentials.clear()] : [3, 6];
                                         case 5:
                                             c.sent(), c.label = 6;
                                         case 6:
-                                            return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(Ih) ? (t.getUserData((function(e, o) {
-                                                return Cs(l, void 0, void 0, (function() {
+                                            return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(Dh) ? (t.getUserData((function(e, o) {
+                                                return Es(l, void 0, void 0, (function() {
                                                     var i, a, s, u, l, c, d;
-                                                    return Es(this, (function(f) {
+                                                    return _s(this, (function(f) {
                                                         switch (f.label) {
                                                             case 0:
                                                                 if (!e) return [3, 7];
-                                                                if (Nh.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
+                                                                if (Ih.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
                                                                 f.label = 1;
                                                             case 1:
                                                                 return f.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                             case 2:
                                                                 return f.sent(), [3, 4];
                                                             case 3:
                                                                 return i = f.sent(), r(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + i.message)), [2];
@@ -68465,114 +68513,114 @@
                                                                 n(t), f.label = 6;
                                                             case 6:
                                                                 return [2];
                                                             case 7:
                                                                 for (a = o.PreferredMfaSetting || "NOMFA", s = [], u = 0; u < o.UserAttributes.length; u++) l = {
                                                                     Name: o.UserAttributes[u].Name,
                                                                     Value: o.UserAttributes[u].Value
-                                                                }, c = new Gp(l), s.push(c);
+                                                                }, c = new Wp(l), s.push(c);
                                                                 return d = this.attributesToObject(s), Object.assign(t, {
                                                                     attributes: d,
                                                                     preferredMFA: a
                                                                 }), [2, n(t)]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 bypassCache: i,
                                                 clientMetadata: a
-                                            }), [3, 8]) : (Nh.debug("Unable to get the user data because the " + Ih + " is not in the scopes of the access token"), [2, n(t)]);
+                                            }), [3, 8]) : (Ih.debug("Unable to get the user data because the " + Dh + " is not in the scopes of the access token"), [2, n(t)]);
                                         case 7:
                                             return u = c.sent(), r(u), [3, 8];
                                         case 8:
                                             return [2]
                                     }
                                 }))
                             }))
                         })).catch((function(e) {
-                            return Nh.debug("Failed to sync cache info into memory", e), r(e)
+                            return Ih.debug("Failed to sync cache info into memory", e), r(e)
                         }))
                     })) : this.rejectNoUserPool()
                 }, e.prototype.isOAuthInProgress = function() {
                     return this.oAuthFlowInProgress
                 }, e.prototype.currentAuthenticatedUser = function(e) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var t, n, r, o, i;
-                        return Es(this, (function(a) {
+                        return _s(this, (function(a) {
                             switch (a.label) {
                                 case 0:
-                                    Nh.debug("getting current authenticated user"), t = null, a.label = 1;
+                                    Ih.debug("getting current authenticated user"), t = null, a.label = 1;
                                 case 1:
                                     return a.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return a.sent(), [3, 4];
                                 case 3:
-                                    throw n = a.sent(), Nh.debug("Failed to sync cache info into memory", n), n;
+                                    throw n = a.sent(), Ih.debug("Failed to sync cache info into memory", n), n;
                                 case 4:
                                     try {
-                                        (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = ks(ks({}, r.user), {
+                                        (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = Cs(Cs({}, r.user), {
                                             token: r.token
                                         }))
                                     } catch (s) {
-                                        Nh.debug("cannot load federated user from auth storage")
+                                        Ih.debug("cannot load federated user from auth storage")
                                     }
-                                    return t ? (this.user = t, Nh.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
+                                    return t ? (this.user = t, Ih.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
                                 case 5:
-                                    Nh.debug("get current authenticated userpool user"), o = null, a.label = 6;
+                                    Ih.debug("get current authenticated userpool user"), o = null, a.label = 6;
                                 case 6:
                                     return a.trys.push([6, 8, , 9]), [4, this.currentUserPoolUser(e)];
                                 case 7:
                                     return o = a.sent(), [3, 9];
                                 case 8:
-                                    return "No userPool" === (i = a.sent()) && Nh.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), Nh.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
+                                    return "No userPool" === (i = a.sent()) && Ih.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), Ih.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
                                 case 9:
                                     return this.user = o, [2, this.user]
                             }
                         }))
                     }))
                 }, e.prototype.currentSession = function() {
                     var e = this;
-                    return Nh.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
+                    return Ih.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
                         e.currentUserPoolUser().then((function(r) {
                             e.userSession(r).then((function(e) {
                                 t(e)
                             })).catch((function(e) {
-                                Nh.debug("Failed to get the current session", e), n(e)
+                                Ih.debug("Failed to get the current session", e), n(e)
                             }))
                         })).catch((function(e) {
-                            Nh.debug("Failed to get the current user", e), n(e)
+                            Ih.debug("Failed to get the current user", e), n(e)
                         }))
                     })) : Promise.reject(new Error("No User Pool in the configuration."))
                 }, e.prototype._userSession = function(e) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var t, n, r = this;
-                        return Es(this, (function(o) {
+                        return _s(this, (function(o) {
                             switch (o.label) {
                                 case 0:
-                                    if (!e) return Nh.debug("the user is null"), [2, this.rejectAuthError(Ss.NoUserSession)];
+                                    if (!e) return Ih.debug("the user is null"), [2, this.rejectAuthError(Ls.NoUserSession)];
                                     t = this._config.clientMetadata, 0 === this.inflightSessionPromiseCounter && (this.inflightSessionPromise = new Promise((function(n, o) {
                                         e.getSession((function(t, i) {
-                                            return Cs(r, void 0, void 0, (function() {
+                                            return Es(r, void 0, void 0, (function() {
                                                 var r;
-                                                return Es(this, (function(a) {
+                                                return _s(this, (function(a) {
                                                     switch (a.label) {
                                                         case 0:
                                                             if (!t) return [3, 5];
-                                                            if (Nh.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
+                                                            if (Ih.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
                                                             a.label = 1;
                                                         case 1:
                                                             return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                         case 2:
                                                             return a.sent(), [3, 4];
                                                         case 3:
                                                             return r = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + r.message)), [2];
                                                         case 4:
                                                             return o(t), [2];
                                                         case 5:
-                                                            return Nh.debug("Succeed to get the user session", i), n(i), [2]
+                                                            return Ih.debug("Succeed to get the user session", i), n(i), [2]
                                                     }
                                                 }))
                                             }))
                                         }), {
                                             clientMetadata: t
                                         })
                                     }))), this.inflightSessionPromiseCounter++, o.label = 1;
@@ -68586,43 +68634,43 @@
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype.userSession = function(e) {
                     return this._userSession(e)
                 }, e.prototype.currentUserCredentials = function() {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var e, t, n = this;
-                        return Es(this, (function(r) {
+                        return _s(this, (function(r) {
                             switch (r.label) {
                                 case 0:
-                                    Nh.debug("Getting current user credentials"), r.label = 1;
+                                    Ih.debug("Getting current user credentials"), r.label = 1;
                                 case 1:
                                     return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return r.sent(), [3, 4];
                                 case 3:
-                                    throw e = r.sent(), Nh.debug("Failed to sync cache info into memory", e), e;
+                                    throw e = r.sent(), Ih.debug("Failed to sync cache info into memory", e), e;
                                 case 4:
                                     t = null;
                                     try {
                                         t = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))
                                     } catch (o) {
-                                        Nh.debug("failed to get or parse item aws-amplify-federatedInfo", o)
+                                        Ih.debug("failed to get or parse item aws-amplify-federatedInfo", o)
                                     }
                                     return t ? [2, this.Credentials.refreshFederatedToken(t)] : [2, this.currentSession().then((function(e) {
-                                        return Nh.debug("getting session success", e), n.Credentials.set(e, "session")
+                                        return Ih.debug("getting session success", e), n.Credentials.set(e, "session")
                                     })).catch((function() {
-                                        return Nh.debug("getting guest credentials"), n.Credentials.set(null, "guest")
+                                        return Ih.debug("getting guest credentials"), n.Credentials.set(null, "guest")
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.currentCredentials = function() {
-                    return Nh.debug("getting current credentials"), this.Credentials.get()
+                    return Ih.debug("getting current credentials"), this.Credentials.get()
                 }, e.prototype.verifyUserAttribute = function(e, t, n) {
                     return void 0 === n && (n = this._config.clientMetadata), new Promise((function(r, o) {
                         e.getAttributeVerificationCode(t, {
                             onSuccess: function(e) {
                                 return r(e)
                             },
                             onFailure: function(e) {
@@ -68636,289 +68684,289 @@
                             onSuccess: function(e) {
                                 r(e)
                             },
                             onFailure: function(e) {
                                 o(e)
                             }
                         })
-                    })) : this.rejectAuthError(Ss.EmptyCode)
+                    })) : this.rejectAuthError(Ls.EmptyCode)
                 }, e.prototype.verifyCurrentUserAttribute = function(e) {
                     var t = this;
                     return t.currentUserPoolUser().then((function(n) {
                         return t.verifyUserAttribute(n, e)
                     }))
                 }, e.prototype.verifyCurrentUserAttributeSubmit = function(e, t) {
                     var n = this;
                     return n.currentUserPoolUser().then((function(r) {
                         return n.verifyUserAttributeSubmit(r, e, t)
                     }))
                 }, e.prototype.cognitoIdentitySignOut = function(e, t) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var n, r, o = this;
-                        return Es(this, (function(i) {
+                        return _s(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return i.trys.push([0, 2, , 3]), [4, this._storageSync];
                                 case 1:
                                     return i.sent(), [3, 3];
                                 case 2:
-                                    throw n = i.sent(), Nh.debug("Failed to sync cache info into memory", n), n;
+                                    throw n = i.sent(), Ih.debug("Failed to sync cache info into memory", n), n;
                                 case 3:
                                     return r = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(n, i) {
                                         if (e && e.global) {
-                                            Nh.debug("user global sign out", t);
+                                            Ih.debug("user global sign out", t);
                                             var a = o._config.clientMetadata;
                                             t.getSession((function(e, a) {
-                                                return Cs(o, void 0, void 0, (function() {
+                                                return Es(o, void 0, void 0, (function() {
                                                     var o, a = this;
-                                                    return Es(this, (function(s) {
+                                                    return _s(this, (function(s) {
                                                         switch (s.label) {
                                                             case 0:
                                                                 if (!e) return [3, 5];
-                                                                if (Nh.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
+                                                                if (Ih.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
                                                                 s.label = 1;
                                                             case 1:
                                                                 return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                             case 2:
                                                                 return s.sent(), [3, 4];
                                                             case 3:
                                                                 return o = s.sent(), i(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                             case 4:
                                                                 return [2, i(e)];
                                                             case 5:
                                                                 return t.globalSignOut({
                                                                     onSuccess: function(e) {
-                                                                        if (Nh.debug("global sign out success"), !r) return n();
+                                                                        if (Ih.debug("global sign out success"), !r) return n();
                                                                         a.oAuthSignOutRedirect(n, i)
                                                                     },
                                                                     onFailure: function(e) {
-                                                                        return Nh.debug("global sign out failed", e), i(e)
+                                                                        return Ih.debug("global sign out failed", e), i(e)
                                                                     }
                                                                 }), [2]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 clientMetadata: a
                                             })
-                                        } else Nh.debug("user sign out", t), t.signOut((function() {
+                                        } else Ih.debug("user sign out", t), t.signOut((function() {
                                             if (!r) return n();
                                             o.oAuthSignOutRedirect(n, i)
                                         }))
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.oAuthSignOutRedirect = function(e, t) {
-                    Xs().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
+                    $s().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
                 }, e.prototype.oAuthSignOutAndResolve = function(e) {
                     this._oAuthHandler.signOut(), e()
                 }, e.prototype.oAuthSignOutRedirectOrReject = function(e) {
                     this._oAuthHandler.signOut(), setTimeout((function() {
                         return e(Error("Signout timeout fail"))
                     }), 3e3)
                 }, e.prototype.signOut = function(e) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var t;
-                        return Es(this, (function(n) {
+                        return _s(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.cleanCachedItems()];
                                 case 1:
                                     return n.sent(), [3, 3];
                                 case 2:
-                                    return n.sent(), Nh.debug("failed to clear cached items"), [3, 3];
+                                    return n.sent(), Ih.debug("failed to clear cached items"), [3, 3];
                                 case 3:
                                     return this.userPool ? (t = this.userPool.getCurrentUser()) ? [4, this.cognitoIdentitySignOut(e, t)] : [3, 5] : [3, 7];
                                 case 4:
                                     return n.sent(), [3, 6];
                                 case 5:
-                                    Nh.debug("no current Cognito user"), n.label = 6;
+                                    Ih.debug("no current Cognito user"), n.label = 6;
                                 case 6:
                                     return [3, 8];
                                 case 7:
-                                    Nh.debug("no Cognito User pool"), n.label = 8;
+                                    Ih.debug("no Cognito User pool"), n.label = 8;
                                 case 8:
-                                    return Sh("signOut", this.user, "A user has been signed out"), this.user = null, [2]
+                                    return Lh("signOut", this.user, "A user has been signed out"), this.user = null, [2]
                             }
                         }))
                     }))
                 }, e.prototype.cleanCachedItems = function() {
-                    return Cs(this, void 0, void 0, (function() {
-                        return Es(this, (function(e) {
+                    return Es(this, void 0, void 0, (function() {
+                        return _s(this, (function(e) {
                             switch (e.label) {
                                 case 0:
                                     return [4, this.Credentials.clear()];
                                 case 1:
                                     return e.sent(), [2]
                             }
                         }))
                     }))
                 }, e.prototype.changePassword = function(e, t, n, r) {
                     var o = this;
                     return void 0 === r && (r = this._config.clientMetadata), new Promise((function(i, a) {
                         o.userSession(e).then((function(o) {
                             e.changePassword(t, n, (function(e, t) {
-                                return e ? (Nh.debug("change password failure", e), a(e)) : i(t)
+                                return e ? (Ih.debug("change password failure", e), a(e)) : i(t)
                             }), r)
                         }))
                     }))
                 }, e.prototype.forgotPassword = function(e, t) {
                     if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(Ss.EmptyUsername);
+                    if (!e) return this.rejectAuthError(Ls.EmptyUsername);
                     var n = this.createCognitoUser(e);
                     return new Promise((function(r, o) {
                         n.forgotPassword({
                             onSuccess: function() {
                                 r()
                             },
                             onFailure: function(t) {
-                                Nh.debug("forgot password failure", t), Sh("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
+                                Ih.debug("forgot password failure", t), Lh("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
                             },
                             inputVerificationCode: function(t) {
-                                Sh("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
+                                Lh("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
                             }
                         }, t)
                     }))
                 }, e.prototype.forgotPasswordSubmit = function(e, t, n, r) {
                     if (void 0 === r && (r = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(Ss.EmptyUsername);
-                    if (!t) return this.rejectAuthError(Ss.EmptyCode);
-                    if (!n) return this.rejectAuthError(Ss.EmptyPassword);
+                    if (!e) return this.rejectAuthError(Ls.EmptyUsername);
+                    if (!t) return this.rejectAuthError(Ls.EmptyCode);
+                    if (!n) return this.rejectAuthError(Ls.EmptyPassword);
                     var o = this.createCognitoUser(e);
                     return new Promise((function(i, a) {
                         o.confirmPassword(t, n, {
                             onSuccess: function(t) {
-                                Sh("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
+                                Lh("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
                             },
                             onFailure: function(t) {
-                                Sh("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
+                                Lh("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
                             }
                         }, r)
                     }))
                 }, e.prototype.currentUserInfo = function() {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var e, t, n, r, o, i, a;
-                        return Es(this, (function(s) {
+                        return _s(this, (function(s) {
                             switch (s.label) {
                                 case 0:
                                     return (e = this.Credentials.getCredSource()) && "aws" !== e && "userPool" !== e ? [3, 9] : [4, this.currentUserPoolUser().catch((function(e) {
-                                        return Nh.error(e)
+                                        return Ih.error(e)
                                     }))];
                                 case 1:
                                     if (!(a = s.sent())) return [2, null];
                                     s.label = 2;
                                 case 2:
                                     return s.trys.push([2, 8, , 9]), [4, this.userAttributes(a)];
                                 case 3:
                                     t = s.sent(), n = this.attributesToObject(t), r = null, s.label = 4;
                                 case 4:
                                     return s.trys.push([4, 6, , 7]), [4, this.currentCredentials()];
                                 case 5:
                                     return r = s.sent(), [3, 7];
                                 case 6:
-                                    return o = s.sent(), Nh.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
+                                    return o = s.sent(), Ih.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
                                 case 7:
                                     return [2, {
                                         id: r ? r.identityId : void 0,
                                         username: a.getUsername(),
                                         attributes: n
                                     }];
                                 case 8:
-                                    return i = s.sent(), Nh.error("currentUserInfo error", i), [2, {}];
+                                    return i = s.sent(), Ih.error("currentUserInfo error", i), [2, {}];
                                 case 9:
                                     return "federated" === e ? [2, (a = this.user) || {}] : [2]
                             }
                         }))
                     }))
                 }, e.prototype.federatedSignIn = function(e, t, n) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var r, o, i, a, s, u, l, c, d, f, p;
-                        return Es(this, (function(h) {
+                        return _s(this, (function(h) {
                             switch (h.label) {
                                 case 0:
                                     if (!this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation requires either a User Pool or Identity Pool in config");
                                     if ("undefined" === typeof e && this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation with Identity Pools requires tokens passed as arguments");
-                                    return Ts(e) || (g = e) && ["customProvider"].find((function(e) {
+                                    return As(e) || (g = e) && ["customProvider"].find((function(e) {
                                         return g.hasOwnProperty(e)
                                     })) || function(e) {
                                         return e && !!["customState"].find((function(t) {
                                             return e.hasOwnProperty(t)
                                         }))
                                     }(e) || "undefined" === typeof e ? (r = e || {
-                                        provider: Ds.Cognito
-                                    }, s = Ts(r) ? r.provider : r.customProvider, Ts(r), o = r.customState, this._config.userPoolId && (i = As(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = As(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
+                                        provider: Ss.Cognito
+                                    }, s = As(r) ? r.provider : r.customProvider, As(r), o = r.customState, this._config.userPoolId && (i = Os(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = Os(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
                                 case 1:
                                     s = e;
                                     try {
-                                        (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && Nh.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
+                                        (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && Ih.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
                                     } catch (y) {}
                                     return l = t.token, c = t.identity_id, d = t.expires_at, [4, this.Credentials.set({
                                         provider: s,
                                         token: l,
                                         identity_id: c,
                                         user: n,
                                         expires_at: d
                                     }, "federation")];
                                 case 2:
                                     return f = h.sent(), [4, this.currentAuthenticatedUser()];
                                 case 3:
-                                    return p = h.sent(), Sh("signIn", p, "A user " + p.username + " has been signed in"), Nh.debug("federated sign in credentials", f), [2, f];
+                                    return p = h.sent(), Lh("signIn", p, "A user " + p.username + " has been signed in"), Ih.debug("federated sign in credentials", f), [2, f];
                                 case 4:
                                     return [2]
                             }
                             var g
                         }))
                     }))
                 }, e.prototype._handleAuthResponse = function(e) {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d, f, p, h;
-                        return Es(this, (function(g) {
+                        return _s(this, (function(g) {
                             switch (g.label) {
                                 case 0:
-                                    if (this.oAuthFlowInProgress) return Nh.debug("Skipping URL " + e + " current flow in progress"), [2];
+                                    if (this.oAuthFlowInProgress) return Ih.debug("Skipping URL " + e + " current flow in progress"), [2];
                                     g.label = 1;
                                 case 1:
                                     if (g.trys.push([1, , 8, 9]), this.oAuthFlowInProgress = !0, !this._config.userPoolId) throw new Error("OAuth responses require a User Pool defined in config");
-                                    if (Sh("parsingCallbackUrl", {
+                                    if (Lh("parsingCallbackUrl", {
                                             url: e
-                                        }, "The callback url is being parsed"), t = e || (Xs().isBrowser ? window.location.href : ""), n = !!((0, ph.Qc)(t).query || "").split("&").map((function(e) {
+                                        }, "The callback url is being parsed"), t = e || ($s().isBrowser ? window.location.href : ""), n = !!((0, hh.Qc)(t).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).find((function(e) {
-                                            var t = _s(e, 1)[0];
+                                            var t = Ts(e, 1)[0];
                                             return "code" === t || "error" === t
-                                        })), r = !!((0, ph.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
+                                        })), r = !!((0, hh.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
                                             return e.split("=")
                                         })).find((function(e) {
-                                            var t = _s(e, 1)[0];
+                                            var t = Ts(e, 1)[0];
                                             return "access_token" === t || "error" === t
                                         })), !n && !r) return [3, 7];
                                     this._storage.setItem("amplify-redirected-from-hosted-ui", "true"), g.label = 2;
                                 case 2:
                                     return g.trys.push([2, 6, , 7]), [4, this._oAuthHandler.handleAuthResponse(t)];
                                 case 3:
-                                    return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new Bp({
-                                        IdToken: new Up({
+                                    return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new Fp({
+                                        IdToken: new Pp({
                                             IdToken: a
                                         }),
-                                        RefreshToken: new Pp({
+                                        RefreshToken: new Rp({
                                             RefreshToken: s
                                         }),
-                                        AccessToken: new Op({
+                                        AccessToken: new zp({
                                             AccessToken: i
                                         })
                                     }), c = void 0, this._config.identityPoolId ? [4, this.Credentials.set(l, "session")] : [3, 5];
                                 case 4:
-                                    c = g.sent(), Nh.debug("AWS credentials", c), g.label = 5;
+                                    c = g.sent(), Ih.debug("AWS credentials", c), g.label = 5;
                                 case 5:
-                                    return d = /-/.test(u), (f = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Sh("signIn", f, "A user " + f.getUsername() + " has been signed in"), Sh("cognitoHostedUI", f, "A user " + f.getUsername() + " has been signed in via Cognito Hosted UI"), d && (p = u.split("-").splice(1).join("-"), Sh("customOAuthState", p.match(/.{2}/g).map((function(e) {
+                                    return d = /-/.test(u), (f = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Lh("signIn", f, "A user " + f.getUsername() + " has been signed in"), Lh("cognitoHostedUI", f, "A user " + f.getUsername() + " has been signed in via Cognito Hosted UI"), d && (p = u.split("-").splice(1).join("-"), Lh("customOAuthState", p.match(/.{2}/g).map((function(e) {
                                         return String.fromCharCode(parseInt(e, 16))
                                     })).join(""), "State for user " + f.getUsername())), [2, c];
                                 case 6:
-                                    return h = g.sent(), Nh.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Sh("signIn_failure", h, "The OAuth response flow failed"), Sh("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), Sh("customState_failure", h, "A failure occurred when returning state"), [3, 7];
+                                    return h = g.sent(), Ih.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Lh("signIn_failure", h, "The OAuth response flow failed"), Lh("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), Lh("customState_failure", h, "A failure occurred when returning state"), [3, 7];
                                 case 7:
                                     return [3, 9];
                                 case 8:
                                     return this.oAuthFlowInProgress = !1, [7];
                                 case 9:
                                     return [2]
                             }
@@ -68943,86 +68991,86 @@
                 }, e.prototype.createCognitoUser = function(e) {
                     var t = {
                         Username: e,
                         Pool: this.userPool
                     };
                     t.Storage = this._storage;
                     var n = this._config.authenticationFlowType,
-                        r = new qp(t);
+                        r = new Jp(t);
                     return n && r.setAuthenticationFlowType(n), r
                 }, e.prototype._isValidAuthStorage = function(e) {
                     return !!e && "function" === typeof e.getItem && "function" === typeof e.setItem && "function" === typeof e.removeItem && "function" === typeof e.clear
                 }, e.prototype.noUserPoolErrorHandler = function(e) {
-                    return !e || e.userPoolId && e.identityPoolId ? Ss.NoConfig : Ss.MissingAuthConfig
+                    return !e || e.userPoolId && e.identityPoolId ? Ls.NoConfig : Ls.MissingAuthConfig
                 }, e.prototype.rejectAuthError = function(e) {
-                    return Promise.reject(new jh(e))
+                    return Promise.reject(new wh(e))
                 }, e.prototype.rejectNoUserPool = function() {
                     var e = this.noUserPoolErrorHandler(this._config);
-                    return Promise.reject(new wh(e))
+                    return Promise.reject(new xh(e))
                 }, e.prototype.rememberDevice = function() {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var e, t;
-                        return Es(this, (function(n) {
+                        return _s(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    return t = n.sent(), Nh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                    return t = n.sent(), Ih.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         e.setDeviceStatusRemembered({
                                             onSuccess: function(e) {
                                                 t(e)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new jh(Ss.DeviceConfig)) : "NetworkError" === e.code ? n(new jh(Ss.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new wh(Ls.DeviceConfig)) : "NetworkError" === e.code ? n(new wh(Ls.NetworkError)) : n(e)
                                             }
                                         })
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.forgetDevice = function() {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var e, t;
-                        return Es(this, (function(n) {
+                        return _s(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    return t = n.sent(), Nh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                    return t = n.sent(), Ih.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         e.forgetDevice({
                                             onSuccess: function(e) {
                                                 t(e)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new jh(Ss.DeviceConfig)) : "NetworkError" === e.code ? n(new jh(Ss.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new wh(Ls.DeviceConfig)) : "NetworkError" === e.code ? n(new wh(Ls.NetworkError)) : n(e)
                                             }
                                         })
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.fetchDevices = function() {
-                    return Cs(this, void 0, void 0, (function() {
+                    return Es(this, void 0, void 0, (function() {
                         var e, t;
-                        return Es(this, (function(n) {
+                        return _s(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    throw t = n.sent(), Nh.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
+                                    throw t = n.sent(), Ih.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         var r = {
                                             onSuccess: function(e) {
                                                 var n = e.Devices.map((function(e) {
                                                     var t = e.DeviceAttributes.find((function(e) {
                                                         return "device_name" === e.Name
@@ -69031,28 +69079,28 @@
                                                         id: e.DeviceKey,
                                                         name: t.Value
                                                     }
                                                 }));
                                                 t(n)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new jh(Ss.DeviceConfig)) : "NetworkError" === e.code ? n(new jh(Ss.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new wh(Ls.DeviceConfig)) : "NetworkError" === e.code ? n(new wh(Ls.NetworkError)) : n(e)
                                             }
                                         };
                                         e.listDevices(60, null, r)
                                     }))]
                             }
                         }))
                     }))
                 }, e
             }(),
-            kh = new Lh(null);
-        fu.register(kh);
-        var Ch = "#FEFEFE",
-            Eh = function(e) {
+            Ch = new kh(null);
+        pu.register(Ch);
+        var Eh = "#FEFEFE",
+            _h = function(e) {
                 var t = e.hide,
                     n = pe().environ,
                     r = ta(),
                     o = Xi(zt.Url("/cognito_config", !1), {
                         cache: !0,
                         onData: function(e) {
                             var t = {
@@ -69064,15 +69112,15 @@
                                     domain: e.domain,
                                     scope: e.scope,
                                     prompt: "select_account",
                                     redirectSignIn: e.callback,
                                     responseType: "code"
                                 }
                             };
-                            kh.configure(t)
+                            Ch.configure(t)
                         }
                     });
                 var i = (0, Kr.jsx)("div", {
                     children: (0, Kr.jsxs)("div", {
                         className: "title-font",
                         style: {
                             marginTop: "4pt",
@@ -69100,52 +69148,52 @@
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         transform: "scale(1.1)",
                         marginTop: "10pt",
                         marginBottom: "40pt"
                     },
-                    children: (0, Kr.jsx)(_h, {
+                    children: (0, Kr.jsx)(Th, {
                         links: i,
                         children: o.loading ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsx)(no, {
                                 condition: !0,
                                 color: Ft.GetForegroundColor(),
                                 bold: !1,
                                 size: "140px",
                                 label: "Loading configuration "
                             })
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     paddingTop: "0pt"
                                 }
-                            }), (0, Kr.jsx)(Th, {
+                            }), (0, Kr.jsx)(Ah, {
                                 signin: function() {
-                                    bt.Set("env", At.PreferredName(n, r)), bt.Set("signinvia", "Google"), kh.federatedSignIn({
+                                    bt.Set("env", At.PreferredName(n, r)), bt.Set("signinvia", "Google"), Ch.federatedSignIn({
                                         provider: "Google",
                                         prompt: "select_account"
                                     }, {
                                         prompt: "select_account"
                                     })
                                 }
                             }), (0, Kr.jsx)("div", {
                                 style: {
                                     paddingTop: "6pt"
                                 }
-                            }), (0, Kr.jsx)(Ah, {
+                            }), (0, Kr.jsx)(Oh, {
                                 signin: function() {
                                     window.alert("Sign in with GitHub via Cognito not supported.")
                                 }
                             })]
                         })
                     })
                 })
             },
-            _h = function(e) {
+            Th = function(e) {
                 var t = e.links,
                     n = e.children;
                 return (0, Kr.jsx)("div", {
                     className: "container",
                     style: {
                         width: "265pt",
                         marginTop: "30pt"
@@ -69156,15 +69204,15 @@
                                 border: "2px solid var(--box-fg)",
                                 padding: "2px 2px 2px 2px",
                                 borderRadius: "6px",
                                 overflow: "hidden"
                             },
                             children: (0, Kr.jsxs)("div", {
                                 style: {
-                                    background: Ch,
+                                    background: Eh,
                                     border: "1px solid var(--box-fg)",
                                     borderRadius: "6px",
                                     overflow: "hidden"
                                 },
                                 children: [(0, Kr.jsx)("div", {
                                     style: {
                                         background: "var(--box-fg)",
@@ -69189,17 +69237,17 @@
                             })
                         }), t && (0, Kr.jsx)(Kr.Fragment, {
                             children: t
                         })]
                     })
                 })
             },
-            Th = function(e) {
+            Ah = function(e) {
                 var t = e.signin;
-                return (0, Kr.jsxs)(Oh, {
+                return (0, Kr.jsxs)(zh, {
                     signin: t,
                     children: [(0, Kr.jsx)("img", {
                         alt: "google",
                         src: Ut.GoogleLoginLogo(),
                         style: {
                             position: "relative",
                             marginTop: "-2px"
@@ -69211,17 +69259,17 @@
                             fontSize: "12pt",
                             marginLeft: "10pt"
                         },
                         children: "Sign in with Google"
                     })]
                 })
             },
-            Ah = function(e) {
+            Oh = function(e) {
                 var t = e.signin;
-                return (0, Kr.jsxs)(Oh, {
+                return (0, Kr.jsxs)(zh, {
                     signin: t,
                     children: [(0, Kr.jsx)("img", {
                         alt: "github",
                         src: Ut.GitHubLoginLogo(),
                         style: {
                             position: "relative",
                             marginTop: "-2px",
@@ -69234,30 +69282,30 @@
                             fontSize: "12pt",
                             marginLeft: "7pt"
                         },
                         children: "Sign in with GitHub"
                     })]
                 })
             },
-            Oh = function(e) {
+            zh = function(e) {
                 var t = e.signin,
                     n = e.children;
                 return (0, Kr.jsx)("div", {
                     style: {
-                        background: Ch,
+                        background: Eh,
                         padding: "0 10pt 0 10pt"
                     },
                     children: (0, Kr.jsx)("button", {
                         className: "signin-as-button",
                         onClick: t,
                         children: n
                     })
                 })
             },
-            zh = function(e) {
+            Uh = function(e) {
                 var t = a(Re(), 1)[0],
                     n = t.get("code"),
                     r = t.get("state"),
                     o = sessionStorage.getItem("oauth_state"),
                     i = sessionStorage.getItem("ouath_pkce_key"),
                     s = fe(),
                     u = "".concat(zt.Url("/cognito/callback", !1), "?code=").concat(n, "&code_verifier=").concat(i, "&state=").concat(r, "&state_verifier=").concat(o),
@@ -69280,28 +69328,28 @@
                     var c = bt.Get("signinvia");
                     return (0, Kr.jsx)("div", {
                         style: {
                             transform: "scale(1.1)",
                             marginTop: "10pt",
                             marginBottom: "40pt"
                         },
-                        children: (0, Kr.jsx)(_h, {
+                        children: (0, Kr.jsx)(Th, {
                             children: (0, Kr.jsx)(no, {
                                 condition: l.loading,
                                 color: Ft.GetForegroundColor(),
                                 bold: !1,
                                 size: 140,
                                 label: "Signing in via ".concat(c)
                             })
                         })
                     })
                 }
             },
-            Uh = __webpack_require__(9712),
-            Ph = function(e) {
+            Ph = __webpack_require__(9712),
+            Rh = function(e) {
                 var n, r, o, i, s, u, l, c, d, f, p, h, g = ta(),
                     y = a((0, t.useState)(!1), 2),
                     m = y[0],
                     v = y[1],
                     M = a((0, t.useState)(!1), 2),
                     b = M[0],
                     j = M[1],
@@ -69347,15 +69395,15 @@
                                 theme: {
                                     primaryColor: "blue",
                                     backgroundColor: "blue",
                                     logo: ""
                                 },
                                 allowedConnections: null === x || void 0 === x || null === (o = x.data) || void 0 === o ? void 0 : o.connections
                             };
-                            return new Uh.default(null === x || void 0 === x || null === (i = x.data) || void 0 === i ? void 0 : i.client, null === x || void 0 === x || null === (a = x.data) || void 0 === a ? void 0 : a.domain, s)
+                            return new Ph.default(null === x || void 0 === x || null === (i = x.data) || void 0 === i ? void 0 : i.client, null === x || void 0 === x || null === (a = x.data) || void 0 === a ? void 0 : a.domain, s)
                         }().show(), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && (document.getElementById("login_auth_container").style.height = "200", document.getElementById("login_auth_container").style.background = "white", document.getElementById("login_auth_container").style.borderStyle = "none"), document.getElementById("login_auth_container").firstChild.firstChild.style.paddingLeft = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingRight = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingTop = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingBottom = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", v(!0)
                 }
                 if ((g.loading || x.loading) && !g.error) return (0, Kr.jsx)(Kr.Fragment, {
                     children: "Loading ..."
                 });
                 if (g.error) return (0, Kr.jsx)(xi, {
                     error: g.error,
@@ -69399,15 +69447,15 @@
                                     position: "bottom",
                                     text: "AWS Account Alias: ".concat(null === g || void 0 === g || null === (c = g.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name)
                                 })]
                             }), (0, Kr.jsx)("br", {})]
                         })]
                     })
                 };
-                return I ? (0, Kr.jsx)(Eh, {
+                return I ? (0, Kr.jsx)(_h, {
                     hide: function() {
                         return D(!1)
                     }
                 }) : (0, Kr.jsx)(Kr.Fragment, {
                     children: Br.IsLoggedIn(g) ? (0, Kr.jsx)(t.Fragment, {
                         children: (0, Kr.jsxs)("div", {
                             className: "container",
@@ -69474,21 +69522,21 @@
                                                 }), (0, Kr.jsxs)("div", {
                                                     style: {
                                                         fontSize: "small",
                                                         marginTop: "6pt",
                                                         paddingTop: "5pt",
                                                         borderTop: "1px solid"
                                                     },
-                                                    children: ["Session started: ", (0, Kr.jsx)(va.FormatDuration, {
+                                                    children: ["Session started: ", (0, Kr.jsx)(Ma.FormatDuration, {
                                                         start: Br.Token().authenticated_at,
                                                         verbose: !0,
                                                         fallback: "just now",
                                                         suffix: "ago",
                                                         tooltip: !0
-                                                    }), "\xa0", (0, Kr.jsx)("br", {}), "Session expires: ", (0, Kr.jsx)(va.FormatDuration, {
+                                                    }), "\xa0", (0, Kr.jsx)("br", {}), "Session expires: ", (0, Kr.jsx)(Ma.FormatDuration, {
                                                         end: Br.Token().authenticated_until,
                                                         verbose: !0,
                                                         fallback: "now",
                                                         suffix: "from now",
                                                         tooltip: !0
                                                     }), "\xa0", (0, Kr.jsx)("br", {}), "Click ", (0, Kr.jsx)("span", {
                                                         style: {
@@ -70026,15 +70074,15 @@
                                     w && !m && T()
                                 }), 10), "")]
                             })]
                         })]
                     })
                 })
             },
-            Rh = function(e) {
+            Bh = function(e) {
                 var n = ta(),
                     r = pe().environCompare,
                     o = a((0, t.useState)(!1), 2),
                     i = o[0],
                     s = o[1],
                     u = a((0, t.useState)("all"), 2),
                     l = u[0],
@@ -70380,15 +70428,15 @@
                                 display: "none"
                             },
                             children: d.yaml()
                         })]
                     })
                 })
             },
-            Bh = function(e) {
+            Fh = function(e) {
                 return {
                     __get: function(t, n, r, o) {
                         var i = e.findIndex((function(e) {
                             return e.type === t
                         }));
                         if (i >= 0) {
                             var a = n ? "".concat(t, ".").concat(n) : t;
@@ -70401,16 +70449,16 @@
                                 }
                             }
                         }
                         return null
                     }
                 }
             },
-            Fh = function(e) {
-                e = Bh(e);
+            Yh = function(e) {
+                e = Fh(e);
                 var n = a((0, t.useState)([]), 2),
                     r = n[0],
                     o = n[1];
                 return (0, t.useState)({
                     count: function() {
                         return r.length
                     },
@@ -70455,23 +70503,23 @@
                     __unselect: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
                             n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null;
                         null == n && (n = this.__lookup(e, t)), n >= 0 && (r.splice(n, 1), o(u(r)))
                     }
                 })[0]
             },
-            Yh = function(e) {
+            Qh = function(e) {
                 var t;
                 return "function" == typeof e && (e = e()), (null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object ? e : {}
             },
-            Qh = function(e, t) {
+            Gh = function(e, t) {
                 return "function" == typeof e && (e = e()), void 0 !== e ? e : {}
             };
 
-        function Gh(e) {
+        function Wh(e) {
             var t, n, r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0,
                 o = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
             if (Object.is(e, r))
                 if ((null === (n = e) || void 0 === n ? void 0 : n.constructor) === Object) e = Ye({}, e);
                 else if (Array.isArray(e)) {
                 var i = function(e) {
                     var t = u(e),
@@ -70486,24 +70534,24 @@
                     return t
                 };
                 e = i(e)
             } else "function" === typeof e && (e = e(r));
             else(null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object && (null === r || void 0 === r ? void 0 : r.constructor) === Object && o && (e = Ye(Ye({}, r), e));
             return e
         }
-        var Wh = function(e, n) {
+        var Hh = function(e, n) {
                 var r = !0 === (null === e || void 0 === e ? void 0 : e.__keyedState) ? !0 === e.__keyedStateUsage ? e : e.keyed("default") : null,
-                    o = r ? r.__state() ? r.__state() : Qh(n) : Yh(e),
+                    o = r ? r.__state() ? r.__state() : Gh(n) : Qh(e),
                     i = a((0, t.useState)(o), 2),
                     s = i[0],
                     u = i[1];
                 return (0, t.useEffect)((function() {
-                    o && r && !r.__state() && r.__updateState(Gh(o, s, !0))
+                    o && r && !r.__state() && r.__updateState(Wh(o, s, !0))
                 }), []), r ? [s, function(e) {
-                    e = Gh(e, s, !0), u(e), r.__updateState(e)
+                    e = Wh(e, s, !0), u(e), r.__updateState(e)
                 }] : {
                     __keyedState: !0,
                     key: null,
                     keyed: function(e) {
                         var t;
                         if (!0 === this.__keyedState) {
                             (null === (t = e) || void 0 === t ? void 0 : t.constructor) === String && 0 !== e.length || (e = "default");
@@ -70527,27 +70575,27 @@
                                     return s[e]
                                 }
                             }
                         }
                     }
                 }
             },
-            Hh = {
+            Zh = {
                 color: "var(--box-fg)",
                 fontWeight: "bold",
                 paddingTop: "1pt",
                 verticalAlign: "top",
                 width: "5%",
                 paddingRight: "8pt",
                 whiteSpace: "nowrap"
             },
-            Zh = {
+            Vh = {
                 verticalAlign: "top"
             },
-            Vh = function(e) {
+            qh = function(e) {
                 var t = e.showVpcs,
                     n = e.toggleVpcs,
                     r = e.showSecurityGroups,
                     o = e.toggleSecurityGroups,
                     i = e.showSubnetsPublic,
                     a = e.toggleSubnetsPublic,
                     s = e.showSubnetsPrivate,
@@ -70600,15 +70648,15 @@
                             },
                             onClick: o,
                             children: "Security Groups"
                         })]
                     })]
                 })
             },
-            qh = function(e) {
+            Jh = function(e) {
                 var t = e.showGac,
                     n = e.toggleGac,
                     r = e.showEcosystem,
                     o = e.toggleEcosystem;
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
                         className: "box margin thickborder",
@@ -70633,15 +70681,15 @@
                             },
                             onClick: o,
                             children: "Ecosystem Definition"
                         })]
                     })
                 })
             },
-            Jh = function(e) {
+            Kh = function(e) {
                 var t, n, r = e.keyedState,
                     o = e.hide,
                     i = "true" === (null === (t = Re()[0]) || void 0 === t || null === (n = t.get("all")) || void 0 === n ? void 0 : n.toLowerCase()),
                     a = Xi("/aws/vpcs".concat(i ? "/all" : ""), {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
@@ -70680,27 +70728,27 @@
                                 marginTop: "2pt"
                             },
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading VPCs"
                             })
                         }), a.map((function(e) {
                             return (0, Kr.jsx)("div", {
-                                children: (0, Kr.jsx)(Kh, {
+                                children: (0, Kr.jsx)(Xh, {
                                     vpc: e,
                                     keyedState: null === r || void 0 === r ? void 0 : r.keyed(e.id)
                                 })
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            Kh = function(e) {
+            Xh = function(e) {
                 var t = e.vpc,
                     n = e.keyedState,
-                    r = a(Wh(n), 2),
+                    r = a(Hh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function(e) {
                         return o[e]
                     },
                     u = function(e) {
                         return i(Be({}, e, !o[e]))
@@ -70746,42 +70794,42 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "ID:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: t.id
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.status
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -70804,15 +70852,15 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return t.id, u("showSubnetsPublic")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Public Subnets:"
                                     }), (0, Kr.jsx)("td", {
                                         children: l() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70828,29 +70876,29 @@
                                 }), l() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Xh, {
+                                            children: (0, Kr.jsx)($h, {
                                                 type: "public",
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-public")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showSubnetsPrivate")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Private Subnets:"
                                     }), (0, Kr.jsx)("td", {
                                         children: c() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70866,29 +70914,29 @@
                                 }), c() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Xh, {
+                                            children: (0, Kr.jsx)($h, {
                                                 type: "private",
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-private")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showSecurityGroups")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Security Groups:"
                                     }), (0, Kr.jsx)("td", {
                                         children: d() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70904,28 +70952,28 @@
                                 }), d() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(eg, {
+                                            children: (0, Kr.jsx)(tg, {
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("security-groups")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showTags")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: f() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70941,26 +70989,26 @@
                                 }), f() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(og, {
+                                            children: (0, Kr.jsx)(ig, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            Xh = function(e) {
+            $h = function(e) {
                 var t, n, r = e.vpcId,
                     o = e.type,
                     i = e.hide,
                     a = e.notitle,
                     s = e.keyedState,
                     u = "true" === (null === (t = Re()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                     l = r ? "?vpc=".concat(r) : "",
@@ -70999,31 +71047,31 @@
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading Subnets"
                             })
                         }), null === (n = c.filter((function(e) {
                             return !o || e.type === o
                         }))) || void 0 === n ? void 0 : n.map((function(e) {
                             return (0, Kr.jsxs)("div", {
-                                children: [(0, Kr.jsx)($h, {
+                                children: [(0, Kr.jsx)(eg, {
                                     subnet: e,
                                     keyedState: null === s || void 0 === s ? void 0 : s.keyed(e.id)
                                 }), (0, Kr.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            $h = function(e) {
+            eg = function(e) {
                 var t = e.subnet,
                     n = e.keyedState,
-                    r = a(Wh(n), 2),
+                    r = a(Hh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function() {
                         return o["showTags"]
                     };
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
@@ -71071,60 +71119,60 @@
                                 })
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "ID:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: [null === t || void 0 === t ? void 0 : t.id, (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
                                             children: null === t || void 0 === t ? void 0 : t.subnet_arn
                                         })]
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Zone:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.zone
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "VPC:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.vpc
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.status
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "4pt"
                                         },
@@ -71148,15 +71196,15 @@
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return i(Be({}, e = "showTags", !o[e]));
                                         var e
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: s() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71172,26 +71220,26 @@
                                 }), s() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(og, {
+                                            children: (0, Kr.jsx)(ig, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            eg = function(e) {
+            tg = function(e) {
                 var t, n = e.vpcId,
                     r = e.notitle,
                     o = e.keyedState,
                     i = e.hide,
                     a = "true" === (null === (t = Re()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                     s = n ? "?vpc=".concat(n) : "",
                     u = Xi("/aws/security_groups".concat(a ? "/all" : "").concat(s), {
@@ -71227,31 +71275,31 @@
                                 marginTop: "2pt"
                             },
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading security groups"
                             })
                         }), u.map((function(e) {
                             return (0, Kr.jsxs)("div", {
-                                children: [(0, Kr.jsx)(tg, {
+                                children: [(0, Kr.jsx)(ng, {
                                     securityGroup: e,
                                     keyedState: null === o || void 0 === o ? void 0 : o.keyed(e.id)
                                 }), (0, Kr.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            tg = function(e) {
+            ng = function(e) {
                 var t = e.securityGroup,
                     n = e.keyedState,
-                    r = a(Wh(n), 2),
+                    r = a(Hh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function(e) {
                         return o[e]
                     },
                     u = function(e) {
                         return i(Be({}, e, !o[e]))
@@ -71293,47 +71341,47 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "ID:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: [null === t || void 0 === t ? void 0 : t.id, (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
                                             children: null === t || void 0 === t ? void 0 : t.securityGroup
                                         })]
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             whiteSpace: "break-spaces",
                                             wordBreak: "break-all"
                                         },
                                         children: null === t || void 0 === t ? void 0 : t.description
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "VPC:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.vpc
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "4pt"
                                         },
@@ -71356,15 +71404,15 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showInboundRules")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Inbound Rules:"
                                     }), (0, Kr.jsx)("td", {
                                         children: l() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsxs)("small", {
                                                 children: [(0, Kr.jsx)("u", {
                                                     children: "Hide"
                                                 }), "\xa0", Fr.DownArrowHollow]
@@ -71380,27 +71428,27 @@
                                 }), l() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(ng, {
+                                            children: (0, Kr.jsx)(rg, {
                                                 securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                 direction: "inbound"
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showOutboundRules")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Outbound Rules:"
                                     }), (0, Kr.jsx)("td", {
                                         children: c() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71416,27 +71464,27 @@
                                 }), c() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(ng, {
+                                            children: (0, Kr.jsx)(rg, {
                                                 securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                 direction: "outbound"
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showTags")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: d() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71452,26 +71500,26 @@
                                 }), d() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(og, {
+                                            children: (0, Kr.jsx)(ig, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            ng = function(e) {
+            rg = function(e) {
                 var t = e.securityGroupId,
                     n = e.direction,
                     r = "inbound" === n ? "?direction=inbound" : "outbound" === n ? "?direction=outbound" : "",
                     o = Xi("/aws/security_group_rules/".concat(t).concat(r), {
                         cache: !0
                     });
                 return (0, Kr.jsxs)(Kr.Fragment, {
@@ -71481,26 +71529,26 @@
                             paddingBottom: "10pt"
                         },
                         children: (0, Kr.jsx)(no, {
                             label: "Loading security group rules"
                         })
                     }), null === o || void 0 === o ? void 0 : o.map((function(e) {
                         return (0, Kr.jsxs)("div", {
-                            children: [(0, Kr.jsx)(rg, {
+                            children: [(0, Kr.jsx)(og, {
                                 securityGroupRule: e
                             }), (0, Kr.jsx)("div", {
                                 style: {
                                     height: "4pt"
                                 }
                             })]
                         }, e.id)
                     }))]
                 })
             },
-            rg = function(e) {
+            og = function(e) {
                 var t = e.securityGroupRule;
 
                 function n(e) {
                     var t, n;
                     if ("TCP" === (null === e || void 0 === e || null === (t = e.protocol) || void 0 === t ? void 0 : t.toUpperCase())) {
                         if (22 === (null === e || void 0 === e ? void 0 : e.port_from) && 22 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "SSH";
                         if (443 === (null === e || void 0 === e ? void 0 : e.port_from) && 443 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "HTTPS";
@@ -71555,78 +71603,78 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Direction:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null !== t && void 0 !== t && t.egress ? "Outbound" : "Inbound"
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Protocol:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: r(t)
                                     })]
                                 }), n(t) !== r(t) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Type:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: n(t)
                                     })]
                                 }), o(t) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Port:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: o(t)
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.cidr) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.description) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             whiteSpace: "break-spaces",
                                             wordBreak: "break-all"
                                         },
                                         children: null === t || void 0 === t ? void 0 : t.description
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Security Group:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === t || void 0 === t ? void 0 : t.security_group
                                     })]
                                 })]
                             })
                         })]
                     })
                 })
             },
-            og = function(e) {
+            ig = function(e) {
                 var t;
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
                     children: (0, Kr.jsx)("div", {
                         className: "box lighten",
@@ -71661,15 +71709,15 @@
                             children: (0, Kr.jsx)("li", {
                                 children: "No tags."
                             })
                         })
                     })
                 })
             },
-            ig = function(e) {
+            ag = function(e) {
                 var t = Xi("/aws/stacks", {
                         cache: !0
                     }),
                     n = {
                         cursor: "pointer"
                     },
                     r = Ye(Ye({}, n), {}, {
@@ -71700,19 +71748,19 @@
                                 },
                                 children: o.name
                             }, o.name)
                         }))]
                     })]
                 })
             },
-            ag = function(e) {
+            sg = function(e) {
                 var t, n, r, o, i, s, u, l, c, d, f, p, h = e.stackName,
                     g = e.keyedState,
                     y = e.hide,
-                    m = a(Wh(g), 2),
+                    m = a(Hh(g), 2),
                     v = m[0],
                     M = m[1],
                     b = Xi("/aws/stacks/".concat(h), {
                         cache: !0
                     }),
                     j = function(e) {
                         return v[e]
@@ -71764,56 +71812,56 @@
                         children: b.loading ? (0, Kr.jsx)(no, {
                             label: "Loading stack info"
                         }) : (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Name:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Ye(Ye({}, Zh), {}, {
+                                        style: Ye(Ye({}, Vh), {}, {
                                             wordBreak: "break-all"
                                         }),
                                         children: [(0, Kr.jsx)("b", {
                                             style: {
                                                 float: "right",
                                                 cursor: "pointer",
                                                 marginTop: "-2pt"
                                             },
                                             onClick: y,
                                             children: Fr.X
                                         }), h]
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "ID:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Ye(Ye({}, Zh), {}, {
+                                        style: Ye(Ye({}, Vh), {}, {
                                             wordBreak: "break-all"
                                         }),
                                         children: (0, Kr.jsx)("small", {
                                             children: null === (n = b.data) || void 0 === n ? void 0 : n.id
                                         })
                                     })]
                                 }), (null === (r = b.data) || void 0 === r ? void 0 : r.role_arn) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Role:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: (null === (o = b.data) || void 0 === o ? void 0 : o.role_arn) || Fr.EmptySet
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === (i = b.data) || void 0 === i ? void 0 : i.description
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -71832,34 +71880,34 @@
                                         style: {
                                             height: "2pt"
                                         },
                                         colSpan: "2"
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === (s = b.data) || void 0 === s ? void 0 : s.status
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Created:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === (u = b.data) || void 0 === u ? void 0 : u.created
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Updated:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: null === (l = b.data) || void 0 === l ? void 0 : l.updated
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -71878,18 +71926,18 @@
                                         style: {
                                             height: "2pt"
                                         },
                                         colSpan: "2"
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Outputs:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: [x() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: N,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71914,25 +71962,25 @@
                                 }), x() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(sg, {
+                                            children: (0, Kr.jsx)(ug, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Parameters:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: [I() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: D,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71957,25 +72005,25 @@
                                 }), I() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(ug, {
+                                            children: (0, Kr.jsx)(lg, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Resources:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: [S() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: L,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -72000,25 +72048,25 @@
                                 }), S() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(lg, {
+                                            children: (0, Kr.jsx)(cg, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Hh,
+                                        style: Zh,
                                         children: "Template:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Zh,
+                                        style: Vh,
                                         children: [k() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: C,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -72043,26 +72091,26 @@
                                 }), k() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(cg, {
+                                            children: (0, Kr.jsx)(dg, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 })]
                             })
                         })
                     })]
                 })
             },
-            sg = function(e) {
+            ug = function(e) {
                 var t, n = Xi("/aws/stacks/".concat(e.stackName, "/outputs"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -72105,15 +72153,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            ug = function(e) {
+            lg = function(e) {
                 var t, n = Xi("/aws/stacks/".concat(e.stackName, "/parameters"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -72156,15 +72204,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            lg = function(e) {
+            cg = function(e) {
                 var t, n = Xi("/aws/stacks/".concat(e.stackName, "/resources"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -72210,15 +72258,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            cg = function(e) {
+            dg = function(e) {
                 var t = Xi("/aws/stacks/".concat(e.stackName, "/template"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -72245,15 +72293,15 @@
                                 },
                                 children: st.IsObject(t.data) ? Bi.Format(t.data) : t.data
                             })
                         })
                     })
                 })
             },
-            dg = function(e) {
+            fg = function(e) {
                 var t, n, r, o, i, a, s = e.hide,
                     u = Xi("/info", {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         maxWidth: "500pt",
@@ -72304,15 +72352,15 @@
                                     }) : u.data.gac.values[e]]
                                 }, e)
                             })))
                         })]
                     })]
                 })
             },
-            fg = function(e) {
+            pg = function(e) {
                 var t, n, r, o, i = e.hide,
                     a = Xi("/info", {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         maxWidth: "500pt",
@@ -72338,81 +72386,81 @@
                         className: "box margin",
                         children: [a.loading && (0, Kr.jsx)(no, {
                             label: "Loading Ecosystem"
                         }), !a.loading && Bi.Format(null === (r = a.data) || void 0 === r || null === (o = r.buckets) || void 0 === o ? void 0 : o.ecosystem)]
                     })]
                 })
             },
-            pg = function() {
-                var e = Wh(),
+            hg = function() {
+                var e = Hh(),
                     n = [{
                         type: "stack",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(ag, {
+                            return (0, Kr.jsx)(sg, {
                                 stackName: e,
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "vpcs",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Jh, {
+                            return (0, Kr.jsx)(Kh, {
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "subnets-public",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Xh, {
+                            return (0, Kr.jsx)($h, {
                                 type: "public",
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "subnets-private",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Xh, {
+                            return (0, Kr.jsx)($h, {
                                 type: "private",
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "security-groups",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(eg, {
+                            return (0, Kr.jsx)(tg, {
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "gac",
                         create: function(e, t, n, r) {
-                            return (0, Kr.jsx)(dg, {
+                            return (0, Kr.jsx)(fg, {
                                 hide: n
                             })
                         }
                     }, {
                         type: "ecosystem",
                         create: function(e, t, n, r) {
-                            return (0, Kr.jsx)(fg, {
+                            return (0, Kr.jsx)(pg, {
                                 hide: n
                             })
                         }
                     }],
-                    r = Fh(n),
-                    o = Fh(n);
+                    r = Yh(n),
+                    o = Yh(n);
                 var i = function() {
                         return r.toggle("vpcs")
                     },
                     a = function() {
                         return r.toggle("ecosystem")
                     };
                 return (0, t.useEffect)((function() {
@@ -72421,15 +72469,15 @@
                     children: (0, Kr.jsx)("tbody", {
                         children: (0, Kr.jsxs)("tr", {
                             children: [(0, Kr.jsxs)("td", {
                                 style: {
                                     verticalAlign: "top",
                                     paddingRight: "8pt"
                                 },
-                                children: [(0, Kr.jsx)(Vh, {
+                                children: [(0, Kr.jsx)(qh, {
                                     keyedState: e,
                                     showVpcs: function() {
                                         return r.selected("vpcs")
                                     },
                                     toggleVpcs: i,
                                     showSubnetsPublic: function() {
                                         return o.selected("subnets-public")
@@ -72445,26 +72493,26 @@
                                     },
                                     showSecurityGroups: function() {
                                         return o.selected("security-groups")
                                     },
                                     toggleSecurityGroups: function() {
                                         return o.toggle("security-groups")
                                     }
-                                }), (0, Kr.jsx)(qh, {
+                                }), (0, Kr.jsx)(Jh, {
                                     showGac: function() {
                                         return r.selected("gac")
                                     },
                                     toggleGac: function() {
                                         return r.toggle("gac")
                                     },
                                     showEcosystem: function() {
                                         return r.selected("ecosystem")
                                     },
                                     toggleEcosystem: a
-                                }), (0, Kr.jsx)(ig, {
+                                }), (0, Kr.jsx)(ag, {
                                     toggleStack: function(e) {
                                         return r.toggle("stack", e)
                                     },
                                     selectedStack: function(e) {
                                         return r.selected("stack", e)
                                     }
                                 })]
@@ -72493,15 +72541,15 @@
                                     }, t.key)
                                 }))
                             })]
                         })
                     })
                 })
             },
-            hg = function(e) {
+            gg = function(e) {
                 var t = ta();
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "container",
                         id: "login_container",
                         children: (0, Kr.jsxs)("div", {
                             className: "boxstyle check-warn",
@@ -72530,56 +72578,56 @@
                                     })
                                 }), " page."]
                             })]
                         })
                     })
                 })
             },
-            gg = function() {
+            yg = function() {
                 var e = ce().state.url;
                 return e.startsWith(window.location.origin) && (e = e.substring(window.location.origin.length)), (0, Kr.jsx)(xe, {
                     to: e,
                     replace: !0
                 })
             },
-            yg = function(e) {
+            mg = function(e) {
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "box thickborder",
                         style: {
                             marginBottom: "6pt"
                         },
                         children: (0, Kr.jsx)(Si, {
                             certificate: e.certificate
                         })
                     })
                 })
             },
-            mg = function(e) {
+            vg = function(e) {
                 var t, n = a(Re(), 1)[0].get("hostname"),
                     r = Xi("/certificates?hostname=".concat(n));
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
                         className: "container",
                         style: {
                             width: "800pt"
                         },
                         children: [(0, Kr.jsx)("b", {
                             children: "SSL Certificates"
                         }), null === r || void 0 === r || null === (t = r.data) || void 0 === t ? void 0 : t.map((function(e) {
                             return (0, Kr.jsx)("div", {
-                                children: (0, Kr.jsx)(yg, {
+                                children: (0, Kr.jsx)(mg, {
                                     certificate: e
                                 })
                             }, e.serial_number)
                         }))]
                     })
                 })
             },
-            vg = function(e) {
+            Mg = function(e) {
                 var t = Xi("/portal_access_key");
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
                         className: "container",
                         style: {
                             width: "800pt"
                         },
@@ -72593,15 +72641,15 @@
                             children: (0, Kr.jsx)(Ii, {
                                 accessKey: t.data
                             })
                         })]
                     })
                 })
             },
-            Mg = function() {
+            bg = function() {
                 var e = Xi("/users/projects", {
                         cache: !0
                     }),
                     t = Xi("/users/roles", {
                         cache: !0
                     }),
                     n = Xi("/users/institutions", {
@@ -72659,15 +72707,15 @@
                             return (null === e || void 0 === e ? void 0 : e.map((function(e) {
                                 return o.title(e)
                             })).join(", ")) || ""
                         }
                     };
                 return o
             },
-            bg = [{
+            jg = [{
                 name: "email",
                 label: "Email Address",
                 type: "email",
                 focus: !0,
                 required: !0
             }, {
                 name: "first_name",
@@ -72712,38 +72760,38 @@
                 label: "Updated",
                 readonly: !0
             }, {
                 name: "uuid",
                 label: "UUID",
                 readonly: !0
             }],
-            jg = {
+            wg = {
                 PrincipalInvestigatorLine: function(e) {
                     var t, n, r = e.institution,
-                        o = Mg();
+                        o = bg();
                     return (0, Kr.jsx)("div", {
                         style: e.style,
                         children: o.principleInvestigator(r) && (0, Kr.jsxs)("small", {
                             children: [(0, Kr.jsxs)("b", {
                                 children: ["Principle Investigator ", Fr.RightArrow]
                             }), " ", null === (t = o.principleInvestigator(r)) || void 0 === t ? void 0 : t.name, "\xa0", (0, Kr.jsx)(Ni, {
                                 href: kr.Path("/users/".concat(null === (n = o.principleInvestigator(r)) || void 0 === n ? void 0 : n.uuid))
                             })]
                         })
                     })
                 },
                 useUserInputs: function() {
                     var e = ta(),
-                        n = At.IsFoursightFourfront(e) ? bg.filter((function(e) {
+                        n = At.IsFoursightFourfront(e) ? jg.filter((function(e) {
                             return "project" !== e.name && "role" !== e.name && "institution" !== e.name
-                        })) : bg;
+                        })) : jg;
                     return (0, t.useState)(Tr.Clone(Tr.Clone(n)))
                 }
             },
-            wg = function(e) {
+            xg = function(e) {
                 var t = Xi("/users/".concat(e.email, "?raw=true"));
                 return (0, Kr.jsxs)("pre", {
                     className: "box",
                     children: [(0, Kr.jsx)("span", {
                         style: {
                             float: "right",
                             marginTop: "-6pt",
@@ -72757,15 +72805,15 @@
                     }), t.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {})
                     }) : (0, Kr.jsx)(Kr.Fragment, {
                         children: Bi.Format(t.data)
                     })]
                 })
             },
-            xg = function(e) {
+            Ng = function(e) {
                 var n = {
                         color: "var(--box-fg)",
                         fontWeight: "bold",
                         fontSize: "small",
                         paddingTop: "1pt",
                         verticalAlign: "top",
                         width: "5%",
@@ -72874,16 +72922,16 @@
                                     })]
                                 }, o.name)
                             }))
                         })
                     })
                 })
             },
-            Ng = function(e) {
-                var t = Mg(),
+            Ig = function(e) {
+                var t = bg(),
                     n = [{
                         label: "Email",
                         name: "email"
                     }, {
                         label: "First Name",
                         name: "first_name"
                     }, {
@@ -72906,26 +72954,26 @@
                         name: "role",
                         map: function(n) {
                             return t.userRoleTitle(e.user, e.user.project)
                         }
                     }, {
                         label: "Roles",
                         name: "roles",
-                        ui: (0, Kr.jsx)(Ig, {
+                        ui: (0, Kr.jsx)(Dg, {
                             user: e.user
                         }),
                         toggle: !0
                     }, {
                         label: "Institution",
                         name: "institution",
                         map: function(e) {
                             return t.institutionTitle(e)
                         },
                         subComponent: function(e) {
-                            return (0, Kr.jsx)(jg.PrincipalInvestigatorLine, {
+                            return (0, Kr.jsx)(wg.PrincipalInvestigatorLine, {
                                 institution: e
                             })
                         }
                     }, {
                         label: "Status",
                         name: "status",
                         map: function(e) {
@@ -72945,22 +72993,22 @@
                         }
                     }, {
                         label: "UUID",
                         name: "uuid"
                     }];
                 return At.IsFoursightFourfront(ta()) && (n = n.filter((function(e) {
                     return "institution" !== e.name && "project" !== e.name && "roles" !== e.name && "role" !== e.name
-                }))), (0, Kr.jsx)(xg, {
+                }))), (0, Kr.jsx)(Ng, {
                     keys: n,
                     value: e.user,
                     separators: !0
                 })
             },
-            Ig = function(e) {
-                var t = Mg();
+            Dg = function(e) {
+                var t = bg();
                 return (0, Kr.jsx)("div", {
                     className: "box lighten",
                     style: {
                         marginTop: "2pt",
                         marginBottom: "2pt"
                     },
                     children: (0, Kr.jsx)("table", {
@@ -73023,15 +73071,15 @@
                                     })]
                                 }, e.project)
                             }))]
                         })
                     })
                 })
             },
-            Dg = function(e) {
+            Sg = function(e) {
                 var n, r, o, i = pe().email,
                     s = a((0, t.useState)(!1), 2),
                     u = s[0],
                     l = s[1],
                     c = fe();
                 var d = Xi({
                     url: "/users/".concat(i),
@@ -73147,25 +73195,25 @@
                                             float: "right",
                                             fontSize: "small",
                                             marginTop: "-1pt",
                                             marginRight: "2pt"
                                         },
                                         children: "Edit"
                                     })]
-                                }), u ? (0, Kr.jsx)(wg, {
+                                }), u ? (0, Kr.jsx)(xg, {
                                     email: e.email
-                                }) : (0, Kr.jsx)(Ng, {
+                                }) : (0, Kr.jsx)(Ig, {
                                     user: e
                                 })]
                             }, e.uuid)
                         }))]
                     })
                 })
             },
-            Sg = function(e) {
+            Lg = function(e) {
                 var n = Xi(e.url, {
                         nofetch: !0,
                         cache: !0
                     }),
                     r = a((0, t.useState)(e.selected), 2),
                     o = r[0],
                     i = r[1];
@@ -73198,15 +73246,15 @@
                             }, e.id) : null
                         }))]
                     }), e.subComponent && (0, Kr.jsx)(Kr.Fragment, {
                         children: e.subComponent(o)
                     })]
                 })
             },
-            Lg = function(e) {
+            kg = function(e) {
                 var n = e.inputs,
                     r = (e.setInputs, e.title, e.loading),
                     o = e.onCreate,
                     i = e.onUpdate,
                     u = e.onDelete,
                     l = e.onCancel,
                     c = e.onRefresh,
@@ -73458,15 +73506,15 @@
                                                         }), (0, Kr.jsx)("option", {
                                                             value: !0,
                                                             children: "True"
                                                         })]
                                                     })
                                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                                     children: "select" === e.type ? (0, Kr.jsx)(Kr.Fragment, {
-                                                        children: (0, Kr.jsx)(Sg, {
+                                                        children: (0, Kr.jsx)(Lg, {
                                                             id: e.name,
                                                             url: e.url,
                                                             required: e.required,
                                                             selected: z(e),
                                                             onChange: T,
                                                             disabled: F() || e.readonly,
                                                             setLoadingCount: S,
@@ -73642,28 +73690,28 @@
                                     })]
                                 })
                             })
                         })
                     })
                 })
             },
-            kg = function() {
+            Cg = function() {
                 var e = Xi(zt.Url("/users"), {
                         method: "POST",
                         nofetch: !0
                     }),
-                    n = a(jg.useUserInputs(), 2),
+                    n = a(wg.useUserInputs(), 2),
                     r = n[0],
                     o = (n[1], fe());
                 return (0, t.useEffect)((function() {
                     var e = r.find((function(e) {
                         return "institution" === e.name
                     }));
                     e && (e.subComponent = function(e) {
-                        return (0, Kr.jsx)(jg.PrincipalInvestigatorLine, {
+                        return (0, Kr.jsx)(wg.PrincipalInvestigatorLine, {
                             institution: e
                         })
                     })
                 }), []), (0, Kr.jsx)("center", {
                     children: (0, Kr.jsx)("table", {
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
@@ -73690,15 +73738,15 @@
                                                 children: "List"
                                             })
                                         })
                                     })]
                                 })
                             }), (0, Kr.jsx)("tr", {
                                 children: (0, Kr.jsx)("td", {
-                                    children: (0, Kr.jsx)(Lg, {
+                                    children: (0, Kr.jsx)(kg, {
                                         title: "Edit User",
                                         inputs: r,
                                         onCreate: function(t) {
                                             t.admin ? (delete t.admin, t = Ye(Ye({}, t), {}, {
                                                 groups: ["admin"]
                                             })) : (delete t.admin, t = Ye(Ye({}, t), {}, {
                                                 groups: []
@@ -73718,23 +73766,23 @@
                                     })
                                 })
                             })]
                         })
                     })
                 })
             },
-            Cg = function() {
+            Eg = function() {
                 var e = pe().uuid,
-                    n = a(jg.useUserInputs(), 2),
+                    n = a(wg.useUserInputs(), 2),
                     r = n[0],
                     o = n[1],
                     i = a((0, t.useState)(!1), 2),
                     l = i[0],
                     c = i[1],
-                    d = a(ya(), 1)[0],
+                    d = a(ma(), 1)[0],
                     f = Xi({
                         url: "/users/".concat(e),
                         nofetch: !0,
                         onData: function(e) {
                             o((function(t) {
                                 var n, r = s(t);
                                 try {
@@ -73752,27 +73800,27 @@
                                 return u(t)
                             }))
                         },
                         onError: function(e) {
                             404 === e.status && c(!0)
                         }
                     }),
-                    p = Mg(),
+                    p = bg(),
                     h = fe();
 
                 function g() {
                     h(kr.Path("/users/".concat(e)))
                 }
                 return (0, t.useEffect)((function() {
                     f.fetch();
                     var e = r.find((function(e) {
                         return "institution" === e.name
                     }));
                     e && (e.subComponent = function(e) {
-                        return (0, Kr.jsx)(jg.PrincipalInvestigatorLine, {
+                        return (0, Kr.jsx)(wg.PrincipalInvestigatorLine, {
                             institution: e
                         })
                     })
                 }), [e]), (0, Kr.jsx)("center", {
                     children: (0, Kr.jsx)("table", {
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
@@ -73813,15 +73861,15 @@
                                             children: ["The specified user was not found: ", e, " ", (0, Kr.jsx)("p", {}), (0, Kr.jsx)("button", {
                                                 className: "button cancel",
                                                 onClick: g,
                                                 children: "Cancel"
                                             })]
                                         })
                                     }) : (0, Kr.jsx)(Kr.Fragment, {
-                                        children: (0, Kr.jsx)(Lg, {
+                                        children: (0, Kr.jsx)(kg, {
                                             title: "Edit User",
                                             inputs: r,
                                             setInputs: o,
                                             onUpdate: function(t) {
                                                 var n, r = (null === (n = f.get("groups")) || void 0 === n ? void 0 : n.filter((function(e) {
                                                     return "admin" !== e
                                                 }))) || [];
@@ -73856,15 +73904,15 @@
                                     })
                                 })
                             })]
                         })
                     })
                 })
             },
-            Eg = function(e) {
+            _g = function(e) {
                 var n, r = e.columns,
                     o = e.data,
                     i = e.update,
                     s = e.initialSort,
                     u = e.children,
                     l = a(Re(), 2),
                     c = l[0],
@@ -73945,15 +73993,15 @@
                         border: "0",
                         children: (0, Kr.jsx)("tbody", {
                             children: (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: {
                                         width: "90%"
                                     },
-                                    children: (0, Kr.jsx)(es, {
+                                    children: (0, Kr.jsx)(ts, {
                                         pages: _,
                                         page: k,
                                         onChange: function(e) {
                                             var t = e.selected;
                                             m(t * p)
                                         },
                                         refresh: R,
@@ -74024,15 +74072,15 @@
                             marginTop: "4pt",
                             paddingTop: "8pt"
                         },
                         children: (0, Kr.jsxs)("table", {
                             style: {
                                 width: "100%"
                             },
-                            children: [(0, Kr.jsx)(pa, {
+                            children: [(0, Kr.jsx)(ha, {
                                 columns: r,
                                 sort: M,
                                 list: null === o || void 0 === o || null === (n = o.data) || void 0 === n ? void 0 : n.list,
                                 update: function(e, t) {
                                     b("".concat(e, ".").concat(t))
                                 },
                                 bottomline: !0,
@@ -74044,27 +74092,27 @@
                             }), (0, Kr.jsx)("tbody", {
                                 children: u
                             })]
                         })
                     })]
                 })
             },
-            _g = function() {
+            Tg = function() {
                 var e = pe().environ,
                     n = a(Re(), 2),
                     r = n[0],
                     o = n[1],
                     i = Xi(),
                     s = a((0, t.useState)(r.get("search") || ""), 2),
                     u = s[0],
                     l = s[1],
                     c = a((0, t.useState)(it.HasValue(u)), 2),
                     d = c[0],
                     f = c[1],
-                    p = Mg();
+                    p = bg();
 
                 function h(t) {
                     var n = t.limit,
                         o = t.offset,
                         a = t.sort,
                         s = t.search,
                         u = t.onDone;
@@ -74191,15 +74239,15 @@
                                 style: {
                                     height: "1px",
                                     background: Ft.GetForegroundColor(),
                                     marginTop: "2pt",
                                     marginBottom: "4pt"
                                 }
                             })]
-                        }), (0, Kr.jsx)(Eg, {
+                        }), (0, Kr.jsx)(_g, {
                             columns: [{
                                 label: ""
                             }, {
                                 label: "User",
                                 key: "email"
                             }, {
                                 label: "Groups",
@@ -74328,30 +74376,30 @@
                                     })]
                                 }, e.uuid)
                             }))
                         })]
                     })
                 })
             },
-            Tg = function() {
+            Ag = function() {
                 var e = ta();
 
                 function t() {
                     return "/api/react/".concat(At.PreferredName(At.Default(e)), "/login")
                 }
                 return (0, Kr.jsx)(Ae, {
-                    children: (0, Kr.jsxs)(Ms, {
-                        children: [(0, Kr.jsx)(vs, {}), (0, Kr.jsx)("div", {
+                    children: (0, Kr.jsxs)(bs, {
+                        children: [(0, Kr.jsx)(Ms, {}), (0, Kr.jsx)("div", {
                             style: {
                                 margin: "14pt"
                             },
                             children: (0, Kr.jsxs)(De, {
                                 children: [(0, Kr.jsx)(Ne, {
                                     path: "/api/react/cognito/callback",
-                                    element: (0, Kr.jsx)(zh, {})
+                                    element: (0, Kr.jsx)(Uh, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/",
                                     element: (0, Kr.jsx)(xe, {
                                         to: t()
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api",
@@ -74367,136 +74415,136 @@
                                     path: "/api/react/:environ",
                                     element: (0, Kr.jsx)(xe, {
                                         to: t()
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/accounts",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(sa, {})
+                                        children: (0, Kr.jsx)(ua, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/env",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(ss, {})
+                                        children: (0, Kr.jsx)(us, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/env",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(ss, {})
+                                        children: (0, Kr.jsx)(us, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/login",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(Ph, {})
+                                        children: (0, Kr.jsx)(Rh, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/checks",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Ka, {})
+                                        children: (0, Kr.jsx)(Xa, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/checks/:check/history",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(is, {})
+                                        children: (0, Kr.jsx)(as, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/home",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(bs, {})
+                                        children: (0, Kr.jsx)(js, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/info",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(xs, {})
+                                        children: (0, Kr.jsx)(Ns, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(_g, {})
+                                        children: (0, Kr.jsx)(Tg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/:email",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Dg, {})
+                                        children: (0, Kr.jsx)(Sg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/edit/:uuid",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Cg, {})
+                                        children: (0, Kr.jsx)(Eg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/create",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(kg, {})
+                                        children: (0, Kr.jsx)(Cg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/gac/:environCompare",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Rh, {})
+                                        children: (0, Kr.jsx)(Bh, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/aws/s3",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(ha, {})
+                                        children: (0, Kr.jsx)(ga, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/aws/infrastructure",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(pg, {})
+                                        children: (0, Kr.jsx)(hg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/certificates",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(mg, {})
+                                        children: (0, Kr.jsx)(vg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/portal_access_key",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(vg, {})
+                                        children: (0, Kr.jsx)(Mg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/apicache",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(fa, {})
+                                        children: (0, Kr.jsx)(pa, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/forbidden",
-                                    element: (0, Kr.jsx)(ls, {})
+                                    element: (0, Kr.jsx)(cs, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/error",
                                     element: (0, Kr.jsx)(_i, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/error",
                                     element: (0, Kr.jsx)(_i, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/redirect",
-                                    element: (0, Kr.jsx)(gg, {})
+                                    element: (0, Kr.jsx)(yg, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "*",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(hg, {})
+                                        children: (0, Kr.jsx)(gg, {})
                                     })
                                 })]
                             })
-                        }), (0, Kr.jsx)(us, {})]
+                        }), (0, Kr.jsx)(ls, {})]
                     })
                 })
             },
-            Ag = r.createRoot(document.getElementById("root"));
-        "1" === bt.Get("test_mode_strict_mode") ? Ag.render((0, Kr.jsx)(t.StrictMode, {
-            children: (0, Kr.jsx)(Tg, {})
-        })) : Ag.render((0, Kr.jsx)("table", {
+            Og = r.createRoot(document.getElementById("root"));
+        "1" === bt.Get("test_mode_strict_mode") ? Og.render((0, Kr.jsx)(t.StrictMode, {
+            children: (0, Kr.jsx)(Ag, {})
+        })) : Og.render((0, Kr.jsx)("table", {
             style: {
                 width: "100%"
             },
             cellPadding: "0",
             cellSpacing: "0",
             children: (0, Kr.jsx)("tbody", {
                 children: (0, Kr.jsx)("tr", {
                     children: (0, Kr.jsx)("td", {
-                        children: (0, Kr.jsx)(Tg, {})
+                        children: (0, Kr.jsx)(Ag, {})
                     })
                 })
             })
         }))
     }()
 })();
```

### Comparing `foursight_core-4.1.1.1b1/foursight_core/route_prefixes.py` & `foursight_core-4.1.2/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/routes.py` & `foursight_core-4.1.2/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/run_result.py` & `foursight_core-4.1.2/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/s3_connection.py` & `foursight_core-4.1.2/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/schedule_decorator.py` & `foursight_core-4.1.2/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.2/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.2/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/sqs_utils.py` & `foursight_core-4.1.2/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/stage.py` & `foursight_core-4.1.2/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/base.html` & `foursight_core-4.1.2/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/header.html` & `foursight_core-4.1.2/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/history.html` & `foursight_core-4.1.2/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/info.html` & `foursight_core-4.1.2/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/unused.html` & `foursight_core-4.1.2/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/user.html` & `foursight_core-4.1.2/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/users.html` & `foursight_core-4.1.2/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/view_checks.html` & `foursight_core-4.1.2/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/foursight_core/templates/view_groups.html` & `foursight_core-4.1.2/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.1.1b1/pyproject.toml` & `foursight_core-4.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.1.1b1"
+version = "4.1.2"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.1.1.1b1/PKG-INFO` & `foursight_core-4.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.1.1b1
+Version: 4.1.2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

