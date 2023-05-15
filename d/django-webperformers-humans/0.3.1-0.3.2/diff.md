# Comparing `tmp/django-webperformers-humans-0.3.1.tar.gz` & `tmp/django-webperformers-humans-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webperformers-humans-0.3.1.tar", last modified: Sat May  6 12:18:54 2023, max compression
+gzip compressed data, was "django-webperformers-humans-0.3.2.tar", last modified: Mon May 15 07:37:15 2023, max compression
```

## Comparing `django-webperformers-humans-0.3.1.tar` & `django-webperformers-humans-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/
--rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-05 09:44:22.000000 django-webperformers-humans-0.3.1/LICENSE
--rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 11:52:59.000000 django-webperformers-humans-0.3.1/MANIFEST.in
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2201 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1136 2023-05-06 12:05:42.000000 django-webperformers-humans-0.3.1/README.rst
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2201 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)      949 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/SOURCES.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/dependency_links.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/requires.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/top_level.txt
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      168 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/admin.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/apps.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/helpers/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 10:11:08.000000 django-webperformers-humans-0.3.1/humans/helpers/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/helpers/images.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/migrations/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1252 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/0001_initial.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      369 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/0002_human_position.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      377 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/0003_human_twitterurl.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      720 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      930 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/models.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/signals/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/signals/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/signals/humans.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.666770 django-webperformers-humans-0.3.1/humans/templates/
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/templates/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     3844 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/templates/humans/personPage.html
--rw-r--r--   0 tadas     (1000) tadas     (1000)     3264 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/templates/humans/teamComponent.html
--rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 11:39:28.000000 django-webperformers-humans-0.3.1/humans/templates/humans/teamPage.html
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/templatetags/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/templatetags/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/templatetags/images.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/tests.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/urls.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2215 2023-05-06 12:18:18.000000 django-webperformers-humans-0.3.1/humans/views.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-05 09:45:45.000000 django-webperformers-humans-0.3.1/pyproject.toml
--rw-r--r--   0 tadas     (1000) tadas     (1000)      939 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/setup.cfg
--rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-05 10:56:42.000000 django-webperformers-humans-0.3.1/setup.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/LICENSE
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/MANIFEST.in
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2186 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1121 2023-05-15 06:54:22.000000 django-webperformers-humans-0.3.2/README.rst
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2186 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1078 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/SOURCES.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/dependency_links.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/requires.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/top_level.txt
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      180 2023-05-15 07:35:41.000000 django-webperformers-humans-0.3.2/humans/admin.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/apps.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/helpers/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/helpers/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      224 2023-05-15 07:08:35.000000 django-webperformers-humans-0.3.2/humans/helpers/generic.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/helpers/images.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      379 2023-05-15 07:33:03.000000 django-webperformers-humans-0.3.2/humans/helpers/team.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/migrations/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1252 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/0001_initial.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      369 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/0002_human_position.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      377 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/0003_human_twitterurl.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      720 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      555 2023-05-15 07:04:27.000000 django-webperformers-humans-0.3.2/humans/migrations/0005_rename_position_human_role_and_more.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1446 2023-05-15 07:34:34.000000 django-webperformers-humans-0.3.2/humans/models.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/signals/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/signals/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/signals/humans.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      251 2023-05-15 07:12:06.000000 django-webperformers-humans-0.3.2/humans/sitemap.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/templates/
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/templates/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3844 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/templates/humans/personPage.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3260 2023-05-15 07:07:41.000000 django-webperformers-humans-0.3.2/humans/templates/humans/teamComponent.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/templates/humans/teamPage.html
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/templatetags/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/templatetags/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/templatetags/images.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/tests.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/urls.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1882 2023-05-15 06:57:26.000000 django-webperformers-humans-0.3.2/humans/views.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/pyproject.toml
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      939 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/setup.cfg
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/setup.py
```

### Comparing `django-webperformers-humans-0.3.1/LICENSE` & `django-webperformers-humans-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.1/PKG-INFO` & `django-webperformers-humans-0.3.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Django app to expose project team in seo-frienly way.
 Home-page: https://www.webperformers.net/
 Author: Your Name
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -28,36 +28,36 @@
 
 Django humans
 =====
 
 Warning - templates are built using TailwindCSS - you need to build a styles for them manually
 
 Humans is a Django app:
