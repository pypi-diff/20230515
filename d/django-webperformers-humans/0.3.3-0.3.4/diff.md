# Comparing `tmp/django-webperformers-humans-0.3.3.tar.gz` & `tmp/django-webperformers-humans-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webperformers-humans-0.3.3.tar", last modified: Mon May 15 08:21:00 2023, max compression
+gzip compressed data, was "django-webperformers-humans-0.3.4.tar", last modified: Mon May 15 10:41:20 2023, max compression
```

## Comparing `django-webperformers-humans-0.3.3.tar` & `django-webperformers-humans-0.3.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/
--rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/LICENSE
--rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/MANIFEST.in
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2186 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1121 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/README.rst
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.788718 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2186 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)      850 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/SOURCES.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/dependency_links.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/requires.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/top_level.txt
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      180 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/admin.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/apps.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/helpers/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/helpers/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      224 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/helpers/generic.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/helpers/images.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      379 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/helpers/team.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/migrations/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1785 2023-05-15 08:19:43.000000 django-webperformers-humans-0.3.3/humans/migrations/0001_initial.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/migrations/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1457 2023-05-15 08:08:59.000000 django-webperformers-humans-0.3.3/humans/models.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/signals/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/signals/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/signals/humans.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      251 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/sitemap.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.788718 django-webperformers-humans-0.3.3/humans/templates/
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/templates/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     3844 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/templates/humans/personPage.html
--rw-r--r--   0 tadas     (1000) tadas     (1000)     3260 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/templates/humans/teamComponent.html
--rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/templates/humans/teamPage.html
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/templatetags/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/templatetags/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/templatetags/images.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/tests.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/urls.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1882 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/views.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/pyproject.toml
--rw-r--r--   0 tadas     (1000) tadas     (1000)      939 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/setup.cfg
--rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/setup.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/LICENSE
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/MANIFEST.in
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2293 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1223 2023-05-15 10:17:15.000000 django-webperformers-humans-0.3.4/README.rst
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/django_webperformers_humans.egg-info/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2293 2023-05-15 10:41:19.000000 django-webperformers-humans-0.3.4/django_webperformers_humans.egg-info/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      850 2023-05-15 10:41:19.000000 django-webperformers-humans-0.3.4/django_webperformers_humans.egg-info/SOURCES.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-15 10:41:19.000000 django-webperformers-humans-0.3.4/django_webperformers_humans.egg-info/dependency_links.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-15 10:41:19.000000 django-webperformers-humans-0.3.4/django_webperformers_humans.egg-info/requires.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-15 10:41:19.000000 django-webperformers-humans-0.3.4/django_webperformers_humans.egg-info/top_level.txt
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      180 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.4/humans/admin.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/apps.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/humans/helpers/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/helpers/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      224 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.4/humans/helpers/generic.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/helpers/images.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      379 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.4/humans/helpers/team.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/humans/migrations/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1785 2023-05-15 08:19:43.000000 django-webperformers-humans-0.3.4/humans/migrations/0001_initial.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/migrations/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1457 2023-05-15 08:08:59.000000 django-webperformers-humans-0.3.4/humans/models.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/humans/signals/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/signals/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/signals/humans.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      251 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.4/humans/sitemap.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/humans/templates/
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/humans/templates/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     4019 2023-05-15 10:14:05.000000 django-webperformers-humans-0.3.4/humans/templates/humans/personPage.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3260 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.4/humans/templates/humans/teamComponent.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/templates/humans/teamPage.html
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/humans/templatetags/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/templatetags/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/templatetags/images.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/tests.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/humans/urls.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1882 2023-05-15 10:14:25.000000 django-webperformers-humans-0.3.4/humans/views.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/pyproject.toml
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      944 2023-05-15 10:41:20.023200 django-webperformers-humans-0.3.4/setup.cfg
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.4/setup.py
```

### Comparing `django-webperformers-humans-0.3.3/LICENSE` & `django-webperformers-humans-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.3/PKG-INFO` & `django-webperformers-humans-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.3.3
-Summary: A Django app to expose project team in seo-frienly way.
+Version: 0.3.4
+Summary: A Django app to expose project team in seo-friendly way.
 Home-page: https://www.webperformers.net/
