# Comparing `tmp/bm_utilities-0.0.6.tar.gz` & `tmp/bm_utilities-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.0.6.tar", last modified: Tue Apr 25 12:06:00 2023, max compression
+gzip compressed data, was "bm_utilities-0.0.7.tar", last modified: Mon May 15 12:30:26 2023, max compression
```

## Comparing `bm_utilities-0.0.6.tar` & `bm_utilities-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 12:06:00.044293 bm_utilities-0.0.6/
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-04-25 12:06:00.045290 bm_utilities-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 12:06:00.027288 bm_utilities-0.0.6/bm_utilities/
--rw-rw-rw-   0        0        0      136 2023-04-25 12:05:41.000000 bm_utilities-0.0.6/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     5732 2023-04-25 12:04:54.000000 bm_utilities-0.0.6/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.6/bm_utilities/common.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:06:00.042293 bm_utilities-0.0.6/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-04-25 12:05:59.000000 bm_utilities-0.0.6/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-04-25 12:05:59.000000 bm_utilities-0.0.6/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 12:05:59.000000 bm_utilities-0.0.6/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-25 12:05:59.000000 bm_utilities-0.0.6/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-25 12:05:59.000000 bm_utilities-0.0.6/bm_utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0      420 2023-04-25 12:06:00.047290 bm_utilities-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-04-25 12:05:28.000000 bm_utilities-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.643794 bm_utilities-0.0.7/
+-rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.491794 bm_utilities-0.0.7/.github/
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.530241 bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.544733 bm_utilities-0.0.7/.github/workflows/
+-rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/docs-build.yml
+-rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/ubuntu.yml
+-rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/windows.yml
+-rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.gitignore
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-05-15 12:30:26.644796 bm_utilities-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.595713 bm_utilities-0.0.7/bm_utilities/
+-rw-rw-rw-   0        0        0     4605 2023-05-15 12:10:28.000000 bm_utilities-0.0.7/bm_utilities/Address_finder.py
+-rw-rw-rw-   0        0        0      136 2023-05-15 12:30:20.000000 bm_utilities-0.0.7/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0      231 2023-05-15 12:28:50.000000 bm_utilities-0.0.7/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/bm_utilities/common.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.609534 bm_utilities-0.0.7/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-05-15 12:30:26.000000 bm_utilities-0.0.7/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2023-05-15 12:30:26.000000 bm_utilities-0.0.7/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 12:30:26.000000 bm_utilities-0.0.7/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-25 12:05:59.000000 bm_utilities-0.0.7/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-15 12:30:26.000000 bm_utilities-0.0.7/bm_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.630797 bm_utilities-0.0.7/docs/
+-rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/bm_utilities.md
+-rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/changelog.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/common.md
+-rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.632796 bm_utilities-0.0.7/docs/examples/
+-rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/examples/intro.ipynb
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/faq.md
+-rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/index.md
+-rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.634805 bm_utilities-0.0.7/docs/overrides/
+-rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/overrides/main.html
+-rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/usage.md
+-rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/mkdocs.yml
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.0.7/requirements_dev.txt
+-rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/requirements_docs.txt
+-rw-rw-rw-   0        0        0      420 2023-05-15 12:30:26.645795 bm_utilities-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-05-15 12:30:14.000000 bm_utilities-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.640798 bm_utilities-0.0.7/tests/
+-rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/tests/test_bm_utilities.py
```

### Comparing `bm_utilities-0.0.6/LICENSE` & `bm_utilities-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.6/PKG-INFO` & `bm_utilities-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.6/README.md` & `bm_utilities-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.6/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.0.7/bm_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.6/setup.py` & `bm_utilities-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='bm_utilities',
     name='bm_utilities',
     packages=find_packages(include=['bm_utilities', 'bm_utilities.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Youssefamroo/bm_utilities',
-    version='0.0.6',
+    version='0.0.7',
     zip_safe=False,
 )
```