-    1. Exposing hunans.txt file
-    2. Exposing project team over /team/ path
-    3. Exposing each project team member over /team/member-name path
+1. Exposing humans.txt file
+2. Exposing project team over /team/ path
+3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
-    1. teamComponent.html - main component of displaying team members
-    2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
-    3. personPage.html - page, displayng each tem member individually, and extending base template. Base template should have humansContent block.
+1. teamComponent.html - main component of displaying team members
+2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
+3. personPage.html - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
 
-To ovveride them, just create same files in your templates dir humans folder
+To override them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
 
-    INSTALLED_APPS = [
+    ``INSTALLED_APPS = [
         ...,
         "humans",
-    ]
+    ]``
 
 2. Include the humans URLconf in your project urls.py like this::
 
-    path('', include('humans.urls')),
+    ``path('', include('humans.urls')),``
 
 3. Run ``python manage.py migrate`` to create the humans models.
```

### Comparing `django-webperformers-humans-0.3.1/README.rst` & `django-webperformers-humans-0.3.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Django humans
 =====
 
 Warning - templates are built using TailwindCSS - you need to build a styles for them manually
 
 Humans is a Django app:
-    1. Exposing hunans.txt file
-    2. Exposing project team over /team/ path
-    3. Exposing each project team member over /team/member-name path
+1. Exposing humans.txt file
+2. Exposing project team over /team/ path
+3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
-    1. teamComponent.html - main component of displaying team members
-    2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
-    3. personPage.html - page, displayng each tem member individually, and extending base template. Base template should have humansContent block.
+1. teamComponent.html - main component of displaying team members
+2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
+3. personPage.html - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
 
-To ovveride them, just create same files in your templates dir humans folder
+To override them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
 
-    INSTALLED_APPS = [
+    ``INSTALLED_APPS = [
         ...,
         "humans",
-    ]
+    ]``
 
 2. Include the humans URLconf in your project urls.py like this::
 
-    path('', include('humans.urls')),
+    ``path('', include('humans.urls')),``
 
 3. Run ``python manage.py migrate`` to create the humans models.
```

### Comparing `django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/PKG-INFO` & `django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Django app to expose project team in seo-frienly way.
 Home-page: https://www.webperformers.net/
 Author: Your Name
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -28,36 +28,36 @@
 
 Django humans
 =====
 
 Warning - templates are built using TailwindCSS - you need to build a styles for them manually
 
 Humans is a Django app:
-    1. Exposing hunans.txt file
-    2. Exposing project team over /team/ path
-    3. Exposing each project team member over /team/member-name path
+1. Exposing humans.txt file
+2. Exposing project team over /team/ path
+3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
-    1. teamComponent.html - main component of displaying team members
-    2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
-    3. personPage.html - page, displayng each tem member individually, and extending base template. Base template should have humansContent block.
+1. teamComponent.html - main component of displaying team members
+2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
+3. personPage.html - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
 
-To ovveride them, just create same files in your templates dir humans folder
+To override them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
 
-    INSTALLED_APPS = [
+    ``INSTALLED_APPS = [
         ...,
         "humans",
-    ]
+    ]``
 
 2. Include the humans URLconf in your project urls.py like this::
 
-    path('', include('humans.urls')),
+    ``path('', include('humans.urls')),``
 
 3. Run ``python manage.py migrate`` to create the humans models.
