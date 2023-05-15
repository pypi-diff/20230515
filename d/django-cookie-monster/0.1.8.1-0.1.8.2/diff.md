# Comparing `tmp/django-cookie-monster-0.1.8.1.tar.gz` & `tmp/django-cookie-monster-0.1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cookie-monster-0.1.8.1.tar", last modified: Thu Apr 20 19:03:21 2023, max compression
+gzip compressed data, was "django-cookie-monster-0.1.8.2.tar", last modified: Mon May 15 15:11:15 2023, max compression
```

## Comparing `django-cookie-monster-0.1.8.1.tar` & `django-cookie-monster-0.1.8.2.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.416188 django-cookie-monster-0.1.8.1/
--rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/AUTHORS.rst
--rw-r--r--   0 phil       (501) staff       (20)     3339 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/CONTRIBUTING.rst
--rw-r--r--   0 phil       (501) staff       (20)      903 2023-04-20 19:01:58.000000 django-cookie-monster-0.1.8.1/HISTORY.rst
--rw-r--r--   0 phil       (501) staff       (20)     1509 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      187 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)     6529 2023-04-20 19:03:21.416287 django-cookie-monster-0.1.8.1/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     4703 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.411466 django-cookie-monster-0.1.8.1/cookie_monster/
--rw-r--r--   0 phil       (501) staff       (20)       24 2023-04-20 19:01:53.000000 django-cookie-monster-0.1.8.1/cookie_monster/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      122 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/apps.py
--rw-r--r--   0 phil       (501) staff       (20)     2370 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/settings.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.405073 django-cookie-monster-0.1.8.1/cookie_monster/static/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.405218 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.411802 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/css/
--rw-r--r--   0 phil       (501) staff       (20)     1920 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/css/minimal.css
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.414087 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/
--rw-r--r--   0 phil       (501) staff       (20)    48527 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js
--rw-r--r--   0 phil       (501) staff       (20)   288273 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js.map
--rw-r--r--   0 phil       (501) staff       (20)    48746 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js
--rw-r--r--   0 phil       (501) staff       (20)   288321 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js.map
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.405362 django-cookie-monster-0.1.8.1/cookie_monster/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.414941 django-cookie-monster-0.1.8.1/cookie_monster/templates/cookie_monster/
--rw-r--r--   0 phil       (501) staff       (20)     3413 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/templates/cookie_monster/base.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.415261 django-cookie-monster-0.1.8.1/cookie_monster/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      634 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/templatetags/cookie_monster.py
--rw-r--r--   0 phil       (501) staff       (20)      239 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/urls.py
--rw-r--r--   0 phil       (501) staff       (20)      540 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/utils.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.416043 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)     6529 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      882 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/not-zip-safe
--rw-r--r--   0 phil       (501) staff       (20)       15 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)      329 2023-04-20 19:03:21.416665 django-cookie-monster-0.1.8.1/setup.cfg
--rwxr-xr-x   0 phil       (501) staff       (20)     2396 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/setup.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.348255 django-cookie-monster-0.1.8.2/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      152 2020-01-08 07:58:00.000000 django-cookie-monster-0.1.8.2/AUTHORS.rst
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     3339 2020-01-08 07:58:00.000000 django-cookie-monster-0.1.8.2/CONTRIBUTING.rst
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      964 2023-05-15 15:00:04.000000 django-cookie-monster-0.1.8.2/HISTORY.rst
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1509 2020-01-08 07:58:00.000000 django-cookie-monster-0.1.8.2/LICENSE
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      187 2023-05-15 14:57:08.000000 django-cookie-monster-0.1.8.2/MANIFEST.in
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     6570 2023-05-15 15:11:15.348403 django-cookie-monster-0.1.8.2/PKG-INFO
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     4703 2022-10-11 06:50:21.000000 django-cookie-monster-0.1.8.2/README.md
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.332507 django-cookie-monster-0.1.8.2/cookie_monster/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       24 2023-05-15 15:00:04.000000 django-cookie-monster-0.1.8.2/cookie_monster/__init__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      102 2023-05-15 15:03:41.000000 django-cookie-monster-0.1.8.2/cookie_monster/apps.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2230 2023-05-15 15:02:40.000000 django-cookie-monster-0.1.8.2/cookie_monster/settings.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.323184 django-cookie-monster-0.1.8.2/cookie_monster/static/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.323606 django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.333114 django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/css/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1920 2021-02-15 12:23:56.000000 django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/css/minimal.css
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.340378 django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)    48527 2022-10-11 06:50:21.000000 django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js
+-rw-r--r--   0 christianschuermann   (501) staff       (20)   288273 2022-10-11 06:50:21.000000 django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js.map
+-rw-r--r--   0 christianschuermann   (501) staff       (20)    48746 2022-10-11 06:50:21.000000 django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js
+-rw-r--r--   0 christianschuermann   (501) staff       (20)   288321 2022-10-11 06:50:21.000000 django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js.map
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.323939 django-cookie-monster-0.1.8.2/cookie_monster/templates/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.342884 django-cookie-monster-0.1.8.2/cookie_monster/templates/cookie_monster/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     3413 2022-10-11 06:50:21.000000 django-cookie-monster-0.1.8.2/cookie_monster/templates/cookie_monster/base.html
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.344231 django-cookie-monster-0.1.8.2/cookie_monster/templatetags/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        0 2020-02-07 13:39:22.000000 django-cookie-monster-0.1.8.2/cookie_monster/templatetags/__init__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      677 2023-05-15 15:04:52.000000 django-cookie-monster-0.1.8.2/cookie_monster/templatetags/cookie_monster.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      191 2023-05-15 15:02:07.000000 django-cookie-monster-0.1.8.2/cookie_monster/urls.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      339 2023-05-15 15:04:04.000000 django-cookie-monster-0.1.8.2/cookie_monster/utils.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.347155 django-cookie-monster-0.1.8.2/django_cookie_monster.egg-info/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     6570 2023-05-15 15:11:15.000000 django-cookie-monster-0.1.8.2/django_cookie_monster.egg-info/PKG-INFO
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      903 2023-05-15 15:11:15.000000 django-cookie-monster-0.1.8.2/django_cookie_monster.egg-info/SOURCES.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        1 2023-05-15 15:11:15.000000 django-cookie-monster-0.1.8.2/django_cookie_monster.egg-info/dependency_links.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        1 2020-02-10 15:34:35.000000 django-cookie-monster-0.1.8.2/django_cookie_monster.egg-info/not-zip-safe
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       15 2023-05-15 15:11:15.000000 django-cookie-monster-0.1.8.2/django_cookie_monster.egg-info/top_level.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      329 2023-05-15 15:11:15.349276 django-cookie-monster-0.1.8.2/setup.cfg
+-rwxr-xr-x   0 christianschuermann   (501) staff       (20)     2396 2020-04-08 15:26:25.000000 django-cookie-monster-0.1.8.2/setup.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-05-15 15:11:15.347594 django-cookie-monster-0.1.8.2/tests/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      369 2020-01-08 07:58:00.000000 django-cookie-monster-0.1.8.2/tests/test_models.py
```

### Comparing `django-cookie-monster-0.1.8.1/CONTRIBUTING.rst` & `django-cookie-monster-0.1.8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/HISTORY.rst` & `django-cookie-monster-0.1.8.2/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 .. :changelog:
 
 History
 -------
