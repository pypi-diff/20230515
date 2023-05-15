# Comparing `tmp/xeauth-0.2.0.tar.gz` & `tmp/xeauth-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeauth-0.2.0.tar", max compression
+gzip compressed data, was "xeauth-0.2.1.tar", max compression
```

## Comparing `xeauth-0.2.0.tar` & `xeauth-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2020-12-17 17:27:26.780407 xeauth-0.2.0/LICENSE
--rw-r--r--   0        0        0      877 2020-12-17 17:27:26.757073 xeauth-0.2.0/README.rst
--rw-r--r--   0        0        0     1432 2023-05-13 20:35:24.214007 xeauth-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       36 2020-12-17 17:27:26.787073 xeauth-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1002 2023-01-19 13:38:16.595387 xeauth-0.2.0/tests/test_xeauth.py
--rw-r--r--   0        0        0      262 2023-05-13 20:35:24.214007 xeauth-0.2.0/xeauth/__init__.py
--rw-r--r--   0        0        0     2266 2023-01-19 15:33:09.669806 xeauth-0.2.0/xeauth/admin.py
--rw-r--r--   0        0        0     3925 2023-01-19 15:32:52.905554 xeauth-0.2.0/xeauth/cli.py
--rw-r--r--   0        0        0     6097 2023-05-13 20:33:32.315405 xeauth-0.2.0/xeauth/github.py
--rw-r--r--   0        0        0     2123 2023-05-13 20:33:32.315405 xeauth-0.2.0/xeauth/settings.py
--rw-r--r--   0        0        0     2463 2023-05-13 20:33:32.315405 xeauth-0.2.0/xeauth/user.py
--rw-r--r--   0        0        0     1162 2023-01-19 13:38:16.922057 xeauth-0.2.0/xeauth/utils.py
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 xeauth-0.2.0/setup.py
--rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 xeauth-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2020-12-17 17:27:26.780407 xeauth-0.2.1/LICENSE
+-rw-r--r--   0        0        0      877 2020-12-17 17:27:26.757073 xeauth-0.2.1/README.rst
+-rw-r--r--   0        0        0     1432 2023-05-15 18:19:36.575580 xeauth-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       36 2020-12-17 17:27:26.787073 xeauth-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1002 2023-01-19 13:38:16.595387 xeauth-0.2.1/tests/test_xeauth.py
+-rw-r--r--   0        0        0      262 2023-05-15 18:19:36.578913 xeauth-0.2.1/xeauth/__init__.py
+-rw-r--r--   0        0        0     2266 2023-01-19 15:33:09.669806 xeauth-0.2.1/xeauth/admin.py
+-rw-r--r--   0        0        0     3925 2023-01-19 15:32:52.905554 xeauth-0.2.1/xeauth/cli.py
+-rw-r--r--   0        0        0     8207 2023-05-15 18:19:16.008607 xeauth-0.2.1/xeauth/github.py
+-rw-r--r--   0        0        0     2123 2023-05-13 20:33:32.315405 xeauth-0.2.1/xeauth/settings.py
+-rw-r--r--   0        0        0     2045 2023-05-15 18:19:16.008607 xeauth-0.2.1/xeauth/user.py
+-rw-r--r--   0        0        0     1162 2023-01-19 13:38:16.922057 xeauth-0.2.1/xeauth/utils.py
+-rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 xeauth-0.2.1/setup.py
+-rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 xeauth-0.2.1/PKG-INFO
```

### Comparing `xeauth-0.2.0/LICENSE` & `xeauth-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.0/README.rst` & `xeauth-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.0/pyproject.toml` & `xeauth-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "xeauth"
-version = "0.2.0"
+version = "0.2.1"
 homepage = "https://github.com/jmosbacher/xeauth"
 description = "Top-level package for xeauth."
 authors = ["Yossi Mosbacher <joe.mosbacher@gmail.com>"]
 readme = "README.rst"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -20,15 +20,15 @@
     { include = "xeauth" },
     { include = "tests", format = "sdist" },
 ]
     
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
 click = "*"
-httpx = ">=0.19,<0.23"
+httpx = ">=0.19,<0.25"
 appdirs = "^1.4.4"
 param = "^1.12.0"
 gnupg = "^2.3.1"
 rich = "^13.1.0"
 
 [tool.poetry.dev-dependencies]
 bumpversion = "*"
```

### Comparing `xeauth-0.2.0/tests/test_xeauth.py` & `xeauth-0.2.1/tests/test_xeauth.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.0/xeauth/admin.py` & `xeauth-0.2.1/xeauth/admin.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.0/xeauth/cli.py` & `xeauth-0.2.1/xeauth/cli.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.0/xeauth/settings.py` & `xeauth-0.2.1/xeauth/settings.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.0/xeauth/user.py` & `xeauth-0.2.1/xeauth/user.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 
 import param
 
-from .github import GithubAuth
 from .settings import config
 
 
 class XenonUser(param.Parameterized):
     """
     XenonUser is a class that represents a user of the Xenon platform.
     """
     
     username = param.String(doc="The Xenon username of the user.")
     email = param.String(doc="The email address of the user.")
