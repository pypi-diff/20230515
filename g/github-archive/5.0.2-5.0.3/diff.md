# Comparing `tmp/github-archive-5.0.2.tar.gz` & `tmp/github-archive-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-archive-5.0.2.tar", last modified: Sat Mar 25 19:01:42 2023, max compression
+gzip compressed data, was "github-archive-5.0.3.tar", last modified: Mon May 15 15:49:47 2023, max compression
```

## Comparing `github-archive-5.0.2.tar` & `github-archive-5.0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 19:01:42.223310 github-archive-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-25 19:01:09.000000 github-archive-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-03-25 19:01:42.223310 github-archive-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-25 19:01:09.000000 github-archive-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 19:01:42.215310 github-archive-5.0.2/github_archive/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-25 19:01:09.000000 github-archive-5.0.2/github_archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-03-25 19:01:09.000000 github-archive-5.0.2/github_archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-25 19:01:09.000000 github-archive-5.0.2/github_archive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-25 19:01:09.000000 github-archive-5.0.2/github_archive/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-03-25 19:01:09.000000 github-archive-5.0.2/github_archive/gists.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-25 19:01:09.000000 github-archive-5.0.2/github_archive/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-03-25 19:01:09.000000 github-archive-5.0.2/github_archive/repos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 19:01:42.219310 github-archive-5.0.2/github_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-03-25 19:01:42.000000 github-archive-5.0.2/github_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-25 19:01:42.000000 github-archive-5.0.2/github_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 19:01:42.000000 github-archive-5.0.2/github_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-25 19:01:42.000000 github-archive-5.0.2/github_archive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-25 19:01:42.000000 github-archive-5.0.2/github_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-25 19:01:42.000000 github-archive-5.0.2/github_archive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-25 19:01:09.000000 github-archive-5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 19:01:42.223310 github-archive-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-25 19:01:09.000000 github-archive-5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 19:01:42.211310 github-archive-5.0.2/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 19:01:42.223310 github-archive-5.0.2/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 19:01:09.000000 github-archive-5.0.2/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-25 19:01:09.000000 github-archive-5.0.2/test/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-03-25 19:01:09.000000 github-archive-5.0.2/test/unit/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-25 19:01:09.000000 github-archive-5.0.2/test/unit/test_gists.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-25 19:01:09.000000 github-archive-5.0.2/test/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-03-25 19:01:09.000000 github-archive-5.0.2/test/unit/test_repos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.515304 github-archive-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 15:49:13.000000 github-archive-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-15 15:49:47.515304 github-archive-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-15 15:49:13.000000 github-archive-5.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.515304 github-archive-5.0.3/github_archive/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/gists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/repos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.515304 github-archive-5.0.3/github_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 15:49:13.000000 github-archive-5.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:49:47.515304 github-archive-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-15 15:49:13.000000 github-archive-5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.511304 github-archive-5.0.3/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.515304 github-archive-5.0.3/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/test_gists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/test_repos.py
```

### Comparing `github-archive-5.0.2/LICENSE` & `github-archive-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/PKG-INFO` & `github-archive-5.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-archive
-Version: 5.0.2
+Version: 5.0.3
 Summary: A powerful tool to concurrently clone, pull, or fork user and org repos and gists to create a GitHub archive.
 Home-page: http://github.com/justintime50/github-archive
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 A powerful tool to concurrently clone, pull, or fork user and org repos and gists to create a GitHub archive.
 
 [![Build Status](https://github.com/Justintime50/github-archive/workflows/build/badge.svg)](https://github.com/Justintime50/github-archive/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Justintime50/github-archive/badge.svg?branch=main)](https://coveralls.io/github/Justintime50/github-archive?branch=main)
 [![PyPi](https://img.shields.io/pypi/v/github-archive)](https://pypi.org/project/github-archive)
 [![Licence](https://img.shields.io/github/license/justintime50/GitHub-archive)](LICENSE)
 
-<img src="https://raw.githubusercontent.com/justintime50/assets/main/src/github-archive/showcase.png" alt="Showcase">
+![Showcase](https://raw.githubusercontent.com/justintime50/assets/main/src/github-archive/showcase.png)
 
 </div>
 
 GitHub Archive is a powerful tool to concurrently clone, pull, or fork repositories or gists from GitHub with incredible flexibility. It's the perfect tool for spinning up a new dev environment, keeping a local copy of your GitHub instance, or quickly pulling in projects from your favorite users and organizations.
 
 The power of GitHub Archive comes in its configuration. Maybe you only want to clone or pull your personal public repos or maybe you want to go all out and include private repos from you and all organizations you belong to along with your gists. GitHub Archive can do it all.
 
@@ -40,15 +40,15 @@
 
 # Install locally
 make install
 ```
 
 ## Usage
 
-```
+```text
 Usage:
     github-archive --users justintime50 --clone
 
 Options:
     -h, --help            show this help message and exit
     -t TOKEN, --token TOKEN
                             Provide your GitHub token to authenticate with the GitHub API and gain access to private repos and gists.
```

### Comparing `github-archive-5.0.2/README.md` & `github-archive-5.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A powerful tool to concurrently clone, pull, or fork user and org repos and gists to create a GitHub archive.
 
 [![Build Status](https://github.com/Justintime50/github-archive/workflows/build/badge.svg)](https://github.com/Justintime50/github-archive/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Justintime50/github-archive/badge.svg?branch=main)](https://coveralls.io/github/Justintime50/github-archive?branch=main)
 [![PyPi](https://img.shields.io/pypi/v/github-archive)](https://pypi.org/project/github-archive)
 [![Licence](https://img.shields.io/github/license/justintime50/GitHub-archive)](LICENSE)
 
-<img src="https://raw.githubusercontent.com/justintime50/assets/main/src/github-archive/showcase.png" alt="Showcase">
+![Showcase](https://raw.githubusercontent.com/justintime50/assets/main/src/github-archive/showcase.png)
 
 </div>
 
 GitHub Archive is a powerful tool to concurrently clone, pull, or fork repositories or gists from GitHub with incredible flexibility. It's the perfect tool for spinning up a new dev environment, keeping a local copy of your GitHub instance, or quickly pulling in projects from your favorite users and organizations.
 
 The power of GitHub Archive comes in its configuration. Maybe you only want to clone or pull your personal public repos or maybe you want to go all out and include private repos from you and all organizations you belong to along with your gists. GitHub Archive can do it all.
 
@@ -25,15 +25,15 @@
 
 # Install locally
 make install
 ```
 
 ## Usage
 
-```
+```text
 Usage:
     github-archive --users justintime50 --clone
 
 Options:
     -h, --help            show this help message and exit
     -t TOKEN, --token TOKEN
                             Provide your GitHub token to authenticate with the GitHub API and gain access to private repos and gists.
```

### Comparing `github-archive-5.0.2/github_archive/archive.py` & `github-archive-5.0.3/github_archive/archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         self.initialize_project()
         logger = woodchips.get(LOGGER_NAME)
         logger.info('# GitHub Archive started...')
         start_time = datetime.now()
         failed_repo_dirs = []
 
         # Personal (includes personal authenticated items)
-        if self.token and self.authenticated_user_in_users and self.users:
+        if self.token and self.users and self.authenticated_user_in_users():
             logger.info('# Making API call to GitHub for personal repos...')
             personal_repos = self.get_all_git_assets(PERSONAL_CONTEXT)
 
             if self.view:
                 logger.info('# Viewing user repos...')
                 view_repos(personal_repos)
             if self.clone:
@@ -118,16 +118,15 @@
                 _ = iterate_repos_to_archive(self, personal_repos, PULL_OPERATION)
             if self.fork:
                 # We can't fork a repo we already have, do nothing
                 pass
 
             # We remove the authenticated user from the list so that we don't double pull their
             # repos for the `users` logic.
-            if self.authenticated_username:
-                self.users.remove(self.authenticated_username)
+            self.users.remove(self.authenticated_username)
 
         # Users (can include personal non-authenticated items, excludes personal authenticated calls)
         if self.users and len(self.users) > 0:
             logger.info('# Making API calls to GitHub for user repos...')
             user_repos = self.get_all_git_assets(USER_CONTEXT)
 
             if self.view:
```

### Comparing `github-archive-5.0.2/github_archive/cli.py` & `github-archive-5.0.3/github_archive/cli.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/github_archive/constants.py` & `github-archive-5.0.3/github_archive/constants.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/github_archive/gists.py` & `github-archive-5.0.3/github_archive/gists.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/github_archive/logger.py` & `github-archive-5.0.3/github_archive/logger.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/github_archive/repos.py` & `github-archive-5.0.3/github_archive/repos.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/github_archive.egg-info/PKG-INFO` & `github-archive-5.0.3/github_archive.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-archive
-Version: 5.0.2
+Version: 5.0.3
 Summary: A powerful tool to concurrently clone, pull, or fork user and org repos and gists to create a GitHub archive.
 Home-page: http://github.com/justintime50/github-archive
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 A powerful tool to concurrently clone, pull, or fork user and org repos and gists to create a GitHub archive.
 
 [![Build Status](https://github.com/Justintime50/github-archive/workflows/build/badge.svg)](https://github.com/Justintime50/github-archive/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Justintime50/github-archive/badge.svg?branch=main)](https://coveralls.io/github/Justintime50/github-archive?branch=main)
 [![PyPi](https://img.shields.io/pypi/v/github-archive)](https://pypi.org/project/github-archive)
 [![Licence](https://img.shields.io/github/license/justintime50/GitHub-archive)](LICENSE)
 
-<img src="https://raw.githubusercontent.com/justintime50/assets/main/src/github-archive/showcase.png" alt="Showcase">
+![Showcase](https://raw.githubusercontent.com/justintime50/assets/main/src/github-archive/showcase.png)
 
 </div>
 
 GitHub Archive is a powerful tool to concurrently clone, pull, or fork repositories or gists from GitHub with incredible flexibility. It's the perfect tool for spinning up a new dev environment, keeping a local copy of your GitHub instance, or quickly pulling in projects from your favorite users and organizations.
 
 The power of GitHub Archive comes in its configuration. Maybe you only want to clone or pull your personal public repos or maybe you want to go all out and include private repos from you and all organizations you belong to along with your gists. GitHub Archive can do it all.
 
@@ -40,15 +40,15 @@
 
 # Install locally
 make install
 ```
 
 ## Usage
 
-```
+```text
 Usage:
     github-archive --users justintime50 --clone
 
 Options:
     -h, --help            show this help message and exit
     -t TOKEN, --token TOKEN
                             Provide your GitHub token to authenticate with the GitHub API and gain access to private repos and gists.
```

### Comparing `github-archive-5.0.2/github_archive.egg-info/SOURCES.txt` & `github-archive-5.0.3/github_archive.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 github_archive/__init__.py
 github_archive/archive.py
 github_archive/cli.py
 github_archive/constants.py
 github_archive/gists.py
 github_archive/logger.py
+github_archive/py.typed
 github_archive/repos.py
 github_archive.egg-info/PKG-INFO
 github_archive.egg-info/SOURCES.txt
 github_archive.egg-info/dependency_links.txt
 github_archive.egg-info/entry_points.txt
 github_archive.egg-info/requires.txt
 github_archive.egg-info/top_level.txt
```

### Comparing `github-archive-5.0.2/setup.py` & `github-archive-5.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,31 +20,30 @@
     'pytest == 7.*',
     'pytest-cov == 4.*',
     'twine == 4.*',
 ]
 
 setuptools.setup(
     name='github-archive',
-    version='5.0.2',
+    version='5.0.3',
     description=(
         'A powerful tool to concurrently clone, pull, or fork user and org repos and gists to create a GitHub archive.'
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/justintime50/github-archive',
     author='Justintime50',
     license='MIT',
     packages=setuptools.find_packages(
         exclude=[
-            'examples',
             'test',
         ]
     ),
     package_data={
-        'github-archive': [
+        'github_archive': [
             'py.typed',
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `github-archive-5.0.2/test/unit/conftest.py` & `github-archive-5.0.3/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/test/unit/test_archive.py` & `github-archive-5.0.3/test/unit/test_archive.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/test/unit/test_gists.py` & `github-archive-5.0.3/test/unit/test_gists.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.2/test/unit/test_repos.py` & `github-archive-5.0.3/test/unit/test_repos.py`

 * *Files identical despite different names*

