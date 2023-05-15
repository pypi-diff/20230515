# Comparing `tmp/django-atris-2.0.0.tar.gz` & `tmp/django-atris-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/radu.dan/django-atris/dist/tmp65wtp8ol/django-atris-2.0.0.tar", last modified: Wed Jul 13 10:05:06 2022, max compression
+gzip compressed data, was "django-atris-2.0.1.tar", last modified: Mon May 15 07:40:00 2023, max compression
```

## Comparing `django-atris-2.0.0.tar` & `django-atris-2.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 radu.dan (41593402) 1138207179        0 2022-07-13 10:05:06.000000 django-atris-2.0.0/
--rw-r--r--   0 radu.dan (41593402) 1138207179      301 2022-07-13 10:05:06.000000 django-atris-2.0.0/PKG-INFO
--rw-r--r--   0 radu.dan (41593402) 1138207179      192 2022-07-13 09:12:41.000000 django-atris-2.0.0/pyproject.toml
--rw-r--r--   0 radu.dan (41593402) 1138207179       36 2022-07-13 09:12:41.000000 django-atris-2.0.0/MANIFEST.in
--rw-r--r--   0 radu.dan (41593402) 1138207179      729 2022-07-13 09:12:41.000000 django-atris-2.0.0/setup.py
--rw-r--r--   0 radu.dan (41593402) 1138207179       38 2022-07-13 10:05:06.000000 django-atris-2.0.0/setup.cfg
--rw-r--r--   0 radu.dan (41593402) 1138207179    10060 2022-07-13 09:12:41.000000 django-atris-2.0.0/README.rst
-drwxr-xr-x   0 radu.dan (41593402) 1138207179        0 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/
-drwxr-xr-x   0 radu.dan (41593402) 1138207179        0 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/django_atris.egg-info/
--rw-r--r--   0 radu.dan (41593402) 1138207179      301 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/django_atris.egg-info/PKG-INFO
--rw-r--r--   0 radu.dan (41593402) 1138207179        1 2022-07-13 09:43:42.000000 django-atris-2.0.0/src/django_atris.egg-info/not-zip-safe
--rw-r--r--   0 radu.dan (41593402) 1138207179     1348 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/django_atris.egg-info/SOURCES.txt
--rw-r--r--   0 radu.dan (41593402) 1138207179       21 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/django_atris.egg-info/requires.txt
--rw-r--r--   0 radu.dan (41593402) 1138207179        6 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/django_atris.egg-info/top_level.txt
--rw-r--r--   0 radu.dan (41593402) 1138207179        1 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/django_atris.egg-info/dependency_links.txt
-drwxr-xr-x   0 radu.dan (41593402) 1138207179        0 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/atris/
-drwxr-xr-x   0 radu.dan (41593402) 1138207179        0 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/atris/migrations/
--rw-r--r--   0 radu.dan (41593402) 1138207179      639 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0008_object_id_text.py
--rw-r--r--   0 radu.dan (41593402) 1138207179        0 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/__init__.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      627 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0003_added_indexes.py
--rw-r--r--   0 radu.dan (41593402) 1138207179     1099 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0006_auto_20160622_0720.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      949 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0007_related_field_history.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      530 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0002_historicalrecord_history_diff.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      916 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0009_auto_20190906_0509.py
--rw-r--r--   0 radu.dan (41593402) 1138207179     1469 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0001_initial.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      749 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0005_auto_20160411_0250.py
--rw-r--r--   0 radu.dan (41593402) 1138207179     1685 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/migrations/0004_archivedhistoricalrecord.py
-drwxr-xr-x   0 radu.dan (41593402) 1138207179        0 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/atris/management/
--rw-r--r--   0 radu.dan (41593402) 1138207179        0 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/management/__init__.py
-drwxr-xr-x   0 radu.dan (41593402) 1138207179        0 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/atris/management/commands/
--rw-r--r--   0 radu.dan (41593402) 1138207179        0 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/management/commands/__init__.py
--rw-r--r--   0 radu.dan (41593402) 1138207179     2917 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/management/commands/archive_old_historical_records.py
--rw-r--r--   0 radu.dan (41593402) 1138207179     1954 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/management/commands/delete_old_historical_records.py
--rw-r--r--   0 radu.dan (41593402) 1138207179     4747 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/management/commands/populate_initial_history.py
--rw-r--r--   0 radu.dan (41593402) 1138207179       46 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/__init__.py
-drwxr-xr-x   0 radu.dan (41593402) 1138207179        0 2022-07-13 10:05:06.000000 django-atris-2.0.0/src/atris/models/
--rw-r--r--   0 radu.dan (41593402) 1138207179     8612 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/models/abstract_historical_record.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      521 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/models/historical_record.py
--rw-r--r--   0 radu.dan (41593402) 1138207179    24044 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/models/history_logging.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      130 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/models/__init__.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      125 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/models/archived_historical_record.py
--rw-r--r--   0 radu.dan (41593402) 1138207179       47 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/models/exceptions.py
--rw-r--r--   0 radu.dan (41593402) 1138207179     5049 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/models/helpers.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      690 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/apps.py
--rw-r--r--   0 radu.dan (41593402) 1138207179     6338 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/admin.py
--rw-r--r--   0 radu.dan (41593402) 1138207179      233 2022-07-13 09:12:41.000000 django-atris-2.0.0/src/atris/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:40:00.477665 django-atris-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 07:39:44.000000 django-atris-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 07:39:44.000000 django-atris-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-05-15 07:40:00.477665 django-atris-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-05-15 07:39:44.000000 django-atris-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 07:39:44.000000 django-atris-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:40:00.477665 django-atris-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:40:00.469665 django-atris-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:40:00.473665 django-atris-2.0.1/src/atris/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:40:00.473665 django-atris-2.0.1/src/atris/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:40:00.473665 django-atris-2.0.1/src/atris/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/management/commands/archive_old_historical_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/management/commands/delete_old_historical_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/management/commands/populate_initial_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:40:00.473665 django-atris-2.0.1/src/atris/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0002_historicalrecord_history_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0003_added_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0004_archivedhistoricalrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0005_auto_20160411_0250.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0006_auto_20160622_0720.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0007_related_field_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0008_object_id_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/0009_auto_20190906_0509.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:40:00.477665 django-atris-2.0.1/src/atris/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/models/abstract_historical_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/models/archived_historical_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/models/historical_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-05-15 07:39:44.000000 django-atris-2.0.1/src/atris/models/history_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:40:00.477665 django-atris-2.0.1/src/django_atris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-05-15 07:40:00.000000 django-atris-2.0.1/src/django_atris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 07:40:00.000000 django-atris-2.0.1/src/django_atris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:40:00.000000 django-atris-2.0.1/src/django_atris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:40:00.000000 django-atris-2.0.1/src/django_atris.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 07:40:00.000000 django-atris-2.0.1/src/django_atris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 07:40:00.000000 django-atris-2.0.1/src/django_atris.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-atris-2.0.0/README.rst` & `django-atris-2.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 
 This app requires:
 
 - Django >= 1.10:
     - for Django < 1.9      please use django-atris < 1.0.0
     - for Django < 1.10     please use django-atris < 1.2.0
     - for Django > 2.0.0    please use django-atris > 1.2.1
