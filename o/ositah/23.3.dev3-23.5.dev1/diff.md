# Comparing `tmp/ositah-23.3.dev3.tar.gz` & `tmp/ositah-23.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ositah-23.3.dev3.tar", last modified: Sat Mar 11 11:11:49 2023, max compression
+gzip compressed data, was "ositah-23.5.dev1.tar", last modified: Mon May 15 16:33:35 2023, max compression
```

## Comparing `ositah-23.3.dev3.tar` & `ositah-23.5.dev1.tar`

### file list

```diff
@@ -1,77 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.151095 ositah-23.3.dev3/
--rw-rw-rw-   0        0        0       84 2022-11-13 21:10:36.000000 ositah-23.3.dev3/.gitignore
--rw-rw-rw-   0        0        0      341 2023-02-13 17:50:27.000000 ositah-23.3.dev3/.gitlab-ci.yml
--rw-rw-rw-   0        0        0     1550 2022-10-27 13:39:35.000000 ositah-23.3.dev3/LICENSE
--rw-rw-rw-   0        0        0     7693 2023-03-11 11:11:49.151095 ositah-23.3.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     7119 2022-11-13 21:13:24.000000 ositah-23.3.dev3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.061528 ositah-23.3.dev3/gunicorn.config/
--rw-rw-rw-   0        0        0      643 2022-11-13 21:10:36.000000 ositah-23.3.dev3/gunicorn.config/README.md
--rw-rw-rw-   0        0        0      141 2022-11-13 21:10:36.000000 ositah-23.3.dev3/gunicorn.config/gunicorn.ositah
--rw-rw-rw-   0        0        0      379 2022-11-13 21:10:36.000000 ositah-23.3.dev3/gunicorn.config/gunicorn@.service
--rw-rw-rw-   0        0        0      369 2022-11-13 21:10:36.000000 ositah-23.3.dev3/gunicorn.config/ositah.conf.py
--rw-rw-rw-   0        0        0     1243 2022-11-13 21:10:36.000000 ositah-23.3.dev3/noxfile.py
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.067523 ositah-23.3.dev3/ositah/
--rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-23.3.dev3/ositah/__init__.py
--rw-rw-rw-   0        0        0      428 2023-03-02 17:58:31.000000 ositah-23.3.dev3/ositah/app.py
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.091534 ositah-23.3.dev3/ositah/apps/
--rw-rw-rw-   0        0        0    28259 2023-02-26 18:01:44.000000 ositah-23.3.dev3/ositah/apps/analysis.py
--rw-rw-rw-   0        0        0    34803 2023-03-11 10:27:03.000000 ositah-23.3.dev3/ositah/apps/configuration.py
--rw-rw-rw-   0        0        0    47246 2023-02-27 19:50:46.000000 ositah-23.3.dev3/ositah/apps/export.py
--rw-rw-rw-   0        0        0    53059 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/apps/validation.py
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.098089 ositah-23.3.dev3/ositah/assets/
--rw-rw-rw-   0        0        0      503 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/arrow_down_up.svg
--rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/ositah.css
--rw-rw-rw-   0        0        0      593 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/sort_ascending.svg
--rw-rw-rw-   0        0        0      618 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/sort_descending.svg
--rw-rw-rw-   0        0        0    17478 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/assets/sorttable.js
--rw-rw-rw-   0        0        0    15685 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/main.py
--rw-rw-rw-   0        0        0     7471 2023-02-24 17:01:35.000000 ositah-23.3.dev3/ositah/ositah.example.cfg
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.101091 ositah-23.3.dev3/ositah/static/
--rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/static/style.css
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.105093 ositah-23.3.dev3/ositah/templates/
--rw-rw-rw-   0        0        0      714 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/templates/base.html
--rw-rw-rw-   0        0        0     1608 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/templates/bootstrap_login.html
--rw-rw-rw-   0        0        0     1033 2022-11-13 21:10:36.000000 ositah-23.3.dev3/ositah/templates/login_form.html
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.124090 ositah-23.3.dev3/ositah/utils/
--rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-23.3.dev3/ositah/utils/__init__.py
--rw-rw-rw-   0        0        0     4453 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/agents.py
--rw-rw-rw-   0        0        0     9149 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/authentication.py
--rw-rw-rw-   0        0        0      504 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/cache.py
--rw-rw-rw-   0        0        0      295 2023-02-26 18:01:44.000000 ositah-23.3.dev3/ositah/utils/core.py
--rw-rw-rw-   0        0        0     1500 2023-02-24 18:11:54.000000 ositah-23.3.dev3/ositah/utils/exceptions.py
--rw-rw-rw-   0        0        0     1510 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/hito_db.py
--rw-rw-rw-   0        0        0     8988 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/hito_db_model.py
--rw-rw-rw-   0        0        0    11127 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/menus.py
--rw-rw-rw-   0        0        0     3617 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/period.py
--rw-rw-rw-   0        0        0    39683 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/projects.py
--rw-rw-rw-   0        0        0     1186 2023-02-24 18:11:54.000000 ositah-23.3.dev3/ositah/utils/teams.py
--rw-rw-rw-   0        0        0    16370 2023-03-10 16:43:58.000000 ositah-23.3.dev3/ositah/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.086534 ositah-23.3.dev3/ositah.egg-info/
--rw-rw-rw-   0        0        0     7693 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2023-03-11 11:11:49.000000 ositah-23.3.dev3/ositah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      181 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-11 11:11:48.000000 ositah-23.3.dev3/ositah.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-03-11 11:10:11.000000 ositah-23.3.dev3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-11 11:11:49.152094 ositah-23.3.dev3/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-11-13 21:10:36.000000 ositah-23.3.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.145105 ositah-23.3.dev3/test-dash/
--rw-rw-rw-   0        0        0       87 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/README.md
--rw-rw-rw-   0        0        0     2965 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/accordion.py
--rw-rw-rw-   0        0        0     4387 2023-02-24 17:01:35.000000 ositah-23.3.dev3/test-dash/authentication.py
--rw-rw-rw-   0        0        0     2092 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/checkbox.py
--rw-rw-rw-   0        0        0     3581 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/checklist.py
--rw-rw-rw-   0        0        0      602 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/file-selector.py
--rw-rw-rw-   0        0        0     3068 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/file-upload.py
--rw-rw-rw-   0        0        0     2734 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/long_running_callback.py
--rw-rw-rw-   0        0        0     2394 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/pandas_split.py
--rw-rw-rw-   0        0        0     1888 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/pandas_split_bug_report.py
--rw-rw-rw-   0        0        0     1413 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/pattern-matching-callback.py
--rw-rw-rw-   0        0        0     4189 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/progess_bar.py
--rw-rw-rw-   0        0        0     2679 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/reset_table_checkboxes.py
--rw-rw-rw-   0        0        0     4377 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/sortable_table.py
--rw-rw-rw-   0        0        0     1159 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/sqlalchemy_test.py
-drwxrwxrwx   0        0        0        0 2023-03-11 11:11:49.149097 ositah-23.3.dev3/test-dash/templates/
--rw-rw-rw-   0        0        0      500 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/templates/base.html
--rw-rw-rw-   0        0        0      680 2022-11-13 21:10:36.000000 ositah-23.3.dev3/test-dash/templates/login_form.html
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:35.024794 ositah-23.5.dev1/
+-rw-rw-rw-   0        0        0       84 2022-11-13 21:10:36.000000 ositah-23.5.dev1/.gitignore
+-rw-rw-rw-   0        0        0      341 2023-02-13 17:50:27.000000 ositah-23.5.dev1/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     1550 2022-10-27 13:39:35.000000 ositah-23.5.dev1/LICENSE
+-rw-rw-rw-   0        0        0     7693 2023-05-15 16:33:35.023793 ositah-23.5.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     7119 2022-11-13 21:13:24.000000 ositah-23.5.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.701452 ositah-23.5.dev1/gunicorn.config/
+-rw-rw-rw-   0        0        0      643 2022-11-13 21:10:36.000000 ositah-23.5.dev1/gunicorn.config/README.md
+-rw-rw-rw-   0        0        0      141 2022-11-13 21:10:36.000000 ositah-23.5.dev1/gunicorn.config/gunicorn.ositah
+-rw-rw-rw-   0        0        0      379 2022-11-13 21:10:36.000000 ositah-23.5.dev1/gunicorn.config/gunicorn@.service
+-rw-rw-rw-   0        0        0      369 2022-11-13 21:10:36.000000 ositah-23.5.dev1/gunicorn.config/ositah.conf.py
+-rw-rw-rw-   0        0        0     1337 2023-05-12 19:47:31.000000 ositah-23.5.dev1/noxfile.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.708237 ositah-23.5.dev1/ositah/
+-rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-23.5.dev1/ositah/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-03-02 17:58:31.000000 ositah-23.5.dev1/ositah/app.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.759908 ositah-23.5.dev1/ositah/apps/
+-rw-rw-rw-   0        0        0        0 2023-05-05 13:26:50.000000 ositah-23.5.dev1/ositah/apps/__init__.py
+-rw-rw-rw-   0        0        0    28259 2023-02-26 18:01:44.000000 ositah-23.5.dev1/ositah/apps/analysis.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.769825 ositah-23.5.dev1/ositah/apps/configuration/
+-rw-rw-rw-   0        0        0        0 2023-05-05 13:26:50.000000 ositah-23.5.dev1/ositah/apps/configuration/__init__.py
+-rw-rw-rw-   0        0        0    33477 2023-05-15 16:13:36.000000 ositah-23.5.dev1/ositah/apps/configuration/callbacks.py
+-rw-rw-rw-   0        0        0    20233 2023-05-15 16:11:17.000000 ositah-23.5.dev1/ositah/apps/configuration/main.py
+-rw-rw-rw-   0        0        0     3862 2023-05-13 00:10:24.000000 ositah-23.5.dev1/ositah/apps/configuration/parameters.py
+-rw-rw-rw-   0        0        0     3982 2023-05-15 16:11:18.000000 ositah-23.5.dev1/ositah/apps/configuration/tools.py
+-rw-rw-rw-   0        0        0    47246 2023-05-05 13:57:21.000000 ositah-23.5.dev1/ositah/apps/export.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.782539 ositah-23.5.dev1/ositah/apps/validation/
+-rw-rw-rw-   0        0        0        0 2023-05-12 19:47:31.000000 ositah-23.5.dev1/ositah/apps/validation/__init__.py
+-rw-rw-rw-   0        0        0     9390 2023-05-12 19:47:31.000000 ositah-23.5.dev1/ositah/apps/validation/callbacks.py
+-rw-rw-rw-   0        0        0     2896 2023-05-12 19:47:31.000000 ositah-23.5.dev1/ositah/apps/validation/main.py
+-rw-rw-rw-   0        0        0     1003 2023-05-12 19:47:31.000000 ositah-23.5.dev1/ositah/apps/validation/parameters.py
+-rw-rw-rw-   0        0        0    23824 2023-05-12 19:47:31.000000 ositah-23.5.dev1/ositah/apps/validation/tables.py
+-rw-rw-rw-   0        0        0    18046 2023-05-12 19:47:31.000000 ositah-23.5.dev1/ositah/apps/validation/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.791581 ositah-23.5.dev1/ositah/assets/
+-rw-rw-rw-   0        0        0      503 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/assets/arrow_down_up.svg
+-rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/assets/ositah.css
+-rw-rw-rw-   0        0        0      593 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/assets/sort_ascending.svg
+-rw-rw-rw-   0        0        0      618 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/assets/sort_descending.svg
+-rw-rw-rw-   0        0        0    17478 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/assets/sorttable.js
+-rw-rw-rw-   0        0        0    15696 2023-05-12 19:47:31.000000 ositah-23.5.dev1/ositah/main.py
+-rw-rw-rw-   0        0        0     7471 2023-02-24 17:01:35.000000 ositah-23.5.dev1/ositah/ositah.example.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.793518 ositah-23.5.dev1/ositah/static/
+-rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/static/style.css
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.800512 ositah-23.5.dev1/ositah/templates/
+-rw-rw-rw-   0        0        0      714 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/templates/base.html
+-rw-rw-rw-   0        0        0     1608 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/templates/bootstrap_login.html
+-rw-rw-rw-   0        0        0     1033 2022-11-13 21:10:36.000000 ositah-23.5.dev1/ositah/templates/login_form.html
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.828083 ositah-23.5.dev1/ositah/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-23.5.dev1/ositah/utils/__init__.py
+-rw-rw-rw-   0        0        0     4453 2023-03-11 12:02:31.000000 ositah-23.5.dev1/ositah/utils/agents.py
+-rw-rw-rw-   0        0        0     9149 2023-03-11 12:02:31.000000 ositah-23.5.dev1/ositah/utils/authentication.py
+-rw-rw-rw-   0        0        0      504 2023-03-11 12:02:31.000000 ositah-23.5.dev1/ositah/utils/cache.py
+-rw-rw-rw-   0        0        0      295 2023-02-26 18:01:44.000000 ositah-23.5.dev1/ositah/utils/core.py
+-rw-rw-rw-   0        0        0     1500 2023-02-24 18:11:54.000000 ositah-23.5.dev1/ositah/utils/exceptions.py
+-rw-rw-rw-   0        0        0     1510 2023-03-11 12:02:31.000000 ositah-23.5.dev1/ositah/utils/hito_db.py
+-rw-rw-rw-   0        0        0     8988 2023-03-11 12:02:31.000000 ositah-23.5.dev1/ositah/utils/hito_db_model.py
+-rw-rw-rw-   0        0        0    11127 2023-03-14 15:36:17.000000 ositah-23.5.dev1/ositah/utils/menus.py
+-rw-rw-rw-   0        0        0     4058 2023-03-15 09:13:49.000000 ositah-23.5.dev1/ositah/utils/period.py
+-rw-rw-rw-   0        0        0    42826 2023-05-15 16:31:58.000000 ositah-23.5.dev1/ositah/utils/projects.py
+-rw-rw-rw-   0        0        0     1186 2023-02-24 18:11:54.000000 ositah-23.5.dev1/ositah/utils/teams.py
+-rw-rw-rw-   0        0        0    16370 2023-03-11 12:02:31.000000 ositah-23.5.dev1/ositah/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:34.754943 ositah-23.5.dev1/ositah.egg-info/
+-rw-rw-rw-   0        0        0     7693 2023-05-15 16:33:34.000000 ositah-23.5.dev1/ositah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1996 2023-05-15 16:33:34.000000 ositah-23.5.dev1/ositah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 16:33:34.000000 ositah-23.5.dev1/ositah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-15 16:33:34.000000 ositah-23.5.dev1/ositah.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      181 2023-05-15 16:33:34.000000 ositah-23.5.dev1/ositah.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 16:33:34.000000 ositah-23.5.dev1/ositah.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-05-15 16:31:58.000000 ositah-23.5.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 16:33:35.024794 ositah-23.5.dev1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-11-13 21:10:36.000000 ositah-23.5.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:35.003742 ositah-23.5.dev1/test-dash/
+-rw-rw-rw-   0        0        0       87 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/README.md
+-rw-rw-rw-   0        0        0     2965 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/accordion.py
+-rw-rw-rw-   0        0        0     4387 2023-02-24 17:01:35.000000 ositah-23.5.dev1/test-dash/authentication.py
+-rw-rw-rw-   0        0        0     2092 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/checkbox.py
+-rw-rw-rw-   0        0        0     3581 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/checklist.py
+-rw-rw-rw-   0        0        0      602 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/file-selector.py
+-rw-rw-rw-   0        0        0     3068 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/file-upload.py
+-rw-rw-rw-   0        0        0     2734 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/long_running_callback.py
+-rw-rw-rw-   0        0        0     2394 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/pandas_split.py
+-rw-rw-rw-   0        0        0     1888 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/pandas_split_bug_report.py
+-rw-rw-rw-   0        0        0     1413 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/pattern-matching-callback.py
+-rw-rw-rw-   0        0        0     4189 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/progess_bar.py
+-rw-rw-rw-   0        0        0     2679 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/reset_table_checkboxes.py
+-rw-rw-rw-   0        0        0     4377 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/sortable_table.py
+-rw-rw-rw-   0        0        0     1159 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/sqlalchemy_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:33:35.021356 ositah-23.5.dev1/test-dash/templates/
+-rw-rw-rw-   0        0        0      500 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/templates/base.html
+-rw-rw-rw-   0        0        0      680 2022-11-13 21:10:36.000000 ositah-23.5.dev1/test-dash/templates/login_form.html
```

### Comparing `ositah-23.3.dev3/LICENSE` & `ositah-23.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/PKG-INFO` & `ositah-23.5.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ositah
-Version: 23.3.dev3
+Version: 23.5.dev1
 Summary: Outils de Suivi d'Activités basé sur Hito
 Author-email: Michel Jouvin <michel.jouvin@ijclab.in2p3.fr>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://gitlab.in2p3.fr/hito/ositah
 Project-URL: Bug Tracker, https://gitlab.in2p3.fr/hito/ositah/-/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ositah-23.3.dev3/README.md` & `ositah-23.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/gunicorn.config/README.md` & `ositah-23.5.dev1/gunicorn.config/README.md`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/noxfile.py` & `ositah-23.5.dev1/noxfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 MAX_LINE_LEN = 100
 
 
 @nox.session()
 def lint(session):
     session.install("black", "flake8", "isort")
     session.run("black", "--check", "-l", str(MAX_LINE_LEN), *SOURCES)