-Author: Your Name
+Author: Tadas Pikutis
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -35,17 +35,17 @@
 1. Exposing humans.txt file
 2. Exposing project team over /team/ path
 3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
-1. teamComponent.html - main component of displaying team members
-2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
-3. personPage.html - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
+1. *teamComponent.html* - main component of displaying team members
+2. *teamPage.html* - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
+3. *personPage.html* - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
 
 To override them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
@@ -57,7 +57,11 @@
 
 2. Include the humans URLconf in your project urls.py like this::
 
     ``path('', include('humans.urls')),``
 
 3. Run ``python manage.py migrate`` to create the humans models.
 
+4. Add ``{% block humansContent %}{% endblock %}`` to your base template to include pages in
+
+
+
```

### Comparing `django-webperformers-humans-0.3.3/README.rst` & `django-webperformers-humans-0.3.4/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 1. Exposing humans.txt file
 2. Exposing project team over /team/ path
 3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
-1. teamComponent.html - main component of displaying team members
-2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
-3. personPage.html - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
+1. *teamComponent.html* - main component of displaying team members
+2. *teamPage.html* - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
+3. *personPage.html* - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
 
 To override them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
@@ -27,8 +27,11 @@
         "humans",
     ]``
 
 2. Include the humans URLconf in your project urls.py like this::
 
     ``path('', include('humans.urls')),``
 
-3. Run ``python manage.py migrate`` to create the humans models.
+3. Run ``python manage.py migrate`` to create the humans models.
+
+4. Add ``{% block humansContent %}{% endblock %}`` to your base template to include pages in
+
```

### Comparing `django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/PKG-INFO` & `django-webperformers-humans-0.3.4/django_webperformers_humans.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.3.3
-Summary: A Django app to expose project team in seo-frienly way.
+Version: 0.3.4
+Summary: A Django app to expose project team in seo-friendly way.
 Home-page: https://www.webperformers.net/
-Author: Your Name
+Author: Tadas Pikutis
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -35,17 +35,17 @@
 1. Exposing humans.txt file
 2. Exposing project team over /team/ path
 3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
-1. teamComponent.html - main component of displaying team members
-2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
-3. personPage.html - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
+1. *teamComponent.html* - main component of displaying team members
+2. *teamPage.html* - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
+3. *personPage.html* - page, displaying each tem member individually, and extending base template. Base template should have humansContent block.
 
 To override them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
@@ -57,7 +57,11 @@
 
 2. Include the humans URLconf in your project urls.py like this::
 
     ``path('', include('humans.urls')),``
 
 3. Run ``python manage.py migrate`` to create the humans models.
 
+4. Add ``{% block humansContent %}{% endblock %}`` to your base template to include pages in
+
+
+
```

### Comparing `django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/SOURCES.txt` & `django-webperformers-humans-0.3.4/django_webperformers_humans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.3/humans/helpers/images.py` & `django-webperformers-humans-0.3.4/humans/helpers/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.3/humans/migrations/0001_initial.py` & `django-webperformers-humans-0.3.4/humans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.3/humans/models.py` & `django-webperformers-humans-0.3.4/humans/models.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.3/humans/signals/humans.py` & `django-webperformers-humans-0.3.4/humans/signals/humans.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.3/humans/templates/humans/personPage.html` & `django-webperformers-humans-0.3.4/humans/templates/humans/personPage.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,63 @@
 {% extends baseTemplate %}
 {% load static %}
 {% load images %}
 {% block humansContent %}