+    - for Django > 3.2      please use django-atris = 2.0.1
 - Postgresql
 - Python:
     - for django-atris < 2.0.0  please use Python >= 2.7 or Python >= 3.4 (after Django 2)
     - for django-atris >= 2.0.0 please use Python >= 3.6
+    - for django-atris >= 2.0.1 please use Python >= 3.7
 
 Integration guide
 -----------------
 
 In order to use the app you must do the following:
 
 * Add 'atris' to INSTALLED_APPS in settings
@@ -221,8 +223,12 @@
 
 1.3.4:
     * Add support for Django 2.2
 
 2.0.0:
     * Dropped support for Django < 2.2 and Python < 3.6
     * Fixed history generation issue after saving an instance for the first time after a new field was added to the model
-        - This issue was causing historical records to be generated when saving (without any changes) existing instances of tracked models
+        - This issue was causing historical records to be generated when saving (without any changes) existing instances of tracked models
+
+2.0.1:
+    * Dropped support for Python <= 3.6
+    * Move away from setup.py to pyproject.toml
```

### Comparing `django-atris-2.0.0/src/django_atris.egg-info/SOURCES.txt` & `django-atris-2.0.1/src/django_atris.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.py
 src/atris/__init__.py
 src/atris/admin.py
 src/atris/apps.py
 src/atris/middleware.py
 src/atris/management/__init__.py
 src/atris/management/commands/__init__.py
 src/atris/management/commands/archive_old_historical_records.py
