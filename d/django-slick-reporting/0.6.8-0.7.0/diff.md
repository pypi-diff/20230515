# Comparing `tmp/django-slick-reporting-0.6.8.tar.gz` & `tmp/django-slick-reporting-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-slick-reporting-0.6.8.tar", last modified: Sun Mar 19 11:45:00 2023, max compression
+gzip compressed data, was "django-slick-reporting-0.7.0.tar", last modified: Mon May 15 07:50:41 2023, max compression
```

## Comparing `django-slick-reporting-0.6.8.tar` & `django-slick-reporting-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-03-19 11:45:00.902860 django-slick-reporting-0.6.8/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     1518 2020-04-23 10:03:51.000000 django-slick-reporting-0.6.8/LICENSE.md
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      152 2020-06-07 07:01:50.000000 django-slick-reporting-0.6.8/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9141 2023-03-19 11:45:00.902860 django-slick-reporting-0.6.8/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7417 2022-08-26 21:11:35.000000 django-slick-reporting-0.6.8/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-03-19 11:45:00.898860 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9141 2023-03-19 11:45:00.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1203 2023-03-19 11:45:00.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1003 2021-07-15 08:55:50.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/SOURCES.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-03-19 11:45:00.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2021-07-15 08:55:50.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/dependency_links.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       71 2023-03-19 11:45:00.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       66 2021-07-15 08:55:50.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/requires.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-03-19 11:45:00.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/top_level.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2021-07-15 08:55:50.000000 django-slick-reporting-0.6.8/django_slick_reporting.egg-info/top_level.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1675 2023-03-19 11:45:00.902860 django-slick-reporting-0.6.8/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-slick-reporting-0.6.8/setup.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-03-19 11:45:00.898860 django-slick-reporting-0.6.8/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      104 2023-03-19 11:44:17.000000 django-slick-reporting-0.6.8/slick_reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1637 2022-08-27 20:11:01.000000 django-slick-reporting-0.6.8/slick_reporting/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      208 2021-04-08 04:55:40.000000 django-slick-reporting-0.6.8/slick_reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      722 2020-11-24 09:32:04.000000 django-slick-reporting-0.6.8/slick_reporting/decorators.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    15713 2023-02-20 05:04:39.000000 django-slick-reporting-0.6.8/slick_reporting/fields.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7022 2023-03-19 11:44:11.000000 django-slick-reporting-0.6.8/slick_reporting/form_factory.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2020-04-21 06:28:25.000000 django-slick-reporting-0.6.8/slick_reporting/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    30938 2023-02-20 05:04:39.000000 django-slick-reporting-0.6.8/slick_reporting/generator.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1546 2020-12-16 19:37:13.000000 django-slick-reporting-0.6.8/slick_reporting/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1650 2020-11-22 17:45:34.000000 django-slick-reporting-0.6.8/slick_reporting/registry.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-03-19 11:45:00.898860 django-slick-reporting-0.6.8/slick_reporting/static/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-03-19 11:45:00.898860 django-slick-reporting-0.6.8/slick_reporting/static/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2020-12-11 18:31:17.000000 django-slick-reporting-0.6.8/slick_reporting/static/slick_reporting/main.js
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     6244 2021-06-14 07:56:57.000000 django-slick-reporting-0.6.8/slick_reporting/static/slick_reporting/ra.chartsjs.js
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    19411 2023-01-24 05:54:42.000000 django-slick-reporting-0.6.8/slick_reporting/static/slick_reporting/ra.highchart.js
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-03-19 11:45:00.898860 django-slick-reporting-0.6.8/slick_reporting/templates/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-03-19 11:45:00.902860 django-slick-reporting-0.6.8/slick_reporting/templates/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2076 2021-01-10 06:56:32.000000 django-slick-reporting-0.6.8/slick_reporting/templates/slick_reporting/base.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8362 2023-01-27 19:26:30.000000 django-slick-reporting-0.6.8/slick_reporting/templates/slick_reporting/simple_report.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      448 2020-07-24 10:59:05.000000 django-slick-reporting-0.6.8/slick_reporting/templates/slick_reporting/table.html
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-03-19 11:45:00.902860 django-slick-reporting-0.6.8/slick_reporting/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2019-11-14 16:41:29.000000 django-slick-reporting-0.6.8/slick_reporting/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      780 2022-07-07 07:19:02.000000 django-slick-reporting-0.6.8/slick_reporting/templatetags/slick_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9296 2023-03-19 11:44:11.000000 django-slick-reporting-0.6.8/slick_reporting/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     1518 2020-04-23 10:03:51.000000 django-slick-reporting-0.7.0/LICENSE.md
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      152 2020-06-07 07:01:50.000000 django-slick-reporting-0.7.0/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9104 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7417 2022-08-26 21:11:35.000000 django-slick-reporting-0.7.0/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9104 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1178 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1003 2021-07-15 08:55:50.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/SOURCES.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2021-07-15 08:55:50.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/dependency_links.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       71 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       66 2021-07-15 08:55:50.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/requires.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/top_level.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2021-07-15 08:55:50.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/top_level.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1675 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-slick-reporting-0.7.0/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      104 2023-05-15 07:50:39.000000 django-slick-reporting-0.7.0/slick_reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1688 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      207 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      722 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/decorators.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    16339 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/fields.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8188 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/form_factory.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    38050 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/generator.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1565 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1693 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/registry.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/static/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2020-12-11 18:31:17.000000 django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/main.js
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7123 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/ra.chartsjs.js
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    19417 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/ra.highchart.js
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/templates/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1937 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/base.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9363 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/simple_report.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      448 2020-07-24 10:59:05.000000 django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/table.html
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2019-11-14 16:41:29.000000 django-slick-reporting-0.7.0/slick_reporting/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      780 2022-07-07 07:19:02.000000 django-slick-reporting-0.7.0/slick_reporting/templatetags/slick_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    14333 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/views.py
```

### Comparing `django-slick-reporting-0.6.8/LICENSE.md` & `django-slick-reporting-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.6.8/PKG-INFO` & `django-slick-reporting-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: django-slick-reporting
-Version: 0.6.8
+Version: 0.7.0
 Summary: A one-stop report and analytics generation and computation with batteries included
 Home-page: https://django-slick-reporting.com/
 Author: Ra Systems
 Author-email: ramez@rasystems.io
-License: UNKNOWN
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/django-slick-reporting/
 Project-URL: Documentation, https://django-slick-reporting.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/django-slick-reporting
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
@@ -254,9 +252,7 @@
 If you like this package, chances are you may like those packages too!
 
 `Django Tabular Permissions <https://github.com/RamezIssac/django-tabular-permissions>`_ Display Django permissions in a HTML table that is translatable and easy customized.
 
 `Django Ra ERP Framework <https://github.com/ra-systems/RA>`_ A framework to build business solutions with ease.
 
 If you find this project useful or promising , You can support us by a github ⭐
-
-
```

### Comparing `django-slick-reporting-0.6.8/README.rst` & `django-slick-reporting-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.6.8/django_slick_reporting.egg-info/PKG-INFO` & `django-slick-reporting-0.7.0/django_slick_reporting.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: django-slick-reporting
-Version: 0.6.8
+Version: 0.7.0
 Summary: A one-stop report and analytics generation and computation with batteries included
 Home-page: https://django-slick-reporting.com/
 Author: Ra Systems
 Author-email: ramez@rasystems.io
-License: UNKNOWN
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/django-slick-reporting/
 Project-URL: Documentation, https://django-slick-reporting.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/django-slick-reporting
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
@@ -254,9 +252,7 @@
 If you like this package, chances are you may like those packages too!
 
 `Django Tabular Permissions <https://github.com/RamezIssac/django-tabular-permissions>`_ Display Django permissions in a HTML table that is translatable and easy customized.
 
 `Django Ra ERP Framework <https://github.com/ra-systems/RA>`_ A framework to build business solutions with ease.
 
 If you find this project useful or promising , You can support us by a github ⭐
-
-
```

### Comparing `django-slick-reporting-0.6.8/django_slick_reporting.egg-info/SOURCES.txt` & `django-slick-reporting-0.7.0/django_slick_reporting.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 django_slick_reporting.egg-info/top_level.txt.py
 slick_reporting/__init__.py
 slick_reporting/app_settings.py
 slick_reporting/apps.py
 slick_reporting/decorators.py
 slick_reporting/fields.py
 slick_reporting/form_factory.py
-slick_reporting/forms.py
 slick_reporting/generator.py
 slick_reporting/helpers.py
 slick_reporting/registry.py
 slick_reporting/views.py
 slick_reporting/static/slick_reporting/main.js
 slick_reporting/static/slick_reporting/ra.chartsjs.js
 slick_reporting/static/slick_reporting/ra.highchart.js
```

### Comparing `django-slick-reporting-0.6.8/setup.cfg` & `django-slick-reporting-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.6.8/slick_reporting/app_settings.py` & `django-slick-reporting-0.7.0/slick_reporting/app_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 import pytz
 from django.conf import settings
 from django.utils.functional import lazy
 
 import datetime
 
+from django.utils.timezone import now
+
 
 def get_first_of_this_year():
     d = datetime.datetime.today()
     return datetime.datetime(d.year, 1, 1, 0, 0)
 
 
 def get_end_of_this_year():
     d = datetime.datetime.today()
     return datetime.datetime(d.year + 1, 1, 1, 0, 0)
 
 
 def get_start_date():
-    start_date = getattr(settings, 'SLICK_REPORTING_DEFAULT_START_DATE', False)
+    start_date = getattr(settings, "SLICK_REPORTING_DEFAULT_START_DATE", False)
     return start_date or get_first_of_this_year()
 
 
 def get_end_date():