+0.1.8.2 (2023-05-15)
+++++++++++++++++++
+
+* Simplify imports
+
 0.1.8.1 (2023-04-20)
 ++++++++++++++++++
 
 * Include *.map files in source distribution
 
 
 0.1.8 (2023-02-02)
```

### Comparing `django-cookie-monster-0.1.8.1/LICENSE` & `django-cookie-monster-0.1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/PKG-INFO` & `django-cookie-monster-0.1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cookie-monster
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: Your project description goes here
 Home-page: https://github.com/victoriameyer/django-cookie-monster
 Author: dreipol GmbH
 Author-email: dev@dreipol.ch
 License: BSD
 Keywords: django-cookie-monster
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
@@ -206,14 +205,19 @@
 
 
 
 
 
 History
 -------
+0.1.8.2 (2023-05-15)
+++++++++++++++++++
+
+* Simplify imports
+
 0.1.8.1 (2023-04-20)
 ++++++++++++++++++
 
 * Include *.map files in source distribution
 
 
 0.1.8 (2023-02-02)
@@ -267,9 +271,7 @@
 * Bugfix
 
 
 0.1.0 (2019-10-16)
 ++++++++++++++++++
 
 * First release on PyPI.
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: django-cookie-monster Version: 0.1.8.1 Summary:
+Metadata-Version: 2.1 Name: django-cookie-monster Version: 0.1.8.2 Summary:
 Your project description goes here Home-page: https://github.com/victoriameyer/
 django-cookie-monster Author: dreipol GmbH Author-email: dev@dreipol.ch