```

### Comparing `django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/SOURCES.txt` & `django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 django_webperformers_humans.egg-info/dependency_links.txt
 django_webperformers_humans.egg-info/requires.txt
 django_webperformers_humans.egg-info/top_level.txt
 humans/__init__.py
 humans/admin.py
 humans/apps.py
 humans/models.py
+humans/sitemap.py
 humans/tests.py
 humans/urls.py
 humans/views.py
 humans/helpers/__init__.py
+humans/helpers/generic.py
 humans/helpers/images.py
+humans/helpers/team.py
 humans/migrations/0001_initial.py
 humans/migrations/0002_human_position.py
 humans/migrations/0003_human_twitterurl.py
 humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
+humans/migrations/0005_rename_position_human_role_and_more.py
 humans/migrations/__init__.py
 humans/signals/__init__.py
 humans/signals/humans.py
 humans/templates/humans/personPage.html
 humans/templates/humans/teamComponent.html
 humans/templates/humans/teamPage.html
 humans/templatetags/__init__.py
```

### Comparing `django-webperformers-humans-0.3.1/humans/helpers/images.py` & `django-webperformers-humans-0.3.2/humans/helpers/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.1/humans/migrations/0001_initial.py` & `django-webperformers-humans-0.3.2/humans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.1/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py` & `django-webperformers-humans-0.3.2/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.1/humans/signals/humans.py` & `django-webperformers-humans-0.3.2/humans/signals/humans.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.1/humans/templates/humans/personPage.html` & `django-webperformers-humans-0.3.2/humans/templates/humans/personPage.html`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.1/humans/templates/humans/teamComponent.html` & `django-webperformers-humans-0.3.2/humans/templates/humans/teamComponent.html`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         </a>
         {% else %}
             <img class="aspect-[3/2] w-full rounded-2xl object-cover" 
                 {{ person.image|srcSet|safe }}
             >
         {% endif %}
         <h3 class="mt-6 text-lg font-semibold leading-8 text-gray-900">{{person.name}}</h3>
-        <p class="text-base leading-7 text-gray-600">{{person.position}}</p>
-        <div class="mt-4 text-base leading-7 text-gray-600">{{person.smallDescription|safe }}</div>
+        <p class="text-base leading-7 text-gray-600">{{person.role}}</p>
+        <div class="mt-4 text-base leading-7 text-gray-600">{{person.shortDescription|safe }}</div>
         <ul role="list" class="mt-6 flex gap-x-6">
             {% if person.twitterUrl %}
             <li>
                 <a href="{{person.twitterUrl}}" class="text-gray-400 hover:text-gray-500">
                 <span class="sr-only">Twitter</span>
                 <svg class="h-5 w-5" fill="currentColor" viewBox="0 0 20 20" aria-hidden="true">
                     <path d="M6.29 18.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0020 3.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.073 4.073 0 01.8 7.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 010 16.407a11.616 11.616 0 006.29 1.84" />
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 Weâre a dynamic group of individuals who are passionate about what we do and
 dedicated to delivering the best results for our clients.
     * {% for person in team %}
     * {% if person.customSlug %} { person.image|srcSet|safe }} >
  {% else %}
 { person.image|srcSet|safe }} > {% endif %}
 **** {{person.name}} ****
-{{person.position}}
-{{person.smallDescription|safe }}
+{{person.role}}
+{{person.shortDescription|safe }}
     * {% if person.twitterUrl %}
     * Twitter___
     * {% endif %} {% if person.linkedInUrl %}
     * LinkedIn___
     * {% endif %}
 {% endfor %}
```

### Comparing `django-webperformers-humans-0.3.1/humans/templatetags/images.py` & `django-webperformers-humans-0.3.2/humans/templatetags/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.1/setup.cfg` & `django-webperformers-humans-0.3.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-webperformers-humans
-version = 0.3.1
+version = 0.3.2
 description = A Django app to expose project team in seo-frienly way.
 url = https://www.webperformers.net/
 author = Your Name
 author_email = tadas@webperformers.net
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

