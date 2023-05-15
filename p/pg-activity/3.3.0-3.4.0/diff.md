# Comparing `tmp/pg_activity-3.3.0.tar.gz` & `tmp/pg-activity-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_activity-3.3.0.tar", last modified: Wed Mar 22 07:50:37 2023, max compression
+gzip compressed data, was "pg-activity-3.4.0.tar", last modified: Mon May 15 09:04:31 2023, max compression
```

## Comparing `pg_activity-3.3.0.tar` & `pg-activity-3.4.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.799165 pg_activity-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 07:50:25.000000 pg_activity-3.3.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-22 07:50:25.000000 pg_activity-3.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-22 07:50:25.000000 pg_activity-3.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-22 07:50:25.000000 pg_activity-3.3.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-22 07:50:25.000000 pg_activity-3.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-03-22 07:50:25.000000 pg_activity-3.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-22 07:50:25.000000 pg_activity-3.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-22 07:50:25.000000 pg_activity-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-03-22 07:50:37.799165 pg_activity-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-03-22 07:50:25.000000 pg_activity-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-22 07:50:25.000000 pg_activity-3.3.0/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.783165 pg_activity-3.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.787165 pg_activity-3.3.0/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-03-22 07:50:25.000000 pg_activity-3.3.0/docs/imgs/logo-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-22 07:50:25.000000 pg_activity-3.3.0/docs/imgs/logo-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-03-22 07:50:25.000000 pg_activity-3.3.0/docs/imgs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   337072 2023-03-22 07:50:25.000000 pg_activity-3.3.0/docs/imgs/screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.787165 pg_activity-3.3.0/docs/man/
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-03-22 07:50:25.000000 pg_activity-3.3.0/docs/man/build-man.sh
--rw-r--r--   0 runner    (1001) docker     (123)    27465 2023-03-22 07:50:25.000000 pg_activity-3.3.0/docs/man/pg_activity.1
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-03-22 07:50:25.000000 pg_activity-3.3.0/docs/man/pg_activity.pod
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-22 07:50:25.000000 pg_activity-3.3.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.787165 pg_activity-3.3.0/pg_activity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-03-22 07:50:37.000000 pg_activity-3.3.0/pg_activity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-22 07:50:37.000000 pg_activity-3.3.0/pg_activity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 07:50:37.000000 pg_activity-3.3.0/pg_activity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 07:50:37.000000 pg_activity-3.3.0/pg_activity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 07:50:37.000000 pg_activity-3.3.0/pg_activity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-22 07:50:37.000000 pg_activity-3.3.0/pg_activity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 07:50:37.000000 pg_activity-3.3.0/pg_activity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.791165 pg_activity-3.3.0/pgactivity/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/activities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11032 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/pg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.799165 pg_activity-3.3.0/pgactivity/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/disable_log_min_duration_sample.sql
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/disable_log_min_duration_statement.sql
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/do_pg_cancel_backend.sql
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/do_pg_terminate_backend.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_blocking_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_blocking_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_blocking_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_data_directory.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_pg_activity_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_100000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_110000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_130000.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_pga_inet_addresses.sql
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_replication_slots_post_140000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_server_info_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_server_info_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_server_info_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_server_info_post_090400.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_server_info_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_server_info_post_100000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_server_info_post_110000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_temporary_files_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_temporary_files_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_temporary_files_post_090500.sql
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_temporary_files_post_120000.sql
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_version.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_waiting_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_waiting_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_wal_receivers_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/get_wal_senders_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/is_superuser.sql
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/queries/reset_statement_timeout.sql
--rw-r--r--   0 runner    (1001) docker     (123)    32059 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pgactivity/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 07:50:25.000000 pg_activity-3.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 07:50:37.799165 pg_activity-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-22 07:50:25.000000 pg_activity-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.799165 pg_activity-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 07:50:37.799165 pg_activity-3.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    62356 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/data/local-processes-input.json
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/test_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/test_scroll.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    41092 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/test_ui.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    24000 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/test_views.txt
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tests/test_widgets.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-22 07:50:25.000000 pg_activity-3.3.0/tox.ini
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.022173 pg-activity-3.4.0/
+-rw-r--r--   0 denis     (1000) denis     (1000)       61 2023-02-01 11:56:00.000000 pg-activity-3.4.0/.codespellrc
+-rw-r--r--   0 denis     (1000) denis     (1000)       45 2021-02-01 14:14:21.000000 pg-activity-3.4.0/.coveragerc
+-rw-r--r--   0 denis     (1000) denis     (1000)      106 2021-02-01 14:14:21.000000 pg-activity-3.4.0/.editorconfig
+-rw-r--r--   0 denis     (1000) denis     (1000)      301 2022-11-28 15:05:59.000000 pg-activity-3.4.0/.flake8
+-rw-r--r--   0 denis     (1000) denis     (1000)     1346 2021-07-19 12:31:38.000000 pg-activity-3.4.0/AUTHORS.md
+-rw-r--r--   0 denis     (1000) denis     (1000)    13650 2023-05-15 08:58:50.000000 pg-activity-3.4.0/CHANGELOG.md
+-rw-r--r--   0 denis     (1000) denis     (1000)      942 2021-02-01 14:14:21.000000 pg-activity-3.4.0/LICENSE.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)      355 2023-04-11 07:41:54.000000 pg-activity-3.4.0/MANIFEST.in
+-rw-r--r--   0 denis     (1000) denis     (1000)    12315 2023-05-15 09:04:31.022173 pg-activity-3.4.0/PKG-INFO
+-rw-r--r--   0 denis     (1000) denis     (1000)    11059 2023-05-15 08:24:59.000000 pg-activity-3.4.0/README.md
+-rw-r--r--   0 denis     (1000) denis     (1000)     1830 2023-01-24 12:51:39.000000 pg-activity-3.4.0/RELEASE.md
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:30.978172 pg-activity-3.4.0/docs/
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:30.990172 pg-activity-3.4.0/docs/imgs/
+-rw-r--r--   0 denis     (1000) denis     (1000)    28659 2020-05-27 08:10:17.000000 pg-activity-3.4.0/docs/imgs/logo-horizontal.png
+-rw-r--r--   0 denis     (1000) denis     (1000)     5296 2020-05-27 08:10:17.000000 pg-activity-3.4.0/docs/imgs/logo-horizontal.svg
+-rw-r--r--   0 denis     (1000) denis     (1000)     4546 2020-05-27 08:10:17.000000 pg-activity-3.4.0/docs/imgs/logo.svg
+-rw-r--r--   0 denis     (1000) denis     (1000)   337072 2022-09-21 07:26:09.000000 pg-activity-3.4.0/docs/imgs/screenshot.png
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:30.990172 pg-activity-3.4.0/docs/man/
+-rwxr-xr-x   0 denis     (1000) denis     (1000)      194 2023-05-15 08:58:50.000000 pg-activity-3.4.0/docs/man/build-man.sh
+-rw-r--r--   0 denis     (1000) denis     (1000)    27465 2023-05-15 08:58:50.000000 pg-activity-3.4.0/docs/man/pg_activity.1
+-rw-r--r--   0 denis     (1000) denis     (1000)    13648 2023-03-10 09:40:53.000000 pg-activity-3.4.0/docs/man/pg_activity.pod
+-rw-r--r--   0 denis     (1000) denis     (1000)      244 2023-03-16 14:51:38.000000 pg-activity-3.4.0/mypy.ini
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:30.994172 pg-activity-3.4.0/pg_activity.egg-info/
+-rw-r--r--   0 denis     (1000) denis     (1000)    12315 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/PKG-INFO
+-rw-r--r--   0 denis     (1000) denis     (1000)     2789 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/SOURCES.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)        1 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/dependency_links.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)       52 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/entry_points.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)      345 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/requires.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)       35 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/top_level.txt
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.002172 pg-activity-3.4.0/pgactivity/
+-rw-r--r--   0 denis     (1000) denis     (1000)       22 2023-05-15 08:58:50.000000 pg-activity-3.4.0/pgactivity/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)       61 2021-07-19 12:31:38.000000 pg-activity-3.4.0/pgactivity/__main__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    11874 2023-04-24 08:53:46.000000 pg-activity-3.4.0/pgactivity/activities.py
+-rwxr-xr-x   0 denis     (1000) denis     (1000)    11203 2023-05-15 08:24:59.000000 pg-activity-3.4.0/pgactivity/cli.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     3081 2023-03-22 07:46:12.000000 pg-activity-3.4.0/pgactivity/colors.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      798 2023-04-20 08:45:15.000000 pg-activity-3.4.0/pgactivity/compat.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     8282 2023-05-15 08:24:59.000000 pg-activity-3.4.0/pgactivity/config.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    20141 2023-03-28 15:13:08.000000 pg-activity-3.4.0/pgactivity/data.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     3861 2023-04-24 10:05:47.000000 pg-activity-3.4.0/pgactivity/handlers.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     3782 2022-04-28 08:55:55.000000 pg-activity-3.4.0/pgactivity/keys.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     9933 2023-03-30 07:02:41.000000 pg-activity-3.4.0/pgactivity/pg.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.014172 pg-activity-3.4.0/pgactivity/queries/
+-rw-r--r--   0 denis     (1000) denis     (1000)      217 2021-03-08 15:28:57.000000 pg-activity-3.4.0/pgactivity/queries/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)       37 2021-07-19 12:31:38.000000 pg-activity-3.4.0/pgactivity/queries/disable_log_min_duration_sample.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)       40 2021-12-16 08:04:47.000000 pg-activity-3.4.0/pgactivity/queries/disable_log_min_duration_statement.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)      146 2021-12-16 08:04:48.000000 pg-activity-3.4.0/pgactivity/queries/do_pg_cancel_backend.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)      128 2021-12-16 08:04:49.000000 pg-activity-3.4.0/pgactivity/queries/do_pg_terminate_backend.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     4716 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_blocking_oldest.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     4527 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_blocking_post_090200.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     4455 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_blocking_post_090600.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)       52 2022-09-07 07:03:25.000000 pg-activity-3.4.0/pgactivity/queries/get_data_directory.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1317 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_oldest.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1063 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_090200.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1086 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_090600.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1130 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_100000.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1045 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_110000.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1040 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_130000.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)      131 2021-12-16 08:05:04.000000 pg-activity-3.4.0/pgactivity/queries/get_pga_inet_addresses.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)      144 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_replication_slots_post_140000.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     2508 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_oldest.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     2571 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090100.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     2516 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090200.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     2619 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090400.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     2626 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090600.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     2980 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_100000.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     3091 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_110000.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1331 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_temporary_files_oldest.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1373 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_090100.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1436 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_090500.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)      245 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_120000.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)       60 2021-12-16 08:05:06.000000 pg-activity-3.4.0/pgactivity/queries/get_version.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1429 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_waiting_oldest.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)     1205 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_waiting_post_090200.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)      130 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_wal_receivers_post_090600.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)      124 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_wal_senders_post_090100.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)       25 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/reset_statement_timeout.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)    30898 2023-05-15 08:24:59.000000 pg-activity-3.4.0/pgactivity/types.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    11181 2023-05-15 08:24:59.000000 pg-activity-3.4.0/pgactivity/ui.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     9806 2023-03-22 07:46:12.000000 pg-activity-3.4.0/pgactivity/utils.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    19014 2023-04-24 10:05:47.000000 pg-activity-3.4.0/pgactivity/views.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      919 2022-01-11 13:53:15.000000 pg-activity-3.4.0/pgactivity/widgets.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2259 2023-04-24 11:18:21.000000 pg-activity-3.4.0/pyproject.toml
+-rw-r--r--   0 denis     (1000) denis     (1000)       37 2021-03-18 15:43:32.000000 pg-activity-3.4.0/pytest.ini
+-rw-r--r--   0 denis     (1000) denis     (1000)       38 2023-05-15 09:04:31.022173 pg-activity-3.4.0/setup.cfg
+-rw-r--r--   0 denis     (1000) denis     (1000)       38 2023-04-20 09:37:05.000000 pg-activity-3.4.0/setup.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.018172 pg-activity-3.4.0/tests/
+-rw-r--r--   0 denis     (1000) denis     (1000)     3103 2023-03-22 07:46:12.000000 pg-activity-3.4.0/tests/conftest.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.018172 pg-activity-3.4.0/tests/data/
+-rw-r--r--   0 denis     (1000) denis     (1000)    62239 2023-04-03 06:51:35.000000 pg-activity-3.4.0/tests/data/local-processes-input.json
+-rw-r--r--   0 denis     (1000) denis     (1000)     4081 2023-03-22 07:46:12.000000 pg-activity-3.4.0/tests/test_activities.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1712 2023-05-15 08:24:59.000000 pg-activity-3.4.0/tests/test_config.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     6413 2023-03-22 07:46:12.000000 pg-activity-3.4.0/tests/test_data.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     3108 2023-04-03 06:51:35.000000 pg-activity-3.4.0/tests/test_scroll.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)      165 2023-04-24 10:05:47.000000 pg-activity-3.4.0/tests/test_types.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    40923 2023-05-15 08:24:59.000000 pg-activity-3.4.0/tests/test_ui.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)     1817 2023-04-24 10:05:47.000000 pg-activity-3.4.0/tests/test_views.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    24193 2023-04-24 10:05:47.000000 pg-activity-3.4.0/tests/test_views.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)      796 2021-03-08 15:28:57.000000 pg-activity-3.4.0/tests/test_widgets.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)      717 2023-04-24 11:18:21.000000 pg-activity-3.4.0/tox.ini
```

### Comparing `pg_activity-3.3.0/AUTHORS.md` & `pg-activity-3.4.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/CHANGELOG.md` & `pg-activity-3.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,31 @@
 # Change log
 