-    session.run("flake8", "--max-line-length", str(MAX_LINE_LEN), *SOURCES)
+    session.run("flake8", "--max-line-length", str(MAX_LINE_LEN), "--per-file-ignores", "ositah/apps/*/callbacks.py:F403,F405 ositah/apps/*/main.py:F403,F405", *SOURCES)
     session.run("isort", "--check", "--profile", "black", "-l", str(MAX_LINE_LEN), *SOURCES)
 
 
 @nox.session(name="format")
 def format_(session):
     session.install("black", "isort")
     session.run("black", "-l", str(MAX_LINE_LEN), *SOURCES)
```

### Comparing `ositah-23.3.dev3/ositah/apps/analysis.py` & `ositah-23.5.dev1/ositah/apps/analysis.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/apps/export.py` & `ositah-23.5.dev1/ositah/apps/export.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/assets/ositah.css` & `ositah-23.5.dev1/ositah/assets/ositah.css`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/assets/sort_ascending.svg` & `ositah-23.5.dev1/ositah/assets/sort_ascending.svg`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/assets/sort_descending.svg` & `ositah-23.5.dev1/ositah/assets/sort_descending.svg`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/assets/sorttable.js` & `ositah-23.5.dev1/ositah/assets/sorttable.js`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/main.py` & `ositah-23.5.dev1/ositah/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import dash_bootstrap_components as dbc
 from dash import dcc, html
 from dash.dependencies import Input, Output, State
 from flask import session
 
 from ositah.app import app
 from ositah.apps.analysis import analysis_layout