-License: BSD Keywords: django-cookie-monster Platform: UNKNOWN Classifier:
-Development Status :: 3 - Alpha Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0 Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Description-Content-Type: text/markdown License-File:
-LICENSE License-File: AUTHORS.rst # django-cookie-monster [https://github.com/
-dreipol/django-cookie-monster/raw/develop/docs/cookie_monster.svg] [![CircleCI]
-(https://circleci.com/gh/dreipol/django-cookie-monster.svg?style=svg)](https://
-circleci.com/gh/dreipol/django-cookie-monster) [![Maintainability](https://
-api.codeclimate.com/v1/badges/3032662f751343e49710/maintainability)](https://
-codeclimate.com/github/dreipol/django-cookie-monster/maintainability) [!
-[Coverage Status](https://coveralls.io/repos/github/dreipol/django-cookie-
-monster/badge.svg?branch=develop)](https://coveralls.io/github/dreipol/django-
-cookie-monster?branch=develop) This package gives you two versions of a cookie
-banner. The simple one is basically just a hint to inform users that you are
-using cookies. The group version let's your users decide which cookies he
-needs. Quickstart ---------- Install django-cookie-monster:: pip install
-django-cookie-monster Add it to your `INSTALLED_APPS`: ``` INSTALLED_APPS =
-( ... 'cookie_monster', ... ) ``` Add a type and data property to all script
-tags that store any cookies. ```html
+License: BSD Keywords: django-cookie-monster Classifier: Development Status ::
+3 - Alpha Classifier: Framework :: Django :: 1.11 Classifier: Framework ::
+Django :: 2.0 Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: BSD License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 2 Classifier: Programming
+Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4 Classifier: Programming
+Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown License-File: LICENSE License-File:
+AUTHORS.rst # django-cookie-monster [https://github.com/dreipol/django-cookie-
+monster/raw/develop/docs/cookie_monster.svg] [![CircleCI](https://circleci.com/
+gh/dreipol/django-cookie-monster.svg?style=svg)](https://circleci.com/gh/
+dreipol/django-cookie-monster) [![Maintainability](https://api.codeclimate.com/
+v1/badges/3032662f751343e49710/maintainability)](https://codeclimate.com/
+github/dreipol/django-cookie-monster/maintainability) [![Coverage Status]
+(https://coveralls.io/repos/github/dreipol/django-cookie-monster/
+badge.svg?branch=develop)](https://coveralls.io/github/dreipol/django-cookie-
+monster?branch=develop) This package gives you two versions of a cookie banner.
+The simple one is basically just a hint to inform users that you are using
+cookies. The group version let's your users decide which cookies he needs.
+Quickstart ---------- Install django-cookie-monster:: pip install django-
+cookie-monster Add it to your `INSTALLED_APPS`: ``` INSTALLED_APPS = ( ...
+'cookie_monster', ... ) ``` Add a type and data property to all script tags
+that store any cookies. ```html
 
  ``` Settings -------- Overwrite strings in your settings file. You will find a
 complete reference below. ```python COOKIE_MONSTER = { 'banner': { 'title': 'My
 Cookie Banner Title', } } ``` To switch from standard to group mode you need to
 specify a list of setting groups. ```python COOKIE_MONSTER = { 'cookie_groups':
 { 'rows': [ 'Name', 'Provider', 'Purpose', ], 'groups': [ { 'title':
 'Necessary', 'required': True, 'cookies': [ { 'id': 'application', 'rows':
@@ -47,17 +47,18 @@
 'Purpose', ], 'groups': [ { 'title': 'Necessary', 'required': True, 'cookies':
 [ { 'id': 'application', 'rows': [ 'Language', 'example.com', 'site language',
 ], }, ], }, { 'title': 'Marketing', 'required': False, 'cookies': [ { 'id':
 'GTM', 'rows': [ 'Google Tag Manager', 'Google.com', 'tracking cookie', ], },
 ], }, ], }, } ``` # Contribute ## Installation To install the frontend you will
 need to run: ```sh npm i ``` ## Building frontend The frontend can be built
 via: ```sh npm run build ``` ## Unit test You can unit test the frontend code
-with: ```sh npm test ``` History ------- 0.1.8.1 (2023-04-20)
-++++++++++++++++++ * Include *.map files in source distribution 0.1.8 (2023-02-
-02) ++++++++++++++++++ * Add Django 4 compatibility 0.1.7 (2022-10-11)
+with: ```sh npm test ``` History ------- 0.1.8.2 (2023-05-15)
+++++++++++++++++++ * Simplify imports 0.1.8.1 (2023-04-20) ++++++++++++++++++ *
+Include *.map files in source distribution 0.1.8 (2023-02-02)
+++++++++++++++++++ * Add Django 4 compatibility 0.1.7 (2022-10-11)
 ++++++++++++++++++ * Add samesite configuration option 0.1.6 (2022-01-31)
 ++++++++++++++++++ * Simplify banner text to prevent fails DEPRECATION WARNING:
 * The setting variable `policy_link` was removed due to errors. Please handle
 any text/link combinations yourself. 0.1.5 (2021-02-15) ++++++++++++++++++ *
 Add plain html support for the groups labels 0.1.4 (2020-05-13)
 ++++++++++++++++++ * Improve backward compatibility of browsers 0.1.3 (2020-05-
 13) ++++++++++++++++++ * Fix translation issue in banner text 0.1.2 (2020-04-
```

### Comparing `django-cookie-monster-0.1.8.1/README.md` & `django-cookie-monster-0.1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/cookie_monster/settings.py` & `django-cookie-monster-0.1.8.2/cookie_monster/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,56 @@
-import six
 from django.conf import settings
-from django.utils.functional import lazy
-from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
-from cookie_monster.utils import get_callable
 
-COOKIE_MONSTER = getattr(settings, 'COOKIE_MONSTER')
-
-
-def get_settings_variable(nested_keys, default, obj=COOKIE_MONSTER):
+def get_settings_variable(nested_keys, default, obj=None):
     """
     :param nested_keys: an array of keys
     :param default: the fallback value
     :param obj: the object
     """
     try:
         current_key = nested_keys.pop(0)
     except IndexError:
         return default
 
+    if not obj:
+        obj = getattr(settings, 'COOKIE_MONSTER')
+
     if current_key in obj:
         if nested_keys:
             return get_settings_variable(nested_keys=nested_keys, default=default, obj=obj[current_key])
         return obj[current_key]
     return default
 
 
-COOKIE_MONSTER_BASE_CONFIG = {
-    'banner': {
-        'title': get_settings_variable(['banner', 'title'], _('Cookie Banner')),
-        'text': get_settings_variable(['banner', 'text'], _('This website uses cookies to provide you with an optimal '
-                                                            'user experience.')),
-    },
-    'cookie': {
-        'identifier': get_settings_variable(['cookie', 'identifier'], _('cookie_consent')),
-        'age': get_settings_variable(['cookie', 'age'], 604800),
-        'samesite': get_settings_variable(['cookie', 'samesite'], 'Lax'),
-    },
-    'accordion_title': get_settings_variable(['accordion_title'], _('{groupTitle} ({amount})')),
-    'buttons': {
-        'confirm': {
-            'label': get_settings_variable(['banner', 'buttons', 'confirm', 'label'], _('Accept all cookies')),
+def get_base_config():
+    return {
+        'banner': {
+            'title': get_settings_variable(['banner', 'title'], _('Cookie Banner')),
+            'text': get_settings_variable(['banner',
+                                           'text'], _('This website uses cookies to provide you with an optimal '
+                                                      'user experience.')),
         },
-        'toggle': {
-            'label': get_settings_variable(['banner', 'buttons', 'toggle', 'label'], _('Toggle settings')),
+        'cookie': {
+            'identifier': get_settings_variable(['cookie', 'identifier'], _('cookie_consent')),
+            'age': get_settings_variable(['cookie', 'age'], 604800),
+            'samesite': get_settings_variable(['cookie', 'samesite'], 'Lax'),
         },
-        'accept_all_cookies': {
-            'label': get_settings_variable(['banner', 'buttons', 'accept_all_cookies', 'label'],
-                                           _('Accept all cookies')),
-        },
-        'accept_all_group_cookies': {
-            'label': get_settings_variable(['banner', 'buttons', 'accept_all_group_cookies', 'label'],
-                                           _('Accept {groupTitle} cookies')),
-        },
-    },
-}
-
-COOKIE_MONSTER_CUSTOM_THEME = get_settings_variable(['custom_theme'], False)
-COOKIE_MONSTER_GROUPS = get_settings_variable(['cookie_groups'], [])
+        'accordion_title': get_settings_variable(['accordion_title'], _('{groupTitle} ({amount})')),
+        'buttons': {
+            'confirm': {
+                'label': get_settings_variable(['banner', 'buttons', 'confirm', 'label'], _('Accept all cookies')),
+            },
+            'toggle': {
+                'label': get_settings_variable(['banner', 'buttons', 'toggle', 'label'], _('Toggle settings')),
+            },
+            'accept_all_cookies': {
+                'label': get_settings_variable(['banner', 'buttons', 'accept_all_cookies', 'label'],
+                                               _('Accept all cookies')),
+            },
+            'accept_all_group_cookies': {
+                'label': get_settings_variable(['banner', 'buttons', 'accept_all_group_cookies', 'label'],
+                                               _('Accept {groupTitle} cookies')),
+            },
+        }
+    }
```

### Comparing `django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/css/minimal.css` & `django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/css/minimal.css`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js` & `django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js.map` & `django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js` & `django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js.map` & `django-cookie-monster-0.1.8.2/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js.map`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/cookie_monster/templates/cookie_monster/base.html` & `django-cookie-monster-0.1.8.2/cookie_monster/templates/cookie_monster/base.html`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/PKG-INFO` & `django-cookie-monster-0.1.8.2/django_cookie_monster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cookie-monster
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: Your project description goes here
 Home-page: https://github.com/victoriameyer/django-cookie-monster
 Author: dreipol GmbH
 Author-email: dev@dreipol.ch
 License: BSD
 Keywords: django-cookie-monster
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
@@ -206,14 +205,19 @@
 
 
 
 
 
 History
 -------
+0.1.8.2 (2023-05-15)
+++++++++++++++++++
+
+* Simplify imports
+
 0.1.8.1 (2023-04-20)
 ++++++++++++++++++
 
 * Include *.map files in source distribution
 
 
 0.1.8 (2023-02-02)
@@ -267,9 +271,7 @@
 * Bugfix
 
 
 0.1.0 (2019-10-16)
 ++++++++++++++++++
 
 * First release on PyPI.
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: django-cookie-monster Version: 0.1.8.1 Summary:
+Metadata-Version: 2.1 Name: django-cookie-monster Version: 0.1.8.2 Summary:
 Your project description goes here Home-page: https://github.com/victoriameyer/
 django-cookie-monster Author: dreipol GmbH Author-email: dev@dreipol.ch
-License: BSD Keywords: django-cookie-monster Platform: UNKNOWN Classifier:
-Development Status :: 3 - Alpha Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0 Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Description-Content-Type: text/markdown License-File:
-LICENSE License-File: AUTHORS.rst # django-cookie-monster [https://github.com/
-dreipol/django-cookie-monster/raw/develop/docs/cookie_monster.svg] [![CircleCI]
-(https://circleci.com/gh/dreipol/django-cookie-monster.svg?style=svg)](https://
-circleci.com/gh/dreipol/django-cookie-monster) [![Maintainability](https://
-api.codeclimate.com/v1/badges/3032662f751343e49710/maintainability)](https://
-codeclimate.com/github/dreipol/django-cookie-monster/maintainability) [!
-[Coverage Status](https://coveralls.io/repos/github/dreipol/django-cookie-
-monster/badge.svg?branch=develop)](https://coveralls.io/github/dreipol/django-
-cookie-monster?branch=develop) This package gives you two versions of a cookie
-banner. The simple one is basically just a hint to inform users that you are
-using cookies. The group version let's your users decide which cookies he
-needs. Quickstart ---------- Install django-cookie-monster:: pip install
-django-cookie-monster Add it to your `INSTALLED_APPS`: ``` INSTALLED_APPS =
-( ... 'cookie_monster', ... ) ``` Add a type and data property to all script
-tags that store any cookies. ```html
+License: BSD Keywords: django-cookie-monster Classifier: Development Status ::
+3 - Alpha Classifier: Framework :: Django :: 1.11 Classifier: Framework ::
+Django :: 2.0 Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: BSD License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 2 Classifier: Programming
+Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4 Classifier: Programming
+Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown License-File: LICENSE License-File:
+AUTHORS.rst # django-cookie-monster [https://github.com/dreipol/django-cookie-
+monster/raw/develop/docs/cookie_monster.svg] [![CircleCI](https://circleci.com/
+gh/dreipol/django-cookie-monster.svg?style=svg)](https://circleci.com/gh/
+dreipol/django-cookie-monster) [![Maintainability](https://api.codeclimate.com/
+v1/badges/3032662f751343e49710/maintainability)](https://codeclimate.com/
+github/dreipol/django-cookie-monster/maintainability) [![Coverage Status]
+(https://coveralls.io/repos/github/dreipol/django-cookie-monster/
+badge.svg?branch=develop)](https://coveralls.io/github/dreipol/django-cookie-
+monster?branch=develop) This package gives you two versions of a cookie banner.
+The simple one is basically just a hint to inform users that you are using
+cookies. The group version let's your users decide which cookies he needs.
+Quickstart ---------- Install django-cookie-monster:: pip install django-
+cookie-monster Add it to your `INSTALLED_APPS`: ``` INSTALLED_APPS = ( ...
+'cookie_monster', ... ) ``` Add a type and data property to all script tags
+that store any cookies. ```html
 
  ``` Settings -------- Overwrite strings in your settings file. You will find a
 complete reference below. ```python COOKIE_MONSTER = { 'banner': { 'title': 'My
 Cookie Banner Title', } } ``` To switch from standard to group mode you need to
 specify a list of setting groups. ```python COOKIE_MONSTER = { 'cookie_groups':
 { 'rows': [ 'Name', 'Provider', 'Purpose', ], 'groups': [ { 'title':
 'Necessary', 'required': True, 'cookies': [ { 'id': 'application', 'rows':
@@ -47,17 +47,18 @@
 'Purpose', ], 'groups': [ { 'title': 'Necessary', 'required': True, 'cookies':
 [ { 'id': 'application', 'rows': [ 'Language', 'example.com', 'site language',
 ], }, ], }, { 'title': 'Marketing', 'required': False, 'cookies': [ { 'id':
 'GTM', 'rows': [ 'Google Tag Manager', 'Google.com', 'tracking cookie', ], },
 ], }, ], }, } ``` # Contribute ## Installation To install the frontend you will
 need to run: ```sh npm i ``` ## Building frontend The frontend can be built
 via: ```sh npm run build ``` ## Unit test You can unit test the frontend code
-with: ```sh npm test ``` History ------- 0.1.8.1 (2023-04-20)
-++++++++++++++++++ * Include *.map files in source distribution 0.1.8 (2023-02-
-02) ++++++++++++++++++ * Add Django 4 compatibility 0.1.7 (2022-10-11)
+with: ```sh npm test ``` History ------- 0.1.8.2 (2023-05-15)
+++++++++++++++++++ * Simplify imports 0.1.8.1 (2023-04-20) ++++++++++++++++++ *
+Include *.map files in source distribution 0.1.8 (2023-02-02)
+++++++++++++++++++ * Add Django 4 compatibility 0.1.7 (2022-10-11)
 ++++++++++++++++++ * Add samesite configuration option 0.1.6 (2022-01-31)
 ++++++++++++++++++ * Simplify banner text to prevent fails DEPRECATION WARNING:
 * The setting variable `policy_link` was removed due to errors. Please handle
 any text/link combinations yourself. 0.1.5 (2021-02-15) ++++++++++++++++++ *
 Add plain html support for the groups labels 0.1.4 (2020-05-13)
 ++++++++++++++++++ * Improve backward compatibility of browsers 0.1.3 (2020-05-
 13) ++++++++++++++++++ * Fix translation issue in banner text 0.1.2 (2020-04-
```

### Comparing `django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/SOURCES.txt` & `django-cookie-monster-0.1.8.2/django_cookie_monster.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 cookie_monster/templates/cookie_monster/base.html
 cookie_monster/templatetags/__init__.py
 cookie_monster/templatetags/cookie_monster.py
 django_cookie_monster.egg-info/PKG-INFO
 django_cookie_monster.egg-info/SOURCES.txt
 django_cookie_monster.egg-info/dependency_links.txt
 django_cookie_monster.egg-info/not-zip-safe
-django_cookie_monster.egg-info/top_level.txt
+django_cookie_monster.egg-info/top_level.txt
+tests/test_models.py
```

### Comparing `django-cookie-monster-0.1.8.1/setup.py` & `django-cookie-monster-0.1.8.2/setup.py`

 * *Files identical despite different names*

