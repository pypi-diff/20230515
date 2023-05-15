# Comparing `tmp/aleksis_app_untis-3.0.tar.gz` & `tmp/aleksis_app_untis-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_untis-3.0.tar", max compression
+gzip compressed data, was "aleksis_app_untis-3.0b0.tar", max compression
```

## Comparing `aleksis_app_untis-3.0.tar` & `aleksis_app_untis-3.0b0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     7262 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/LICENCE.rst
--rw-r--r--   0        0        0     1714 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/README.rst
--rw-r--r--   0        0        0      211 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/__init__.py
--rw-r--r--   0        0        0      512 2023-05-15 18:20:42.488403 aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1194 2023-05-15 18:20:43.012428 aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     1987 2023-05-15 18:20:43.984474 aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/data_checks.cpython-311.pyc
--rw-r--r--   0        0        0     4622 2023-05-15 18:20:44.240486 aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/model_extensions.cpython-311.pyc
--rw-r--r--   0        0        0   150762 2023-05-15 18:20:43.984474 aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     6763 2023-05-15 18:20:44.432495 aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0      552 2023-05-15 18:20:44.196484 aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     1030 2023-05-15 18:20:42.488403 aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0      744 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/apps.py
--rw-r--r--   0        0        0     2966 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/commands.py
--rw-r--r--   0        0        0     1099 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/data_checks.py
--rw-r--r--   0        0        0      463 2023-05-15 18:20:44.624504 aleksis_app_untis-3.0/aleksis/apps/untis/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5139 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4449 2023-05-15 18:20:44.644505 aleksis_app_untis-3.0/aleksis/apps/untis/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10899 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-05-15 18:20:44.636505 aleksis_app_untis-3.0/aleksis/apps/untis/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5055 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      476 2023-05-15 18:20:44.616504 aleksis_app_untis-3.0/aleksis/apps/untis/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5182 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-15 18:20:44.636505 aleksis_app_untis-3.0/aleksis/apps/untis/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5009 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5524 2023-05-15 18:20:44.640505 aleksis_app_untis-3.0/aleksis/apps/untis/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7939 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-15 18:20:44.652506 aleksis_app_untis-3.0/aleksis/apps/untis/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5009 2023-05-15 18:15:36.069857 aleksis_app_untis-3.0/aleksis/apps/untis/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5554 2023-05-15 18:20:44.608504 aleksis_app_untis-3.0/aleksis/apps/untis/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8334 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/management/commands/__init__.py
--rw-r--r--   0        0        0     4070 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/management/commands/move_dates_for_testing.py
--rw-r--r--   0        0        0     1007 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/management/commands/untis_import_mysql.py
--rw-r--r--   0        0        0   268050 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/migrations/0001_initial.py
--rw-r--r--   0        0        0      426 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/migrations/0002_auto_20200820_1542.py
--rw-r--r--   0        0        0      681 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/migrations/0003_guess_school_id.py
--rw-r--r--   0        0        0        0 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/migrations/__init__.py
--rw-r--r--   0        0        0     3188 2023-05-15 18:15:36.073857 aleksis_app_untis-3.0/aleksis/apps/untis/model_extensions.py
--rw-r--r--   0        0        0   187446 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/models.py
--rw-r--r--   0        0        0     3935 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/preferences.py
--rw-r--r--   0        0        0      292 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/rules.py
--rw-r--r--   0        0        0      689 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/settings.py
--rw-r--r--   0        0        0      404 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/tasks.py
--rw-r--r--   0        0        0     3511 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/tests/util/test_mysql_util.py
--rw-r--r--   0        0        0     6450 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/absences.py
--rw-r--r--   0        0        0    20582 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/common_data.py
--rw-r--r--   0        0        0     4613 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/events.py
--rw-r--r--   0        0        0     5566 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/exams.py
--rw-r--r--   0        0        0     2088 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/holidays.py
--rw-r--r--   0        0        0    14111 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/lessons.py
--rw-r--r--   0        0        0    10793 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/substitutions.py
--rw-r--r--   0        0        0     7028 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/terms.py
--rw-r--r--   0        0        0     3268 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/main.py
--rw-r--r--   0        0        0     5971 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/util.py
--rw-r--r--   0        0        0      581 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/docs/Makefile
--rw-r--r--   0        0        0      130 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/docs/admin/00_index.rst
--rw-r--r--   0        0        0     1564 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/docs/admin/10_features.rst
--rw-r--r--   0        0        0     5572 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/docs/admin/20_configuration.rst
--rw-r--r--   0        0        0     6545 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/docs/conf.py
--rw-r--r--   0        0        0      522 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/docs/index.rst
--rw-r--r--   0        0        0      787 2023-05-15 18:15:36.077857 aleksis_app_untis-3.0/docs/make.bat
--rw-r--r--   0        0        0     1919 2023-05-15 18:16:18.627878 aleksis_app_untis-3.0/pyproject.toml
--rw-r--r--   0        0        0     2563 2023-05-15 18:15:36.101858 aleksis_app_untis-3.0/tox.ini
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 aleksis_app_untis-3.0/setup.py
--rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 aleksis_app_untis-3.0/PKG-INFO
+-rw-r--r--   0        0        0     7128 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1714 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/README.rst
+-rw-r--r--   0        0        0      211 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/__init__.py
+-rw-r--r--   0        0        0      512 2023-02-27 22:16:46.583188 aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1194 2023-02-27 22:16:47.071187 aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     1987 2023-02-27 22:16:47.907185 aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/data_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     4622 2023-02-27 22:16:48.127184 aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/model_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0   150762 2023-02-27 22:16:47.907185 aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     6763 2023-02-27 22:16:48.303184 aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0      552 2023-02-27 22:16:48.087185 aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     1030 2023-02-27 22:16:46.583188 aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0      744 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/apps.py
+-rw-r--r--   0        0        0     2966 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/commands.py
+-rw-r--r--   0        0        0     1099 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/data_checks.py
+-rw-r--r--   0        0        0      463 2023-02-27 22:16:48.455184 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5139 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4449 2023-02-27 22:16:48.451184 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10899 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-02-27 22:16:48.451184 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5055 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      476 2023-02-27 22:16:48.467184 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5182 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 22:16:48.463184 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5009 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5524 2023-02-27 22:16:48.451184 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7939 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 22:16:48.451184 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5009 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5554 2023-02-27 22:16:48.467184 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8334 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/management/commands/__init__.py
+-rw-r--r--   0        0        0     4070 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/management/commands/move_dates_for_testing.py
+-rw-r--r--   0        0        0     1007 2023-02-27 22:13:41.519562 aleksis_app_untis-3.0b0/aleksis/apps/untis/management/commands/untis_import_mysql.py
+-rw-r--r--   0        0        0   268050 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/migrations/0001_initial.py
+-rw-r--r--   0        0        0      426 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/migrations/0002_auto_20200820_1542.py
+-rw-r--r--   0        0        0      681 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/migrations/0003_guess_school_id.py
+-rw-r--r--   0        0        0        0 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/migrations/__init__.py
+-rw-r--r--   0        0        0     3188 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/model_extensions.py
+-rw-r--r--   0        0        0   187446 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/models.py
+-rw-r--r--   0        0        0     3935 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/preferences.py
+-rw-r--r--   0        0        0      292 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/rules.py
+-rw-r--r--   0        0        0      689 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/settings.py
+-rw-r--r--   0        0        0      404 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/tasks.py
+-rw-r--r--   0        0        0     3511 2023-02-27 22:13:41.523562 aleksis_app_untis-3.0b0/aleksis/apps/untis/tests/util/test_mysql_util.py
+-rw-r--r--   0        0        0     6450 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/absences.py
+-rw-r--r--   0        0        0    20582 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/common_data.py
+-rw-r--r--   0        0        0     4613 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/events.py
+-rw-r--r--   0        0        0     5566 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/exams.py
+-rw-r--r--   0        0        0     2088 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/holidays.py
+-rw-r--r--   0        0        0    14111 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/lessons.py
+-rw-r--r--   0        0        0    10793 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/substitutions.py
+-rw-r--r--   0        0        0     7028 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/terms.py
+-rw-r--r--   0        0        0     3268 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/main.py
+-rw-r--r--   0        0        0     5971 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/util.py
+-rw-r--r--   0        0        0      581 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/docs/Makefile
+-rw-r--r--   0        0        0      130 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     1564 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/docs/admin/10_features.rst
+-rw-r--r--   0        0        0     5572 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/docs/admin/20_configuration.rst
+-rw-r--r--   0        0        0     6547 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/docs/conf.py
+-rw-r--r--   0        0        0      522 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-02-27 22:13:41.527562 aleksis_app_untis-3.0b0/docs/make.bat
+-rw-r--r--   0        0        0     1925 2023-02-27 22:14:17.583489 aleksis_app_untis-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2563 2023-02-27 22:13:41.555562 aleksis_app_untis-3.0b0/tox.ini
+-rw-r--r--   0        0        0     3363 1970-01-01 00:00:00.000000 aleksis_app_untis-3.0b0/setup.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 aleksis_app_untis-3.0b0/PKG-INFO
```

### Comparing `aleksis_app_untis-3.0/CHANGELOG.rst` & `aleksis_app_untis-3.0b0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,16 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0`_ - 2023-05-15
--------------------
-
-Nothing changed.
-
-`3.0b0`_ - 2023-02-27
----------------------
+`3.0b0` - 2022-02-27
+--------------------
 
 Removed
 ~~~~~~~
 
 * Legacy menu integration for AlekSIS-Core pre-3.0
 
 Added
@@ -275,8 +270,7 @@
 .. _2.1.2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-Untis/-/tags/2.1.2
 .. _2.1.3: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-Untis/-/tags/2.1.3
 .. _2.2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-Untis/-/tags/2.2
 .. _2.3: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-Untis/-/tags/2.3
 .. _2.3.1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-Untis/-/tags/2.3.1
 .. _2.3.2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-Untis/-/tags/2.3.2
 .. _3.0b0: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-Untis/-/tags/3.0b0
-.. _3.0: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-Untis/-/tags/3.0
```

