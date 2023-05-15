# Comparing `tmp/django_import_export_extensions-0.1.1.tar.gz` & `tmp/django_import_export_extensions-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_import_export_extensions-0.1.1.tar", last modified: Thu Apr 27 11:49:11 2023, max compression
+gzip compressed data, was "django_import_export_extensions-0.1.2.tar", last modified: Mon May 15 13:17:46 2023, max compression
```

## Comparing `django_import_export_extensions-0.1.1.tar` & `django_import_export_extensions-0.1.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.056997 django_import_export_extensions-0.1.1/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      176 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/AUTHORS.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3236 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      206 2023-04-27 11:07:57.000000 django_import_export_extensions-0.1.1/HISTORY.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1066 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/LICENSE
--rw-r--r--   0 yalef     (1000) yalef     (1000)      282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/MANIFEST.in
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3242 2023-04-27 11:49:11.056997 django_import_export_extensions-0.1.1/PKG-INFO
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2072 2023-04-27 10:39:21.000000 django_import_export_extensions-0.1.1/README.rst
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.023662 django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3242 2023-04-27 11:49:10.000000 django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/PKG-INFO
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3773 2023-04-27 11:49:10.000000 django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-04-27 11:49:10.000000 django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)       79 2023-04-27 11:49:10.000000 django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/entry_points.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-04-27 11:49:10.000000 django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/not-zip-safe
--rw-r--r--   0 yalef     (1000) yalef     (1000)      126 2023-04-27 11:49:10.000000 django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/requires.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)       25 2023-04-27 11:49:10.000000 django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.030329 django_import_export_extensions-0.1.1/docs/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      625 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/Makefile
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:10.993660 django_import_export_extensions-0.1.1/docs/_build/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.003661 django_import_export_extensions-0.1.1/docs/_build/html/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.033662 django_import_export_extensions-0.1.1/docs/_build/html/_static/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      286 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.1/docs/_build/html/_static/file.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/authors.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4476 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/conf.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)       33 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/contributing.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/history.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      334 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/index.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2754 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/installation.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      822 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/make.bat
--rw-r--r--   0 yalef     (1000) yalef     (1000)       27 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/readme.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3447 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/docs/usage.rst
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.036996 django_import_export_extensions-0.1.1/import_export_extensions/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      144 2023-04-27 11:03:10.000000 django_import_export_extensions-0.1.1/import_export_extensions/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.036996 django_import_export_extensions-0.1.1/import_export_extensions/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      166 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.040329 django_import_export_extensions-0.1.1/import_export_extensions/admin/forms/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      100 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/forms/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      997 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/forms/export_admin_form.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1177 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/forms/import_admin_form.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.040329 django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      155 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      797 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/base.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10885 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/export_mixin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      340 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/import_export_mixin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    12731 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/import_mixin.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.043663 django_import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5715 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/export_job_admin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     7018 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/import_job_admin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3817 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/mixins.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1394 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/admin/widgets.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.046996 django_import_export_extensions-0.1.1/import_export_extensions/api/
--rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/api/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.046996 django_import_export_extensions-0.1.1/import_export_extensions/api/serializers/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      156 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/api/serializers/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3566 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/api/serializers/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3158 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/api/serializers/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      378 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/api/serializers/progress.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.046996 django_import_export_extensions-0.1.1/import_export_extensions/api/views/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       82 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/api/views/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4418 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/api/views/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     6243 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/api/views/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      716 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/apps.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     7233 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/fields.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1315 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/forms.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.050330 django_import_export_extensions-0.1.1/import_export_extensions/migrations/
--rw-r--r--   0 yalef     (1000) yalef     (1000)    12282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/migrations/0001_initial.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/migrations/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.050330 django_import_export_extensions-0.1.1/import_export_extensions/models/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       68 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/models/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1267 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/models/core.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10445 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/models/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    17389 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/models/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      752 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/models/tools.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     8148 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/resources.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.013661 django_import_export_extensions-0.1.1/import_export_extensions/static/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.016995 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.016995 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.050330 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       67 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/admin/admin.css
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.050330 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/widgets/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      626 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.020328 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.053663 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      768 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/admin/admin.js
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.053663 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/widgets/
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1712 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js
--rw-r--r--   0 yalef     (1000) yalef     (1000)      537 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/tasks.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.020328 django_import_export_extensions-0.1.1/import_export_extensions/templates/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.056997 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       37 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/base.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1081 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1482 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2440 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export_status.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1215 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5062 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2413 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import_status.html
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:49:11.056997 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      391 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_export_item.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_import.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      248 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_import_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_import_item.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2571 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/import_job_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5135 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/utils.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10744 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.1/import_export_extensions/widgets.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1791 2023-04-27 11:49:11.060330 django_import_export_extensions-0.1.1/setup.cfg
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2486 2023-04-27 11:45:15.000000 django_import_export_extensions-0.1.1/setup.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.799049 django_import_export_extensions-0.1.2/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      176 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/AUTHORS.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3236 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      293 2023-05-15 13:15:23.000000 django_import_export_extensions-0.1.2/HISTORY.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1066 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/LICENSE
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/MANIFEST.in
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3343 2023-05-15 13:17:46.802382 django_import_export_extensions-0.1.2/PKG-INFO
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2086 2023-04-27 11:56:03.000000 django_import_export_extensions-0.1.2/README.rst
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.785715 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3343 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3773 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       79 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/entry_points.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      126 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/requires.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       25 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.789049 django_import_export_extensions-0.1.2/docs/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      625 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/Makefile
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.772382 django_import_export_extensions-0.1.2/docs/_build/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.772382 django_import_export_extensions-0.1.2/docs/_build/html/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.789049 django_import_export_extensions-0.1.2/docs/_build/html/_static/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      286 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/authors.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4483 2023-04-27 12:13:39.000000 django_import_export_extensions-0.1.2/docs/conf.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       33 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/contributing.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/history.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      334 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/index.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2754 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/installation.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      822 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/make.bat
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       27 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/readme.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3447 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/usage.rst
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.789049 django_import_export_extensions-0.1.2/import_export_extensions/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      144 2023-05-15 13:01:32.000000 django_import_export_extensions-0.1.2/import_export_extensions/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.789049 django_import_export_extensions-0.1.2/import_export_extensions/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      166 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      100 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      997 2023-05-02 06:15:21.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/export_admin_form.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1177 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/import_admin_form.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      155 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      797 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/base.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10885 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/export_mixin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      340 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/import_export_mixin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    12731 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/import_mixin.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5715 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/export_job_admin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     7018 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/import_job_admin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3817 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/mixins.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1394 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/widgets.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/api/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      156 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3566 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3158 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      378 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/progress.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/api/views/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       82 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/views/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4418 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/views/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     6243 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/views/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      716 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/apps.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     7233 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/fields.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1315 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/forms.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/migrations/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    12282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/migrations/0001_initial.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/migrations/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/models/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       68 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1267 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/core.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10445 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    17389 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      752 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/tools.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     8148 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/resources.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.779048 django_import_export_extensions-0.1.2/import_export_extensions/static/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.782382 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.782382 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       67 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/admin/admin.css
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/widgets/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      626 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.782382 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      768 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/admin/admin.js
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/widgets/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1712 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      537 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/tasks.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.782382 django_import_export_extensions-0.1.2/import_export_extensions/templates/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.799049 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       37 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/base.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1081 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1482 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2440 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export_status.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1215 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5062 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2413 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import_status.html
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.799049 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      391 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_export_item.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_import.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      248 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_import_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_import_item.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2571 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/import_job_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5135 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/utils.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    11277 2023-05-15 13:15:23.000000 django_import_export_extensions-0.1.2/import_export_extensions/widgets.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1791 2023-05-15 13:17:46.805716 django_import_export_extensions-0.1.2/setup.cfg
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2486 2023-05-15 13:15:23.000000 django_import_export_extensions-0.1.2/setup.py
```

### Comparing `django_import_export_extensions-0.1.1/CONTRIBUTING.rst` & `django_import_export_extensions-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/LICENSE` & `django_import_export_extensions-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/PKG-INFO` & `django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_import_export_extensions
-Version: 0.1.1
+Name: django-import-export-extensions
+Version: 0.1.2
 Summary: Extend functionality of `django-import-export`
 Home-page: https://github.com/saritasa-nest/django-import-export-extensions
 Author: Saritasa
 Author-email: pypi@saritasa.com
 License: MIT license
 Keywords: django_import_export_extensions
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -29,19 +29,19 @@
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
-        :target: https://pypi.org/project/import-export-extensions/
+        :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
-        :target: https://pypi.org/project/import-export-extensions/
+        :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported django versions
 
 .. image:: https://readthedocs.org/projects/django-import-export-extensions/badge/?version=latest
     :target: https://django-import-export-extensions.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 Description