-<main class="pt-20 lg:pt-24 space-y-12 pb-12 px-4 lg:px-20">
-
-    <div class="grid grid-cols-1 lg:grid-cols-2 gap-x-20">
-
-      <div class="px-8">
-        <img class="w-full rounded-lg"
-        {{ person.image|srcSet|safe }}
-        alt="">
-      </div>
-
-      <div class="h-full w-full space-y-16 p-8 lg:p-0">
-
-        <div class="text-3xl md:text-6xl font-bold">
-
-          {{person.name}}
-
-
-        </div>
-
-        <div class="max-w-prose space-y-8 text-base md:text-lg">
-
-          <p>{{person.description|safe}}</p>
-
-        </div>
-
-            <ul role="list" class="flex gap-x-8 lg:gap-x-4">
+<div class="pt-20 lg:pt-24 space-y-12 pb-12 px-16 max-w-6xl mx-auto">
+    <div class="flex flex-col md:flex-row gap-x-8">
+        <div class="px-8 md:w-4/5 lg:w-3/4">
+            <img class="w-full rounded-lg"
+            {{ person.image|srcSet|safe }}
+            alt="">
+            <ul role="list" class="flex gap-x-8 lg:gap-x-4 py-4 text-blue-500">
                 {% if person.twitterUrl %}
                     <li>
-                        <a target="_blank" href="{{person.twitterUrl}}" class="text-gray-400 hover:text-gray-500">
+                        <a target="_blank" href="{{person.twitterUrl}}">
                             <span class="sr-only">Twitter</span>
-                            <svg class="h-5 w-5" fill="currentColor" viewBox="0 0 20 20" aria-hidden="true">
+                            <svg class="h-5 w-5 hover:text-gray-500" fill="currentColor" viewBox="0 0 20 20" aria-hidden="true">
                                 <path d="M6.29 18.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0020 3.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.073 4.073 0 01.8 7.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 010 16.407a11.616 11.616 0 006.29 1.84" />
                             </svg>
                         </a>
                     </li>
                 {% endif %}
                 {% if person.linkedInUrl %}
                     <li>
-                        <a href="{{person.linkedInUrl}}" target="_blank" class="text-gray-400 hover:text-gray-500">
+                        <a href="{{person.linkedInUrl}}" target="_blank">
                                 <span class="sr-only">LinkedIn</span>
-                                <svg class="h-5 w-5" fill="currentColor" viewBox="0 0 20 20" aria-hidden="true">
+                                <svg class="h-8 w-8  hover:text-gray-500" fill="currentColor" viewBox="0 0 20 20" aria-hidden="true">
                                     <path fill-rule="evenodd" d="M16.338 16.338H13.67V12.16c0-.995-.017-2.277-1.387-2.277-1.39 0-1.601 1.086-1.601 2.207v4.248H8.014v-8.59h2.559v1.174h.037c.356-.675 1.227-1.387 2.526-1.387 2.703 0 3.203 1.778 3.203 4.092v4.711zM5.005 6.575a1.548 1.548 0 11-.003-3.096 1.548 1.548 0 01.003 3.096zm-1.337 9.763H6.34v-8.59H3.667v8.59zM17.668 1H2.328C1.595 1 1 1.581 1 2.298v15.403C1 18.418 1.595 19 2.328 19h15.34c.734 0 1.332-.582 1.332-1.299V2.298C19 1.581 18.402 1 17.668 1z" clip-rule="evenodd" />
                                 </svg>
                         </a>
                     </li>
                 {% endif %}
                 {% if person.websiteUrl %}
                     <li>
-                        <a href="{{person.websiteUrl}}" target="_blank" class="text-gray-400 hover:text-gray-500">
+                        <a href="{{person.websiteUrl}}" target="_blank">
                                 <span class="sr-only">Website</span>