-    start_date = getattr(settings, 'SLICK_REPORTING_DEFAULT_END_DATE', False)
-    return start_date or get_end_of_this_year()
+    end_date = getattr(settings, "SLICK_REPORTING_DEFAULT_END_DATE", False)
+    return end_date or datetime.datetime.today()
 
 
 SLICK_REPORTING_DEFAULT_START_DATE = lazy(get_start_date, datetime.datetime)()
 SLICK_REPORTING_DEFAULT_END_DATE = lazy(get_end_date, datetime.datetime)()
 
 SLICK_REPORTING_FORM_MEDIA_DEFAULT = {
-    'css': {
-        'all': (
-            'https://cdn.datatables.net/v/bs4/dt-1.10.20/datatables.min.css',
-            'https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.3/Chart.min.css',
+    "css": {
+        "all": (
+            "https://cdn.datatables.net/v/bs4/dt-1.10.20/datatables.min.css",
+            "https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.3/Chart.min.css",
         )
     },
-    'js': (
-        'https://code.jquery.com/jquery-3.3.1.slim.min.js',
-        'https://cdn.datatables.net/v/bs4/dt-1.10.20/datatables.min.js',
-        'https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.3/Chart.bundle.min.js',
-        'https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.3/Chart.min.js',
-        'https://code.highcharts.com/highcharts.js',
-    )
+    "js": (
+        "https://code.jquery.com/jquery-3.3.1.slim.min.js",
+        "https://cdn.datatables.net/v/bs4/dt-1.10.20/datatables.min.js",
+        "https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.3/Chart.bundle.min.js",
+        "https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.3/Chart.min.js",
+        "https://code.highcharts.com/highcharts.js",
+    ),
 }
 
-SLICK_REPORTING_FORM_MEDIA = getattr(settings, 'SLICK_REPORTING_FORM_MEDIA', SLICK_REPORTING_FORM_MEDIA_DEFAULT)
-SLICK_REPORTING_DEFAULT_CHARTS_ENGINE = getattr(settings, 'SLICK_REPORTING_DEFAULT_CHARTS_ENGINE', 'highcharts')
+SLICK_REPORTING_FORM_MEDIA = getattr(
+    settings, "SLICK_REPORTING_FORM_MEDIA", SLICK_REPORTING_FORM_MEDIA_DEFAULT
+)
+SLICK_REPORTING_DEFAULT_CHARTS_ENGINE = getattr(
+    settings, "SLICK_REPORTING_DEFAULT_CHARTS_ENGINE", "highcharts"
+)
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/decorators.py` & `django-slick-reporting-0.7.0/slick_reporting/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     admin site will be used.
     """
     from .fields import SlickReportField
     from .registry import field_registry
 
     def _model_admin_wrapper(admin_class):
         if not issubclass(admin_class, SlickReportField):
-            raise ValueError('Wrapped class must subclass SlickReportField.')
+            raise ValueError("Wrapped class must subclass SlickReportField.")
 
         field_registry.register(report_field)
 
     _model_admin_wrapper(report_field)
     return report_field
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/fields.py` & `django-slick-reporting-0.7.0/slick_reporting/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
 class SlickReportField(object):
     """
     Computation field responsible for making the calculation unit
     """
 
     _field_registry = field_registry
-    name = ''
+    name = ""
     """The name to be used in the ReportGenerator"""
 
-    calculation_field = 'value'
+    calculation_field = "value"
     """the Field to compute on"""
 
     calculation_method = Sum
     """The computation Method"""
 
     verbose_name = None
     """Verbose name to be used in front end when needed"""
 
     requires = None
     """This can be a list of sibling classes,
     they will be asked to compute and their value would be available to you in the `resolve` method
     requires = [BasicCalculationA, BasicCalculationB]
     """
 
-    type = 'number'
+    type = "number"
     """Just a string describing what this computation field return, usually passed to frontend"""
 
     is_summable = True
     """Indicate if this computation can be summed over. Useful to be passed to frontend or whenever needed"""
 
     report_model = None
     group_by = None
@@ -48,91 +48,122 @@
 
     _require_classes = None
     _debit_and_credit = True
 
     prevent_group_by = False
     """Will prevent group by calculation for this specific field, serves when you want to compute overall results"""
 
+    def __new__(cls, *args, **kwargs):
+        """
+        This is where we register the class in the registry
+        :param args:
+        :param kwargs:
+        :return:
+        """
+        if not cls.name:
+            raise ValueError(f"ReportField {cls} must have a name")
+        return super(SlickReportField, cls).__new__(cls)
+
     @classmethod
     def create(cls, method, field, name=None, verbose_name=None, is_summable=True):
         """
         Creates a ReportField class on the fly
         :param method: The computation Method to be used
         :param field: The field on which the computation would occur
         :param name: a name to refer to this field else where
         :param verbose_name: Verbose name
         :param is_summable:
         :return:
         """
         if not name:
-            identifier = str(uuid.uuid4()).split('-')[-1]
+            identifier = str(uuid.uuid4()).split("-")[-1]
             name = name or f"{method.name.lower()}__{field}"
             assert name not in cls._field_registry.get_all_report_fields_names()
 
-        verbose_name = verbose_name or f'{method.name} {field}'
-        report_klass = type(f'ReportField_{name}', (cls,), {
-            'name': name,
-            'verbose_name': verbose_name,
-            'calculation_field': field,
-            'calculation_method': method,
-            'is_summable': is_summable,
-        })
+        verbose_name = verbose_name or f"{method.name} {field}"
+        report_klass = type(
+            f"ReportField_{name}",
+            (cls,),
+            {
+                "name": name,
+                "verbose_name": verbose_name,
+                "calculation_field": field,
+                "calculation_method": method,
+                "is_summable": is_summable,
+            },
+        )
         return report_klass
 
-    def __init__(self, plus_side_q=None, minus_side_q=None,
-                 report_model=None,
-                 qs=None,
-                 calculation_field=None, calculation_method=None, date_field='', group_by=None):
+    def __init__(
+        self,
+        plus_side_q=None,
+        minus_side_q=None,
+        report_model=None,
+        qs=None,
+        calculation_field=None,
+        calculation_method=None,
+        date_field="",
+        group_by=None,
+    ):
         super(SlickReportField, self).__init__()
         self.date_field = date_field
         self.report_model = self.report_model or report_model
-        self.calculation_field = calculation_field if calculation_field else self.calculation_field
-        self.calculation_method = calculation_method if calculation_method else self.calculation_method
+        self.calculation_field = (
+            calculation_field if calculation_field else self.calculation_field
+        )
+        self.calculation_method = (
+            calculation_method if calculation_method else self.calculation_method
+        )
         self.plus_side_q = self.plus_side_q or plus_side_q
         self.minus_side_q = self.minus_side_q or minus_side_q
         self.requires = self.requires or []
         self.group_by = self.group_by or group_by
         self._cache = None, None, None
         self._require_classes = self._get_required_classes()
 
         if not self.plus_side_q and not self.minus_side_q:
             self._debit_and_credit = False
 
     @classmethod
     def _get_required_classes(cls):
         requires = cls.requires or []
-        return [field_registry.get_field_by_name(x) if type(x) is str else x for x in requires]
+        return [
+            field_registry.get_field_by_name(x) if type(x) is str else x
+            for x in requires
+        ]
 
     def apply_q_plus_filter(self, qs):
         return qs.filter(*self.plus_side_q)
 
     def apply_q_minus_filter(self, qs):
         return qs.filter(*self.minus_side_q)
 
-    def apply_aggregation(self, queryset, group_by=''):
+    def apply_aggregation(self, queryset, group_by=""):
         annotation = self.calculation_method(self.calculation_field)
         if group_by:
             queryset = queryset.values(group_by).annotate(annotation)
         else:
             queryset = queryset.aggregate(annotation)
         return queryset
 
     def init_preparation(self, q_filters=None, kwargs_filters=None, **kwargs):
         """
-        Called by the generator to preparet he calculation of this field + it's requirements
+        Called by the generator to prepare the calculation of this field + it's requirements
         :param q_filters:
         :param kwargs_filters:
         :param kwargs:
         :return:
         """
         kwargs_filters = kwargs_filters or {}
 
         dep_values = self._prepare_dependencies(q_filters, kwargs_filters.copy())
 
-        debit_results, credit_results = self.prepare(q_filters, kwargs_filters, **kwargs)
+        debit_results, credit_results = self.prepare(
+            q_filters, kwargs_filters, **kwargs
+        )
         self._cache = debit_results, credit_results, dep_values
         return self._cache
 
     def prepare(self, q_filters=None, kwargs_filters=None, **kwargs):
         """
         This is the first hook where you can customize the calculation away from the Django Query aggregation method
         This method et called with all available parameters , so you can prepare the results for the whole set and save
@@ -141,15 +172,15 @@
 
         :param q_filters:
         :param kwargs_filters:
         :param kwargs:
         :return:
         """
         queryset = self.get_queryset()
-        group_by = '' if self.prevent_group_by else self.group_by
+        group_by = "" if self.prevent_group_by else self.group_by
         if q_filters:
             queryset = queryset.filter(*q_filters)
         if kwargs_filters:
             queryset = queryset.filter(**kwargs_filters)
 
         if self.plus_side_q:
             queryset = self.apply_q_plus_filter(queryset)
@@ -178,34 +209,44 @@
         return queryset.order_by()
 
     def get_annotation_name(self):
         """
         Get the annotation per the database
         :return: string used ex:
         """
-        return get_calculation_annotation(self.calculation_field, self.calculation_method)
-
-    def _prepare_dependencies(self, q_filters=None, extra_filters=None, ):
+        return get_calculation_annotation(
+            self.calculation_field, self.calculation_method
+        )
+
+    def _prepare_dependencies(
+        self,
+        q_filters=None,
+        extra_filters=None,
+    ):
         values = {}
         for dep_class in self._require_classes:
-            dep = dep_class(self.plus_side_q, self.minus_side_q, self.report_model,
-                            date_field=self.date_field, group_by=self.group_by)
+            dep = dep_class(
+                self.plus_side_q,
+                self.minus_side_q,
+                self.report_model,
+                date_field=self.date_field,
+                group_by=self.group_by,
+            )
             results = dep.init_preparation(q_filters, extra_filters)
-            values[dep.name] = {'results': results,
-                                'instance': dep}
+            values[dep.name] = {"results": results, "instance": dep}
         return values
 
     def resolve(self, current_obj, current_row=None):
-        '''
+        """
         Reponsible for getting the exact data from the prepared value
         :param cached: the returned data from prepare
         :param current_obj: he value of group by id
         :param current_row: the row in iteration
         :return: a solid number or value
-        '''
+        """
         cached = self._cache
         debit_value, credit_value = self.extract_data(cached, current_obj)
         dependencies_value = self._resolve_dependencies(current_obj)
 
         return self.final_calculation(debit_value, credit_value, dependencies_value)
 
     def get_dependency_value(self, current_obj, name=None):
@@ -220,27 +261,26 @@
         """
         values = self._resolve_dependencies(current_obj, name=None)
         if name:
             return values.get(name)
         return values
 
     def _resolve_dependencies(self, current_obj, name=None):
-
         dep_results = {}
         cached_debit, cached_credit, dependencies_value = self._cache
         dependencies_value = dependencies_value or {}
         for d in dependencies_value.keys():
             if name and d != name:
                 continue
-            d_instance = dependencies_value[d]['instance']
+            d_instance = dependencies_value[d]["instance"]
             dep_results[d] = d_instance.resolve(current_obj)
         return dep_results
 
     def extract_data(self, cached, current_obj):
-        group_by = '' if self.prevent_group_by else self.group_by
+        group_by = "" if self.prevent_group_by else self.group_by
         debit_value = 0
         credit_value = 0
         annotation = self.get_annotation_name()
 
         cached_debit, cached_credit, dependencies_value = cached
 
         if cached_debit or cached_credit:
@@ -281,15 +321,14 @@
     def get_full_dependency_list(cls):
         """
         Get the full Hirearchy of dependencies and dependencies dependency.
         :return: List of dependecies classes
         """
 
         def get_dependency(field_class):
-
             dependencies = field_class._get_required_classes()
             klasses = []
             for klass in dependencies:
                 klasses.append(klass)
                 other = get_dependency(klass)
                 if other:
                     klasses += other
@@ -301,148 +340,148 @@
     def get_crosstab_field_verbose_name(cls, model, id):
         """
         Construct a verbose name for the crosstab field
         :param model: the model name
         :param id: the id of the current crosstab object
         :return: a verbose string
         """
-        if id == '----':
-            return _('The reminder')
-        return f'{cls.verbose_name} {model} {id}'
+        if id == "----":
+            return _("The reminder")
+        return f"{cls.verbose_name} {model} {id}"
 
     @classmethod
     def get_time_series_field_verbose_name(cls, date_period, index, dates, pattern):
         """
         Get the name of the verbose name of a computaion field that's in a time_series.
         should be a mix of the date period if the column an it's verbose name.
         :param date_period: a tuple of (start_date, end_date)
         :param index: the index of the current field in the whole dates to be calculated
         :param dates a list of tuples representing the start and the end date
         :return: a verbose string
         """
-        dt_format = '%Y/%m/%d'
+        dt_format = "%Y/%m/%d"
 
-        if pattern == 'monthly':
-            month_name = date_filter(date_period[0], 'F Y')
-            return f'{cls.verbose_name} {month_name}'
-        elif pattern == 'daily':
-            return f'{cls.verbose_name} {date_period[0].strftime(dt_format)}'
-        elif pattern == 'weekly':
-            return f' {cls.verbose_name} {_("Week")} {index} {date_period[0].strftime(dt_format)}'
-        elif pattern == 'yearly':
-            year = date_filter(date_period[0], 'Y')
-            return f'{cls.verbose_name} {year}'
+        if pattern == "monthly":
+            month_name = date_filter(date_period[0], "F Y")
+            return f"{cls.verbose_name} {month_name}"
+        elif pattern == "daily":
+            return f"{cls.verbose_name} {date_period[0].strftime(dt_format)}"
+        elif pattern == "weekly":
+            return f' {cls.verbose_name} {_("Week")} {index + 1} {date_period[0].strftime(dt_format)}'
+        elif pattern == "yearly":
+            year = date_filter(date_period[0], "Y")
+            return f"{cls.verbose_name} {year}"
 
-        return f'{cls.verbose_name} {date_period[0].strftime(dt_format)} - {date_period[1].strftime(dt_format)}'
+        return f"{cls.verbose_name} {date_period[0].strftime(dt_format)} - {date_period[1].strftime(dt_format)}"
 
 
 class FirstBalanceField(SlickReportField):
-    name = '__fb__'
-    verbose_name = _('first balance')
+    name = "__fb__"
+    verbose_name = _("first balance")
 
     def prepare(self, q_filters=None, extra_filters=None, **kwargs):
         extra_filters = extra_filters or {}
 
-        from_date_value = extra_filters.get(f'{self.date_field}__gte')
-        extra_filters.pop(f'{self.date_field}__gte', None)
-        extra_filters[f'{self.date_field}__lt'] = from_date_value
+        from_date_value = extra_filters.get(f"{self.date_field}__gte")
+        extra_filters.pop(f"{self.date_field}__gte", None)
+        extra_filters[f"{self.date_field}__lt"] = from_date_value
         return super(FirstBalanceField, self).prepare(q_filters, extra_filters)
 
 
 field_registry.register(FirstBalanceField)
 
 
 class TotalReportField(SlickReportField):
-    name = '__total__'
-    verbose_name = _('Sum of value')
-    requires = ['__debit__', '__credit__']
+    name = "__total__"
+    verbose_name = _("Sum of value")
+    requires = ["__debit__", "__credit__"]
 
 
 field_registry.register(TotalReportField)
 
 
 class BalanceReportField(SlickReportField):
-    name = '__balance__'
-    verbose_name = _('Cumulative Total')
-    requires = ['__fb__']
+    name = "__balance__"
+    verbose_name = _("Cumulative Total")
+    requires = ["__fb__"]
 
     def final_calculation(self, debit, credit, dep_dict):
-        fb = dep_dict.get('__fb__')
+        fb = dep_dict.get("__fb__")
         debit = debit or 0
         credit = credit or 0
         fb = fb or 0
         return fb + debit - credit
 
 
 field_registry.register(BalanceReportField)
 
 
 class PercentageToBalance(SlickReportField):
     requires = [BalanceReportField]
-    name = 'PercentageToBalance'
-    verbose_name = _('%')
+    name = "PercentageToBalance"
+    verbose_name = _("%")
 
     prevent_group_by = True
 
     def final_calculation(self, debit, credit, dep_dict):
-        obj_balance = dep_dict.get('__balance__')
+        obj_balance = dep_dict.get("__balance__")
         total = debit - credit
         return (obj_balance / total) * 100
 
 
 class CreditReportField(SlickReportField):
-    name = '__credit__'
-    verbose_name = _('Credit')
+    name = "__credit__"
+    verbose_name = _("Credit")
 
     def final_calculation(self, debit, credit, dep_dict):
         return credit
 
 
 field_registry.register(CreditReportField)
 
 
 class DebitReportField(SlickReportField):
-    name = '__debit__'
-    verbose_name = _('Debit')
+    name = "__debit__"
+    verbose_name = _("Debit")
 
     def final_calculation(self, debit, credit, dep_dict):
         return debit
 
 
 field_registry.register(DebitReportField)
 
 
 class TotalQTYReportField(SlickReportField):
-    name = '__total_quantity__'
-    verbose_name = _('Total QTY')
-    calculation_field = 'quantity'
+    name = "__total_quantity__"
+    verbose_name = _("Total QTY")
+    calculation_field = "quantity"
     is_summable = False
 
 
 field_registry.register(TotalQTYReportField)
 
 
 class FirstBalanceQTYReportField(FirstBalanceField):
-    name = '__fb_quan__'
-    verbose_name = _('starting QTY')
-    calculation_field = 'quantity'
+    name = "__fb_quan__"
+    verbose_name = _("starting QTY")
+    calculation_field = "quantity"
     is_summable = False
 
 
 field_registry.register(FirstBalanceQTYReportField)
 
 
 class BalanceQTYReportField(SlickReportField):
-    name = '__balance_quantity__'
-    verbose_name = _('Cumulative QTY')
-    calculation_field = 'quantity'
-    requires = ['__fb_quan__']
+    name = "__balance_quantity__"
+    verbose_name = _("Cumulative QTY")
+    calculation_field = "quantity"
+    requires = ["__fb_quan__"]
     is_summable = False
 
     def final_calculation(self, debit, credit, dep_dict):
         # Use `get` so it fails loud if its not there
-        fb = dep_dict.get('__fb_quan__')
+        fb = dep_dict.get("__fb_quan__")
         fb = fb or 0
         return fb + debit - credit
 
 
 field_registry.register(BalanceQTYReportField)
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/form_factory.py` & `django-slick-reporting-0.7.0/slick_reporting/form_factory.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,113 +3,163 @@
 from django import forms
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 
 from . import app_settings
 from .helpers import get_foreign_keys
 
+TIME_SERIES_CHOICES = (
+    ("monthly", _("Monthly")),
+    ("weekly", _("Weekly")),
+    ("annually", _("Yearly")),
+    ("daily", _("Daily")),
+)
+
+
+def default_formfield_callback(f, **kwargs):
+    kwargs["required"] = False
+    kwargs["help_text"] = ""
+    return f.formfield(**kwargs)
+
+
+def get_crispy_helper(
+    foreign_keys_map=None,
+    crosstab_model=None,
+    crosstab_key_name=None,
+    crosstab_display_compute_reminder=False,
+    add_date_range=True,
+):
+    from crispy_forms.helper import FormHelper
+    from crispy_forms.layout import Column, Layout, Div, Row, Field
+
+    helper = FormHelper()
+    helper.form_class = "form-horizontal"
+    helper.label_class = "col-sm-2 col-md-2 col-lg-2"
+    helper.field_class = "col-sm-10 col-md-10 col-lg-10"
+    helper.form_tag = False
+    helper.disable_csrf = True
+    helper.render_unmentioned_fields = True
+
+    helper.layout = Layout()
+    if add_date_range:
+        helper.layout.fields.append(
+            Row(
+                Column(Field("start_date"), css_class="col-sm-6"),
+                Column(Field("end_date"), css_class="col-sm-6"),
+                css_class="raReportDateRange",
+            ),
+        )
+    filters_container = Div(css_class="mt-20", style="margin-top:20px")
+    # first add the crosstab model and its display reimder then the rest of the fields
+    if crosstab_model:
+        filters_container.append(Field(crosstab_key_name))
+        if crosstab_display_compute_reminder:
+            filters_container.append(Field("crosstab_compute_reminder"))
+
+    for k in foreign_keys_map:
+        if k != crosstab_key_name:
+            filters_container.append(Field(k))
+    helper.layout.fields.append(filters_container)
+
+    return helper
+
 
 class BaseReportForm:
-    '''
+    """
     Holds basic function
-    '''
+    """
 
     @property
     def media(self):
         from .app_settings import SLICK_REPORTING_FORM_MEDIA
-        return forms.Media(css=SLICK_REPORTING_FORM_MEDIA.get('css', {}), js=SLICK_REPORTING_FORM_MEDIA.get('js', []))
+
+        return forms.Media(
+            css=SLICK_REPORTING_FORM_MEDIA.get("css", {}),
+            js=SLICK_REPORTING_FORM_MEDIA.get("js", []),
+        )
 
     def get_filters(self):
         """
         Get the foreign key filters for report queryset, excluding crosstab ids, handled by `get_crosstab_ids()`
         :return: a dicttionary of filters to be used with QuerySet.filter(**returned_value)
         """
         _values = {}
         if self.is_valid():
-            fk_keys = getattr(self, 'foreign_keys', [])
+            fk_keys = getattr(self, "foreign_keys", [])
             if fk_keys:
                 fk_keys = fk_keys.items()
             for key, field in fk_keys:
                 if key in self.cleaned_data and not key == self.crosstab_key_name:
                     val = self.cleaned_data[key]
                     if val:
-                        val = [x for x in val.values_list('pk', flat=True)]
-                        _values['%s__in' % key] = val
+                        val = [x for x in val.values_list("pk", flat=True)]
+                        _values["%s__in" % key] = val
             return None, _values
 
     @cached_property
     def crosstab_key_name(self):
         """
         return the actual foreignkey field name by simply adding an '_id' at the end.
         This is hook is to customize this naieve approach.
         :return: key: a string that should be in self.cleaned_data
         """
-        return f'{self.crosstab_model}_id'
+        return f"{self.crosstab_model}_id"
 
     def get_crosstab_ids(self):
         """
         Get the crosstab ids so they can be sent to the report generator.
-        :return: 
+        :return:
         """
         if self.crosstab_model:
             qs = self.cleaned_data.get(self.crosstab_key_name)
-            return [x for x in qs.values_list('pk', flat=True)]
+            return [x for x in qs.values_list("pk", flat=True)]
         return []
 
     def get_crosstab_compute_reminder(self):
-        return self.cleaned_data.get('crosstab_compute_reminder', True)
+        return self.cleaned_data.get("crosstab_compute_reminder", True)
 
     def get_crispy_helper(self, foreign_keys_map=None, crosstab_model=None, **kwargs):
-        from crispy_forms.helper import FormHelper
-        from crispy_forms.layout import Column, Layout, Div, Row, Field
-
-        helper = FormHelper()
-        helper.form_class = 'form-horizontal'
-        helper.label_class = 'col-sm-2 col-md-2 col-lg-2'
-        helper.field_class = 'col-sm-10 col-md-10 col-lg-10'
-        helper.form_tag = False
-        helper.disable_csrf = True
-        helper.render_unmentioned_fields = True
-
-        foreign_keys_map = foreign_keys_map or self.foreign_keys
-
-        helper.layout = Layout(
-            Row(
-                Column(
-                    Field('start_date'), css_class='col-sm-6'),
-                Column(
-                    Field('end_date'), css_class='col-sm-6'),
-                css_class='raReportDateRange'),
-            Div(css_class="mt-20", style='margin-top:20px')
+        return get_crispy_helper(
+            self.foreign_keys,
+            crosstab_model=getattr(self, "crosstab_model", None),
+            crosstab_key_name=getattr(self, "crosstab_key_name", None),
+            crosstab_display_compute_reminder=getattr(
+                self, "crosstab_display_compute_reminder", False
+            ),
+            **kwargs,
         )
 
-        # first add the crosstab model and its display reimder then the rest of the fields
-        if self.crosstab_model:
-            helper.layout.fields[1].append(Field(self.crosstab_key_name))
-            if self.crosstab_display_compute_reminder:
-                helper.layout.fields[1].append(Field('crosstab_compute_reminder'))
-
-        for k in foreign_keys_map:
-            if k != self.crosstab_key_name:
-                helper.layout.fields[1].append(Field(k))
-
-        return helper
-
 
 def _default_foreign_key_widget(f_field):
-    return {'form_class': forms.ModelMultipleChoiceField, 'required': False, }
-
-
-def report_form_factory(model, crosstab_model=None, display_compute_reminder=True, fkeys_filter_func=None,
-                        foreign_key_widget_func=None, excluded_fields=None, initial=None, required=None):
+    return {
+        "form_class": forms.ModelMultipleChoiceField,
+        "required": False,
+    }
+
+
+def report_form_factory(
+    model,
+    crosstab_model=None,
+    display_compute_reminder=True,
+    fkeys_filter_func=None,
+    foreign_key_widget_func=None,
+    excluded_fields=None,
+    initial=None,
+    required=None,
+    show_time_series_selector=False,
+    time_series_selector_choices=None,
+    time_series_selector_default="",
+    time_series_selector_label=None,
+    time_series_selector_allow_empty=False,
+):
     """
     Create a Report Form based on the report_model passed by
     1. adding a start_date and end_date fields
     2. extract all ForeignKeys on the report_model
-    
+
     :param model: the report_model
     :param crosstab_model: crosstab model if any
     :param display_compute_reminder:  relevant only if crosstab_model is specified. Control if we show the check to
     display the rest.
     :param fkeys_filter_func:  a receives an OrderedDict of Foreign Keys names and their model field instances found on the model, return the OrderedDict that would be used
     :param foreign_key_widget_func: receives a Field class return the used widget like this {'form_class': forms.ModelMultipleChoiceField, 'required': False, }
     :param excluded_fields: a list of fields to be excluded from the report form
@@ -129,38 +179,63 @@
         del fkeys_map[excluded]
 
     fkeys_map = fkeys_filter_func(fkeys_map)
 
     fkeys_list = []
     fields = OrderedDict()
 
-    fields['start_date'] = forms.DateTimeField(required=False, label=_('From date'),
-                                               initial=initial.get('start_date',
-                                                                   app_settings.SLICK_REPORTING_DEFAULT_START_DATE),
-                                               widget=forms.DateTimeInput(attrs={'autocomplete': "off"}))
-
-    fields['end_date'] = forms.DateTimeField(required=False, label=_('To  date'),
-                                             initial=initial.get('end_date',
-                                                                 app_settings.SLICK_REPORTING_DEFAULT_END_DATE),
-                                             widget=forms.DateTimeInput(attrs={'autocomplete': "off"}))
+    fields["start_date"] = forms.DateTimeField(
+        required=False,
+        label=_("From date"),
+        initial=initial.get(
+            "start_date", app_settings.SLICK_REPORTING_DEFAULT_START_DATE
+        ),
+        widget=forms.DateTimeInput(attrs={"autocomplete": "off"}),
+    )
+
+    fields["end_date"] = forms.DateTimeField(
+        required=False,
+        label=_("To  date"),
+        initial=initial.get("end_date", app_settings.SLICK_REPORTING_DEFAULT_END_DATE),
+        widget=forms.DateTimeInput(attrs={"autocomplete": "off"}),
+    )
+
+    if show_time_series_selector:
+        time_series_choices = tuple(TIME_SERIES_CHOICES)
+        if time_series_selector_allow_empty:
+            time_series_choices.insert(0, ("", "---------"))
+
+        fields["time_series_pattern"] = forms.ChoiceField(
+            required=False,
+            initial=time_series_selector_default,
+            label=time_series_selector_label or _("Period Pattern"),
+            choices=time_series_selector_choices or TIME_SERIES_CHOICES,
+        )
 
     for name, f_field in fkeys_map.items():
         fkeys_list.append(name)
         field_attrs = foreign_key_widget_func(f_field)
         if name in required:
-            field_attrs['required'] = True
+            field_attrs["required"] = True
         fields[name] = f_field.formfield(**field_attrs)
 
     if crosstab_model and display_compute_reminder:
-        fields['crosstab_compute_reminder'] = forms.BooleanField(required=False,
-                                                                 label=_('Display the crosstab reminder'),
-                                                                 initial=True)
-
-    bases = (BaseReportForm, forms.BaseForm,)
-    new_form = type('ReportForm', bases,
-                    {"base_fields": fields,
-                     '_fkeys': fkeys_list,
-                     'foreign_keys': fkeys_map,
-                     'crosstab_model': crosstab_model,
-                     'crosstab_display_compute_reminder': display_compute_reminder,
-                     })
+        fields["crosstab_compute_reminder"] = forms.BooleanField(
+            required=False, label=_("Display the crosstab reminder"), initial=True
+        )
+
+    bases = (
+        BaseReportForm,
+        forms.BaseForm,
+    )
+    new_form = type(
+        "ReportForm",
+        bases,
+        {
+            "base_fields": fields,
+            "_fkeys": fkeys_list,
+            "foreign_keys": fkeys_map,
+            "crosstab_model": crosstab_model,
+            "crosstab_display_compute_reminder": display_compute_reminder,
+        },
+    )
     return new_form
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/generator.py` & `django-slick-reporting-0.7.0/slick_reporting/generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,50 @@
 from __future__ import unicode_literals
 
 import datetime
 import logging
+from dataclasses import dataclass
+from inspect import isclass
+
 from django.core.exceptions import ImproperlyConfigured, FieldDoesNotExist
 from django.db.models import Q, ForeignKey
-from inspect import isclass
 
 from .app_settings import SLICK_REPORTING_DEFAULT_CHARTS_ENGINE
 from .fields import SlickReportField
 from .helpers import get_field_from_query_text
 from .registry import field_registry
 
 logger = logging.getLogger(__name__)
 
 
+@dataclass
+class Chart:
+    title: str
+    type: str
+    data_source: list
+    title_source: list
+    plot_total: bool = False
+    engine: str = SLICK_REPORTING_DEFAULT_CHARTS_ENGINE
+    COLUMN = "column"
+    LINE = "line"
+    PIE = "pie"
+    BAR = "bar"
+    AREA = "area"
+
+    def to_dict(self):
+        return dict(
+            title=self.title,
+            type=self.type,
+            data_source=self.data_source,
+            title_source=self.title_source,
+            plot_total=self.plot_total,
+            engine=self.engine,
+        )
+
+
 class ReportGenerator(object):
     """
     The main class responsible generating the report and managing the flow
     """
 
     field_registry_class = field_registry
     """You can have a custom computation field locator! It only needs a `get_field_by_name(string)` 
@@ -59,15 +86,15 @@
     
     You can customize aspects of the column by adding it as a tuple like this 
         ('field_name', dict(verbose_name=_('My Enhanced Verbose_name'))
         
          
      """
 
-    time_series_pattern = ''
+    time_series_pattern = ""
     """
     If set the Report will compute a time series.
     
     Possible options are: daily, weekly, semimonthly, monthly, quarterly, semiannually, annually and custom.
     
     if `custom` is set, you'd need to override  `get_custom_time_series_dates`
     """
@@ -113,22 +140,41 @@
 
     limit_records = None
     """Serves are a main limit to  the returned data of teh report_model.
     Can be beneficial if the results may be huge.
     """
     swap_sign = False
 
-    def __init__(self, report_model=None, main_queryset=None, start_date=None, end_date=None, date_field=None,
-                 q_filters=None, kwargs_filters=None,
-                 group_by=None, columns=None,
-                 time_series_pattern=None, time_series_columns=None, time_series_custom_dates=None,
-                 crosstab_model=None, crosstab_columns=None, crosstab_ids=None, crosstab_compute_reminder=None,
-                 swap_sign=False, show_empty_records=None,
-                 print_flag=False,
-                 doc_type_plus_list=None, doc_type_minus_list=None, limit_records=False, format_row_func=None):
+    def __init__(
+        self,
+        report_model=None,
+        main_queryset=None,
+        start_date=None,
+        end_date=None,
+        date_field=None,
+        q_filters=None,
+        kwargs_filters=None,
+        group_by=None,
+        columns=None,
+        time_series_pattern=None,
+        time_series_columns=None,
+        time_series_custom_dates=None,
+        crosstab_model=None,
+        crosstab_columns=None,
+        crosstab_ids=None,
+        crosstab_compute_reminder=None,
+        swap_sign=False,
+        show_empty_records=None,
+        print_flag=False,
+        doc_type_plus_list=None,
+        doc_type_minus_list=None,
+        limit_records=False,
+        format_row_func=None,
+        container_class=None,
+    ):
         """
 
         :param report_model: Main model containing the data
         :param main_queryset: Default to report_model.objects
         :param start_date:
         :param end_date:
         :param date_field:
@@ -146,80 +192,112 @@
         :param show_empty_records:
         :param base_model:
         :param print_flag:
         :param doc_type_plus_list:
         :param doc_type_minus_list:
         :param limit_records:
         """
-        from .app_settings import SLICK_REPORTING_DEFAULT_START_DATE, SLICK_REPORTING_DEFAULT_END_DATE
+        from .app_settings import (
+            SLICK_REPORTING_DEFAULT_START_DATE,
+            SLICK_REPORTING_DEFAULT_END_DATE,
+        )
 
         super(ReportGenerator, self).__init__()
 
         self.report_model = self.report_model or report_model
         if not self.report_model:
-            raise ImproperlyConfigured('report_model must be set on a class level or via init')
-
-        self.start_date = start_date or datetime.datetime.combine(SLICK_REPORTING_DEFAULT_START_DATE.date(),
-                                                                  SLICK_REPORTING_DEFAULT_START_DATE.time())
+            raise ImproperlyConfigured(
+                "report_model must be set on a class level or via init"
+            )
+
+        self.start_date = start_date or datetime.datetime.combine(
+            SLICK_REPORTING_DEFAULT_START_DATE.date(),
+            SLICK_REPORTING_DEFAULT_START_DATE.time(),
+        )
 
-        self.end_date = end_date or datetime.datetime.combine(SLICK_REPORTING_DEFAULT_END_DATE.date(),
-                                                              SLICK_REPORTING_DEFAULT_END_DATE.time())
+        self.end_date = end_date or datetime.datetime.combine(
+            SLICK_REPORTING_DEFAULT_END_DATE.date(),
+            SLICK_REPORTING_DEFAULT_END_DATE.time(),
+        )
         self.date_field = self.date_field or date_field
-        if not self.date_field:
-            raise ImproperlyConfigured('date_field must be set on a class level or via init')
 
         self.q_filters = q_filters or []
         self.kwargs_filters = kwargs_filters or {}
 
         self.crosstab_model = self.crosstab_model or crosstab_model
         self.crosstab_columns = crosstab_columns or self.crosstab_columns or []
         self.crosstab_ids = self.crosstab_ids or crosstab_ids or []
-        self.crosstab_compute_reminder = self.crosstab_compute_reminder if crosstab_compute_reminder is None else crosstab_compute_reminder
+        self.crosstab_compute_reminder = (
+            self.crosstab_compute_reminder
+            if crosstab_compute_reminder is None
+            else crosstab_compute_reminder
+        )
 
         self.format_row = format_row_func or self._default_format_row
 
         main_queryset = main_queryset or self.report_model.objects
         main_queryset = main_queryset.order_by()
 
         self.columns = columns or self.columns or []
         self.group_by = group_by or self.group_by
 
         self.time_series_pattern = self.time_series_pattern or time_series_pattern
         self.time_series_columns = self.time_series_columns or time_series_columns
-        self.time_series_custom_dates = self.time_series_custom_dates or time_series_custom_dates
+        self.time_series_custom_dates = (
+            self.time_series_custom_dates or time_series_custom_dates
+        )
+        self.container_class = container_class
+
+        if not self.date_field and (
+            self.time_series_pattern or self.crosstab_model or self.group_by
+        ):
+            raise ImproperlyConfigured(
+                "date_field must be set on a class level or via init"
+            )
 
         self._prepared_results = {}
         self.report_fields_classes = {}
 
-        self._report_fields_dependencies = {'time_series': {}, 'crosstab': {}, 'normal': {}}
-        self.existing_dependencies = {'series': [], 'matrix': [], 'normal': []}
+        self._report_fields_dependencies = {
+            "time_series": {},
+            "crosstab": {},
+            "normal": {},
+        }
+        self.existing_dependencies = {"series": [], "matrix": [], "normal": []}
 
         self.print_flag = print_flag or self.print_flag
 
         # todo validate columns is not empty (if no time series / cross tab)
 
         if self.group_by:
             try:
-                self.group_by_field = get_field_from_query_text(self.group_by, self.report_model)
+                self.group_by_field = get_field_from_query_text(
+                    self.group_by, self.report_model
+                )
 
             except (IndexError, AttributeError):
                 raise ImproperlyConfigured(
-                    f'Can not find group_by field:{self.group_by} in report_model {self.report_model} ')
-            if '__' not in self.group_by:
+                    f"Can not find group_by field:{self.group_by} in report_model {self.report_model} "
+                )
+            if "__" not in self.group_by:
                 self.group_by_field_attname = self.group_by_field.attname
             else:
                 self.group_by_field_attname = self.group_by
 
         else:
             self.group_by_field_attname = None
 
         # doc_types = form.get_doc_type_plus_minus_lists()
         doc_types = [], []
-        self.doc_type_plus_list = list(doc_type_plus_list) if doc_type_plus_list else doc_types[0]
-        self.doc_type_minus_list = list(doc_type_minus_list) if doc_type_minus_list else doc_types[1]
+        self.doc_type_plus_list = (
+            list(doc_type_plus_list) if doc_type_plus_list else doc_types[0]
+        )
+        self.doc_type_minus_list = (
+            list(doc_type_minus_list) if doc_type_minus_list else doc_types[1]
+        )
 
         self.swap_sign = self.swap_sign or swap_sign
         self.limit_records = self.limit_records or limit_records
 
         # passed to the report fields
         # self.date_field = date_field or self.date_field
 
@@ -227,183 +305,228 @@
         # a client who didnt make a transaction during the date period.
         self.show_empty_records = False  # show_empty_records if show_empty_records else self.show_empty_records
         # Looks like this options is harder then what i thought as it interfere with the usual filtering of the report
 
         # Preparing actions
         self._parse()
         if self.group_by:
-
             if self.show_empty_records:
                 pass
                 # group_by_filter = self.kwargs_filters.get(self.group_by, '')
                 # qs = self.group_by_field.related_model.objects
                 # if group_by_filter:
                 #     lookup = 'pk__in' if isinstance(group_by_filter, Iterable) else 'pk'
                 #     qs = qs.filter(**{lookup: group_by_filter})
                 # self.main_queryset = qs.values()
 
             else:
                 self.main_queryset = self._apply_queryset_options(main_queryset)
                 if type(self.group_by_field) is ForeignKey:
-                    ids = self.main_queryset.values_list(self.group_by_field_attname).distinct()
+                    ids = self.main_queryset.values_list(
+                        self.group_by_field_attname
+                    ).distinct()
                     # uses the same logic that is in Django's query.py when fields is empty in values() call
-                    concrete_fields = [f.name for f in self.group_by_field.related_model._meta.concrete_fields]
+                    concrete_fields = [
+                        f.name
+                        for f in self.group_by_field.related_model._meta.concrete_fields
+                    ]
                     # add database columns that are not already in concrete_fields
-                    final_fields = concrete_fields + list(set(self.get_database_columns()) - set(concrete_fields))
-                    self.main_queryset = self.group_by_field.related_model.objects.filter(pk__in=ids).values(
-                        *final_fields)
+                    final_fields = concrete_fields + list(
+                        set(self.get_database_columns()) - set(concrete_fields)
+                    )
+                    self.main_queryset = (
+                        self.group_by_field.related_model.objects.filter(
+                            pk__in=ids
+                        ).values(*final_fields)
+                    )
                 else:
-                    self.main_queryset = self.main_queryset.distinct().values(self.group_by_field_attname)
+                    self.main_queryset = self.main_queryset.distinct().values(
+                        self.group_by_field_attname
+                    )
         else:
             if self.time_series_pattern:
                 self.main_queryset = [{}]
             else:
-                self.main_queryset = self._apply_queryset_options(main_queryset, self.get_database_columns())
+                self.main_queryset = self._apply_queryset_options(
+                    main_queryset, self.get_database_columns()
+                )
         self._prepare_report_dependencies()
 
     def _apply_queryset_options(self, query, fields=None):
         """
         Apply the filters to the main queryset which will computed results be mapped to
         :param query:
         :param fields:
         :return:
         """
-
-        filters = {
-            f'{self.date_field}__gt': self.start_date,
-            f'{self.date_field}__lte': self.end_date,
-        }
+        filters = {}
+        if self.date_field:
+            filters = {
+                f"{self.date_field}__gt": self.start_date,
+                f"{self.date_field}__lte": self.end_date,
+            }
         filters.update(self.kwargs_filters)
 
         if filters:
             query = query.filter(**filters)
         if fields:
             return query.values(*fields)
         return query.values()
 
     def _construct_crosstab_filter(self, col_data):
         """
         In charge of adding the needed crosstab filter, specific to the case of is_reminder or not
         :param col_data:
         :return:
         """
-        if col_data['is_reminder']:
+        if col_data["is_reminder"]:
             filters = [~Q(**{f"{col_data['model']}_id__in": self.crosstab_ids})]
         else:
-            filters = [Q(**{f"{col_data['model']}_id": col_data['id']})]
+            filters = [Q(**{f"{col_data['model']}_id": col_data["id"]})]
         return filters
 
     def _prepare_report_dependencies(self):
         from .fields import SlickReportField
+
         all_columns = (
-            ('normal', self._parsed_columns),
-            ('time_series', self._time_series_parsed_columns),
-            ('crosstab', self._crosstab_parsed_columns),
+            ("normal", self._parsed_columns),
+            ("time_series", self._time_series_parsed_columns),
+            ("crosstab", self._crosstab_parsed_columns),
         )
         for window, window_cols in all_columns:
             for col_data in window_cols:
-                klass = col_data['ref']
+                klass = col_data["ref"]
 
                 if isclass(klass) and issubclass(klass, SlickReportField):
                     dependencies_names = klass.get_full_dependency_list()
 
                     # check if any of these dependencies is on the report, if found we call the child to
                     # resolve the value for its parent avoiding extra database call
-                    fields_on_report = [x for x in window_cols if x['ref'] in dependencies_names
-                                        and ((window == 'time_series' and x.get('start_date', '') == col_data.get('start_date', '') and x.get('end_date') == col_data.get('end_date')) or
-                                             window == 'crosstab' and x.get('id') == col_data.get('id'))]
+                    fields_on_report = [
+                        x
+                        for x in window_cols
+                        if x["ref"] in dependencies_names
+                        and (
+                            (
+                                window == "time_series"
+                                and x.get("start_date", "")
+                                == col_data.get("start_date", "")
+                                and x.get("end_date") == col_data.get("end_date")
+                            )
+                            or window == "crosstab"
+                            and x.get("id") == col_data.get("id")
+                        )
+                    ]
                     for field in fields_on_report:
-                        self._report_fields_dependencies[window][field['name']] = col_data['name']
+                        self._report_fields_dependencies[window][
+                            field["name"]
+                        ] = col_data["name"]
             for col_data in window_cols:
-                klass = col_data['ref']
-                name = col_data['name']
+                klass = col_data["ref"]
+                name = col_data["name"]
 
                 # if column has a dependency then skip it
                 if not (isclass(klass) and issubclass(klass, SlickReportField)):
                     continue
                 if self._report_fields_dependencies[window].get(name, False):
                     continue
 
-                report_class = klass(self.doc_type_plus_list, self.doc_type_minus_list,
-                                     group_by=self.group_by,
-                                     report_model=self.report_model, date_field=self.date_field)
+                report_class = klass(
+                    self.doc_type_plus_list,
+                    self.doc_type_minus_list,
+                    group_by=self.group_by,
+                    report_model=self.report_model,
+                    date_field=self.date_field,
+                )
 
                 q_filters = None
                 date_filter = {
-                    f'{self.date_field}__gte': col_data.get('start_date', self.start_date),
-                    f'{self.date_field}__lt': col_data.get('end_date', self.end_date),
+                    f"{self.date_field}__gte": col_data.get(
+                        "start_date", self.start_date
+                    ),
+                    f"{self.date_field}__lt": col_data.get("end_date", self.end_date),
                 }
                 date_filter.update(self.kwargs_filters)
-                if window == 'crosstab':
+                if window == "crosstab":
                     q_filters = self._construct_crosstab_filter(col_data)
 
                 report_class.init_preparation(q_filters, date_filter)
                 self.report_fields_classes[name] = report_class
 
     @staticmethod
     def get_primary_key_name(model):
         for field in model._meta.fields:
             if field.primary_key:
                 return field.attname
-        return ''
+        return ""
 
     def _get_record_data(self, obj, columns):
         """
         the function is run for every obj in the main_queryset
         :param obj: current row
         :param: columns： The columns we iterate on
         :return: a dict object containing all needed data
         """
 
         data = {}
         group_by_val = None
         if self.group_by:
-            if self.group_by_field.related_model and '__' not in self.group_by:
-                primary_key_name = self.get_primary_key_name(self.group_by_field.related_model)
+            if self.group_by_field.related_model and "__" not in self.group_by:
+                primary_key_name = self.get_primary_key_name(
+                    self.group_by_field.related_model
+                )
             else:
                 primary_key_name = self.group_by_field_attname
 
-            column_data = obj.get(primary_key_name, obj.get('id'))
+            column_data = obj.get(primary_key_name, obj.get("id"))
             group_by_val = str(column_data)
 
         for window, window_cols in columns:
             for col_data in window_cols:
+                name = col_data["name"]
 
-                name = col_data['name']
-
-                if col_data.get('source', '') == 'attribute_field':
-                    data[name] = col_data['ref'](self, obj, data)
-
-                elif (col_data.get('source', '') == 'magic_field' and self.group_by) or (
-                        self.time_series_pattern and not self.group_by):
+                if col_data.get("source", "") == "attribute_field":
+                    data[name] = col_data["ref"](self, obj, data)
+                elif col_data.get("source", "") == "container_class_attribute_field":
+                    data[name] = col_data["ref"](obj, data)
+
+                elif (
+                    col_data.get("source", "") == "magic_field" and self.group_by
+                ) or (self.time_series_pattern and not self.group_by):
                     source = self._report_fields_dependencies[window].get(name, False)
                     if source:
                         computation_class = self.report_fields_classes[source]
-                        value = computation_class.get_dependency_value(group_by_val,
-                                                                       col_data['ref'].name)
+                        value = computation_class.get_dependency_value(
+                            group_by_val, col_data["ref"].name
+                        )
                     else:
                         try:
                             computation_class = self.report_fields_classes[name]
                         except KeyError:
                             continue
                         value = computation_class.resolve(group_by_val, data)
-                    if self.swap_sign: value = -value
+                    if self.swap_sign:
+                        value = -value
                     data[name] = value
 
                 else:
-                    data[name] = obj.get(name, '')
+                    data[name] = obj.get(name, "")
         return data
 
     def get_report_data(self):
-        main_queryset = self.main_queryset[:self.limit_records] if self.limit_records else self.main_queryset
+        main_queryset = (
+            self.main_queryset[: self.limit_records]
+            if self.limit_records
+            else self.main_queryset
+        )
 
         all_columns = (
-            ('normal', self._parsed_columns),
-            ('time_series', self._time_series_parsed_columns),
-            ('crosstab', self._crosstab_parsed_columns),
+            ("normal", self._parsed_columns),
+            ("time_series", self._time_series_parsed_columns),
+            ("crosstab", self._crosstab_parsed_columns),
         )
 
         get_record_data = self._get_record_data
         format_row = self.format_row
         data = [format_row(get_record_data(obj, all_columns)) for obj in main_queryset]
         return data
 
@@ -412,129 +535,165 @@
         Hook where you can format row values like properly format a date
         :param row_obj:
         :return:
         """
         return row_obj
 
     @classmethod
-    def check_columns(cls, columns, group_by, report_model, ):
+    def check_columns(cls, columns, group_by, report_model, container_class=None):
         """
         Check and parse the columns, throw errors in case an item in the columns cant not identified
         :param columns: List of columns
         :param group_by: group by field if any
         :param report_model: the report model
+        :param container_class: a class to search for custom columns attribute in, typically the SlickReportView
         :return: List of dict, each dict contains relevant data to the respective field in `columns`
         """
-        group_by_field = ''
+        group_by_field = ""
         group_by_model = None
         if group_by:
             try:
-                group_by_field = [x for x in report_model._meta.get_fields() if x.name == group_by.split('__')[0]][0]
+                group_by_field = [
+                    x
+                    for x in report_model._meta.get_fields()
+                    if x.name == group_by.split("__")[0]
+                ][0]
             except IndexError:
-                raise ImproperlyConfigured(f"Could not find {group_by} in {report_model}")
+                raise ImproperlyConfigured(
+                    f"Could not find {group_by} in {report_model}"
+                )
             if group_by_field.is_relation:
                 group_by_model = group_by_field.related_model
             else:
                 group_by_model = report_model
 
         parsed_columns = []
         for col in columns:
             options = {}
             if type(col) is tuple:
                 col, options = col
 
-            if col in ['__time_series__', '__crosstab__']:
+            if col in ["__time_series__", "__crosstab__"]:
                 #     These are placeholder not real computation field
                 continue
 
             magic_field_class = None
             attribute_field = None
+            is_container_class_attribute = False
 
             if type(col) is str:
                 attribute_field = getattr(cls, col, None)
+                if attribute_field is None:
+                    is_container_class_attribute = True
+                    attribute_field = getattr(container_class, col, None)
+
             elif issubclass(col, SlickReportField):
                 magic_field_class = col
 
             try:
-                magic_field_class = magic_field_class or field_registry.get_field_by_name(col)
+                magic_field_class = (
+                    magic_field_class or field_registry.get_field_by_name(col)
+                )
             except KeyError:
                 magic_field_class = None
 
             if attribute_field:
-                col_data = {'name': col,
-                            'verbose_name': getattr(attribute_field, 'verbose_name', col),
-                            'source': 'attribute_field',
-                            'ref': attribute_field,
-                            'type': 'text'
-                            }
+                col_data = {
+                    "name": col,
+                    "verbose_name": getattr(attribute_field, "verbose_name", col),
+                    "source": "container_class_attribute_field"
+                    if is_container_class_attribute
+                    else "attribute_field",
+                    "ref": attribute_field,
+                    "type": "text",
+                }
             elif magic_field_class:
                 # a magic field
-                col_data = {'name': magic_field_class.name,
-                            'verbose_name': magic_field_class.verbose_name,
-                            'source': 'magic_field',
-                            'ref': magic_field_class,
-                            'type': magic_field_class.type,
-                            'is_summable': magic_field_class.is_summable
-                            }
+                col_data = {
+                    "name": magic_field_class.name,
+                    "verbose_name": magic_field_class.verbose_name,
+                    "source": "magic_field",
+                    "ref": magic_field_class,
+                    "type": magic_field_class.type,
+                    "is_summable": magic_field_class.is_summable,
+                }
             else:
                 # A database field
-                model_to_use = group_by_model if group_by and '__' not in group_by else report_model
+                model_to_use = (
+                    group_by_model
+                    if group_by and "__" not in group_by
+                    else report_model
+                )
                 group_by_str = str(group_by)
-                if '__' in group_by_str:
-                    related_model = get_field_from_query_text(group_by, model_to_use).related_model
+                if "__" in group_by_str:
+                    related_model = get_field_from_query_text(
+                        group_by, model_to_use
+                    ).related_model
                     model_to_use = related_model if related_model else model_to_use
 
                 try:
-                    if '__' in col:
+                    if "__" in col:
                         # A traversing link order__client__email
                         field = get_field_from_query_text(col, model_to_use)
                     else:
                         field = model_to_use._meta.get_field(col)
                 except FieldDoesNotExist:
-                    raise FieldDoesNotExist(
-                        f'Field "{col}" not found either as an attribute to the generator class {cls}, '
-                        f'or a computation field, or a database column for the model "{model_to_use}"')
-
-                col_data = {'name': col,
-                            'verbose_name': getattr(field, 'verbose_name', col),
-                            'source': 'database',
-                            'ref': field,
-                            'type': field.get_internal_type()
-                            }
+                    field = getattr(container_class, col, False)
+
+                    if not field:
+                        raise FieldDoesNotExist(
+                            f'Field "{col}" not found either as an attribute to the generator class {cls}, '
+                            f'{f"Container class {container_class}," if container_class else ""}'
+                            f'or a computation field, or a database column for the model "{model_to_use}"'
+                        )
+
+                col_data = {
+                    "name": col,
+                    "verbose_name": getattr(field, "verbose_name", col),
+                    "source": "database",
+                    "ref": field,
+                    "type": "choice" if field.choices else field.get_internal_type(),
+                }
             col_data.update(options)
             parsed_columns.append(col_data)
         return parsed_columns
 
     def _parse(self):
-        self.parsed_columns = self.check_columns(self.columns, self.group_by, self.report_model)
+        self.parsed_columns = self.check_columns(
+            self.columns, self.group_by, self.report_model, self.container_class
+        )
         self._parsed_columns = list(self.parsed_columns)
         self._time_series_parsed_columns = self.get_time_series_parsed_columns()
         self._crosstab_parsed_columns = self.get_crosstab_parsed_columns()
 
     def get_database_columns(self):
-        return [col['name'] for col in self.parsed_columns if 'source' in col and col['source'] == 'database']
+        return [
+            col["name"]
+            for col in self.parsed_columns
+            if "source" in col and col["source"] == "database"
+        ]
 
     # def get_method_columns(self):
     #     return [col['name'] for col in self.parsed_columns if col['type'] == 'method']
 
     def get_list_display_columns(self):
         columns = self.parsed_columns
         if self.time_series_pattern:
             time_series_columns = self.get_time_series_parsed_columns()
             try:
-                index = self.columns.index('__time_series__')
+                index = self.columns.index("__time_series__")
                 columns[index:index] = time_series_columns
             except ValueError:
                 columns += time_series_columns
 
         if self.crosstab_model:
             crosstab_columns = self.get_crosstab_parsed_columns()
 
             try:
-                index = self.columns.index('__crosstab__')
+                index = self.columns.index("__crosstab__")
                 columns[index:index] = crosstab_columns
             except ValueError:
                 columns += crosstab_columns
 
         return columns
 
     def get_time_series_parsed_columns(self):
@@ -553,73 +712,85 @@
                 magic_field_class = None
 
                 if type(col) is str:
                     magic_field_class = field_registry.get_field_by_name(col)
                 elif issubclass(col, SlickReportField):
                     magic_field_class = col
 
-                _values.append({
-                    'name': magic_field_class.name + 'TS' + dt[1].strftime('%Y%m%d'),
-                    'original_name': magic_field_class.name,
-                    'verbose_name': self.get_time_series_field_verbose_name(magic_field_class, dt, index, series),
-                    'ref': magic_field_class,
-                    'start_date': dt[0],
-                    'end_date': dt[1],
-                    'source': 'magic_field' if magic_field_class else '',
-                    'is_summable': magic_field_class.is_summable,
-                })
+                _values.append(
+                    {
+                        "name": magic_field_class.name
+                        + "TS"
+                        + dt[1].strftime("%Y%m%d"),
+                        "original_name": magic_field_class.name,
+                        "verbose_name": self.get_time_series_field_verbose_name(
+                            magic_field_class, dt, index, series
+                        ),
+                        "ref": magic_field_class,
+                        "start_date": dt[0],
+                        "end_date": dt[1],
+                        "source": "magic_field" if magic_field_class else "",
+                        "is_summable": magic_field_class.is_summable,
+                    }
+                )
         return _values
 
-    def get_time_series_field_verbose_name(self, computation_class, date_period, index, series, pattern=None):
+    def get_time_series_field_verbose_name(
+        self, computation_class, date_period, index, series, pattern=None
+    ):
         """
         Sent the column data to construct a verbose name.
         Default implementation is delegated to the ReportField.get_time_series_field_verbose_name
         (which is  name + the end date %Y%m%d)
 
         :param computation_class: the computation field_name
         :param date_period: a tuple of (start_date, end_date)
         :return: a verbose string
         """
         pattern = pattern or self.time_series_pattern
-        return computation_class.get_time_series_field_verbose_name(date_period, index, series,
-                                                                    pattern)
+        return computation_class.get_time_series_field_verbose_name(
+            date_period, index, series, pattern
+        )
 
     def get_custom_time_series_dates(self):
         """
         Hook to get custom , maybe separated date periods
         :return: [ (date1,date2) , (date3,date4), .... ]
         """
         return self.time_series_custom_dates or []
 
     def _get_time_series_dates(self, series=None, start_date=None, end_date=None):
         from dateutil.relativedelta import relativedelta
+
         series = series or self.time_series_pattern
         start_date = start_date or self.start_date
         end_date = end_date or self.end_date
         _values = []
 
         if series:
-            if series == 'daily':
+            if series == "daily":
                 time_delta = datetime.timedelta(days=1)
-            elif series == 'weekly':
+            elif series == "weekly":
                 time_delta = relativedelta(weeks=1)
-            elif series == 'semimonthly':
+            elif series == "semimonthly":
                 time_delta = relativedelta(weeks=2)
-            elif series == 'monthly':
+            elif series == "monthly":
                 time_delta = relativedelta(months=1)
-            elif series == 'quarterly':
+            elif series == "quarterly":
                 time_delta = relativedelta(months=3)
-            elif series == 'semiannually':
+            elif series == "semiannually":
                 time_delta = relativedelta(months=6)
-            elif series == 'annually':
+            elif series == "annually":
                 time_delta = relativedelta(years=1)
-            elif series == 'custom':
+            elif series == "custom":
                 return self.get_custom_time_series_dates()
             else:
-                raise NotImplementedError(f'"{series}" is not implemented for time_series_pattern')
+                raise NotImplementedError(
+                    f'"{series}" is not implemented for time_series_pattern'
+                )
 
             done = False
 
             while not done:
                 to_date = start_date + time_delta
                 _values.append((start_date, to_date))
                 start_date = to_date
@@ -631,36 +802,40 @@
         """
         Return a list of the columns analyzed , with reference to computation field and everything
         :return:
         """
         report_columns = self.crosstab_columns or []
         ids = list(self.crosstab_ids)
         if self.crosstab_compute_reminder:
-            ids.append('----')
+            ids.append("----")
         output_cols = []
         ids_length = len(ids) - 1
         for counter, id in enumerate(ids):
             for col in report_columns:
                 magic_field_class = None
                 if type(col) is str:
                     magic_field_class = field_registry.get_field_by_name(col)
                 elif issubclass(col, SlickReportField):
                     magic_field_class = col
 
-                output_cols.append({
-                    'name': f'{magic_field_class.name}CT{id}',
-                    'original_name': magic_field_class.name,
-                    'verbose_name': self.get_crosstab_field_verbose_name(magic_field_class, self.crosstab_model, id),
-                    'ref': magic_field_class,
-                    'id': id,
-                    'model': self.crosstab_model,
-                    'is_reminder': counter == ids_length,
-                    'source': 'magic_field' if magic_field_class else '',
-                    'is_summable': magic_field_class.is_summable,
-                })
+                output_cols.append(
+                    {
+                        "name": f"{magic_field_class.name}CT{id}",
+                        "original_name": magic_field_class.name,
+                        "verbose_name": self.get_crosstab_field_verbose_name(
+                            magic_field_class, self.crosstab_model, id
+                        ),
+                        "ref": magic_field_class,
+                        "id": id,
+                        "model": self.crosstab_model,
+                        "is_reminder": counter == ids_length,
+                        "source": "magic_field" if magic_field_class else "",
+                        "is_summable": magic_field_class.is_summable,
+                    }
+                )
 
         return output_cols
 
     def get_crosstab_field_verbose_name(self, computation_class, model, id):
         """
         Hook to change the crosstab field verbose name, default it delegate this function to the ReportField
         :param computation_class: ReportField Class
@@ -668,67 +843,169 @@
         :param id: the current crosstab id
         :return: a verbose string
         """
         return computation_class.get_crosstab_field_verbose_name(model, id)
 
     def get_metadata(self):
         """
-                A hook to send data about the report for front end which can later be used in charting
-                :return:
-                """
+        A hook to send data about the report for front end which can later be used in charting
+        :return:
+        """
         time_series_columns = self.get_time_series_parsed_columns()
         crosstab_columns = self.get_crosstab_parsed_columns()
         metadata = {
-            'time_series_pattern': self.time_series_pattern,
-            'time_series_column_names': [x['name'] for x in time_series_columns],
-            'time_series_column_verbose_names': [x['verbose_name'] for x in time_series_columns],
-            'crosstab_model': self.crosstab_model or '',
-            'crosstab_column_names': [x['name'] for x in crosstab_columns],
-            'crosstab_column_verbose_names': [x['verbose_name'] for x in crosstab_columns],
+            "time_series_pattern": self.time_series_pattern,
+            "time_series_column_names": [x["name"] for x in time_series_columns],
+            "time_series_column_verbose_names": [
+                x["verbose_name"] for x in time_series_columns
+            ],
+            "crosstab_model": self.crosstab_model or "",
+            "crosstab_column_names": [x["name"] for x in crosstab_columns],
+            "crosstab_column_verbose_names": [
+                x["verbose_name"] for x in crosstab_columns
+            ],
         }
         return metadata
 
     def get_columns_data(self):
         """
         Hook to get the columns information to front end
         :param columns:
         :return:
         """
         columns = self.get_list_display_columns()
         data = []
 
         for col in columns:
-            data.append({
-                'name': col['name'],
-                'computation_field': col.get('original_name', ''),
-                'verbose_name': col['verbose_name'],
-                'visible': col.get('visible', True),
-                'type': col.get('type', 'text'),
-                'is_summable': col.get('is_summable', ''),
-            })
+            data.append(
+                {
+                    "name": col["name"],
+                    "computation_field": col.get("original_name", ""),
+                    "verbose_name": col["verbose_name"],
+                    "visible": col.get("visible", True),
+                    "type": col.get("type", "text"),
+                    "is_summable": col.get("is_summable", ""),
+                }
+            )
         return data
 
-    def get_full_response(self, data=None, report_slug=None, chart_settings=None, default_chart_title=None):
+    def get_full_response(
+        self, data=None, report_slug=None, chart_settings=None, default_chart_title=None
+    ):
         data = data or self.get_report_data()
         data = {
-            'report_slug': report_slug or self.__class__.__name__,
-            'data': data,
-            'columns': self.get_columns_data(),
-            'metadata': self.get_metadata(),
-            'chart_settings': self.get_chart_settings(chart_settings, default_chart_title=default_chart_title)
+            "report_slug": report_slug or self.__class__.__name__,
+            "data": data,
+            "columns": self.get_columns_data(),
+            "metadata": self.get_metadata(),
+            "chart_settings": self.get_chart_settings(
+                chart_settings, default_chart_title=default_chart_title
+            ),
         }
         return data
 
     def get_chart_settings(self, chart_settings=None, default_chart_title=None):
         """
         Ensure the sane settings are passed to the front end.
         """
         output = []
         chart_settings = chart_settings or []
-        report_title = default_chart_title or ''
-        for i, x in enumerate(chart_settings):
-            x['id'] = x.get('id', f"{x['type']}-{i}")
-            if not x.get('title', False):
-                x['title'] = report_title
-            x['engine_name'] = x.get('engine_name', SLICK_REPORTING_DEFAULT_CHARTS_ENGINE)
-            output.append(x)
+        report_title = default_chart_title or ""
+        for i, chart in enumerate(chart_settings):
+            if type(chart) is Chart:
+                chart = chart.to_dict()
+
+            chart["id"] = chart.get("id", f"{i}")
+            chart_type = chart.get("type", "line")
+            if (
+                chart_type == "column"
+                and SLICK_REPORTING_DEFAULT_CHARTS_ENGINE == "chartsjs"
+            ):
+                chart["type"] = "bar"
+
+            if not chart.get("title", False):
+                chart["title"] = report_title
+            chart["engine_name"] = chart.get(
+                "engine_name", SLICK_REPORTING_DEFAULT_CHARTS_ENGINE
+            )
+            output.append(chart)
         return output
+
+
+class ListViewReportGenerator(ReportGenerator):
+    def _apply_queryset_options(self, query, fields=None):
+        """
+        Apply the filters to the main queryset which will computed results be mapped to
+        :param query:
+        :param fields:
+        :return:
+        """
+        filters = {}
+        if self.date_field:
+            filters = {
+                f"{self.date_field}__gt": self.start_date,
+                f"{self.date_field}__lte": self.end_date,
+            }
+        filters.update(self.kwargs_filters)
+
+        if filters:
+            query = query.filter(**filters)
+        # if fields:
+        #     return query.values(*fields)
+        return query
+
+    def _get_record_data(self, obj, columns):
+        """
+        the function is run for every obj in the main_queryset
+        :param obj: current row
+        :param: columns： The columns we iterate on
+        :return: a dict object containing all needed data
+        """
+
+        data = {}
+        group_by_val = None
+        if self.group_by:
+            if self.group_by_field.related_model and "__" not in self.group_by:
+                primary_key_name = self.get_primary_key_name(
+                    self.group_by_field.related_model
+                )
+            else:
+                primary_key_name = self.group_by_field_attname
+
+            column_data = obj.get(primary_key_name, obj.get("id"))
+            group_by_val = str(column_data)
+
+        for window, window_cols in columns:
+            for col_data in window_cols:
+                name = col_data["name"]
+
+                if col_data.get("source", "") == "attribute_field":
+                    data[name] = col_data["ref"](self, obj, data)
+                    # changed line
+                elif col_data.get("source", "") == "container_class_attribute_field":
+                    data[name] = col_data["ref"](obj)
+
+                elif (
+                    col_data.get("source", "") == "magic_field" and self.group_by
+                ) or (self.time_series_pattern and not self.group_by):
+                    source = self._report_fields_dependencies[window].get(name, False)
+                    if source:
+                        computation_class = self.report_fields_classes[source]
+                        value = computation_class.get_dependency_value(
+                            group_by_val, col_data["ref"].name
+                        )
+                    else:
+                        try:
+                            computation_class = self.report_fields_classes[name]
+                        except KeyError:
+                            continue
+                        value = computation_class.resolve(group_by_val, data)
+                    if self.swap_sign:
+                        value = -value
+                    data[name] = value
+
+                else:
+                    if col_data.get("type", "") == "choice":
+                        data[name] = getattr(obj, f"get_{name}_display", "")()
+                    else:
+                        data[name] = getattr(obj, name, "")
+        return data
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/helpers.py` & `django-slick-reporting-0.7.0/slick_reporting/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,44 +7,48 @@
     """
     Returns the default django annotation
     @param calculation_field: the field to calculate ex 'value'
     @param calculation_method: the aggregation method ex: Sum
     @return: the annotation ex value__sum
     """
 
-    return '__'.join([calculation_field.lower(), calculation_method.name.lower()])
+    return "__".join([calculation_field.lower(), calculation_method.name.lower()])
 
 
 def get_foreign_keys(model):
     """
     Scans a model and return an Ordered Dictionary with the foreign keys found
     :param model: the model to scan
     :return: Ordered Dict
     """
     from django.db import models
+
     fields = model._meta.get_fields()
     fkeys = OrderedDict()
     for f in fields:
-        if f.is_relation and type(f) is not models.OneToOneRel \
-                and type(f) is not models.ManyToOneRel \
-                and type(f) is not models.ManyToManyRel \
-                and type(f) is not GenericForeignKey:
+        if (
+            f.is_relation
+            and type(f) is not models.OneToOneRel
+            and type(f) is not models.ManyToOneRel
+            and type(f) is not models.ManyToManyRel
+            and type(f) is not GenericForeignKey
+        ):
             fkeys[f.attname] = f
     return fkeys
 
 
 def get_field_from_query_text(path, model):
     """
     return the field of a query text
     `modelA__modelB__foo_field` would return foo_field on modelsB
     :param path:
     :param model:
     :return:
     """
-    relations = path.split('__')
+    relations = path.split("__")
     _rel = model
     field = None
     for i, m in enumerate(relations):
         field = _rel._meta.get_field(m)
         if i == len(relations) - 1:
             return field
         _rel = field.related_model
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/registry.py` & `django-slick-reporting-0.7.0/slick_reporting/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
         """
         Register a report_field into the registry,
         :param report_field:
         :param override: if True, a report_field will get replaced if found, else it would throw an AlreadyRegistered
         :return: report_field passed
         """
         if report_field.name in self._registry and not override:
-            raise AlreadyRegistered(f'The field name {report_field.name} is used before and `override` is False')
+            raise AlreadyRegistered(
+                f"The field name {report_field.name} is used before and `override` is False"
+            )
 
         self._registry[report_field.name] = report_field
         return report_field
 
     def unregister(self, report_field):
         """
         To unregister a Report Field
@@ -33,14 +35,15 @@
         del self._registry[name]
 
     def get_field_by_name(self, name):
         if name in self._registry:
             return self._registry[name]
         else:
             raise KeyError(
-                f'{name} is not found in the report field registry. Options are {",".join(self.get_all_report_fields_names())}')
+                f'{name} is not found in the report field registry. Options are {",".join(self.get_all_report_fields_names())}'
+            )
 
     def get_all_report_fields_names(self):
         return list(self._registry.keys())
 
 
 field_registry = ReportFieldRegistry()
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/static/slick_reporting/main.js` & `django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/main.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.6.8/slick_reporting/static/slick_reporting/ra.chartsjs.js` & `django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/ra.chartsjs.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,16 @@
 // title
 
 (function($) {
 
 
     var COLORS = ['#7cb5ec', '#f7a35c', '#90ee7e', '#7798BF', '#aaeeee', '#ff0066', '#eeaaee', '#55BF3B', '#DF5353', '#7798BF', '#aaeeee'];
 
+    let _chart_cache = {};
+
     function is_time_series(response, chartOptions) {
         if (chartOptions.time_series_support === false) return false;
         return response['metadata']['time_series_pattern'] !== ""
     }
 
     function getTimeSeriesColumnNames(response) {
         return response['metadata']['time_series_column_names'];
@@ -68,16 +70,14 @@
                 }],
             }
         }
         return chartObject
     }
 
 
-
-
     function extractDataFromResponse(response, chartOptions) {
         let dataFieldName = chartOptions['data_source'];
         let titleFieldName = chartOptions['title_source'];
         let isTimeSeries = is_time_series(response, chartOptions);
         let datasets = [];
         let legendResults = [];
         let datasetData = [];
@@ -154,30 +154,52 @@
     function getBackgroundColors(i) {
         if (typeof(i) !== 'undefined') {
             return COLORS[i]
         }
         return COLORS
     }
 
+    function displayChart(data, $elem, chart_id) {
+        chart_id = chart_id || $elem.attr('data-report-default-chart') || '';
+        // let chart = $elem;
+        // let chartObject = getObjFromArray(data.chart_settings, 'id', chart_id, true);
+        let cache_key = data.report_slug
+        try {
+            let existing_chart = _chart_cache[cache_key];
+            if (typeof(existing_chart) !== 'undefined') {
+                existing_chart.destroy();
+            }
+        } catch (e) {
+            console.error(e)
+        }
+
+        let chartObject = $.slick_reporting.chartsjs.createChartObject(data, chart_id);
+        // _chart_cache[cache_key] = chart.highcharts(chartObject);
+        var $chart = $elem.find('canvas');
+        _chart_cache[cache_key] = new Chart($chart, chartObject);
+
+    }
+
 
     if (typeof($.slick_reporting) === 'undefined') {
         $.slick_reporting = {}
     }
     $.slick_reporting.chartsjs = {
         createChartObject: createChartObject,
+        displayChart: displayChart,
         defaults: {
             // normalStackedTooltipFormatter: normalStackedTooltipFormatter,
             messages: {
                 noData: 'No Data to display ... :-/',
                 total: 'Total',
                 percent: 'Percent',
             },
             credits: {
-                text: 'RaSystems.io',
-                href: 'https://rasystems.io'
+                // text: 'RaSystems.io',
+                // href: 'https://rasystems.io'
             },
             notify_error: function() {},
             enable3d: false,
 
         }
     };
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/static/slick_reporting/ra.highchart.js` & `django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/ra.highchart.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -470,16 +470,16 @@
                 normalStackedTooltipFormatter: normalStackedTooltipFormatter,
                 messages: {
                     noData: 'No Data to display ... :-/',
                     total: 'Total',
                     percent: 'Percent',
                 },
                 credits: {
-                    text: 'RaSystems.io',
-                    href: 'https://rasystems.io'
+                    // text: 'RaSystems.io',
+                    // href: 'https://rasystems.io'
                 },
                 // notify_error: notify_error,
                 enable3d: false,
 
             }
         };
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/templates/slick_reporting/base.html` & `django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/base.html`

 * *Files 16% similar despite different names*

```diff
@@ -33,19 +33,22 @@
         crossorigin="anonymous"></script>
 
 {#Date picker #}
 <script type="text/javascript" src="https://cdn.jsdelivr.net/momentjs/latest/moment.min.js"></script>
 <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/daterangepicker/daterangepicker.min.js"></script>
 <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/daterangepicker/daterangepicker.css"/>
 
-<link href="https://cdn.jsdelivr.net/npm/select2@4.0.13/dist/css/select2.min.css" rel="stylesheet"/>
-<script src="https://cdn.jsdelivr.net/npm/select2@4.0.13/dist/js/select2.min.js"
-        integrity="sha384-JnbsSLBmv2/R0fUmF2XYIcAEMPHEAO51Gitn9IjL4l89uFTIgtLF1+jqIqqd9FSk"
-        crossorigin="anonymous"></script>
+{#select2#}
+
+
+
+
+{# datatable #}
+<script type="text/javascript" src="https://cdn.datatables.net/v/bs4/dt-1.10.20/datatables.min.js"></script>
+    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/v/bs4/dt-1.10.20/datatables.min.css"/>
+
+
 
-<script>$(document).ready(function () {
-    $('select').select2();
-})</script>
-{% block js_script %}
+{% block extrajs %}
 {% endblock %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -2,9 +2,10 @@
 
 
 
 
 {% block content %} {% endblock %}
  {#Date picker #}
 
+ {#select2#} {# datatable #}
 
- {% block js_script %} {% endblock %}
+ {% block extrajs %} {% endblock %}
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/templates/slick_reporting/simple_report.html` & `django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/simple_report.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,95 @@
 {% extends 'slick_reporting/base.html' %}
 {% load crispy_forms_tags i18n slick_reporting_tags static %}
 
 
 {% block content %}
 
-{% if form %}
-    <h4>Filters</h4>
-    <form>
-        {% crispy form form.get_crispy_helper %}
-        <input type="submit" value="Filter" class="btn btn-primary btn-lg btn-block refreshReport">
-    </form>
-{% endif %}
-    <h4 class="py-5">Results</h4>
-    <div class="card" id="{{ report_data.report_slug }}">
-        <div class="card-body">
-            <div class="chartContainer screenOnly">
-                <div class="controls text-center">
-                    <ul class="nav-charts list-inline">
-
-                        {% for chart in report_data.chart_settings %}
-                            <li class="list-inline-item">
-                                <a href="#" data-chart-id="{{ chart.id }}" data-charts-engine="{{ chart.engine_name }}">
-                                    {% if chart.type == 'pie' %}
-                                        <i class="fa fa-pie-chart"></i>
-                                    {% elif chart.type == 'line' %}
-                                        <i class="fa fa-line-chart"></i>
-                                    {% else %}
-                                        <i class="fa fa-bar-chart"></i>
-                                    {% endif %} {{ chart.title }}
-                                </a></li>
-                        {% endfor %}
-                    </ul>
-                </div>
-                <div class="reportChart screenOnly" dir="ltr"></div>
-                {% if report_data.chart_settings %}
-                    {#                    #}
-                    {% if report_data.charts_engine == 'chartsjs' %}
-                        <canvas width="400" height="100"></canvas>
-                    {% elif report_data.charts_engine == 'highcharts' %}
-                        {#                        <div id="highchartContainer" style="width:100%; height:400px;"></div>#}
-                    {% endif %}
+    <div class="col-12">
+        {% if form %}
 
+            <h4>Filters</h4>
+            <form id="reportForm">
+                {% crispy form crispy_helper %}
+                <input type="submit" value="Filter" class="btn btn-primary btn-lg btn-block refreshReport">
+                <input type="button" value="Export Csv" class="btn btn-secondary btn-lg btn-block exportCsvBtn">
+            </form>
+        {% endif %}
+        <h4 class="py-5">Results</h4>
+        <div class="card" id="{{ report_data.report_slug }}">
+            <div class="card-body">
+                <div class="chartContainer screenOnly">
+                    <div class="controls text-center">
+                        <ul class="nav-charts list-inline">
+
+                            {% for chart in report_data.chart_settings %}
+                                <li class="list-inline-item">
+                                    <a href="#" data-chart-id="{{ chart.id }}"
+                                       data-charts-engine="{{ chart.engine_name }}">
+                                        {% if chart.type == 'pie' %}
+                                            <i class="fa fa-pie-chart"></i>
+                                        {% elif chart.type == 'line' %}
+                                            <i class="fa fa-line-chart"></i>
+                                        {% else %}
+                                            <i class="fa fa-bar-chart"></i>
+                                        {% endif %} {{ chart.title }}
+                                    </a></li>
+                            {% endfor %}
+                        </ul>
+                    </div>
+                    <div class="reportChart screenOnly" dir="ltr"></div>
+                    {% if report_data.chart_settings %}
+                        {#                    #}
+                        {% if report_data.charts_engine == 'chartsjs' %}
+                            <canvas width="400" height="100"></canvas>
+                        {% elif report_data.charts_engine == 'highcharts' %}
+                            {#                        <div id="highchartContainer" style="width:100%; height:400px;"></div>#}
+                        {% endif %}
 
-                {% endif %}
-            </div>
-            <div class="report-table">
-                {% include 'slick_reporting/table.html' with table=report_data %}
+
+                    {% endif %}
+                </div>
+                <div class="report-table">
+                    {% include 'slick_reporting/table.html' with table=report_data %}
+                </div>
             </div>
         </div>
-    </div>
 
+    </div>
 
 {% endblock %}
-{% block js_script %}
+{% block extrajs %}
+    {{ block.super }}
     <script src="{% static 'slick_reporting/main.js' %}"></script>
     <script src="{% static 'slick_reporting/ra.chartsjs.js' %}"></script>
     <script src="{% static 'slick_reporting/ra.highchart.js' %}"></script>
 
+    <link href="https://cdn.jsdelivr.net/npm/select2@4.0.13/dist/css/select2.min.css" rel="stylesheet"/>
+<script src="https://cdn.jsdelivr.net/npm/select2@4.0.13/dist/js/select2.min.js"
+        integrity="sha384-JnbsSLBmv2/R0fUmF2XYIcAEMPHEAO51Gitn9IjL4l89uFTIgtLF1+jqIqqd9FSk"
+        crossorigin="anonymous"></script>
+
 
     <script>
         $(document).ready(function () {
+
+
+            $('select').select2();
+
             let data = {{ report_data|jsonify }};
 
             let chartContainer = $('.reportChart')
 
+            $('.exportCsvBtn').on('click', function (e) {
+                e.preventDefault()
+                let form = $('#reportForm');
+                window.location = '?' + form.serialize() + '&_export=csv'
+            });
+
+
             function setDatePicker() {
                 function setDatePickerObj() {
                     var range_start = new Date();
                     var range_end = new Date();
                     let container = $(document);
                     let $startDate = container.find('input[name=start_date]');
                     let $endDate = container.find('input[name=end_date]');
```

### Comparing `django-slick-reporting-0.6.8/slick_reporting/templatetags/slick_reporting_tags.py` & `django-slick-reporting-0.7.0/slick_reporting/templatetags/slick_reporting_tags.py`

 * *Files identical despite different names*