@@ -74,14 +74,19 @@
 * Documentation: https://django-import-export-extensions.readthedocs.io.
 
 
 =======
 History
 =======
 
+0.1.2 (2023-05-12)
+------------------
+
+* Add support for `STORAGES` settings variable
+
 0.1.1 (2023-04-27)
 ------------------
 
 * Add package description
 * Add configuration file for read-the-docs service
 
 0.1.0 (2023-04-01)
```

### Comparing `django_import_export_extensions-0.1.1/README.rst` & `django_import_export_extensions-0.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
-        :target: https://pypi.org/project/import-export-extensions/
+        :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
-        :target: https://pypi.org/project/import-export-extensions/
+        :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported django versions
 
 .. image:: https://readthedocs.org/projects/django-import-export-extensions/badge/?version=latest
     :target: https://django-import-export-extensions.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 Description
```

### Comparing `django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/PKG-INFO` & `django_import_export_extensions-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-import-export-extensions
-Version: 0.1.1
+Name: django_import_export_extensions
+Version: 0.1.2
 Summary: Extend functionality of `django-import-export`
 Home-page: https://github.com/saritasa-nest/django-import-export-extensions
 Author: Saritasa
 Author-email: pypi@saritasa.com
 License: MIT license
 Keywords: django_import_export_extensions
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -29,19 +29,19 @@
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
-        :target: https://pypi.org/project/import-export-extensions/
+        :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
-        :target: https://pypi.org/project/import-export-extensions/
+        :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported django versions
 
 .. image:: https://readthedocs.org/projects/django-import-export-extensions/badge/?version=latest
     :target: https://django-import-export-extensions.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 Description