-from ositah.apps.configuration import configuration_layout
+from ositah.apps.configuration.main import configuration_layout
 from ositah.apps.export import export_layout
-from ositah.apps.validation import validation_layout
+from ositah.apps.validation.main import validation_layout
 from ositah.utils.agents import get_agent_by_email
 from ositah.utils.authentication import (
     LOGIN_URL,
     LOGOUT_URL,
     SESSION_MAX_DURATION,
     configure_multipass_ldap,
     identity_list,
@@ -323,15 +323,15 @@
 
     protect_views(app)
 
     # Import from hito_db must not be done after configuration has been loaded
     from ositah.utils.hito_db import get_db
 
     # Initialize DB connection by calling get_db()
-    get_db(init_session=None)
+    get_db(init_session=False)
 
     sidebar = html.Div(
         [
             html.H2("OSITAH", className="display-4"),
             html.Hr(),
             html.P("Suivi des déclarations de temps", className="lead"),
             dbc.Nav(
```

### Comparing `ositah-23.3.dev3/ositah/ositah.example.cfg` & `ositah-23.5.dev1/ositah/ositah.example.cfg`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/static/style.css` & `ositah-23.5.dev1/ositah/static/style.css`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/templates/base.html` & `ositah-23.5.dev1/ositah/templates/base.html`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/templates/bootstrap_login.html` & `ositah-23.5.dev1/ositah/templates/bootstrap_login.html`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/templates/login_form.html` & `ositah-23.5.dev1/ositah/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/utils/agents.py` & `ositah-23.5.dev1/ositah/utils/agents.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/utils/authentication.py` & `ositah-23.5.dev1/ositah/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/utils/exceptions.py` & `ositah-23.5.dev1/ositah/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/utils/hito_db.py` & `ositah-23.5.dev1/ositah/utils/hito_db.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/utils/hito_db_model.py` & `ositah-23.5.dev1/ositah/utils/hito_db_model.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/utils/menus.py` & `ositah-23.5.dev1/ositah/utils/menus.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/utils/period.py` & `ositah-23.5.dev1/ositah/utils/period.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from datetime import datetime
 from typing import List
 
 from ositah.utils.exceptions import ValidationPeriodAmbiguous, ValidationPeriodMissing
 
 
 class OSITAHDeclarationPeriod:
-    def __init__(self, name: str, start_date: str, end_date: str):
+    def __init__(self, name: str, start_date: str, end_date: str, validation_date: str):
         self._name = name
         self._start_date = start_date
         self._end_date = end_date
+        self._validation_date = validation_date
 
     @property
     def name(self):
         return self._name
 
     @property
     def dates(self):
@@ -28,14 +29,18 @@
     def end_date(self):
         return self._end_date
 
     @property
     def start_date(self):
         return self._start_date
 
+    @property
+    def validation_date(self):
+        return self._validation_date
+
 
 def get_validation_period_data(period_date: str):
     """
     Return the current declaration period object.
 
     :param period_date: a date that must be inside the declaration period
     :return: declaration period object (OSITAHValidationPeriod)
@@ -75,36 +80,40 @@
     :param period_date: a date that must be inside the declaration period
     :return: UUID
     """
 
     return get_validation_period_data(period_date).id
 
 
-def get_declaration_periods():
+def get_declaration_periods(descending: bool = True) -> List[OSITAHDeclarationPeriod]:
     """
     Return a list of declaration period name and dates, sorted by start date in descending order.
     Dates are strings, without the time information.
 
+    :param descending: if True, sort in descending order (default), else in ascending order
     :return: list of OSITAHDeclarationPeriod
     """
 
     from ositah.utils.hito_db_model import OSITAHValidationPeriod
 
     periods = []
 
     periods_data = OSITAHValidationPeriod.query.order_by(
         OSITAHValidationPeriod.start_date.desc()
+        if descending
+        else OSITAHValidationPeriod.start_date.asc()
     ).all()
 
     for row in periods_data:
         periods.append(
             OSITAHDeclarationPeriod(
                 row.name,
                 row.start_date.date().isoformat(),
                 row.end_date.date().isoformat(),
+                row.validation_date.date().isoformat(),
             )
         )
 
     return periods
 
 
 def get_default_period_date(periods: List[OSITAHDeclarationPeriod], date: datetime.date):
```

### Comparing `ositah-23.3.dev3/ositah/utils/projects.py` & `ositah-23.5.dev1/ositah/utils/projects.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 DATA_SOURCE_HITO = "hito"
 DATA_SOURCE_OSITAH = "ositah"
 
 NSIP_CLASS_OTHER_ACTIVITY = "activitensipreferentiel"
 NSIP_CLASS_PROJECT = "projetnsipreferentiel"
 
-NSIP_DELETED_ACTIVITY_MASTERPROJECT = "Disabled"
+MASTERPROJECT_DELETED_ACTIVITY = "Disabled"
+MASTERPROJECT_LOCAL_PROJECT = "Local Projects"
 
 NSIP_PROJECT_ORDER = 1
 LOCAL_PROJECT_ORDER = 2
 NSIP_ACIVITY_ORDER = 3
 DISABLED_ACTIVITY_ORDER = 9999
 
 
@@ -368,21 +369,21 @@
             values=[columns["hours"], columns["quotite"]],
             aggfunc={columns["hours"]: np.sum, columns["quotite"]: np.mean},
         )
         declarations = pd.DataFrame(global_declarations_pt.to_records())
         declarations[[columns["masterproject"], columns["project"]]] = declarations[
             columns["activity"]
         ].str.split(" / ", n=1, expand=True)
-        # An entry in the pseudo master project NSIP_DELETED_ACTIVITY_MASTERPROJECT is a special
+        # An entry in the pseudo master project MASTERPROJECT_DELETED_ACTIVITY is a special
         # case corresponding to deleted NSIP projects: the real name is in the project part that
         # must be parsed as for any other project
         declarations["project_saved"] = np.NaN
         declarations["project_saved"] = declarations["project_saved"].astype("object")
         declarations.loc[
-            declarations[columns["masterproject"]] == NSIP_DELETED_ACTIVITY_MASTERPROJECT,
+            declarations[columns["masterproject"]] == MASTERPROJECT_DELETED_ACTIVITY,
             "project_saved",
         ] = declarations[columns["project"]]
         # Not sure why the following line doesn't work (masterproject and project set to NaN
         # if no row matches the indexing condition... An issue has been open:
         # https://github.com/pandas-dev/pandas/issues/44726.
         # declarations.loc[
         #     declarations.project_saved.notna(),
@@ -967,15 +968,15 @@
         else:
             activity_entry.activite_nsip_referentiel_id = None
         change_log_msg = f"Desactivé le {datetime.now()} (NSIP ID={nsip_id})"
         if activity_entry.description:
             activity_entry.description += f"; {change_log_msg}"
         else:
             activity_entry.description = change_log_msg
-        activity_entry.libelle = f"{NSIP_DELETED_ACTIVITY_MASTERPROJECT} / {activity_entry.libelle}"
+        activity_entry.libelle = f"{MASTERPROJECT_DELETED_ACTIVITY} / {activity_entry.libelle}"
         activity_entry.ordre = DISABLED_ACTIVITY_ORDER
         if len(activity_entry.teams) > 0:
             activity_entry.teams.clear()
         db.session.delete(referentiel_entry)
         db.session.commit()
     except Exception as e:
         status = 1
@@ -1065,7 +1066,97 @@
             db.session.commit()
         except Exception as e:
             status = 1
             error_msg = getattr(e, "message", repr(e))
             db.session.rollback()
 
     return status, error_msg
+
+
+def reenable_activity(activity_name: str, project_activity: bool, name_prefix: str = None):
+    """
+    Reenable a disabled activity. This involves:
+    - Updating master project to match the original one
+    - If it was an NSIP project, recreate the referentiel entry
+
+    :param activity_name: activity name
+    :param project_activity: if true, an Hito project else an Hito activity
+    :param name_prefix: activity name prefix for deleted or local activities
+    :return: status and error message if any
+    """
+
+    from ositah.utils.hito_db_model import Activite, Projet, Referentiel
+
+    db = get_db()
+
+    status = 0  # Assume success
+    error_msg = ""
+
+    if project_activity:
+        Activity = Projet
+    else:
+        Activity = Activite
+
+    # Retrieve activity attributes and NSIP ID if present in description
+    if name_prefix:
+        activity_full_name = f"{name_prefix} / {activity_name}"
+    else:
+        activity_full_name = activity_name
+    activity_entry = Activity.query.filter(Activity.libelle == activity_full_name).first()
+
+    m = re.search(r"\(NSIP ID\=(?P<id>\d+)\)$", activity_entry.description)
+    if m:
+        nsip_id = m.group("id")
+    else:
+        nsip_id = None
+
+    # Check if an entry exist in the referentiel for the NSIP ID: if not, create it
+    nsip_entry = Referentiel.query.filter(
+        Referentiel.libelle.ilike(f"%(NSIP ID = {nsip_id})")
+    ).first()
+    if not nsip_entry:
+        master_project, activity = hito2ositah_project_name(activity_name)
+        project_name, referentiel_name = build_activity_libelle(
+            nsip_id,
+            master_project,
+            activity,
+        )
+
+        if project_activity:
+            entry_class = "projetnsipreferentiel"
+            entry_order = NSIP_PROJECT_ORDER
+        else:
+            entry_class = "activitensipreferentiel"
+            entry_order = NSIP_ACIVITY_ORDER
+
+        referentiel_entry = Referentiel(
+            libelle=referentiel_name,
+            object_class=entry_class,
+            ordre=entry_order,
+        )
+    else:
+        referentiel_entry = None
+
+    # Create referentiel entry if necessary and update activity
+    try:
+        if referentiel_entry:
+            db.session.add(referentiel_entry)
+        activity_entry.libelle = activity_name
+        activity_entry.description = f"Modifié le {datetime.now()}"
+        db.session.commit()
+        # Define relationship between activity and referentiel entry after creating them so that
+        # the referentiel ID generated by the DB server can be accessed
+        if project_activity:
+            activity_entry.projet_nsip_referentiel_id = referentiel_entry.id
+        else:
+            activity_entry.activite_nsip_referentiel_id = referentiel_entry.id
+        db.session.commit()
+
+    except Exception as e:
+        status = 1
+        error_msg = getattr(e, "message", repr(e))
+        db.session.rollback()
+
+    # Clear cached data to force a refresh of project list
+    clear_cached_data()
+
+    return status, error_msg
```

### Comparing `ositah-23.3.dev3/ositah/utils/teams.py` & `ositah-23.5.dev1/ositah/utils/teams.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah/utils/utils.py` & `ositah-23.5.dev1/ositah/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/ositah.egg-info/PKG-INFO` & `ositah-23.5.dev1/ositah.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ositah
-Version: 23.3.dev3
+Version: 23.5.dev1
 Summary: Outils de Suivi d'Activités basé sur Hito
 Author-email: Michel Jouvin <michel.jouvin@ijclab.in2p3.fr>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://gitlab.in2p3.fr/hito/ositah
 Project-URL: Bug Tracker, https://gitlab.in2p3.fr/hito/ositah/-/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ositah-23.3.dev3/ositah.egg-info/SOURCES.txt` & `ositah-23.5.dev1/ositah.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -15,18 +15,28 @@
 ositah/ositah.example.cfg
 ositah.egg-info/PKG-INFO
 ositah.egg-info/SOURCES.txt
 ositah.egg-info/dependency_links.txt
 ositah.egg-info/entry_points.txt
 ositah.egg-info/requires.txt
 ositah.egg-info/top_level.txt
+ositah/apps/__init__.py
 ositah/apps/analysis.py
-ositah/apps/configuration.py
 ositah/apps/export.py
-ositah/apps/validation.py
+ositah/apps/configuration/__init__.py
+ositah/apps/configuration/callbacks.py
+ositah/apps/configuration/main.py
+ositah/apps/configuration/parameters.py
+ositah/apps/configuration/tools.py
+ositah/apps/validation/__init__.py
+ositah/apps/validation/callbacks.py
+ositah/apps/validation/main.py
+ositah/apps/validation/parameters.py
+ositah/apps/validation/tables.py
+ositah/apps/validation/tools.py
 ositah/assets/arrow_down_up.svg
 ositah/assets/ositah.css
 ositah/assets/sort_ascending.svg
 ositah/assets/sort_descending.svg
 ositah/assets/sorttable.js
 ositah/static/style.css
 ositah/templates/base.html
```

### Comparing `ositah-23.3.dev3/pyproject.toml` & `ositah-23.5.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools", "setuptools-scm",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ositah"
-version = "23.3.dev3"
+version = "23.5.dev1"
 description = "Outils de Suivi d'Activités basé sur Hito"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
```

### Comparing `ositah-23.3.dev3/test-dash/accordion.py` & `ositah-23.5.dev1/test-dash/accordion.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/authentication.py` & `ositah-23.5.dev1/test-dash/authentication.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/checkbox.py` & `ositah-23.5.dev1/test-dash/checkbox.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/checklist.py` & `ositah-23.5.dev1/test-dash/checklist.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/file-selector.py` & `ositah-23.5.dev1/test-dash/file-selector.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/file-upload.py` & `ositah-23.5.dev1/test-dash/file-upload.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/long_running_callback.py` & `ositah-23.5.dev1/test-dash/long_running_callback.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/pandas_split.py` & `ositah-23.5.dev1/test-dash/pandas_split.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/pandas_split_bug_report.py` & `ositah-23.5.dev1/test-dash/pandas_split_bug_report.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/pattern-matching-callback.py` & `ositah-23.5.dev1/test-dash/pattern-matching-callback.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/progess_bar.py` & `ositah-23.5.dev1/test-dash/progess_bar.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/reset_table_checkboxes.py` & `ositah-23.5.dev1/test-dash/reset_table_checkboxes.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/sortable_table.py` & `ositah-23.5.dev1/test-dash/sortable_table.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/sqlalchemy_test.py` & `ositah-23.5.dev1/test-dash/sqlalchemy_test.py`

 * *Files identical despite different names*

### Comparing `ositah-23.3.dev3/test-dash/templates/login_form.html` & `ositah-23.5.dev1/test-dash/templates/login_form.html`

 * *Files identical despite different names*