+## pg\_activity 3.4.0 - 2023-05-15
+
+### Added
+
+* Improve rendering of the `client` column by possibly abbreviating IP
+  addresses.
+* Add support for configuring pg\_activity from a configuration file in INI
+  format and installed at `${XDG_CONFIG_HOME:~/.config}/pg_activity.conf` or
+  `/etc/pg_activity.conf`.
+* Determine which columns to hide from reading the configuration file (`hidden =
+  yes|no` option).
+* Determine columns width from the configuration file (`width = <positive
+  integer>` option).
+
+### Fixed
+
+* Fix a crash when trying to reconnect.
+
+### Misc.
+
+* Move packaging metadata to `pyproject.toml`.
+
 ## pg\_activity 3.3.0 - 2023-03-22
 
 ### Fixed
 
 * Replace the previous header column separator (`⋅`) by a comma to improve user
   experience in situations where that character did not render well (#356,
   #230).
```

### Comparing `pg_activity-3.3.0/LICENSE.txt` & `pg-activity-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/PKG-INFO` & `pg-activity-3.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,58 @@
-Metadata-Version: 2.1
-Name: pg_activity
-Version: 3.3.0
-Summary: Command line tool for PostgreSQL server activity monitoring.
-Home-page: https://github.com/dalibo/pg_activity
-Author: Dalibo
-Author-email: contact@dalibo.com
-License: PostgreSQL
-Project-URL: Bug Tracker, https://github.com/dalibo/pg_activity/issues/
-Project-URL: Changelog, https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
-Project-URL: Source code, https://github.com/dalibo/pg_activity/
-Keywords: postgresql activity monitoring cli sql top
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Console :: Curses
-Classifier: License :: OSI Approved :: PostgreSQL License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Database
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: psycopg2
-Provides-Extra: psycopg
-Provides-Extra: testing
-License-File: LICENSE.txt
-License-File: AUTHORS.md
-
 ![pg_activity](https://github.com/dalibo/pg_activity/raw/master/docs/imgs/logo-horizontal.png)
 
 Command line tool for PostgreSQL server activity monitoring.
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/pg_activity.svg)](https://pypi.python.org/pypi/pg_activity)
 [![Lint](https://github.com/dalibo/pg_activity/actions/workflows/lint.yml/badge.svg)](https://github.com/dalibo/pg_activity/actions/workflows/lint.yml)
 [![Tests](https://github.com/dalibo/pg_activity/actions/workflows/tests.yml/badge.svg)](https://github.com/dalibo/pg_activity/actions/workflows/tests.yml)
 
 ![pg_activity screenshot](https://raw.github.com/dalibo/pg_activity/master/docs/imgs/screenshot.png)
 
-Installation from packages (recommended)
-----------------------------------------
+# Installation
 
-pg\_activity is available in many Linux distributions; the PostgreSQL Global
-Development Group (PGDG) also provides packages for RPM-based
-(https://yum.postgresql.org/) and Debian-based distributions
-(https://wiki.postgresql.org/wiki/Apt):
+## From distribution packages
 
-    $ sudo yum install pg_activity
+The simplest way to install pg\_activity is through the package manager of your
+Linux distribution, if it ships with a package. E.g., on Debian-based
+distributions (e.g. Debian, Ubuntu, Mint...):
 
     $ sudo apt install pg-activity
 
-Using distribution packages is the recommended way to install pg\_activity.
+(on Debian bullseye, the current stable version, a backport is available: `apt
+install pg-activity/bullseye-backports`).
+
+The PostgreSQL Global Development Group (PGDG) also provides packages for
+RPM-based (https://yum.postgresql.org/) and Debian-based distributions
+(https://wiki.postgresql.org/wiki/Apt).
+
+**Note:** distribution packages may not be up to date with the latest
+pg\_activity releases. Before submitting a bug report here:
+-   check the package version, compare that to our latest release and then
+    review the [change log][changelog] to see if the bug has been fixed;
+-   if the issue is about packaging, e.g. missing dependencies, reach out
+    the package maintainer (or PGDG) first.
 
-Installation from pip
----------------------
+## From PyPI
 
-Alternatively, pg\_activity can be installed using pip on Python 3.7 or later
-along with psycopg:
+pg\_activity can be installed using pip on Python 3.7 or later along with
+psycopg:
 
     $ python3 -m pip install "pg_activity[psycopg]"
 
+Alternatively, [pipx](https://pypi.org/project/pipx/) can be used to install
+and run pg\_activity in an isolated environment:
+
+    $ pipx install "pg_activity[psycopg]"
+
 In case your `$PATH` does not already contain it, the full path is:
 
     $ ~/.local/bin/pg_activity
 
-Installation from the git repository
-------------------------------------
+## From source, using git
 
 This is only necessary to test development versions. First, clone the repository:
 
     $ git clone https://github.com/dalibo/pg_activity.git
 
 Change the branch if necessary. Then create a dedicated environment,
 and install pg\_activity with the psycopg database driver:
@@ -78,31 +64,29 @@
     (.venv) $ pg_activity
 
 To quit this env and destroy it:
 
     $ deactivate
     $ rm -r .venv
 
-Usage
------
+# Usage
 
 `pg_activity` works locally or remotely. In local execution context, to obtain
 sufficient rights to display system information, the system user running
 `pg_activity` must be the same user running postgresql server (`postgres` by
 default), or have more rights like `root`. The PostgreSQL user used to connect
 to the database must be super-user in order to get as much data as possible.
 Otherwise, `pg_activity` can fall back to a degraded mode where some data like
 system information or temporary file data are not displayed.
 
 ex:
 
     sudo -u postgres pg_activity -U postgres
 
-Options
--------
+## Options
 
     pg_activity [options] [connection string]
 
     Options:
       --blocksize BLOCKSIZE
                             Filesystem blocksize (default: 4096).
       --rds                 Enable support for AWS RDS (implies --no-tempfiles and filters out the rdsadmin database from space calculation).
@@ -150,25 +134,40 @@
       --hide-queries-in-logs
                             Disable log_min_duration_statements and log_min_duration_sample for pg_activity.
       --no-inst-info        Display instance information in header.
       --no-sys-info         Display system information in header.
       --no-proc-info        Display workers process information in header.
       --refresh REFRESH     Refresh rate. Values: 0.5, 1, 2, 3, 4, 5 (default: 2).
 
-Notes
------
+## Configuration
+
+`pg_activity` may be configured through configuration file, in [INI format][],
+read from `${XDG_CONFIG_HOME:~/.config}/pg_activity.conf` or
+`/etc/pg_activity.conf` in that order. Command-line options may override
+configuration file settings.
+This is used to control how columns in the processes table are rendered, e.g.:
+```ini
+[client]
+hidden = yes
+
+[database]
+width = 9
+```
+
+[INI format]: https://docs.python.org/3/library/configparser.html#supported-ini-file-structure
+
+## Notes
 
 Length of SQL query text that `pg_activity` reports relies on PostgreSQL
 parameter `track_activity_query_size`. Default value is `1024` (expressed in
 bytes). If your SQL query text look truncated, you should increase
 `track_activity_query_size`.
 
 
-Interactives commands
----------------------
+## Interactives commands
 
 | Key       | Action                                                           |
 |-----------|------------------------------------------------------------------|
 | `r`       | Sort by READ/s, descending                                       |
 | `w`       | Sort by WRITE/s, descending                                      |
 | `c`       | Sort by CPU%, descending                                         |
 | `m`       | Sort by MEM%, descending                                         |
@@ -187,29 +186,27 @@
 | `h`       | Help page                                                        |
 | `R`       | Refresh                                                          |
 | `D`       | Refresh Database Size (including when --no-dbzise option applied)|
 | `s`       | Display system information in header                             |
 | `i`       | Display general instance information in header                   |
 | `o`       | Display worker information in header                             |
 
-Navigation mode
----------------
+## Navigation mode
 
 | Key        | Action                                        |
 |------------|-----------------------------------------------|
 | `UP`/`k`   | Move up the cursor                            |
 | `DOWN`/`j` | Move down the cursor                          |
 | `K`        | Terminate the current backend/tagged backends |
 | `C`        | Cancel the current backend/tagged backends    |
 | `Space`    | Tag or untag the process                      |
 | `q`        | Quit                                          |
 | `Other`    | Back to activity                              |
 
-FAQ
----
+## FAQ
 
 **I can't see my queries only TPS is shown**
 
 `pg_activity` scans the view `pg_stat_activity` with a user defined refresh
 time comprised between 0.5 and 5 seconds. It can be modified in the interface
 with the `+` and `-` keys. Any query executed between two scans won't be
 displayed.
@@ -241,11 +238,12 @@
 You can pass the password for the database connection in a password file.
 Information can also be given via PostgreSQL's environment variables
 (PGPASSFILE or PGPASSWORD) or via the connection string parameters.
 
 The password file is preferred since it's more secure (security is deferred to
 the OS). Please avoid password in connection strings at all cost.
 
-Change log
-----------
+# Change log
+
+See [CHANGELOG.md][changelog].
 
-See [CHANGELOG.md](https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md).
+[changelog]: https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
```

### Comparing `pg_activity-3.3.0/RELEASE.md` & `pg-activity-3.4.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/docs/imgs/logo-horizontal.png` & `pg-activity-3.4.0/docs/imgs/logo-horizontal.png`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/docs/imgs/logo-horizontal.svg` & `pg-activity-3.4.0/docs/imgs/logo-horizontal.svg`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/docs/imgs/logo.svg` & `pg-activity-3.4.0/docs/imgs/logo.svg`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/docs/imgs/screenshot.png` & `pg-activity-3.4.0/docs/imgs/screenshot.png`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/docs/man/pg_activity.1` & `pg-activity-3.4.0/docs/man/pg_activity.1`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 .    ds ae ae
 .    ds Ae AE
 .\}
 .rm #[ #] #H #V #F C
 .\" ========================================================================
 .\"
 .IX Title "PG_ACTIVITY 1"
-.TH PG_ACTIVITY 1 "2023-03-22" "pg_activity 3.3.0" "Command line tool for PostgreSQL server activity monitoring."
+.TH PG_ACTIVITY 1 "2023-05-15" "pg_activity 3.4.0" "Command line tool for PostgreSQL server activity monitoring."
 .\" For nroff, turn off justification.  Always turn off hyphenation; it makes
 .\" way too many mistakes in technical documents.
 .if n .ad l
 .nh
 .SH "NAME"
 pg_activity \- Realtime PostgreSQL database server monitoring tool
 .SH "SYNOPSIS"
```

### Comparing `pg_activity-3.3.0/docs/man/pg_activity.pod` & `pg-activity-3.4.0/docs/man/pg_activity.pod`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pg_activity.egg-info/PKG-INFO` & `pg-activity-3.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,86 @@
 Metadata-Version: 2.1
 Name: pg-activity
-Version: 3.3.0
+Version: 3.4.0
 Summary: Command line tool for PostgreSQL server activity monitoring.
-Home-page: https://github.com/dalibo/pg_activity
-Author: Dalibo
-Author-email: contact@dalibo.com
+Author-email: Julien Tachoires <julmon@gmail.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>, Denis Laxalde <denis.laxalde@dalibo.com>, Dalibo <contact@dalibo.com>
+Maintainer-email: Denis Laxalde <denis.laxalde@dalibo.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>
 License: PostgreSQL
 Project-URL: Bug Tracker, https://github.com/dalibo/pg_activity/issues/
 Project-URL: Changelog, https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
+Project-URL: Homepage, https://github.com/dalibo/pg_activity
 Project-URL: Source code, https://github.com/dalibo/pg_activity/
-Keywords: postgresql activity monitoring cli sql top
+Keywords: activity,cli,monitoring,postgresql,sql,top
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: License :: OSI Approved :: PostgreSQL License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: psycopg2
+Provides-Extra: typing
 Provides-Extra: psycopg
+Provides-Extra: psycopg2
 Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.md
 
 ![pg_activity](https://github.com/dalibo/pg_activity/raw/master/docs/imgs/logo-horizontal.png)
 
 Command line tool for PostgreSQL server activity monitoring.
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/pg_activity.svg)](https://pypi.python.org/pypi/pg_activity)
 [![Lint](https://github.com/dalibo/pg_activity/actions/workflows/lint.yml/badge.svg)](https://github.com/dalibo/pg_activity/actions/workflows/lint.yml)
 [![Tests](https://github.com/dalibo/pg_activity/actions/workflows/tests.yml/badge.svg)](https://github.com/dalibo/pg_activity/actions/workflows/tests.yml)
 
 ![pg_activity screenshot](https://raw.github.com/dalibo/pg_activity/master/docs/imgs/screenshot.png)
 
-Installation from packages (recommended)
-----------------------------------------
+# Installation
 
-pg\_activity is available in many Linux distributions; the PostgreSQL Global
-Development Group (PGDG) also provides packages for RPM-based
-(https://yum.postgresql.org/) and Debian-based distributions
-(https://wiki.postgresql.org/wiki/Apt):
+## From distribution packages
 
-    $ sudo yum install pg_activity
+The simplest way to install pg\_activity is through the package manager of your
+Linux distribution, if it ships with a package. E.g., on Debian-based
+distributions (e.g. Debian, Ubuntu, Mint...):
 
     $ sudo apt install pg-activity
 
-Using distribution packages is the recommended way to install pg\_activity.
+(on Debian bullseye, the current stable version, a backport is available: `apt
+install pg-activity/bullseye-backports`).
+
+The PostgreSQL Global Development Group (PGDG) also provides packages for
+RPM-based (https://yum.postgresql.org/) and Debian-based distributions
+(https://wiki.postgresql.org/wiki/Apt).
+
+**Note:** distribution packages may not be up to date with the latest
+pg\_activity releases. Before submitting a bug report here:
+-   check the package version, compare that to our latest release and then
+    review the [change log][changelog] to see if the bug has been fixed;
+-   if the issue is about packaging, e.g. missing dependencies, reach out
+    the package maintainer (or PGDG) first.
 
-Installation from pip
----------------------
+## From PyPI
 
-Alternatively, pg\_activity can be installed using pip on Python 3.7 or later
-along with psycopg:
+pg\_activity can be installed using pip on Python 3.7 or later along with
+psycopg:
 
     $ python3 -m pip install "pg_activity[psycopg]"
 
+Alternatively, [pipx](https://pypi.org/project/pipx/) can be used to install
+and run pg\_activity in an isolated environment:
+
+    $ pipx install "pg_activity[psycopg]"
+
 In case your `$PATH` does not already contain it, the full path is:
 
     $ ~/.local/bin/pg_activity
 
-Installation from the git repository
-------------------------------------
+## From source, using git
 
 This is only necessary to test development versions. First, clone the repository:
 
     $ git clone https://github.com/dalibo/pg_activity.git
 
 Change the branch if necessary. Then create a dedicated environment,
 and install pg\_activity with the psycopg database driver:
@@ -78,31 +92,29 @@
     (.venv) $ pg_activity
 
 To quit this env and destroy it:
 
     $ deactivate
     $ rm -r .venv
 
-Usage
------
+# Usage
 
 `pg_activity` works locally or remotely. In local execution context, to obtain
 sufficient rights to display system information, the system user running
 `pg_activity` must be the same user running postgresql server (`postgres` by
 default), or have more rights like `root`. The PostgreSQL user used to connect
 to the database must be super-user in order to get as much data as possible.
 Otherwise, `pg_activity` can fall back to a degraded mode where some data like
 system information or temporary file data are not displayed.
 
 ex:
 
     sudo -u postgres pg_activity -U postgres
 
-Options
--------
+## Options
 
     pg_activity [options] [connection string]
 
     Options:
       --blocksize BLOCKSIZE
                             Filesystem blocksize (default: 4096).
       --rds                 Enable support for AWS RDS (implies --no-tempfiles and filters out the rdsadmin database from space calculation).
@@ -150,25 +162,40 @@
       --hide-queries-in-logs
                             Disable log_min_duration_statements and log_min_duration_sample for pg_activity.
       --no-inst-info        Display instance information in header.
       --no-sys-info         Display system information in header.
       --no-proc-info        Display workers process information in header.
       --refresh REFRESH     Refresh rate. Values: 0.5, 1, 2, 3, 4, 5 (default: 2).
 
-Notes
------
+## Configuration
+
+`pg_activity` may be configured through configuration file, in [INI format][],
+read from `${XDG_CONFIG_HOME:~/.config}/pg_activity.conf` or
+`/etc/pg_activity.conf` in that order. Command-line options may override
+configuration file settings.
+This is used to control how columns in the processes table are rendered, e.g.:
+```ini
+[client]
+hidden = yes
+
+[database]
+width = 9
+```
+
+[INI format]: https://docs.python.org/3/library/configparser.html#supported-ini-file-structure
+
+## Notes
 
 Length of SQL query text that `pg_activity` reports relies on PostgreSQL
 parameter `track_activity_query_size`. Default value is `1024` (expressed in
 bytes). If your SQL query text look truncated, you should increase
 `track_activity_query_size`.
 
 
-Interactives commands
----------------------
+## Interactives commands
 
 | Key       | Action                                                           |
 |-----------|------------------------------------------------------------------|
 | `r`       | Sort by READ/s, descending                                       |
 | `w`       | Sort by WRITE/s, descending                                      |
 | `c`       | Sort by CPU%, descending                                         |
 | `m`       | Sort by MEM%, descending                                         |
@@ -187,29 +214,27 @@
 | `h`       | Help page                                                        |
 | `R`       | Refresh                                                          |
 | `D`       | Refresh Database Size (including when --no-dbzise option applied)|
 | `s`       | Display system information in header                             |
 | `i`       | Display general instance information in header                   |
 | `o`       | Display worker information in header                             |
 
-Navigation mode
----------------
+## Navigation mode
 
 | Key        | Action                                        |
 |------------|-----------------------------------------------|
 | `UP`/`k`   | Move up the cursor                            |
 | `DOWN`/`j` | Move down the cursor                          |
 | `K`        | Terminate the current backend/tagged backends |
 | `C`        | Cancel the current backend/tagged backends    |
 | `Space`    | Tag or untag the process                      |
 | `q`        | Quit                                          |
 | `Other`    | Back to activity                              |
 
-FAQ
----
+## FAQ
 
 **I can't see my queries only TPS is shown**
 
 `pg_activity` scans the view `pg_stat_activity` with a user defined refresh
 time comprised between 0.5 and 5 seconds. It can be modified in the interface
 with the `+` and `-` keys. Any query executed between two scans won't be
 displayed.
@@ -241,11 +266,12 @@
 You can pass the password for the database connection in a password file.
 Information can also be given via PostgreSQL's environment variables
 (PGPASSFILE or PGPASSWORD) or via the connection string parameters.
 
 The password file is preferred since it's more secure (security is deferred to
 the OS). Please avoid password in connection strings at all cost.
 
-Change log
-----------
+# Change log
+
+See [CHANGELOG.md][changelog].
 
-See [CHANGELOG.md](https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md).
+[changelog]: https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pg_activity-3.3.0/pg_activity.egg-info/SOURCES.txt` & `pg-activity-3.4.0/pg_activity.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 docs/man/build-man.sh
 docs/man/pg_activity.1
 docs/man/pg_activity.pod
 pg_activity.egg-info/PKG-INFO
 pg_activity.egg-info/SOURCES.txt
 pg_activity.egg-info/dependency_links.txt
 pg_activity.egg-info/entry_points.txt
-pg_activity.egg-info/not-zip-safe
 pg_activity.egg-info/requires.txt
 pg_activity.egg-info/top_level.txt
 pgactivity/__init__.py
 pgactivity/__main__.py
 pgactivity/activities.py
 pgactivity/cli.py
 pgactivity/colors.py
 pgactivity/compat.py
+pgactivity/config.py
 pgactivity/data.py
 pgactivity/handlers.py
 pgactivity/keys.py
 pgactivity/pg.py
 pgactivity/types.py
 pgactivity/ui.py
 pgactivity/utils.py
@@ -71,18 +71,18 @@
 pgactivity/queries/get_temporary_files_post_090500.sql
 pgactivity/queries/get_temporary_files_post_120000.sql
 pgactivity/queries/get_version.sql
 pgactivity/queries/get_waiting_oldest.sql
 pgactivity/queries/get_waiting_post_090200.sql
 pgactivity/queries/get_wal_receivers_post_090600.sql
 pgactivity/queries/get_wal_senders_post_090100.sql
-pgactivity/queries/is_superuser.sql
 pgactivity/queries/reset_statement_timeout.sql
 tests/conftest.py
 tests/test_activities.py
+tests/test_config.py
 tests/test_data.py
 tests/test_scroll.txt
 tests/test_types.py
 tests/test_ui.txt
 tests/test_views.py
 tests/test_views.txt
 tests/test_widgets.txt
```

### Comparing `pg_activity-3.3.0/pgactivity/activities.py` & `pg-activity-3.4.0/pgactivity/activities.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,22 +145,24 @@
 
 T = TypeVar("T", RunningProcess, WaitingProcess, BlockingProcess, LocalRunningProcess)
 
 
 def sorted(processes: List[T], *, key: SortKey, reverse: bool = False) -> List[T]:
     """Return processes sorted.
 
+    >>> from ipaddress import IPv4Interface, ip_address
+
     PostgreSQL 13+
     >>> processes = [
     ...     LocalRunningProcess(
     ...         pid="6240",
     ...         application_name="pgbench",
     ...         database="pgbench",
     ...         user="postgres",
-    ...         client="local",
+    ...         client=ip_address("127.0.0.2"),
     ...         cpu=0.1,
     ...         mem=0.993_254_939_413_836,
     ...         read=0.1,
     ...         write=0.282_725_318_098_656_75,
     ...         state="idle in transaction",
     ...         query="UPDATE pgbench_accounts SET abalance = abalance + 3062 WHERE aid = 1932841;",
     ...         encoding="UTF-8",
@@ -171,15 +173,15 @@
     ...         is_parallel_worker=False,
     ...     ),
     ...     LocalRunningProcess(
     ...         pid="6239",
     ...         application_name="pgbench",
     ...         database="pgbench",
     ...         user="postgres",
-    ...         client="local",
+    ...         client=IPv4Interface("192.0.2.5/24"),
     ...         cpu=0.1,
     ...         mem=0.994_254_939_413_836,
     ...         read=0.1,
     ...         write=0.282_725_318_098_656_75,
     ...         state="idle in transaction",
     ...         query="UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 7289374;",
     ...         encoding=None,
@@ -190,15 +192,15 @@
     ...         is_parallel_worker=False,
     ...     ),
     ...     LocalRunningProcess(
     ...         pid="6228",
     ...         application_name="pgbench",
     ...         database="pgbench",
     ...         user="postgres",
-    ...         client="local",
+    ...         client=ip_address("2001:db8::"),
     ...         cpu=0.2,
     ...         mem=1.024_758_418_061_11,
     ...         read=0.2,
     ...         write=0.113_090_128_201_154_74,
     ...         state="active",
     ...         query="UPDATE pgbench_accounts SET abalance = abalance + 3062 WHERE aid = 1932841;",
     ...         encoding="UTF-8",
@@ -226,15 +228,15 @@
     PostgreSQL 12- (query_leader_pid is None)
     >>> processes = [
     ...     LocalRunningProcess(
     ...         pid="6240",
     ...         application_name="pgbench",
     ...         database="pgbench",
     ...         user="postgres",
-    ...         client="local",
+    ...         client=ip_address("192.168.1.2"),
     ...         cpu=0.1,
     ...         mem=0.993_254_939_413_836,
     ...         read=0.1,
     ...         write=0.282_725_318_098_656_75,
     ...         state="idle in transaction",
     ...         query="UPDATE pgbench_accounts SET abalance = abalance + 3062 WHERE aid = 1932841;",
     ...         encoding=None,
@@ -245,15 +247,15 @@
     ...         is_parallel_worker=False,
     ...     ),
     ...     LocalRunningProcess(
     ...         pid="6239",
     ...         application_name="pgbench",
     ...         database="pgbench",
     ...         user="postgres",
-    ...         client="local",
+    ...         client=ip_address("0000:0000:0000:0000:0000:0abc:0007:0def"),
     ...         cpu=0.1,
     ...         mem=0.994_254_939_413_836,
     ...         read=0.1,
     ...         write=0.282_725_318_098_656_75,
     ...         state="idle in transaction",
     ...         query="UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 7289374;",
     ...         encoding="UTF-8",
@@ -264,15 +266,15 @@
     ...         is_parallel_worker=False,
     ...     ),
     ...     LocalRunningProcess(
     ...         pid="6228",
     ...         application_name="pgbench",
     ...         database="pgbench",
     ...         user="postgres",
-    ...         client="local",
+    ...         client=None,
     ...         cpu=0.2,
     ...         mem=1.024_758_418_061_11,
     ...         read=0.2,
     ...         write=0.113_090_128_201_154_74,
     ...         state="active",
     ...         query="UPDATE pgbench_accounts SET abalance = abalance + 3062 WHERE aid = 1932841;",
     ...         encoding="latin1",
```

### Comparing `pg_activity-3.3.0/pgactivity/cli.py` & `pg-activity-3.4.0/pgactivity/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from argparse import ArgumentParser
 from io import StringIO
 from typing import Optional
 
 from blessed import Terminal
 
 from . import __version__, data, types, ui
+from .config import Configuration, ConfigurationError
 from .pg import OperationalError
 
 
 def configure_logger(debug_file: Optional[str] = None) -> StringIO:
     logger = logging.getLogger("pgactivity")
     logger.setLevel(logging.DEBUG)
 
@@ -381,14 +382,19 @@
     try:
         filters = types.Filters.from_options(args.filters)
     except ValueError as e:
         parser.error(str(e))
     if args.rds:
         args.notempfile = True
 
+    try:
+        cfg = Configuration.lookup()
+    except ConfigurationError as e:
+        parser.error(str(e))
+
     dataobj = data.pg_connect(
         args,
         args.connection_string,
         min_duration=args.minduration,
         filters=filters,
     )
     hostname = socket.gethostname()
@@ -400,15 +406,15 @@
         int(conninfo.port),
         conninfo.dbname,
     )
 
     term = Terminal()
     while True:
         try:
-            ui.main(term, dataobj, host, args)
+            ui.main(term, cfg, dataobj, host, args)
         except OperationalError:
             while True:
                 print(term.clear + term.home, end="")
                 print("Connection to PostgreSQL lost, trying to reconnect...")
                 try:
                     time.sleep(5)
                 except KeyboardInterrupt:
```

### Comparing `pg_activity-3.3.0/pgactivity/colors.py` & `pg-activity-3.4.0/pgactivity/colors.py`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/compat.py` & `pg-activity-3.4.0/pgactivity/compat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+import sys
 from typing import Any, Dict
 
 import attr
 import blessed
 
-ATTR_VERSION = tuple(int(x) for x in attr.__version__.split(".", 2)[:2])
-BLESSED_VERSION = tuple(int(x) for x in blessed.__version__.split(".", 2)[:2])
+if sys.version_info < (3, 8):
+    from importlib_metadata import version
+else:
+    from importlib.metadata import version
+
+ATTR_VERSION = tuple(int(x) for x in version("attrs").split(".", 2)[:2])
+BLESSED_VERSION = tuple(int(x) for x in version("blessed").split(".", 2)[:2])
 
 if ATTR_VERSION < (18, 1):
 
     def fields_dict(cls: Any) -> Dict[str, Any]:
         return {a.name: a for a in cls.__attrs_attrs__}
 
 else:
```

### Comparing `pg_activity-3.3.0/pgactivity/data.py` & `pg-activity-3.4.0/pgactivity/data.py`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/handlers.py` & `pg-activity-3.4.0/pgactivity/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 from blessed.keyboard import Keystroke
 
 from . import keys
-from .types import DurationMode, Flag, QueryMode, SortKey, enum_next
+from .config import Flag
+from .types import DurationMode, QueryMode, SortKey, enum_next
 
 
 def refresh_time(
     key: Optional[str], value: float, minimum: float = 0.5, maximum: float = 5
 ) -> float:
     """Return an updated refresh time interval from input key respecting bounds.
```

### Comparing `pg_activity-3.3.0/pgactivity/keys.py` & `pg-activity-3.4.0/pgactivity/keys.py`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/pg.py` & `pg-activity-3.4.0/pgactivity/pg.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     class AutoTextLoader(Loader):
         def load(self, data: Buffer) -> str:
             if not isinstance(data, bytes):
                 data = bytes(data)
             return data.decode(errors="replace")
 
-    def connect(dsn: str, **kwargs: Any) -> Connection:
+    def connect(dsn: str = "", **kwargs: Any) -> Connection:
         if "PGCLIENTENCODING" not in os.environ:
             # Set client_encoding to 'auto', if not set by the user.
             # This is (more or less) what's done by psql.
             conninfo = conninfo_to_dict(dsn)
             conninfo.setdefault("client_encoding", "auto")
             dsn = make_conninfo(**conninfo)
         conn = psycopg.connect(dsn, autocommit=True, row_factory=dict_row, **kwargs)
@@ -198,15 +198,15 @@
 
     # isort: on
     from psycopg2.extensions import connection as Connection  # type: ignore[no-redef]
     from psycopg2.extras import DictCursor
 
     __version__ = psycopg2.__version__
 
-    def connect(dsn: str, **kwargs: Any) -> Connection:
+    def connect(dsn: str = "", **kwargs: Any) -> Connection:
         try:
             kwargs.setdefault("database", kwargs.pop("dbname"))
         except KeyError:
             pass
         conn = psycopg2.connect(dsn, cursor_factory=DictCursor, **kwargs)
         conn.autocommit = True
         return conn  # type: ignore[no-any-return]
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_blocking_oldest.sql` & `pg-activity-3.4.0/pgactivity/queries/get_blocking_oldest.sql`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,15 @@
             blocking.pid,
             '<unknown>' AS application_name,
             pg_stat_activity.current_query AS query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             NULL AS state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.waiting
         FROM
             pg_locks AS blocking
@@ -61,18 +58,15 @@
             blocking.pid,
             '<unknown>' AS application_name,
             pg_stat_activity.current_query AS query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             NULL AS state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.waiting
         FROM
             pg_locks AS blocking
@@ -94,18 +88,15 @@
             blocking.pid,
             '<unknown>' AS application_name,
             pg_stat_activity.current_query AS query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             NULL AS state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.waiting
         FROM
             pg_locks AS blocking
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_blocking_post_090200.sql` & `pg-activity-3.4.0/pgactivity/queries/get_blocking_post_090200.sql`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,15 @@
             blocking.pid,
             pg_stat_activity.application_name,
             pg_stat_activity.query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             pg_stat_activity.state as state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.waiting
         FROM
             pg_locks AS blocking
@@ -56,18 +53,15 @@
             blocking.pid,
             pg_stat_activity.application_name,
             pg_stat_activity.query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             pg_stat_activity.state as state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.waiting
         FROM
             pg_locks AS blocking
@@ -89,18 +83,15 @@
             blocking.pid,
             pg_stat_activity.application_name,
             pg_stat_activity.query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             pg_stat_activity.state as state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.waiting
         FROM
             pg_locks AS blocking
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_blocking_post_090600.sql` & `pg-activity-3.4.0/pgactivity/queries/get_blocking_post_090600.sql`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,15 @@
             blocking.pid,
             pg_stat_activity.application_name,
             pg_stat_activity.query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             pg_stat_activity.state as state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.wait_event
         FROM
             pg_locks AS blocking
@@ -54,18 +51,15 @@
             blocking.pid,
             pg_stat_activity.application_name,
             pg_stat_activity.query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             pg_stat_activity.state as state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.wait_event
         FROM
             pg_locks AS blocking
@@ -87,18 +81,15 @@
             blocking.pid,
             pg_stat_activity.application_name,
             pg_stat_activity.query,
             blocking.mode,
             pg_stat_activity.datname,
             pg_stat_activity.datid,
             pg_stat_activity.usename,
-            CASE WHEN pg_stat_activity.client_addr IS NULL
-                THEN 'local'
-                ELSE pg_stat_activity.client_addr::TEXT
-            END AS client,
+            pg_stat_activity.client_addr AS client,
             blocking.locktype,
             EXTRACT(epoch FROM (NOW() - pg_stat_activity.{duration_column})) AS duration,
             pg_stat_activity.state as state,
             blocking.relation::regclass AS relation,
             pg_stat_activity.wait_event
         FROM
             pg_locks AS blocking
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_pg_activity_oldest.sql` & `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_oldest.sql`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 -- Get data from pg_activity before pg 9.2
 SELECT
       a.procpid AS pid,
       '<unknown>' AS application_name,
       a.datname AS database,
-      CASE WHEN a.client_addr IS NULL
-          THEN 'local'
-          ELSE a.client_addr::TEXT
-      END AS client,
+      a.client_addr AS client,
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) AS duration,
       a.waiting AS wait,
       a.usename AS user,
       CASE
           WHEN a.current_query = '<IDLE> in transaction (aborted)' THEN 'idle in transaction (aborted)'
           WHEN a.current_query = '<IDLE> in transaction' THEN 'idle in transaction'
           WHEN a.current_query = '<IDLE>' THEN 'idle'
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_090200.sql` & `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_090200.sql`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 -- Get data from pg_activity from pg 9.2 to pg 9.5
 -- NEW pg_stat_activity.current_query => pg_stat_activity.query
 -- NEW pg_stat_activity.procpid => pg_stat_activity.pid
 SELECT
       a.pid AS pid,
       a.application_name AS application_name,
       a.datname AS database,
-      CASE WHEN a.client_addr IS NULL
-          THEN 'local'
-          ELSE a.client_addr::TEXT
-      END AS client,
+      a.client_addr AS client,
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) AS duration,
       a.waiting AS wait,
       a.usename AS user,
       a.state AS state,
       a.query AS query,
       pg_catalog.pg_encoding_to_char(b.encoding) AS encoding,
       NULL AS query_leader_pid,
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_090600.sql` & `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_110000.sql`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,30 @@
--- Get data from pg_activity from pg 9.6 to 10
--- In this version there is no way to distinguish parallel workers from the rest
--- NEW pg_stat_activity.waiting => pg_stat_activity.wait_event
+-- Get data from pg_activity since pg 11
+-- NEW pg_activity.backend_type value for 'parallel worker'
 SELECT
       a.pid AS pid,
       a.application_name AS application_name,
       a.datname AS database,
-      CASE WHEN a.client_addr IS NULL
-          THEN 'local'
-          ELSE a.client_addr::TEXT
-      END AS client,
+      a.client_addr AS client,
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) AS duration,
       a.wait_event AS wait,
       a.usename AS user,
       a.state AS state,
       a.query AS query,
       pg_catalog.pg_encoding_to_char(b.encoding) AS encoding,
       NULL AS query_leader_pid,
-      false AS is_parallel_worker
-  FROM
+      a.backend_type = 'parallel worker' AS is_parallel_worker
+ FROM
       pg_stat_activity a
       LEFT OUTER JOIN pg_database b ON a.datid = b.oid
  WHERE
-      state <> 'idle'
-  AND pid <> pg_backend_pid()
+      a.state <> 'idle'
+  AND a.pid <> pg_catalog.pg_backend_pid()
   AND CASE WHEN {min_duration} = 0
           THEN true
           ELSE extract(epoch from now() - {duration_column}) > %(min_duration)s
       END
-  AND CASE WHEN {dbname_filter} IS NULL THEN true
-      ELSE a.datname ~* %(dbname_filter)s
-      END
+    AND CASE WHEN {dbname_filter} IS NULL THEN true
+        ELSE a.datname ~* %(dbname_filter)s
+        END
 ORDER BY
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) DESC;
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_100000.sql` & `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_100000.sql`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 -- Get data from pg_activity from pg 10 to pg 11
 -- We assume a background_worker with a not null query is a parallel worker.
 -- NEW pg_activity.backend_type
 SELECT
       a.pid AS pid,
       a.application_name AS application_name,
       a.datname AS database,
-      CASE WHEN a.client_addr IS NULL
-          THEN 'local'
-          ELSE a.client_addr::TEXT
-      END AS client,
+      a.client_addr AS client,
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) AS duration,
       a.wait_event as wait,
       a.usename AS user,
       a.state AS state,
       a.query AS query,
       pg_catalog.pg_encoding_to_char(b.encoding) AS encoding,
       NULL AS query_leader_pid,
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_110000.sql` & `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_130000.sql`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,21 @@
--- Get data from pg_activity since pg 11
--- NEW pg_activity.backend_type value for 'parallel worker'
+-- Get data from pg_activity since pg 13
+-- NEW pg_activity.leader_pid
 SELECT
       a.pid AS pid,
       a.application_name AS application_name,
       a.datname AS database,
-      CASE WHEN a.client_addr IS NULL
-          THEN 'local'
-          ELSE a.client_addr::TEXT
-      END AS client,
+      a.client_addr AS client,
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) AS duration,
       a.wait_event AS wait,
       a.usename AS user,
       a.state AS state,
       a.query AS query,
       pg_catalog.pg_encoding_to_char(b.encoding) AS encoding,
-      NULL AS query_leader_pid,
+      coalesce(a.leader_pid, a.pid) AS query_leader_pid,
       a.backend_type = 'parallel worker' AS is_parallel_worker
  FROM
       pg_stat_activity a
       LEFT OUTER JOIN pg_database b ON a.datid = b.oid
  WHERE
       a.state <> 'idle'
   AND a.pid <> pg_catalog.pg_backend_pid()
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_pg_activity_post_130000.sql` & `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_090600.sql`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,31 @@
--- Get data from pg_activity since pg 13
--- NEW pg_activity.leader_pid
+-- Get data from pg_activity from pg 9.6 to 10
+-- In this version there is no way to distinguish parallel workers from the rest
+-- NEW pg_stat_activity.waiting => pg_stat_activity.wait_event
 SELECT
       a.pid AS pid,
       a.application_name AS application_name,
       a.datname AS database,
-      CASE WHEN a.client_addr IS NULL
-          THEN 'local'
-          ELSE a.client_addr::TEXT
-      END AS client,
+      a.client_addr AS client,
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) AS duration,
       a.wait_event AS wait,
       a.usename AS user,
       a.state AS state,
       a.query AS query,
       pg_catalog.pg_encoding_to_char(b.encoding) AS encoding,
-      coalesce(a.leader_pid, a.pid) AS query_leader_pid,
-      a.backend_type = 'parallel worker' AS is_parallel_worker
- FROM
+      NULL AS query_leader_pid,
+      false AS is_parallel_worker
+  FROM
       pg_stat_activity a
       LEFT OUTER JOIN pg_database b ON a.datid = b.oid
  WHERE
-      a.state <> 'idle'
-  AND a.pid <> pg_catalog.pg_backend_pid()
+      state <> 'idle'
+  AND pid <> pg_backend_pid()
   AND CASE WHEN {min_duration} = 0
           THEN true
           ELSE extract(epoch from now() - {duration_column}) > %(min_duration)s
       END
-    AND CASE WHEN {dbname_filter} IS NULL THEN true
-        ELSE a.datname ~* %(dbname_filter)s
-        END
+  AND CASE WHEN {dbname_filter} IS NULL THEN true
+      ELSE a.datname ~* %(dbname_filter)s
+      END
 ORDER BY
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) DESC;
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_server_info_oldest.sql` & `pg-activity-3.4.0/pgactivity/queries/get_server_info_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_server_info_post_090100.sql` & `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090100.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_server_info_post_090200.sql` & `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_server_info_post_090400.sql` & `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090400.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_server_info_post_090600.sql` & `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_server_info_post_100000.sql` & `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_100000.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_server_info_post_110000.sql` & `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_110000.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_temporary_files_oldest.sql` & `pg-activity-3.4.0/pgactivity/queries/get_temporary_files_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_temporary_files_post_090100.sql` & `pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_090100.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_temporary_files_post_090500.sql` & `pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_090500.sql`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_waiting_oldest.sql` & `pg-activity-3.4.0/pgactivity/queries/get_waiting_oldest.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 -- Get waiting queries for versions before 9.2
 SELECT
       pg_locks.pid AS pid,
       '<unknown>' AS application_name,
       a.datname AS database,
       a.usename AS user,
-      CASE WHEN a.client_addr IS NULL
-          THEN 'local'
-          ELSE a.client_addr::TEXT
-      END AS client,
+      a.client_addr AS client,
       pg_locks.mode AS mode,
       pg_locks.locktype AS type,
       pg_locks.relation::regclass AS relation,
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) AS duration,
       CASE
           WHEN a.current_query = '<IDLE> in transaction (aborted)' THEN 'idle in transaction (aborted)'
           WHEN a.current_query = '<IDLE> in transaction' THEN 'idle in transaction'
```

### Comparing `pg_activity-3.3.0/pgactivity/queries/get_waiting_post_090200.sql` & `pg-activity-3.4.0/pgactivity/queries/get_waiting_post_090200.sql`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 -- NEW pg_stat_activity.current_query => pg_stat_activity.query
 -- NEW pg_stat_activity.procpid => pg_stat_activity.pid
 SELECT
       pg_locks.pid AS pid,
       a.application_name AS application_name,
       a.datname AS database,
       a.usename AS user,
-      CASE WHEN a.client_addr IS NULL
-          THEN 'local'
-          ELSE a.client_addr::TEXT
-      END AS client,
+      a.client_addr AS client,
       pg_locks.mode AS mode,
       pg_locks.locktype AS type,
       pg_locks.relation::regclass AS relation,
       EXTRACT(epoch FROM (NOW() - a.{duration_column})) AS duration,
       a.state as state,
       a.query AS query,
       pg_catalog.pg_encoding_to_char(b.encoding) AS encoding
```

### Comparing `pg_activity-3.3.0/pgactivity/types.py` & `pg-activity-3.4.0/pgactivity/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 import functools
 from datetime import timedelta
+from ipaddress import IPv4Address, IPv6Address
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     Iterator,
     List,
@@ -20,14 +21,15 @@
 )
 
 import attr
 import psutil
 from attr import validators
 
 from . import colors, compat, pg, utils
+from .config import Configuration, Flag
 
 
 class Pct(float):
     """Used to distinguish percentage from float when displaying the header"""
 
 
 T = TypeVar("T")
@@ -49,95 +51,14 @@
     'summer'
     >>> enum_next(Seasons.autumn).name
     'winter'
     """
     return e.__class__((e.value % max(e.__class__)) + 1)
 
 
-@enum.unique
-class Flag(enum.IntFlag):
-    """Column flag."""
-
-    DATABASE = 1
-    APPNAME = 2
-    CLIENT = 4
-    USER = 8
-    CPU = 16
-    MEM = 32
-    READ = 64
-    WRITE = 128
-    TIME = 256
-    WAIT = 512
-    RELATION = 1024
-    TYPE = 2048
-    MODE = 4096
-    IOWAIT = 8192
-    PID = 16384
-
-    @classmethod
-    def all(cls) -> "Flag":
-        return cls(sum(cls))
-
-    @classmethod
-    def from_options(
-        cls,
-        *,
-        is_local: bool,
-        noappname: bool,
-        noclient: bool,
-        nocpu: bool,
-        nodb: bool,
-        nomem: bool,
-        nopid: bool,
-        noread: bool,
-        notime: bool,
-        nouser: bool,
-        nowait: bool,
-        nowrite: bool,
-        **kwargs: Any,
-    ) -> "Flag":
-        """Build a Flag value from command line options."""
-        flag = cls.all()
-        if nodb:
-            flag ^= cls.DATABASE
-        if nouser:
-            flag ^= cls.USER
-        if nocpu:
-            flag ^= cls.CPU
-        if noclient:
-            flag ^= cls.CLIENT
-        if nomem:
-            flag ^= cls.MEM
-        if noread:
-            flag ^= cls.READ
-        if nowrite:
-            flag ^= cls.WRITE
-        if notime:
-            flag ^= cls.TIME
-        if nowait:
-            flag ^= cls.WAIT
-        if noappname:
-            flag ^= cls.APPNAME
-        if nopid:
-            flag ^= cls.PID
-
-        # Remove some if no running against local pg server.
-        if not is_local and (flag & cls.CPU):
-            flag ^= cls.CPU
-        if not is_local and (flag & cls.MEM):
-            flag ^= cls.MEM
-        if not is_local and (flag & cls.READ):
-            flag ^= cls.READ
-        if not is_local and (flag & cls.WRITE):
-            flag ^= cls.WRITE
-        if not is_local and (flag & cls.IOWAIT):
-            flag ^= cls.IOWAIT
-        return flag
-
-
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class Filters:
     dbname: Optional[str] = None
 
     @classmethod
     def from_options(cls, filters: Sequence[str]) -> "Filters":
         fields = compat.fields_dict(cls)
@@ -189,14 +110,23 @@
     transaction = 2
     backend = 3
 
 
 _color_key_marker = f"{id(object())}"
 
 
+def if_none(default: str) -> Callable[[Any], str]:
+    def transform(value: Any) -> str:
+        if value is None:
+            return default
+        return str(value)
+
+    return transform
+
+
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class Column:
     """A column in stats table.
 
     >>> c = Column("pid", "PID", mandatory=True, sort_key=SortKey.cpu,
     ...            min_width=6, max_width=6,
     ...            transform=lambda v: str(v)[::-1])
@@ -227,17 +157,15 @@
     mandatory: bool = False
     sort_key: Optional[SortKey] = None
     min_width: int = attr.ib(default=0, repr=False)
     max_width: Optional[int] = attr.ib(default=None, repr=False)
     justify: str = attr.ib(
         "left", validator=validators.in_(["left", "center", "right"])
     )
-    transform: Callable[[Any], str] = attr.ib(
-        default=lambda v: str(v) if v is not None else "", repr=False
-    )
+    transform: Callable[[Any], str] = attr.ib(default=if_none(""), repr=False)
     color_key: Union[str, Callable[[Any], str]] = attr.ib(
         default=_color_key_marker, repr=False
     )
 
     _justify: Callable[[str], str] = attr.ib(init=False)
 
     def __attrs_post_init__(self) -> None:
@@ -296,23 +224,32 @@
     show_instance_info_in_header: bool = True
     show_system_info_in_header: bool = True
     show_worker_info_in_header: bool = True
 
     @classmethod
     def make(
         cls,
+        config: Optional[Configuration] = None,
         flag: Flag = Flag.all(),
         *,
         max_db_length: int = 16,
         filters: Filters = NO_FILTER,
         **kwargs: Any,
     ) -> "UI":
         possible_columns: Dict[str, Column] = {}
 
         def add_column(key: str, name: str, **kwargs: Any) -> None:
+            if config is not None:
+                try:
+                    cfg = config[name.lower()]
+                except KeyError:
+                    pass
+                else:
+                    if cfg.width is not None:
+                        kwargs["min_width"] = kwargs["max_width"] = cfg.width
             assert key not in possible_columns, f"duplicated key {key}"
             possible_columns[key] = Column(key=key, name=name, **kwargs)
 
         if Flag.APPNAME & flag:
             add_column(
                 key="application_name",
                 name="APP",
@@ -323,14 +260,15 @@
         if Flag.CLIENT & flag:
             add_column(
                 key="client",
                 name="CLIENT",
                 min_width=16,
                 max_width=16,
                 justify="right",
+                transform=if_none("local"),
             )
         if Flag.CPU & flag:
             add_column(
                 key="cpu",
                 name="CPU%",
                 min_width=6,
                 sort_key=SortKey.cpu,
@@ -900,15 +838,15 @@
 
 @attr.s(auto_attribs=True, slots=True)
 class BaseProcess:
     pid: int
     application_name: str
     database: Optional[str]
     user: str
-    client: str
+    client: Union[None, IPv4Address, IPv6Address]
     duration: Optional[float]
     state: str
     query: Optional[str]
     encoding: Optional[str]
     query_leader_pid: Optional[int]
     is_parallel_worker: bool
```

### Comparing `pg_activity-3.3.0/pgactivity/ui.py` & `pg-activity-3.4.0/pgactivity/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 from functools import partial
 from typing import Dict, List, Optional, cast
 
 import attr
 from blessed import Terminal
 
 from . import __version__, activities, handlers, keys, types, utils, views, widgets
+from .config import Configuration, Flag
 from .data import Data
 
 
 def main(
     term: Terminal,
+    config: Optional[Configuration],
     data: Data,
     host: types.Host,
     options: Namespace,
     *,
     render_header: bool = True,
     render_footer: bool = True,
     width: Optional[int] = None,
@@ -30,16 +32,17 @@
         prev_server_info=None,
         using_rds=options.rds,
         skip_db_size=options.nodbsize,
         skip_tempfile=options.notempfiles,
         skip_walreceiver=options.nowalreceiver,
     )
 
-    flag = types.Flag.from_options(is_local=is_local, **vars(options))
+    flag = Flag.load(config, is_local=is_local, **vars(options))
     ui = types.UI.make(
+        config=config,
         flag=flag,
         refresh_time=options.refresh,
         min_duration=options.minduration,
         duration_mode=int(options.durationmode),
         wrap_query=options.wrap_query,
         max_db_length=min(max(server_information.max_dbname_length, 8), 16),
         filters=data.filters,
```

### Comparing `pg_activity-3.3.0/pgactivity/utils.py` & `pg-activity-3.4.0/pgactivity/utils.py`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/pgactivity/views.py` & `pg-activity-3.4.0/pgactivity/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,16 @@
         htitles.append(f"{color}{column.title_render()}")
     yield term.ljust(" ".join(htitles), fillchar=" ") + term.normal
 
 
 def get_indent(ui: UI) -> str:
     """Return indentation for Query column.
 
-    >>> from pgactivity.types import Flag, UI
+    >>> from pgactivity.config import Flag
+    >>> from pgactivity.types import UI
     >>> ui = UI.make(flag=Flag.CPU)
     >>> get_indent(ui)
     '                         '
     >>> ui = UI.make(flag=Flag.PID | Flag.DATABASE | Flag.APPNAME | Flag.RELATION)
     >>> get_indent(ui)
     '                                                           '
     """
```

### Comparing `pg_activity-3.3.0/pgactivity/widgets.py` & `pg-activity-3.4.0/pgactivity/widgets.py`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/tests/conftest.py` & `pg-activity-3.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/tests/data/local-processes-input.json` & `pg-activity-3.4.0/tests/data/local-processes-input.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950980392156862%*

 * *Differences: {"'new_processes'": "{'6221': {'client': None}, '6222': {'client': None}, '6223': {'client': "*

 * *                    "None}, '6224': {'client': None}, '6225': {'client': None}, '6226': {'client': "*

 * *                    "None}, '6227': {'client': None}, '6228': {'client': None}, '6229': {'client': "*

 * *                    "None}, '6230': {'client': None}, '6231': {'client': None}, '6232': {'client': "*

 * *                    "None}, '6233': {'client': None}, '6234': {'client': None}, '6235': {'client': "*

 * *              […]*

```diff
@@ -1,13 +1,13 @@
 {
     "fs_blocksize": 4096,
     "new_processes": {
         "6221": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002731,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -52,15 +52,15 @@
             "state": "active",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6222": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003539,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -105,15 +105,15 @@
             "state": "active",
             "user": "postgres",
             "wait": null,
             "write": null
         },
         "6223": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002385,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -158,15 +158,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6224": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.00302,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -211,15 +211,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6225": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002305,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -264,15 +264,15 @@
             "state": "active",
             "user": "postgres",
             "wait": "ClientRead",
             "write": null
         },
         "6226": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002623,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -317,15 +317,15 @@
             "state": "active",
             "user": "postgres",
             "wait": "LogicalRepWorkerLock",
             "write": null
         },
         "6227": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002693,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -370,15 +370,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6228": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003339,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -423,15 +423,15 @@
             "state": "active",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6229": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003353,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -476,15 +476,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6230": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003495,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -529,15 +529,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6231": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003384,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -582,15 +582,15 @@
             "state": "active",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6232": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002212,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -635,15 +635,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6233": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002273,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -688,15 +688,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6234": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002408,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -741,15 +741,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6235": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002635,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -794,15 +794,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6237": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003559,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -847,15 +847,15 @@
             "state": "active",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6238": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003481,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -900,15 +900,15 @@
             "state": "active",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6239": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003428,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -953,15 +953,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6240": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002256,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1008,15 +1008,15 @@
             "wait": true,
             "write": null
         }
     },
     "processes": {
         "6221": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002794,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1061,15 +1061,15 @@
             "state": "active",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6222": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003188,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1114,15 +1114,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6223": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.00347,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1167,15 +1167,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6224": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003245,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1220,15 +1220,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6225": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003286,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1273,15 +1273,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6226": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003431,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1326,15 +1326,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6227": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002061,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1379,15 +1379,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6228": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003475,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1432,15 +1432,15 @@
             "state": "active",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6229": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003226,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1485,15 +1485,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6230": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002711,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1538,15 +1538,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6231": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.001462,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1591,15 +1591,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6232": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003435,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1644,15 +1644,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6233": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.00339,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1697,15 +1697,15 @@
             "state": "active",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6234": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003179,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1750,15 +1750,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6235": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003405,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1803,15 +1803,15 @@
             "state": "idle in transaction",
             "user": "postgres",
             "wait": false,
             "write": null
         },
         "6236": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002822,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1856,15 +1856,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6237": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.002788,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1909,15 +1909,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6238": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003436,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -1962,15 +1962,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6239": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.00305,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
@@ -2015,15 +2015,15 @@
             "state": "active",
             "user": "postgres",
             "wait": true,
             "write": null
         },
         "6240": {
             "application_name": "pgbench",
-            "client": "local",
+            "client": null,
             "cpu": null,
             "database": "pgbench",
             "duration": -0.003586,
             "encoding": "UTF-8",
             "extras": {
                 "cpu_percent": 0.0,
                 "cpu_times": [
```

### Comparing `pg_activity-3.3.0/tests/test_activities.py` & `pg-activity-3.4.0/tests/test_activities.py`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/tests/test_data.py` & `pg-activity-3.4.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pg_activity-3.3.0/tests/test_scroll.txt` & `pg-activity-3.4.0/tests/test_scroll.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 >>> processes_scroll = [
 ...     RunningProcess(
 ...         pid=x,
 ...         application_name="pgbench",
 ...         database="pgbench",
 ...         user="postgres",
-...         client="local",
+...         client=None,
 ...         state="active",
 ...         query=f"SELECT {x}",
 ...         encoding=None,
 ...         duration=0.0,
 ...         wait=False,
 ...         query_leader_pid=x,
 ...         is_parallel_worker=False,
```

### Comparing `pg_activity-3.3.0/tests/test_ui.txt` & `pg-activity-3.4.0/tests/test_ui.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 >>> import os
 >>> import time
 >>> from unittest.mock import patch
 
 >>> import blessed
 >>> from blessed.keyboard import Keystroke
 
->>> from pgactivity import data, types, ui, widgets
+>>> from pgactivity import config, data, types, ui, widgets
 
 >>> postgres = getfixture("postgresql")
 
 Default CLI options, passed to ui.main():
 >>> defaults = {
 ...     "blocksize": 4096,
 ...     "dbname": f"{postgres.info.dbname}",
@@ -68,15 +68,21 @@
 ...     host=postgres.info.host,
 ...     port=postgres.info.port,
 ...     user=postgres.info.user,
 ...     database=postgres.info.dbname,
 ...     min_duration=options.minduration,
 ... )
 
->>> def run_ui(options, keys, expected_timeouts=None,
+>>> def mkconfig(value):
+...     return config.Configuration(
+...         **{k: config.UISection(**v) for k, v in value.items()}
+... )
+>>> CONFIG = mkconfig({"database": {"width": 9}, "client": {"width": 12}})
+
+>>> def run_ui(options, keys, config=CONFIG, expected_timeouts=None,
 ...            render_header=True, render_footer=False,
 ...            width=200):
 ...     """Wrapper to ui.main() with a fake term.inkey()."""
 ...
 ...     call_args_list = []
 ...
 ...     def inkey(*, timeout):
@@ -88,15 +94,15 @@
 ...             ks = Keystroke(key)
 ...         if render_footer:
 ...             print()
 ...         print(term.center(f" sending key '{ks}' ", fillchar="-", width=width))
 ...         return ks
 ...
 ...     with patch.object(term, "inkey", new=inkey):
-...         ui.main(term, dataobj, host, options,
+...         ui.main(term, config, dataobj, host, options,
 ...                 render_header=render_header, render_footer=render_footer,
 ...                 width=width, wait_on_actions=1)
 ...
 ...     if expected_timeouts is not None:
 ...         assert call_args_list == expected_timeouts
 
 Force local mode and mock server and system info
@@ -176,15 +182,15 @@
  * Worker processes: 3/8 total, 1/8 logical workers, 2/8 parallel workers
    Other processes & info: 3/3 autovacuum workers, 1/10 wal senders, 0 wal receivers, 10/10 repl. slots
  * Mem.: 8B total, 2B (25.00%) free, 2B (25.00%) used, 4B (50.00%) buff+cached
    Swap: 2B total, 1B (50.00%) free, 1B (50.00%) used
    IO: 300/s max iops, 200B/s - 100/s read, 300B/s - 200/s write
    Load average: 1 5 15
                                 RUNNING QUERIES
-PID    DATABASE                     USER           CLIENT IOW              state Query
+PID    DATABASE              USER       CLIENT IOW              state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -199,15 +205,15 @@
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 2s - Duration mode: query
  * Global: 132 days, 3 hours and 21 minutes uptime, 19.53M dbs size - 1.00K/s growth, 90.12% cache hit ratio
    Sessions: 6/100 total, 1 active, 1 idle, 10 idle in txn, 0 idle in txn abrt, 3 waiting
    Activity: 15 tps, 10 insert/s, 20 update/s, 30 delete/s, 40 tuples returned/s, 5 temp files, 11.50M temp size
  * Worker processes: 3/8 total, 1/8 logical workers, 2/8 parallel workers
    Other processes & info: 3/3 autovacuum workers, 1/10 wal senders, 0 wal receivers, 10/10 repl. slots
                                 RUNNING QUERIES
-PID    DATABASE                     USER           CLIENT IOW              state Query
+PID    DATABASE              USER       CLIENT IOW              state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -224,15 +230,15 @@
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key 'o' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 2s - Duration mode: query
  * Global: 132 days, 3 hours and 21 minutes uptime, 19.53M dbs size - 1.00K/s growth, 90.12% cache hit ratio
    Sessions: 6/100 total, 1 active, 1 idle, 10 idle in txn, 0 idle in txn abrt, 3 waiting
    Activity: 15 tps, 10 insert/s, 20 update/s, 30 delete/s, 40 tuples returned/s, 5 temp files, 11.50M temp size
                                 RUNNING QUERIES
-PID    DATABASE                     USER           CLIENT IOW              state Query
+PID    DATABASE              USER       CLIENT IOW              state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -248,15 +254,15 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key 'i' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 2s - Duration mode: query
                                 RUNNING QUERIES
-PID    DATABASE                     USER           CLIENT IOW              state Query
+PID    DATABASE              USER       CLIENT IOW              state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -302,15 +308,15 @@
       F2/2: waiting queries
       F3/3: blocking queries
 <BLANKLINE>
 Press any key to exit.
 ------------------------------------------------------------------------------------------- sending key 'z' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 2s - Duration mode: query
                                 RUNNING QUERIES
-PID    DATABASE                     USER           CLIENT IOW              state Query
+PID    DATABASE              USER       CLIENT IOW              state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -347,15 +353,15 @@
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 2s - Duration mode: query
  * Global: 132 days, 3 hours and 21 minutes uptime, 19.53M dbs size - 1.00K/s growth, 90.12% cache hit ratio
    Sessions: 6/100 total, 1 active, 1 idle, 10 idle in txn, 0 idle in txn abrt, 3 waiting
    Activity: 15 tps, 10 insert/s, 20 update/s, 30 delete/s, 40 tuples returned/s, 5 temp files, 11.50M temp size
  * Worker processes: 3/8 total, 1/8 logical workers, 2/8 parallel workers
    Other processes & info: 3/3 autovacuum workers, 1/10 wal senders, 0 wal receivers, 10/10 repl. slots
                                 RUNNING QUERIES
-PID    DATABASE                     USER           CLIENT             state Query
+PID    DATABASE              USER       CLIENT             state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -394,15 +400,15 @@
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 2s - Duration mode: query
  * Global: 132 days, 3 hours and 21 minutes uptime, 19.53M dbs size - 1.00K/s growth, 90.12% cache hit ratio
    Sessions: 6/100 total, 1 active, 1 idle, 10 idle in txn, 0 idle in txn abrt, 3 waiting
    Activity: 15 tps, 10 insert/s, 20 update/s, 30 delete/s, 40 tuples returned/s, 5 temp files, 11.50M temp size
  * Worker processes: 3/8 total, 1/8 logical workers, 2/8 parallel workers
    Other processes & info: 3/3 autovacuum workers, 1/10 wal senders, 0 wal receivers, 10/10 repl. slots
                                 RUNNING QUERIES
-PID    DATABASE                     USER           CLIENT             state Query
+PID    DATABASE              USER       CLIENT             state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -432,16 +438,16 @@
 
 >>> keys = ["-", "-", "+", " ", "T", "3", "r", " ", "T", "c", "2", "1", "3", "q"]
 >>> expected_timeouts = [2.0, 1.0, 0.5, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
 >>> assert len(keys) == len(expected_timeouts)
 >>> run_ui(options, keys, expected_timeouts=expected_timeouts)  # doctest: +ELLIPSIS
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 2s - Duration mode: query
                                 RUNNING QUERIES
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -458,16 +464,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key '-' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: query
                                 RUNNING QUERIES
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -484,16 +490,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key '-' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 0.5s - Duration mode: query
                                 RUNNING QUERIES
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -510,16 +516,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key '+' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: query
                                 RUNNING QUERIES
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -536,16 +542,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key ' ' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: query
                                      PAUSE
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -562,16 +568,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key 'T' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: query
                                      PAUSE
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -588,16 +594,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key '3' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: query
                                      PAUSE
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -614,16 +620,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key 'r' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: query
                                      PAUSE
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -640,16 +646,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key ' ' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: query
                                 RUNNING QUERIES
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -666,16 +672,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key 'T' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: transaction
                                 RUNNING QUERIES
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -692,16 +698,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key 'c' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: transaction
                                 RUNNING QUERIES
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -718,15 +724,15 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key '2' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: transaction
                                 WAITING QUERIES
-DATABASE                     USER           CLIENT  RELATION             TYPE             MODE             state Query
+DATABASE              USER       CLIENT  RELATION             TYPE             MODE             state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -744,16 +750,16 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key '1' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: transaction
                                 RUNNING QUERIES
-DATABASE                     USER           CLIENT             state Query
-tests                    postgres     127.0.0.1/32     idle in trans SELECT pg_sleep(0)
+DATABASE              USER       CLIENT             state Query
+tests             postgres    127.0.0.1     idle in trans SELECT pg_sleep(0)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -770,15 +776,15 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 ------------------------------------------------------------------------------------------- sending key '3' --------------------------------------------------------------------------------------------
 PostgreSQL ... - test - postgres@127.0.0.1:.../tests - Ref.: 1s - Duration mode: transaction
                                 BLOCKING QUERIES
-DATABASE                     USER           CLIENT  RELATION             TYPE             MODE             state Query
+DATABASE              USER       CLIENT  RELATION             TYPE             MODE             state Query
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -807,26 +813,31 @@
 >>> output = getfixture("tmp_path") / "activities.csv"
 >>> options = argparse.Namespace(
 ...     **dict(
 ...         defaults,
 ...         durationmode="2",
 ...         wrap_query=True,
 ...         noclient=True,
-...         nouser=True,
 ...         nodbsize=True,
 ...         notempfiles=False,
 ...         nowalreceiver=False,
 ...         output=str(output),
 ...     ),
 ... )
->>> run_ui(options, ["D", "v", "q"], width=100, render_header=False)
+>>> cfg = mkconfig({
+...     "client": {"hidden": False},
+...     "state": {"width": 6},
+...     "database": {"width": 10},
+...     "user": {"hidden": True},
+... })
+>>> run_ui(options, ["D", "v", "q"], config=cfg, width=80, render_header=False)
                                 RUNNING QUERIES
-DATABASE                     state Query
-tests                idle in trans CREATE TABLE persons (firstname text, lastname text, age int,
-                                    address text)
+DATABASE    state Query
+tests      idle i CREATE TABLE persons (firstname text, lastname text, age int,
+                   address text)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -840,19 +851,19 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
------------------------------------------ sending key 'D' ------------------------------------------
+------------------------------- sending key 'D' --------------------------------
                                 RUNNING QUERIES
-DATABASE                     state Query
-tests                idle in trans CREATE TABLE persons (firstname text, lastname text, age int,
-                                    address text)
+DATABASE    state Query
+tests      idle i CREATE TABLE persons (firstname text, lastname text, age int,
+                   address text)
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -866,18 +877,18 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
------------------------------------------ sending key 'v' ------------------------------------------
+------------------------------- sending key 'v' --------------------------------
                                 RUNNING QUERIES
-DATABASE                     state Query
-tests                idle in trans CREATE TABLE persons (firstname text, lastname text, age int, ad
+DATABASE    state Query
+tests      idle i CREATE TABLE persons (firstname text, lastname text, age int,
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
@@ -892,15 +903,15 @@
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
 <BLANKLINE>
------------------------------------------ sending key 'q' ------------------------------------------
+------------------------------- sending key 'q' --------------------------------
 >>> with output.open() as f:
 ...     lines = f.readlines()
 >>> len(lines)
 4
 
 >>> _ = postgres.execute("CREATE TABLE t (s text)")
 >>> _ = postgres.execute("INSERT INTO t VALUES ('init')")
```

### Comparing `pg_activity-3.3.0/tests/test_views.py` & `pg-activity-3.4.0/tests/test_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from blessed import Terminal
 
 from pgactivity import views
-from pgactivity.types import UI, Flag, QueryMode, SortKey
+from pgactivity.config import Flag
+from pgactivity.types import UI, QueryMode, SortKey
 
 
 @pytest.fixture
 def term() -> Terminal:
     return Terminal()
```

### Comparing `pg_activity-3.3.0/tests/test_views.txt` & `pg-activity-3.4.0/tests/test_views.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+>>> from ipaddress import ip_address, ip_interface
 >>> import attr
 >>> from blessed import Terminal
 >>> import os
+>>> from pgactivity.config import Flag
 >>> from pgactivity.types import *
 >>> from pgactivity.views import *
 
 >>> os.environ["LINES"] = "26"
 >>> term = Terminal(force_styling=None)
 >>> term.width, term.height
 (80, 26)
@@ -206,15 +208,15 @@
 
 >>> processes1 = [
 ...     LocalRunningProcess(
 ...         pid="6239",
 ...         application_name="pgbench",
 ...         database="pgbench",
 ...         user="postgres",
-...         client="local",
+...         client=None,
 ...         cpu=0.1,
 ...         mem=0.993_254_939_413_836,
 ...         read=7,
 ...         write=12.3,
 ...         state="idle in transaction",
 ...         query="UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 1932841;",
 ...         encoding="UTF-8",
@@ -225,15 +227,15 @@
 ...         is_parallel_worker=False,
 ...     ),
 ...     LocalRunningProcess(
 ...         pid="6228",
 ...         application_name="pgbench",
 ...         database="pgbench",
 ...         user="postgres",
-...         client="local",
+...         client=None,
 ...         cpu=0.2,
 ...         mem=1.024_758_418_061_11,
 ...         read=0.2,
 ...         write=1_128_201,
 ...         state="active",
 ...         query="UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 1932841;",
 ...         encoding="UTF-8",
@@ -244,15 +246,15 @@
 ...         is_parallel_worker=True,
 ...     ),
 ...     LocalRunningProcess(
 ...         pid="1234",
 ...         application_name="accounting",
 ...         database="business",
 ...         user="bob",
-...         client="local",
+...         client=None,
 ...         cpu=2.4,
 ...         mem=1.031_191_760_016_45,
 ...         read=9_876_543.21,
 ...         write=1_234,
 ...         state="active",
 ...         query="SELECT product_id, p.name FROM products p LEFT JOIN sales s USING (product_id) WHERE s.date > CURRENT_DATE - INTERVAL '4 weeks' GROUP BY product_id, p.name, p.price, p.cost HAVING sum(p.price * s.units) > 5000;",
 ...         encoding="UTF-8",
@@ -326,30 +328,30 @@
 
 >>> processes2 = [
 ...     BlockingProcess(
 ...         pid="6239",
 ...         application_name="pgbench",
 ...         database="pgbench",
 ...         user="postgres",
-...         client="1.2.3.4",
+...         client=ip_address("1.2.3.4"),
 ...         mode="ExclusiveLock",
 ...         type="transactionid",
 ...         relation="None",
 ...         duration=666,
 ...         wait="Client Read",
 ...         state="active",
 ...         query="END;",
 ...         encoding="UTF-8",
 ...     ),
 ...     BlockingProcess(
 ...         pid="6228",
 ...         application_name="pgbench",
 ...         database="pgbench",
 ...         user="postgres",
-...         client="local",
+...         client=ip_interface("2001:4f8:3:ba:2e0:81ff:fe22:d1f1/128"),
 ...         mode="RowExclusiveLock",
 ...         type="tuple",
 ...         relation="ahah",
 ...         duration=0.000413,
 ...         wait="Client Read",
 ...         state="idle in transaction",
 ...         query="UPDATE pgbench_branches SET bbalance = bbalance + 1788 WHERE bid = 68;",
@@ -360,65 +362,65 @@
 >>> processes_rows(term, ui, SelectableProcesses(processes2), 100)
 6239   pgbench                     active END;
 6228   pgbench              idle in trans UPDATE pgbench_branches SET bbalance
                                            = bbalance + 1788 WHERE bid = 68;
 >>> ui = UI.make(query_mode=QueryMode.blocking, flag=allflags)
 >>> processes_rows(term, ui, SelectableProcesses(processes2), 100, width=250)
 6239   pgbench                   pgbench         postgres          1.2.3.4      None    transactionid    ExclusiveLock  11:06.00      Client Read            active END;
-6228   pgbench                   pgbench         postgres            local      ahah            tuple RowExclusiveLock  0.000413      Client Read     idle in trans UPDATE pgbench_branches SET bbalance = bbalance + 1788 WHERE bid = 68;
+6228   pgbench                   pgbench         postgres 2001:4f8:3:ba:2e      ahah            tuple RowExclusiveLock  0.000413      Client Read     idle in trans UPDATE pgbench_branches SET bbalance = bbalance + 1788 WHERE bid = 68;
 
 >>> processes1b = [
 ...     RunningProcess(
 ...         pid=6239,
 ...         application_name="pgbench",
 ...         database="pgbench",
 ...         user="postgres",
-...         client="local",
+...         client=ip_interface("2001:db8::1/96"),
 ...         state="idle in transaction",
 ...         query="UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 1932841;",
 ...         encoding="UTF-8",
 ...         duration=0.0,
 ...         wait=False,
 ...         query_leader_pid=6239,
 ...         is_parallel_worker=False,
 ...     ),
 ...     RunningProcess(
 ...         pid=6228,
 ...         application_name="none",
 ...         database="pgbench",
 ...         user="postgres",
-...         client="local",
+...         client=ip_interface("10.1.0.0/16"),
 ...         state="active",
 ...         query="UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 1932841;",
 ...         encoding="UTF-8",
 ...         duration=0.000413,
 ...         wait=True,
 ...         query_leader_pid=6239,
 ...         is_parallel_worker=True,
 ...     ),
 ...     RunningProcess(
 ...         pid=1234,
 ...         application_name="accounting",
 ...         database="business",
 ...         user="bob",
-...         client="192.168.0.47",
+...         client=ip_address("192.168.0.47"),
 ...         state="active",
 ...         query="SELECT product_id, p.name FROM products p LEFT JOIN sales s USING (product_id) WHERE s.date > CURRENT_DATE - INTERVAL '4 weeks' GROUP BY product_id, p.name, p.price, p.cost HAVING sum(p.price * s.units) > 5000;",
 ...         encoding="UTF-8",
 ...         duration=1234,
 ...         wait="clog",
 ...         query_leader_pid=1234,
 ...         is_parallel_worker=False,
 ...     ),
 ... ]
 >>> all_but_local_flags = Flag.PID|Flag.DATABASE|Flag.APPNAME|Flag.USER|Flag.CLIENT|Flag.TIME|Flag.WAIT
 >>> ui = UI.make(query_mode=QueryMode.activities,flag=all_but_local_flags)
 >>> processes_rows(term, ui, SelectableProcesses(processes1b), 100, width=200)
-6239   pgbench                   pgbench         postgres            local  0.000000                N     idle in trans UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 1932841;
-6228   pgbench                      none         postgres            local  0.000413                Y            active \_ UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 1932841;
+6239   pgbench                   pgbench         postgres   2001:db8::1/96  0.000000                N     idle in trans UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 1932841;
+6228   pgbench                      none         postgres      10.1.0.0/16  0.000413                Y            active \_ UPDATE pgbench_accounts SET abalance = abalance + 141 WHERE aid = 1932841;
 1234   business               accounting              bob     192.168.0.47  20:34.00             clog            active SELECT product_id, p.name FROM products p LEFT JOIN sales s USING (product_id)
 
 Tests for footer_*()
 --------------------
 
 >>> footer_help(term, width=85)
 F1/1 Running  F2/2 Waiting  F3/3 Blocking Space Pause/u q Quit        h Help
```

### Comparing `pg_activity-3.3.0/tests/test_widgets.txt` & `pg-activity-3.4.0/tests/test_widgets.txt`

 * *Files identical despite different names*

