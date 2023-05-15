# Comparing `tmp/chino-2.8.0.tar.gz` & `tmp/chino-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chino-2.8.0.tar", last modified: Wed Jul 21 07:33:45 2021, max compression
+gzip compressed data, was "dist/chino-2.9.0.tar", last modified: Mon Nov 22 11:12:11 2021, max compression
```

## Comparing `chino-2.8.0.tar` & `chino-2.9.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 07:33:45.000000 chino-2.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      296 2021-07-21 07:33:35.000000 chino-2.8.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1737 2021-07-21 07:33:35.000000 chino-2.8.0/.travis.yml
--rw-r--r--   0 root         (0) root         (0)      364 2021-07-21 07:33:45.000000 chino-2.8.0/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)     1430 2021-07-21 07:33:35.000000 chino-2.8.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      572 2021-07-21 07:33:35.000000 chino-2.8.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     5564 2021-07-21 07:33:45.000000 chino-2.8.0/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)     7760 2021-07-21 07:33:35.000000 chino-2.8.0/INSTRUCTIONS.md
--rw-r--r--   0 root         (0) root         (0)      801 2021-07-21 07:33:45.000000 chino-2.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      103 2021-07-21 07:33:35.000000 chino-2.8.0/PopupNotification.vbs
--rw-rw-rw-   0 root         (0) root         (0)     1968 2021-07-21 07:33:35.000000 chino-2.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      340 2021-07-21 07:33:35.000000 chino-2.8.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 07:33:45.000000 chino-2.8.0/chino/
--rw-rw-rw-   0 root         (0) root         (0)       55 2021-07-21 07:33:35.000000 chino-2.8.0/chino/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    56349 2021-07-21 07:33:35.000000 chino-2.8.0/chino/api.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2021-07-21 07:33:35.000000 chino-2.8.0/chino/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    27360 2021-07-21 07:33:35.000000 chino-2.8.0/chino/objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 07:33:45.000000 chino-2.8.0/chino.egg-info/
--rw-r--r--   0 root         (0) root         (0)      801 2021-07-21 07:33:45.000000 chino-2.8.0/chino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      625 2021-07-21 07:33:45.000000 chino-2.8.0/chino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-21 07:33:45.000000 chino-2.8.0/chino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-21 07:33:45.000000 chino-2.8.0/chino.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2021-07-21 07:33:45.000000 chino-2.8.0/chino.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       51 2021-07-21 07:33:45.000000 chino-2.8.0/chino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-07-21 07:33:45.000000 chino-2.8.0/chino.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     9311 2021-07-21 07:33:35.000000 chino-2.8.0/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-07-21 07:33:35.000000 chino-2.8.0/docs.rst
--rw-rw-rw-   0 root         (0) root         (0)      260 2021-07-21 07:33:35.000000 chino-2.8.0/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2021-07-21 07:33:35.000000 chino-2.8.0/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     1065 2021-07-21 07:33:35.000000 chino-2.8.0/license.txt
--rw-rw-rw-   0 root         (0) root         (0)       53 2021-07-21 07:33:35.000000 chino-2.8.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      558 2021-07-21 07:33:45.000000 chino-2.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1444 2021-07-21 07:33:35.000000 chino-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 07:33:45.000000 chino-2.8.0/test/
--rw-rw-rw-   0 root         (0) root         (0)       55 2021-07-21 07:33:35.000000 chino-2.8.0/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2021-07-21 07:33:35.000000 chino-2.8.0/test/cfg.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2021-07-21 07:33:35.000000 chino-2.8.0/test/logging.conf
--rw-rw-rw-   0 root         (0) root         (0)    15291 2021-07-21 07:33:35.000000 chino-2.8.0/test/logo.png
--rw-rw-rw-   0 root         (0) root         (0)       27 2021-07-21 07:33:35.000000 chino-2.8.0/test/outtest.sh
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-21 07:33:35.000000 chino-2.8.0/test/test.file
--rwxrwxrwx   0 root         (0) root         (0)       27 2021-07-21 07:33:35.000000 chino-2.8.0/test/test.sh
--rw-rw-rw-   0 root         (0) root         (0)    93827 2021-07-21 07:33:35.000000 chino-2.8.0/test/tests_chino.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2021-07-21 07:33:35.000000 chino-2.8.0/test.bat
--rwxrwxrwx   0 root         (0) root         (0)      211 2021-07-21 07:33:35.000000 chino-2.8.0/test.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:12:11.000000 chino-2.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      296 2021-11-22 11:12:00.000000 chino-2.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2021-11-22 11:12:00.000000 chino-2.9.0/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)      364 2021-11-22 11:12:10.000000 chino-2.9.0/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2021-11-22 11:12:00.000000 chino-2.9.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      572 2021-11-22 11:12:00.000000 chino-2.9.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     5600 2021-11-22 11:12:10.000000 chino-2.9.0/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)     7760 2021-11-22 11:12:00.000000 chino-2.9.0/INSTRUCTIONS.md
+-rw-r--r--   0 root         (0) root         (0)      801 2021-11-22 11:12:11.000000 chino-2.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      103 2021-11-22 11:12:00.000000 chino-2.9.0/PopupNotification.vbs
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2021-11-22 11:12:00.000000 chino-2.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      340 2021-11-22 11:12:00.000000 chino-2.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:12:11.000000 chino-2.9.0/chino/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2021-11-22 11:12:00.000000 chino-2.9.0/chino/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    56374 2021-11-22 11:12:00.000000 chino-2.9.0/chino/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2021-11-22 11:12:00.000000 chino-2.9.0/chino/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    27360 2021-11-22 11:12:00.000000 chino-2.9.0/chino/objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:12:11.000000 chino-2.9.0/chino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      801 2021-11-22 11:12:10.000000 chino-2.9.0/chino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      601 2021-11-22 11:12:10.000000 chino-2.9.0/chino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-22 11:12:10.000000 chino-2.9.0/chino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-22 11:12:10.000000 chino-2.9.0/chino.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2021-11-22 11:12:10.000000 chino-2.9.0/chino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2021-11-22 11:12:10.000000 chino-2.9.0/chino.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     9311 2021-11-22 11:12:00.000000 chino-2.9.0/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2021-11-22 11:12:00.000000 chino-2.9.0/docs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      260 2021-11-22 11:12:00.000000 chino-2.9.0/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2021-11-22 11:12:00.000000 chino-2.9.0/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2021-11-22 11:12:00.000000 chino-2.9.0/license.txt
+-rw-rw-rw-   0 root         (0) root         (0)       53 2021-11-22 11:12:00.000000 chino-2.9.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      558 2021-11-22 11:12:11.000000 chino-2.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2021-11-22 11:12:00.000000 chino-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:12:11.000000 chino-2.9.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2021-11-22 11:12:00.000000 chino-2.9.0/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2021-11-22 11:12:00.000000 chino-2.9.0/test/cfg.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2021-11-22 11:12:00.000000 chino-2.9.0/test/logging.conf
+-rw-rw-rw-   0 root         (0) root         (0)    15291 2021-11-22 11:12:00.000000 chino-2.9.0/test/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)       27 2021-11-22 11:12:00.000000 chino-2.9.0/test/outtest.sh
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-22 11:12:00.000000 chino-2.9.0/test/test.file
+-rwxrwxrwx   0 root         (0) root         (0)       27 2021-11-22 11:12:00.000000 chino-2.9.0/test/test.sh
+-rw-rw-rw-   0 root         (0) root         (0)    94296 2021-11-22 11:12:00.000000 chino-2.9.0/test/tests_chino.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2021-11-22 11:12:00.000000 chino-2.9.0/test.bat
+-rwxrwxrwx   0 root         (0) root         (0)      211 2021-11-22 11:12:00.000000 chino-2.9.0/test.sh
```

### Comparing `chino-2.8.0/.travis.yml` & `chino-2.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/CHANGELOG.md` & `chino-2.9.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+## [2.9.0] 2021-11-22
+- Added support for urlparam uid_type in token introspection call
+
 ## [2.8.0] 2021-07-21
 - Added support for OAuth token introspection
 
 ## [2.7.0] 2021-05-24
 - Added support for Dump UserSchema
 
 ## [2.6.1] 2021-05-17