### Comparing `aleksis_app_untis-3.0/LICENCE.rst` & `aleksis_app_untis-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/README.rst` & `aleksis_app_untis-3.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/__init__.cpython-311.pyc` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/__init__.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8766264 (Mon May 15 18:15:36 2023 UTC)
+moddate:  0x152bfd63 (Mon Feb 27 22:13:41 2023 UTC)
 files sz: 211
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/apps.cpython-311.pyc` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/apps.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8766264 (Mon May 15 18:15:36 2023 UTC)
+moddate:  0x152bfd63 (Mon Feb 27 22:13:41 2023 UTC)
 files sz: 744
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/data_checks.cpython-311.pyc` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/data_checks.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8766264 (Mon May 15 18:15:36 2023 UTC)
+moddate:  0x152bfd63 (Mon Feb 27 22:13:41 2023 UTC)
 files sz: 1099
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/model_extensions.cpython-311.pyc` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/model_extensions.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8766264 (Mon May 15 18:15:36 2023 UTC)
+moddate:  0x152bfd63 (Mon Feb 27 22:13:41 2023 UTC)
 files sz: 3188
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/models.cpython-311.pyc` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/models.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8766264 (Mon May 15 18:15:36 2023 UTC)
+moddate:  0x152bfd63 (Mon Feb 27 22:13:41 2023 UTC)
 files sz: 187446
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/preferences.cpython-311.pyc` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/preferences.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8766264 (Mon May 15 18:15:36 2023 UTC)
+moddate:  0x152bfd63 (Mon Feb 27 22:13:41 2023 UTC)
 files sz: 3935
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/rules.cpython-311.pyc` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/rules.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8766264 (Mon May 15 18:15:36 2023 UTC)
+moddate:  0x152bfd63 (Mon Feb 27 22:13:41 2023 UTC)
 files sz: 292
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/__pycache__/settings.cpython-311.pyc` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/__pycache__/settings.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8766264 (Mon May 15 18:15:36 2023 UTC)
+moddate:  0x152bfd63 (Mon Feb 27 22:13:41 2023 UTC)
 files sz: 689
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/apps.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/commands.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/commands.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/data_checks.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/la/LC_MESSAGES/django.po` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/management/commands/move_dates_for_testing.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/management/commands/move_dates_for_testing.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/management/commands/untis_import_mysql.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/management/commands/untis_import_mysql.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/migrations/0001_initial.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/migrations/0003_guess_school_id.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/migrations/0003_guess_school_id.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/model_extensions.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/model_extensions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/models.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/preferences.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/settings.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/settings.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/tests/util/test_mysql_util.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/tests/util/test_mysql_util.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/absences.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/absences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/common_data.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/common_data.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/events.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/events.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/exams.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/exams.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/holidays.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/holidays.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/lessons.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/lessons.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/substitutions.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/substitutions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/importers/terms.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/importers/terms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/main.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/main.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/aleksis/apps/untis/util/mysql/util.py` & `aleksis_app_untis-3.0b0/aleksis/apps/untis/util/mysql/util.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/docs/Makefile` & `aleksis_app_untis-3.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/docs/admin/10_features.rst` & `aleksis_app_untis-3.0b0/docs/admin/10_features.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/docs/admin/20_configuration.rst` & `aleksis_app_untis-3.0b0/docs/admin/20_configuration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/docs/conf.py` & `aleksis_app_untis-3.0b0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-Untis"
 copyright = "2018-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0"