@@ -74,14 +74,19 @@
 * Documentation: https://django-import-export-extensions.readthedocs.io.
 
 
 =======
 History
 =======
 
+0.1.2 (2023-05-12)
+------------------
+
+* Add support for `STORAGES` settings variable
+
 0.1.1 (2023-04-27)
 ------------------
 
 * Add package description
 * Add configuration file for read-the-docs service
 
 0.1.0 (2023-04-01)
```

### Comparing `django_import_export_extensions-0.1.1/django_import_export_extensions.egg-info/SOURCES.txt` & `django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/docs/Makefile` & `django_import_export_extensions-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/docs/conf.py` & `django_import_export_extensions-0.1.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
```

### Comparing `django_import_export_extensions-0.1.1/docs/installation.rst` & `django_import_export_extensions-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/docs/make.bat` & `django_import_export_extensions-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/docs/usage.rst` & `django_import_export_extensions-0.1.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/forms/export_admin_form.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/export_admin_form.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/forms/import_admin_form.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/import_admin_form.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/base.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/base.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/export_mixin.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/export_mixin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/mixins/import_mixin.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/import_mixin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/export_job_admin.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/export_job_admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/import_job_admin.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/import_job_admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/mixins.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/admin/widgets.py` & `django_import_export_extensions-0.1.2/import_export_extensions/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/api/serializers/export_job.py` & `django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/export_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/api/serializers/import_job.py` & `django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/import_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/api/views/export_job.py` & `django_import_export_extensions-0.1.2/import_export_extensions/api/views/export_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/api/views/import_job.py` & `django_import_export_extensions-0.1.2/import_export_extensions/api/views/import_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/apps.py` & `django_import_export_extensions-0.1.2/import_export_extensions/apps.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/fields.py` & `django_import_export_extensions-0.1.2/import_export_extensions/fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/forms.py` & `django_import_export_extensions-0.1.2/import_export_extensions/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/migrations/0001_initial.py` & `django_import_export_extensions-0.1.2/import_export_extensions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/models/core.py` & `django_import_export_extensions-0.1.2/import_export_extensions/models/core.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/models/export_job.py` & `django_import_export_extensions-0.1.2/import_export_extensions/models/export_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/models/import_job.py` & `django_import_export_extensions-0.1.2/import_export_extensions/models/import_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/models/tools.py` & `django_import_export_extensions-0.1.2/import_export_extensions/models/tools.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/resources.py` & `django_import_export_extensions-0.1.2/import_export_extensions/resources.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css` & `django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/admin/admin.js` & `django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/admin/admin.js`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js` & `django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/tasks.py` & `django_import_export_extensions-0.1.2/import_export_extensions/tasks.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export.html` & `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export_results.html` & `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export_status.html` & `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export_status.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import.html` & `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import_results.html` & `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import_status.html` & `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import_status.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/templates/admin/import_job_results.html` & `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/import_job_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/utils.py` & `django_import_export_extensions-0.1.2/import_export_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/import_export_extensions/widgets.py` & `django_import_export_extensions-0.1.2/import_export_extensions/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from .utils import (
     clean_sequence_of_string_values,
     download_file,
     get_clear_q_filter,
     url_to_internal_value,
 )
 
+DEFAULT_SYSTEM_STORAGE = "django.core.files.storage.FileSystemStorage"
+
 
 class IntermediateManyToManyWidget(ManyToManyWidget):
     """Widget for M2M field with custom ``through`` model.
 
     Default M2M widget store just IDs of related objects.
     With intermediate model additional data may be stored.
 
@@ -288,18 +290,15 @@
         self.filename = filename
 
     def render(self, value: Model, *args, **kwargs) -> typing.Optional[str]:
         """Convert DB value to URL to file."""
         if not value:
             return None
 
-        if (
-            settings.DEFAULT_FILE_STORAGE
-            == "django.core.files.storage.FileSystemStorage"
-        ):
+        if self._get_default_storage() == DEFAULT_SYSTEM_STORAGE:
             return f"http://localhost:8000{value.url}"
 
         return value.url
 
     def clean(self, value: str, *args, **kwargs) -> typing.Optional[str]:
         """Get the file and check for exists."""
         if not value:
@@ -321,7 +320,21 @@
     def _get_file(self, url: str) -> File:
         """Download file from the external resource."""
         file = download_file(url)
         ext = mimetypes.guess_extension(file.content_type)
         filename = f"{self.filename}.{ext}" if ext else self.filename
 
         return File(file, filename)
+
+    def _get_default_storage(self) -> str:
+        """Return default system storage used in project.
+
+        Use the value from `STORAGES` if it's available,
+        otherwise use `DEFAULT_FILE_STORAGE`.
+
+        `STORAGES` variable replaced `DEFAULT_FILE_STORAGE`, in django 4.2
+        https://docs.djangoproject.com/en/4.2/ref/settings/#default-file-storage
+
+        """
+        if hasattr(settings, "STORAGES"):
+            return settings.STORAGES["default"]["BACKEND"]
+        return settings.DEFAULT_FILE_STORAGE
```

### Comparing `django_import_export_extensions-0.1.1/setup.cfg` & `django_import_export_extensions-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.1/setup.py` & `django_import_export_extensions-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,10 +72,10 @@
     include_package_data=True,
     keywords="django_import_export_extensions",
     name="django_import_export_extensions",
     packages=find_packages(include=["import_export_extensions", "import_export_extensions.*"]),
     test_suite="tests",
     tests_require=reqs("development.txt"),
     url="https://github.com/saritasa-nest/django-import-export-extensions",
-    version="0.1.1",
+    version="0.1.2",
     zip_safe=False,
 )
```