```

### Comparing `chino-2.8.0/CONTRIBUTING.md` & `chino-2.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/ChangeLog` & `chino-2.9.0/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+2.9.0
+-----
+
+* Updated changelog before releasing
+* Updated changelog
+* Added support for urlparam uid\_type in introspect
+
 2.8.0
 -----
 
 * Updated changelog
 * Replaced local client with instance property
 * Implemented introspection call, with tests
 
@@ -240,23 +247,20 @@
 * fixing repr and str of ids
 * fixing repr and str of ids
 * fixing pagination of ids
 * fixing pagination of ids
 * style
 * style
 * updated some call endpoint
-* updated some call endpoint
 * timout
 * ignore
 * index in fields & fixes on id()
 * fixing permissions
 * fix testing
 * add some testing for the permission.. still not finished
 * fix readme
 * commiting first version with enough coverage
 * adding test. fixing to\_dict()
 * partial update, problem with to\_dict
 * no message
 * fixing problem with blob
 * enable auth for user or admin. add functiont o upload blob from file
-* adding missing methods. NEEDS TESTING
-* Update README.md
```

### Comparing `chino-2.8.0/INSTRUCTIONS.md` & `chino-2.9.0/INSTRUCTIONS.md`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/PKG-INFO` & `chino-2.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chino
-Version: 2.8.0
+Version: 2.9.0
 Summary: Wrapper for Chino.io API
 Home-page: https://www.chino.io
 Author: Chino.io
 Author-email: dev@chino.io
 License: MIT
 Project-URL: Source Code, https://gitlab.com/chinoio-public/chino-python
 Platform: UNKNOWN
```