-    full_name = param.String(doc="The full name of the user.", default=None)
+    name = param.String(doc="The full name of the user.", default=None)
     github = param.String(doc="The Github username of the user.", default=None)
     cell = param.String(doc="The cell phone number of the user.", default=None)
     groups = param.List(doc="The groups the user is a member of.", default=[])
     institute = param.String(doc="The institute the user belongs to.", default=None)
     picture_url = param.String(doc="The URL of the user's picture.",  default=None)
     lngs_ldap_email = param.String(doc="The email address of the user.", default=None)
     lngs_ldap_cn = param.String(doc="The common name of the user.", default=None)
     lngs_ldap_uid = param.String(doc="The UID of the user.", default=None)
     active = param.Boolean(doc="Whether the user is active.", default=None)
     first_name = param.String(doc="The first name of the user.", default=None)
     last_name = param.String(doc="The last name of the user.", default=None)
-    github_orgs = param.List(doc="The Github organizations the user is a member of.", default=[])
-    github_teams = param.List(doc="The Github teams the user is a member of.", default=[])
+
 
     @classmethod
-    def from_github_token(cls, token):
+    def from_github_username(cls, username):
         """
-        Creates a XenonUser from a Github token.
+        Creates a XenonUser from a Github username.
 
         Args:
-            token (str): The Github token.
+            username (str): The Github username.
 
         Returns:
             XenonUser: The XenonUser.
         """
         
-        
+
         users_db = config.mongo_collection('users')
-        api = GithubAuth(oauth_token=token).api
-        github_user = api.username
-        teams = api.teams
-        orgs = api.organizations
-        data = users_db.find_one({'github': github_user})
+    
+        data = users_db.find_one({'github': username})
         if data is None:
-            raise ValueError(f'User {github_user} not found in Xenon database.')
-        data['full_name'] = data.get('name', data.get('first_name', '') + ' ' + data.get('last_name', ''))
+            raise ValueError(f'User {username} not found in Xenon database.')
+        if not data.get('name'):
+            data['name'] = data.get('first_name', '') + ' ' + data.get('last_name', '')
         data['active'] = data.get('active', False) in [True, 'True', 'true']
-        data['github_teams'] = teams
-        data['github_orgs'] = orgs
         data = {k: v for k,v in data.items() if k in cls.param.params()}
         return cls(**data)
```

### Comparing `xeauth-0.2.0/xeauth/utils.py` & `xeauth-0.2.1/xeauth/utils.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.0/setup.py` & `xeauth-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['appdirs>=1.4.4,<2.0.0',
  'click',
  'gnupg>=2.3.1,<3.0.0',
- 'httpx>=0.19,<0.23',
+ 'httpx>=0.19,<0.25',
  'param>=1.12.0,<2.0.0',
  'rich>=13.1.0,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['xeauth = xeauth.cli:main'],
  'eve_panel.auth': ['XenonAuth = xeauth.integrations.eve_panel:XenonEveAuth'],
  'panel.auth': ['xeauth = xeauth.integrations.panel_server:XenonPanelAuth']}
 
 setup_kwargs = {
     'name': 'xeauth',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Top-level package for xeauth.',
     'long_description': '======\nxeauth\n======\n\n\n.. image:: https://img.shields.io/pypi/v/xeauth.svg\n        :target: https://pypi.python.org/pypi/xeauth\n\n.. image:: https://img.shields.io/travis/jmosbacher/xeauth.svg\n        :target: https://travis-ci.com/jmosbacher/xeauth\n\n.. image:: https://readthedocs.org/projects/xeauth/badge/?version=latest\n        :target: https://xeauth.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n\n\n\n\nAuthentication client for the Xenon edark matter experiment.\n\n\n* Free software: MIT\n* Documentation: https://xeauth.readthedocs.io.\n\n\nFeatures\n--------\n\n* TODO\n\nCredits\n-------\n\nThis package was created with Cookiecutter_ and the `briggySmalls/cookiecutter-pypackage`_ project template.\n\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`briggySmalls/cookiecutter-pypackage`: https://github.com/briggySmalls/cookiecutter-pypackage\n',
     'author': 'Yossi Mosbacher',
     'author_email': 'joe.mosbacher@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jmosbacher/xeauth',
```

### Comparing `xeauth-0.2.0/PKG-INFO` & `xeauth-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeauth
-Version: 0.2.0
+Version: 0.2.1
 Summary: Top-level package for xeauth.
 Home-page: https://github.com/jmosbacher/xeauth
 License: MIT
 Author: Yossi Mosbacher
 Author-email: joe.mosbacher@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click
 Requires-Dist: gnupg (>=2.3.1,<3.0.0)
-Requires-Dist: httpx (>=0.19,<0.23)
+Requires-Dist: httpx (>=0.19,<0.25)
 Requires-Dist: param (>=1.12.0,<2.0.0)
 Requires-Dist: rich (>=13.1.0,<14.0.0)
 Description-Content-Type: text/x-rst
 
 ======
 xeauth
 ======
```