```

### Comparing `django-atris-2.0.0/src/atris/migrations/0008_object_id_text.py` & `django-atris-2.0.1/src/atris/migrations/0008_object_id_text.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/migrations/0003_added_indexes.py` & `django-atris-2.0.1/src/atris/migrations/0003_added_indexes.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/migrations/0006_auto_20160622_0720.py` & `django-atris-2.0.1/src/atris/migrations/0006_auto_20160622_0720.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/migrations/0007_related_field_history.py` & `django-atris-2.0.1/src/atris/migrations/0007_related_field_history.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/migrations/0002_historicalrecord_history_diff.py` & `django-atris-2.0.1/src/atris/migrations/0002_historicalrecord_history_diff.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/migrations/0009_auto_20190906_0509.py` & `django-atris-2.0.1/src/atris/migrations/0009_auto_20190906_0509.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/migrations/0001_initial.py` & `django-atris-2.0.1/src/atris/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/migrations/0005_auto_20160411_0250.py` & `django-atris-2.0.1/src/atris/migrations/0005_auto_20160411_0250.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/migrations/0004_archivedhistoricalrecord.py` & `django-atris-2.0.1/src/atris/migrations/0004_archivedhistoricalrecord.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/management/commands/archive_old_historical_records.py` & `django-atris-2.0.1/src/atris/management/commands/archive_old_historical_records.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,40 +26,40 @@
 
     def add_arguments(self, parser):
         parser.add_argument(
             "--days",
             dest="days",
             type=int,
             default=None,
-            help="Any historical record older than the number of days "
-            "specified gets archived.",
+            help=(
+                "Any historical record older than "
+                "the number of days specified gets archived."
+            ),
         )
         parser.add_argument(
             "--weeks",
             dest="weeks",
             type=int,
             default=None,
-            help="Any historical record older than the number of "
-            "months specified gets archived.",
+            help=(
+                "Any historical record older than "
+                "the number of months specified gets archived."
+            ),
         )
 
     def handle(self, *args, **options):
         days = options.get("days")
         weeks = options.get("weeks")
         if not (days or weeks):
-            self.stderr.write(
-                "{msg}\n".format(
-                    msg=self.PARAM_ERROR,
-                ),
-            )
+            self.stderr.write(f"{self.PARAM_ERROR}\n")
             return
         old_history_entries = HistoricalRecord.objects.older_than(days, weeks)
         handled_entries_nr = old_history_entries.count()
         self.migrate_data(days, weeks)