-                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5">
+                                <svg class="w-8 h-8  hover:text-gray-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" >
                                     <path stroke-linecap="round" stroke-linejoin="round" d="M12 21a9.004 9.004 0 008.716-6.747M12 21a9.004 9.004 0 01-8.716-6.747M12 21c2.485 0 4.5-4.03 4.5-9S14.485 3 12 3m0 18c-2.485 0-4.5-4.03-4.5-9S9.515 3 12 3m0 0a8.997 8.997 0 017.843 4.582M12 3a8.997 8.997 0 00-7.843 4.582m15.686 0A11.953 11.953 0 0112 10.5c-2.998 0-5.74-1.1-7.843-2.918m15.686 0A8.959 8.959 0 0121 12c0 .778-.099 1.533-.284 2.253m0 0A17.919 17.919 0 0112 16.5c-3.162 0-6.133-.815-8.716-2.247m0 0A9.015 9.015 0 013 12c0-1.605.42-3.113 1.157-4.418" />
                                 </svg>
                         
                         </a>
                     </li>
                 {% endif %}
             </ul>
+        </div>
+        <div class="h-full w-full space-y-8 p-8 lg:p-0">
+        
+        <div class="text-3xl md:text-4xl font-bold">
+            {{person.name}}
+            <div class="text-lg pt-2 lg:pl-1 text-blue-500">
+                {{person.role}}
+            </div>
+        </div>
 
-
-      </div>
-
+        <div class="max-w-prose space-y-8">
+            <div class="mt-4 text-base text-gray-700 text-left">
+                {{person.description|safe}}
+            </div>
+        </div>
+            
+        </div>
     </div>
-
-
-  </main>
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends baseTemplate %} {% load static %} {% load images %} {% block
 humansContent %}
 { person.image|srcSet|safe }} alt="">
-{{person.name}}
-{{person.description|safe}}
     * {% if person.twitterUrl %}
     * Twitter___
     * {% endif %} {% if person.linkedInUrl %}
     * LinkedIn___
     * {% endif %} {% if person.websiteUrl %}
     * Website___
     * {% endif %}
- {% endblock %}
+{{person.name}}
+{{person.role}}
+{{person.description|safe}}
+{% endblock %}
```

### Comparing `django-webperformers-humans-0.3.3/humans/templates/humans/teamComponent.html` & `django-webperformers-humans-0.3.4/humans/templates/humans/teamComponent.html`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.3/humans/templatetags/images.py` & `django-webperformers-humans-0.3.4/humans/templatetags/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.3/humans/views.py` & `django-webperformers-humans-0.3.4/humans/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 def humans_txt(request):
     response:str = "/* TEAM */\n\n"
     team:QuerySet = getTeam(request)
     if (team.__len__() > 0 or request.user.is_superuser):
         person:Human
         for person in team:
             personString:str = "--------------------------------------------\n"
-            personString = personString + f"""Title: {person.position}\nName: {person.name}\nSite: {person.websiteUrl}\nTwitter: {person.twitterUrl}\nLinkedIn: {person.linkedInUrl}\nAbout:\n{strip_tags(person.smallDescription)}\n"""
+            personString = personString + f"""Title: {person.position}\nName: {person.name}\nSite: {person.websiteUrl}\nTwitter: {person.twitterUrl}\nLinkedIn: {person.linkedInUrl}\nAbout:\n{strip_tags(person.shortDescription)}\n"""
             personString = personString + "--------------------------------------------\n"
             response = response + personString
         return HttpResponse (response, content_type="text/plain")
     else:
         return HttpResponseNotFound()
```

### Comparing `django-webperformers-humans-0.3.3/setup.cfg` & `django-webperformers-humans-0.3.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = django-webperformers-humans
-version = 0.3.3
-description = A Django app to expose project team in seo-frienly way.
+version = 0.3.4
+description = A Django app to expose project team in seo-friendly way.
 url = https://www.webperformers.net/
-author = Your Name
+author = Tadas Pikutis
 author_email = tadas@webperformers.net
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
```