### Comparing `chino-2.8.0/README.md` & `chino-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/chino/api.py` & `chino-2.9.0/chino/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,24 +260,24 @@
             return result
         except Exception as ex:
             # reset auth if things go wrong
             self.auth = auth
             # propagate exception
             raise ex
 
-    def introspect(self, token):
+    def introspect(self, token, **params):
         url = "auth/introspect/"
 
         # auth basic app_id:app_secret needed
         if not self.auth.client_id or not self.auth.client_secret:
             raise ValueError('client_id and/or client_secret not set')
         self.auth.set_auth_application()
 
         pars = dict(token=token)
-        result = self.apicall('POST', url, form=pars)
+        result = self.apicall('POST', url, form=pars, params=params)
 
         # restore token auth
         self.auth.set_auth_user()
         return result
 
     def current(self):
         url = "users/me"
```

### Comparing `chino-2.8.0/chino/exceptions.py` & `chino-2.9.0/chino/exceptions.py`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/chino/objects.py` & `chino-2.9.0/chino/objects.py`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/chino.egg-info/PKG-INFO` & `chino-2.9.0/chino.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chino
-Version: 2.8.0
+Version: 2.9.0
 Summary: Wrapper for Chino.io API
 Home-page: https://www.chino.io
 Author: Chino.io
 Author-email: dev@chino.io
 License: MIT
 Project-URL: Source Code, https://gitlab.com/chinoio-public/chino-python
 Platform: UNKNOWN
```

### Comparing `chino-2.8.0/chino.egg-info/SOURCES.txt` & `chino-2.9.0/chino.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 chino/api.py
 chino/exceptions.py
 chino/objects.py
 chino.egg-info/PKG-INFO
 chino.egg-info/SOURCES.txt
 chino.egg-info/dependency_links.txt
 chino.egg-info/not-zip-safe
-chino.egg-info/pbr.json
 chino.egg-info/requires.txt
 chino.egg-info/top_level.txt
 test/__init__.py
 test/cfg.py
 test/logging.conf
 test/logo.png
 test/outtest.sh
```

### Comparing `chino-2.8.0/conf.py` & `chino-2.9.0/conf.py`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/license.txt` & `chino-2.9.0/license.txt`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/setup.cfg` & `chino-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/setup.py` & `chino-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/test/logging.conf` & `chino-2.9.0/test/logging.conf`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/test/logo.png` & `chino-2.9.0/test/logo.png`

 * *Files identical despite different names*

### Comparing `chino-2.8.0/test/tests_chino.py` & `chino-2.9.0/test/tests_chino.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,25 @@
         for key, value in expected_data.items():
             self.assertIn(key, res)
             self.assertEqual(value, res[key])
 
         # we also expect the 'exp' key - we cannot know the value
         self.assertIn('exp', res)
 
+        # check that with url param ?uid_type=uuid we have the user_id (uuid)
+        # inside the username field
+        expected_data['username'] = user.user_id
+        res = self.chino_user.users.introspect(token, uid_type='uuid')
+        for key, value in expected_data.items():
+            self.assertIn(key, res)
+            self.assertEqual(value, res[key])
+
+        # we also expect the 'exp' key - we cannot know the value
+        self.assertIn('exp', res)
+
     def test_auth_public(self):
         # login
         NAME = 'test.user.new'
         EDIT = NAME + '.edited'
         self.app = self.chino.applications.create("test",
                                                   grant_type='password',
                                                   client_type='public')
@@ -1384,15 +1395,15 @@
     #         self.chino.documents.delete(document._id, force=True)
     #     self.chino.schemas.delete(self.schema, True)
     #     self.chino.repositories.delete(self.repo, True)
 
     # DEPRECATED: to be removed in v>=3.0.0
     def test_search_docs(self):
         tot = 9
-        print(self.schema)
+        # print(self.schema)
         for i in range(tot):
             res = self.chino.documents.create(self.schema,
                                               content=dict(fieldInt=123,
                                                            fieldString='test',
                                                            fieldBool=False,
                                                            fieldDate='2015-02-19',
                                                            fieldDateTime='2015-02-19T16:39:47'),
```