-        self.stdout.write("{} archived.\n".format(handled_entries_nr))
+        self.stdout.write(f"{handled_entries_nr} archived.\n")
 
     @transaction.atomic
     def migrate_data(self, days=None, weeks=None):
         if days and weeks:
             logger.info(
                 "Both days and weeks parameters were supplied for migrating"
                 "history records! The weeks parameter will be used as the"
```

### Comparing `django-atris-2.0.0/src/atris/management/commands/delete_old_historical_records.py` & `django-atris-2.0.1/src/atris/management/commands/delete_old_historical_records.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,47 +19,47 @@
 
     def add_arguments(self, parser):
         parser.add_argument(
             "--days",
             dest="days",
             type=int,
             default=None,
-            help="Any historical record older than the number of days "
-            "specified gets deleted.",
+            help=(
+                "Any historical record older than "
+                "the number of days specified gets deleted."
+            ),
         )
         parser.add_argument(
             "--weeks",
             dest="weeks",
             type=int,
             default=None,
-            help="Any historical record older than the number of months "
-            "specified gets deleted.",
+            help=(
+                "Any historical record older than "
+                "the number of months specified gets deleted."
+            ),
         )
         parser.add_argument(
             "--from-archive",
             dest="from_archive",
             default=False,
             action="store_true",
-            help='Delete occurs on the "archived historical records" table '
-            'instead of the default "historical records" table.',
+            help=(
+                'Delete occurs on the "archived historical records" table '
+                'instead of the default "historical records" table.'
+            ),
         )
 
     def handle(self, *args, **options):
         days = options.get("days")
         weeks = options.get("weeks")
         if not (days or weeks):
-            self.stderr.write(
-                "{msg}\n".format(
-                    msg=self.PARAM_ERROR,
-                ),
-            )
+            self.stderr.write(f"{self.PARAM_ERROR}\n")
             return
 
         model = (
             ArchivedHistoricalRecord
             if options.get("from_archive")
             else HistoricalRecord
         )
         deleted_entries = model.objects.older_than(days, weeks).delete()
-        self.stdout.write(
-            "{} {} deleted.\n".format(deleted_entries[0], model.__name__)
-        )
+        self.stdout.write(f"{deleted_entries[0]} {model.__name__} deleted.\n")
```

### Comparing `django-atris-2.0.0/src/atris/management/commands/populate_initial_history.py` & `django-atris-2.0.1/src/atris/management/commands/populate_initial_history.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,37 +19,36 @@
 
     def add_arguments(self, parser):
         parser.add_argument(
             "--select-batch-size",
             dest="select_batch_size",
             type=int,
             default=self.SELECT_BATCH_SIZE,
-            help="The number of target objects that will be retrieved from "
-            "the DB at one time.",
+            help=(
+                "The number of target objects that "
+                "will be retrieved from the DB at one time."
+            ),
         )
         parser.add_argument(
             "--create-batch-size",
             dest="create_batch_size",
             type=int,
             default=self.CREATE_BATCH_SIZE,
-            help="The number of history objects that will be created "
-            "in one batch. Should be at most SELECT_BATCH_SIZE.",
+            help=(
+                "The number of history objects that will be created "
+                "in one batch. Should be at most SELECT_BATCH_SIZE."
+            ),
         )
 
     def handle(self, *args, **options):
         for model, model_specific_info in registered_models.items():
             if HistoricalRecord.objects.by_model(model).exists():
-                self.stderr.write(
-                    "{msg} {model}\n".format(
-                        msg=self.EXISTING_HISTORY_FOUND,
-                        model=model,
-                    ),
-                )
+                self.stderr.write(f"{self.EXISTING_HISTORY_FOUND} {model}\n")
                 continue
-            self.stdout.write("Initializing history for {}\n".format(model))
+            self.stdout.write(f"Initializing history for {model}\n")
             additional_data_param_name = model_specific_info[
                 "additional_data_param_name"
             ]
             additional_data_field = getattr(
                 model,
                 additional_data_param_name,
                 {},
@@ -67,19 +66,19 @@
                 self.stdout,
             )
             try:
                 with atomic():
                     create_history_for_model()
             except DatabaseError as e:
                 self.stderr.write(
-                    "Error creating history for {}: {}".format(model, e),
+                    f"Error creating history for {model}: {e}",
                 )
 
 
-class ModelHistoryCreator(object):
+class ModelHistoryCreator:
     def __init__(
         self,
         model,
         additional_data_field,
         excluded_fields,
         select_batch_size,
         create_batch_size,
@@ -121,16 +120,15 @@
             historical_instances,
             batch_size=self.create_batch_size,
         )
 
     def create_history_for_object(self, obj):
         data = get_instance_field_data(obj)
         additional_data = {
-            key: str(value)
-            for key, value in self.additional_data_field.items()
+            key: str(value) for key, value in self.additional_data_field.items()
         }
         historical_record = HistoricalRecord(
             history_user=None,
             history_type=HistoricalRecord.CREATE,
             content_object=obj,
             data=data,
             additional_data=additional_data,
```

### Comparing `django-atris-2.0.0/src/atris/models/abstract_historical_record.py` & `django-atris-2.0.1/src/atris/models/abstract_historical_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         """
         Generates a string which describes the changes that occurred between
         this historical record instance (self) and its previous version.
 
         :return: Said string.
         :rtype String
         """
-        diff_string = "{}d ".format(self.get_history_type_display())
+        diff_string = f"{self.get_history_type_display()}d "
         if self.history_type == self.UPDATE:
             if not self.history_diff:
                 if not self.previous_version:
                     diff_string = "No prior information available."
                 else:
                     diff_string += "with no change"
             else:
```

### Comparing `django-atris-2.0.0/src/atris/models/historical_record.py` & `django-atris-2.0.1/src/atris/models/historical_record.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/models/history_logging.py` & `django-atris-2.0.1/src/atris/models/history_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,27 +23,27 @@
     Useful when a change on an untracked object does not generate history on a
     related tracked object or when using bulk_create, which does not trigger
     the pre/post_save signals by default.
     """
     obj._meta.history_logging.post_save(obj, created=created)
 
 
-class HistoryManager(object):
+class HistoryManager:
     def __get__(self, instance, model):
         if instance and model:
             return HistoricalRecord.objects.by_model_and_model_id(
                 model,
                 instance.pk,
             )
         if model:
             return HistoricalRecord.objects.by_model(model)
 
 
 # noinspection PyProtectedMember,PyAttributeOutsideInit
-class HistoryLogging(object):
+class HistoryLogging:
 
     thread = threading.local()
     _cleared_related_objects = dict()
 
     def __init__(
         self,
         additional_data_param_name="",
@@ -100,17 +100,15 @@
             )
             logger.debug(
                 "Set class attribute {}.{}".format(
                     class_name,
                     self.class_additional_data_name,
                 ),
             )
-            default_data_param_name = (
-                "default_" + self.additional_data_param_name
-            )
+            default_data_param_name = "default_" + self.additional_data_param_name
             setattr(
                 cls,
                 default_data_param_name,
                 self.default_additional_data_property_maker(),
             )
             logger.debug(
                 "Set property {}.{}".format(
@@ -220,18 +218,15 @@
                 field_name = find_m2m_field_name_by_model(
                     instance._meta,
                     model,
                     reverse,
                 )
                 related_objects = getattr(instance, field_name).all()
                 self._cleared_related_objects[instance] = list(related_objects)
-            elif (
-                action == "post_clear"
-                and instance in self._cleared_related_objects
-            ):
+            elif action == "post_clear" and instance in self._cleared_related_objects:
                 related_objects = self._cleared_related_objects.pop(instance)
                 for related_object in related_objects:
                     self._create_historical_record(
                         related_object,
                         HistoricalRecord.UPDATE,
                         False,
                     )
@@ -301,15 +296,15 @@
         fields = in_model_meta.many_to_many
     for field in fields:
         target_models = [for_model] + [p for p in for_model._meta.parents]
         if field.many_to_many and field.related_model in target_models:
             return field.name
 
 
-class M2MThroughClassesGatherer(object):
+class M2MThroughClassesGatherer:
     def __init__(self, cls):
         self.cls = cls
 
     def __call__(self):
         m2m_related_throughs = [
             self.get_through_class(ro.through)
             for ro in self.cls._meta.related_objects
@@ -339,15 +334,15 @@
         return modules[module_path]
 
 
 def is_str(obj):
     return isinstance(obj, str)
 
 
-class HistoricalRecordGenerator(object):
+class HistoricalRecordGenerator:
     def __init__(
         self,
         instance,
         history_type,
         user_id,
         user_name,
         ignored_users=None,
@@ -409,17 +404,15 @@
                 self.previous_data,
             )
             generate_for_interested_objects()
 
     def should_skip_history_for_user(self):
         ids_to_skip = self.ignored_users.get("user_ids", [])
         user_names_to_skip = self.ignored_users.get("user_names", [])
-        return (
-            self.user_name in user_names_to_skip or self.user_id in ids_to_skip
-        )
+        return self.user_name in user_names_to_skip or self.user_id in ids_to_skip
 
     def get_differing_fields(self, data):
         if self.history_type == HistoricalRecord.UPDATE:
             diff_fields = get_diff_fields(
                 self.instance,
                 data,
                 self.previous_data,
@@ -428,15 +421,15 @@
             should_generate_history = diff_fields is None or diff_fields
         else:
             diff_fields = list()
             should_generate_history = True
         return diff_fields, should_generate_history
 
 
-class RelatedFieldHistoryGenerator(object):
+class RelatedFieldHistoryGenerator:
     def __init__(self, instance, instance_history, previous_data):
         self.instance = instance
         self.instance_history = instance_history
         self.history_logging = self.instance._meta.history_logging
         self.previous_data = previous_data
 
     def __call__(self):
@@ -480,33 +473,30 @@
                 # prevent infinite generation of history among related fields.
                 propagate_to_related_fields=False,
                 extra_info=self.instance_history.additional_data,
             )
             generate_history()
 
 
-class InterestedObjectHistoryGenerator(object):
-    def __init__(
-        self, instance, instance_history, interested_fields, previous_data
-    ):
+class InterestedObjectHistoryGenerator:
+    def __init__(self, instance, instance_history, interested_fields, previous_data):
         self.instance = instance
         self.instance_history = instance_history
         self.interested_fields = interested_fields
         self.previous_data = previous_data
 
     def __call__(self):
         # Make sure the value changed check is made against
         # an empty list in case history_diff is None
         fields_to_check = self.instance_history.history_diff or []
 
         for field_name in self.interested_fields:
             field_value_changed = (
                 field_name in fields_to_check
-                or self.instance_history.history_type
-                == HistoricalRecord.DELETE
+                or self.instance_history.history_type == HistoricalRecord.DELETE
             )
             get_related_objects = HistoryEnabledRelatedObjectsCollector(
                 self.instance,
                 field_name,
                 self.previous_data if field_value_changed else None,
             )
             interested_objects = get_related_objects()
@@ -524,23 +514,17 @@
     def generate_history_for_interested_object(
         self, interested_object, status, field_changed
     ):
         additional_data = get_additional_data(interested_object)
         additional_data.update(self.instance_history.additional_data)
         instance_class_name = self.instance.__class__.__name__
         instance_name = instance_class_name.lower()
-        if (
-            field_changed
-            and status is HistoryEnabledRelatedObjectsCollector.ADDED
-        ):
+        if field_changed and status is HistoryEnabledRelatedObjectsCollector.ADDED:
             action = "Added"
-        elif (
-            field_changed
-            and status is HistoryEnabledRelatedObjectsCollector.REMOVED
-        ):
+        elif field_changed and status is HistoryEnabledRelatedObjectsCollector.REMOVED:
             action = "Removed"
         else:
             action = self.instance_history.get_history_type_display() + "d"
         additional_data[instance_name] = "{action} {object_type}".format(
             action=action, object_type=instance_class_name
         )
         HistoricalRecord.objects.create(
@@ -551,15 +535,15 @@
             data=get_instance_field_data(interested_object),
             history_diff=[instance_name],
             additional_data=additional_data,
             related_field_history=self.instance_history,
         )
 
 
-class HistoryEnabledRelatedObjectsCollector(object):
+class HistoryEnabledRelatedObjectsCollector:
 
     ADDED = True
     REMOVED = False
     UNMODIFIED = None
 
     def __init__(self, instance, field_name, previous_data=None):
         self.instance = instance
@@ -598,17 +582,15 @@
             related_objects = [referenced_object] if referenced_object else []
         elif self.field.one_to_many or self.field.many_to_many:
             # The attribute is a RelatedManager instance.
             related_objects = list(referenced_object.all())
         else:
             raise TypeError(
                 "Field {} did not match any known related field types. Known "
-                "types: 1-to-1, 1-to-many, many-to-1, many-to-many.".format(
-                    self.field
-                )
+                "types: 1-to-1, 1-to-many, many-to-1, many-to-many.".format(self.field)
             )
         return related_objects
 
     def get_previous_objects(self):
         previous_pks = self.get_previous_object_pks()
         if self.field.related_model:
             model_class = self.field.related_model
```

### Comparing `django-atris-2.0.0/src/atris/models/helpers.py` & `django-atris-2.0.1/src/atris/models/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import json
 import re
 
 from typing import Dict, List, Optional, Type, Union
 
-from django.contrib.contenttypes.fields import GenericForeignKey
+from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import router
 from django.db.models import Model
 
 
 def get_diff_fields(
     model: Union[Model, Type[Model]],
@@ -49,14 +49,18 @@
                 diff_fields.append(model_field.name)
     return diff_fields
 
 
 def get_default_value(field):
     try:
         default_value = field.get_default()
+        # this is an ugly fix needed for django 3.2 compatibility - I don't like it
+        # either but have no better solution
+        if isinstance(field, GenericRelation) and default_value is None:
+            return ''
         return str(default_value) if default_value is not None else None
     except AttributeError as e:
         error_message = str(e)
         if "ManyTo" in error_message:
             # ManyToManyRel or ManyToOneRel
             return ""
         return None
@@ -131,15 +135,15 @@
         attname = field.fk_field
     elif hasattr(field, "get_accessor_name"):  # many-to-* relation field
         attname = field.get_accessor_name()
     elif hasattr(field, accessor_for_simple_fields):
         # regular field or foreign key
         attname = getattr(field, accessor_for_simple_fields)
     else:
-        raise TypeError("Can't determine accessor for field {}".format(field))
+        raise TypeError(f"Can't determine accessor for field {field}")
     return attname
 
 
 def from_writable_db(manager):
     """
     When using a DB router in which the reads are done through a different
     connection than the writes, the data may differ, resulting in incorrect
```

### Comparing `django-atris-2.0.0/src/atris/apps.py` & `django-atris-2.0.1/src/atris/apps.py`

 * *Files identical despite different names*

### Comparing `django-atris-2.0.0/src/atris/admin.py` & `django-atris-2.0.1/src/atris/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from django.contrib import admin
 from django.contrib.contenttypes.models import ContentType
 from django.db import connections, models
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
-from atris.models import (
-    ArchivedHistoricalRecord,
-    HistoricalRecord,
-    history_logging,
-)
+from atris.models import ArchivedHistoricalRecord, HistoricalRecord, history_logging
 
 
 class ContentTypeListFilter(admin.SimpleListFilter):
     # Human-readable title which will be displayed in the
     # right admin sidebar just above the filter options.
     title = _("Content type")
 
@@ -61,17 +57,15 @@
                 and query.low_mark == 0
                 and not query.select
                 and not query.group_by
                 and not query.having
                 and not query.distinct
             )
             if no_filtration_used:
-                parts = [
-                    p.strip('"') for p in self.model._meta.db_table.split(".")
-                ]
+                parts = [p.strip('"') for p in self.model._meta.db_table.split(".")]
                 if 1 <= len(parts) <= 2:
                     cursor = connections[self.db].cursor()
                     if len(parts) == 1:
                         cursor.execute(
                             "SELECT reltuples::bigint "
                             "FROM pg_class "
                             "WHERE relname = %s",
@@ -119,15 +113,15 @@
 
     show_full_result_count = False
 
     def get_queryset(self, request):
         # Capturing the request object in order to build the absolute URI in
         # `related_field_history_admin`
         self._request = request
-        qs = super(GenericHistoryAdmin, self).get_queryset(request)
+        qs = super().get_queryset(request)
         return qs
 
     def history_snapshot(self, obj):
         return self._dict_to_table(obj.data)
 
     def more_info(self, obj):
         return self._dict_to_table(obj.additional_data)
```

