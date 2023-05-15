# Comparing `tmp/justpass-me-django-3.0.0.tar.gz` & `tmp/justpass-me-django-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justpass-me-django-3.0.0.tar", last modified: Mon May 15 18:27:46 2023, max compression
+gzip compressed data, was "justpass-me-django-3.0.1.tar", last modified: Mon May 15 18:30:54 2023, max compression
```

## Comparing `justpass-me-django-3.0.0.tar` & `justpass-me-django-3.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 18:27:46.625296 justpass-me-django-3.0.0/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 16:53:18.000000 justpass-me-django-3.0.0/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5097 2023-05-15 18:27:46.625296 justpass-me-django-3.0.0/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3836 2023-05-15 18:25:31.000000 justpass-me-django-3.0.0/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 18:27:46.625296 justpass-me-django-3.0.0/justpass_me_django.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5097 2023-05-15 18:27:46.000000 justpass-me-django-3.0.0/justpass_me_django.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      456 2023-05-15 18:27:46.000000 justpass-me-django-3.0.0/justpass_me_django.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 18:27:46.000000 justpass-me-django-3.0.0/justpass_me_django.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 16:54:06.000000 justpass-me-django-3.0.0/justpass_me_django.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       39 2023-05-15 18:27:46.000000 justpass-me-django-3.0.0/justpass_me_django.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-05-15 18:27:46.000000 justpass-me-django-3.0.0/justpass_me_django.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 18:27:46.625296 justpass-me-django-3.0.0/justpassme/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6758 2023-05-15 18:16:10.000000 justpass-me-django-3.0.0/justpassme/OIDC_CLIENT.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 16:53:18.000000 justpass-me-django-3.0.0/justpassme/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 16:53:18.000000 justpass-me-django-3.0.0/justpassme/admin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 16:53:18.000000 justpass-me-django-3.0.0/justpassme/apps.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1096 2023-05-15 17:40:25.000000 justpass-me-django-3.0.0/justpassme/helpers.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-05-15 17:54:17.000000 justpass-me-django-3.0.0/justpassme/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 16:53:18.000000 justpass-me-django-3.0.0/justpassme/utils.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      968 2023-05-15 17:42:22.000000 justpass-me-django-3.0.0/justpassme/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1659 2023-05-15 18:27:27.000000 justpass-me-django-3.0.0/setup-3.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-15 18:27:46.625296 justpass-me-django-3.0.0/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1459 2023-05-15 18:27:30.000000 justpass-me-django-3.0.0/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 18:30:54.148929 justpass-me-django-3.0.1/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 16:53:18.000000 justpass-me-django-3.0.1/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5099 2023-05-15 18:30:54.148929 justpass-me-django-3.0.1/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3838 2023-05-15 18:30:27.000000 justpass-me-django-3.0.1/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 18:30:54.148929 justpass-me-django-3.0.1/justpass_me_django.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5099 2023-05-15 18:30:54.000000 justpass-me-django-3.0.1/justpass_me_django.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      456 2023-05-15 18:30:54.000000 justpass-me-django-3.0.1/justpass_me_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 18:30:54.000000 justpass-me-django-3.0.1/justpass_me_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 16:54:06.000000 justpass-me-django-3.0.1/justpass_me_django.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       39 2023-05-15 18:30:54.000000 justpass-me-django-3.0.1/justpass_me_django.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-05-15 18:30:54.000000 justpass-me-django-3.0.1/justpass_me_django.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 18:30:54.148929 justpass-me-django-3.0.1/justpassme/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6758 2023-05-15 18:16:10.000000 justpass-me-django-3.0.1/justpassme/OIDC_CLIENT.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 16:53:18.000000 justpass-me-django-3.0.1/justpassme/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 16:53:18.000000 justpass-me-django-3.0.1/justpassme/admin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 16:53:18.000000 justpass-me-django-3.0.1/justpassme/apps.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1096 2023-05-15 17:40:25.000000 justpass-me-django-3.0.1/justpassme/helpers.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-05-15 17:54:17.000000 justpass-me-django-3.0.1/justpassme/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 16:53:18.000000 justpass-me-django-3.0.1/justpassme/utils.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      968 2023-05-15 17:42:22.000000 justpass-me-django-3.0.1/justpassme/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1659 2023-05-15 18:30:49.000000 justpass-me-django-3.0.1/setup-3.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-15 18:30:54.148929 justpass-me-django-3.0.1/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1421 2023-05-15 18:29:56.000000 justpass-me-django-3.0.1/setup.py
```

### Comparing `justpass-me-django-3.0.0/LICENSE` & `justpass-me-django-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.0/PKG-INFO` & `justpass-me-django-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 3.0.0
+Version: 3.0.1
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
 Download-URL: https://github.com/justpass-me/justpass-me-django
 Platform: UNKNOWN