+release = "3.0b0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_app_untis-3.0/docs/index.rst` & `aleksis_app_untis-3.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/docs/make.bat` & `aleksis_app_untis-3.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/pyproject.toml` & `aleksis_app_untis-3.0b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Untis"
-version = "3.0"
+version = "3.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -37,16 +37,16 @@
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 mysqlclient = "^2.0.0"
 tqdm = "^4.44.1"
 defusedxml = "^0.7.0"
-aleksis-core = "^3.0"
-aleksis-app-chronos = "^3.0"
+aleksis-core = "^3.0b0"
+aleksis-app-chronos = "^3.0b0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 untis = "aleksis.apps.untis.apps:UntisConfig"
```

### Comparing `aleksis_app_untis-3.0/tox.ini` & `aleksis_app_untis-3.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_untis-3.0/setup.py` & `aleksis_app_untis-3.0b0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,26 +18,26 @@
                         'locale/la/LC_MESSAGES/*',
                         'locale/nb_NO/LC_MESSAGES/*',
                         'locale/ru/LC_MESSAGES/*',
                         'locale/tr_TR/LC_MESSAGES/*',
                         'locale/uk/LC_MESSAGES/*']}
 
 install_requires = \
-['aleksis-app-chronos>=3.0,<4.0',
- 'aleksis-core>=3.0,<4.0',
+['aleksis-app-chronos>=3.0b0,<4.0',
+ 'aleksis-core>=3.0b0,<4.0',
  'defusedxml>=0.7.0,<0.8.0',
  'mysqlclient>=2.0.0,<3.0.0',
  'tqdm>=4.44.1,<5.0.0']
 
 entry_points = \
 {'aleksis.app': ['untis = aleksis.apps.untis.apps:UntisConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-untis',
-    'version': '3.0',
+    'version': '3.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp for Untis import',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp for Untis import\n==========================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\n* Import absence reasons\n* Import absences\n* Import breaks\n* Import classes\n* Import events\n* Import exams\n* Import exported Untis database via MySQL import\n* Import exported Untis XML files\n* Import holidays\n* Import lessons\n* Import rooms\n* Import subjects\n* Import substitutions\n* Import supervision areas\n* Import teachers\n* Import time periods\n\nLicence\n-------\n\n::\n\n  Copyright © 2018, 2019, 2020, 2021, 2022 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2018, 2019 Frank Poetzsch-Heffter <p-h@katharineum.de>\n  Copyright © 2019, 2020, 2021, 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2019, 2020 Tom Teichler <tom.teichler@teckids.org>\n  Copyright © 2019 Julian Leucker <leuckeju@katharineum.de>\n  Copyright © 2019 mirabilos <thorsten.glaser@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://aleksis.org/\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Dominik George',
     'author_email': 'dominik.george@teckids.org',
     'maintainer': 'Jonathan Weth',
     'maintainer_email': 'dev@jonathanweth.de',
     'url': 'https://aleksis.org/',
```

### Comparing `aleksis_app_untis-3.0/PKG-INFO` & `aleksis_app_untis-3.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-untis
-Version: 3.0
+Version: 3.0b0
 Summary: AlekSIS (School Information System) — App for Untis import
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,timetable,plans
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
@@ -17,16 +17,16 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Typing :: Typed
-Requires-Dist: aleksis-app-chronos (>=3.0,<4.0)
-Requires-Dist: aleksis-core (>=3.0,<4.0)
+Requires-Dist: aleksis-app-chronos (>=3.0b0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Requires-Dist: defusedxml (>=0.7.0,<0.8.0)
 Requires-Dist: mysqlclient (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.44.1,<5.0.0)
 Project-URL: Documentation, https://aleksis.org/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-Untis
 Description-Content-Type: text/x-rst
```