@@ -32,16 +32,16 @@
 License-File: LICENSE
 
 ## Django Client for justpass.me
 
 
 1. Install the justpassme app
 
-    For django 2.2, use justpass-me-django==2.0.0
-    For django 3.1+, use justpass-me-django==3.0.0
+    * For django 2.2, use justpass-me-django<3.0.0
+    * For django 3.1+, use justpass-me-django>3.0.0
     
    ```sh
    pip install justpass-me-django
    ```
 
 2. Add the following to your INSTALLED_APPS
```

### Comparing `justpass-me-django-3.0.0/README.md` & `justpass-me-django-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Django Client for justpass.me
 
 
 1. Install the justpassme app
 
-    For django 2.2, use justpass-me-django==2.0.0
-    For django 3.1+, use justpass-me-django==3.0.0
+    * For django 2.2, use justpass-me-django<3.0.0
+    * For django 3.1+, use justpass-me-django>3.0.0
     
    ```sh
    pip install justpass-me-django
    ```
 
 2. Add the following to your INSTALLED_APPS
```

### Comparing `justpass-me-django-3.0.0/justpass_me_django.egg-info/PKG-INFO` & `justpass-me-django-3.0.1/justpass_me_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 3.0.0
+Version: 3.0.1
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
 Download-URL: https://github.com/justpass-me/justpass-me-django
 Platform: UNKNOWN
@@ -32,16 +32,16 @@
 License-File: LICENSE
 
 ## Django Client for justpass.me
 
 
 1. Install the justpassme app
 
-    For django 2.2, use justpass-me-django==2.0.0
-    For django 3.1+, use justpass-me-django==3.0.0
+    * For django 2.2, use justpass-me-django<3.0.0
+    * For django 3.1+, use justpass-me-django>3.0.0
     
    ```sh
    pip install justpass-me-django
    ```
 
 2. Add the following to your INSTALLED_APPS
```

### Comparing `justpass-me-django-3.0.0/justpassme/OIDC_CLIENT.py` & `justpass-me-django-3.0.1/justpassme/OIDC_CLIENT.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.0/justpassme/helpers.py` & `justpass-me-django-3.0.1/justpassme/helpers.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.0/justpassme/urls.py` & `justpass-me-django-3.0.1/justpassme/urls.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.0/justpassme/views.py` & `justpass-me-django-3.0.1/justpassme/views.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.0/setup-3.py` & `justpass-me-django-3.0.1/setup-3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='justpass-me-django',
-    version='3.0.0',
+    version='3.0.1',
     description='Django Integration with JustPass.me',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='JustPassMe',
     author_email = 'sameh@justpass.me',
     url = 'https://github.com/justpass-me/justpass-me-django',
     download_url='https://github.com/justpass-me/justpass-me-django',
```

### Comparing `justpass-me-django-3.0.0/setup.py` & `justpass-me-django-3.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='justpass-me-django',
-    version='2.0.0',
+    version='2.0.1',
     description='Django Integration with JustPass.me',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='JustPassMe',
     author_email = 'sameh@justpass.me',
     url = 'https://github.com/justpass-me/justpass-me-django',
     download_url='https://github.com/justpass-me/justpass-me-django',
@@ -26,15 +26,14 @@
         #"Development Status :: 5 - Production/Stable",
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
-        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

