# Comparing `tmp/TestingBm_123-0.0.3.tar.gz` & `tmp/TestingBm_123-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestingBm_123-0.0.3.tar", last modified: Mon May 15 10:29:25 2023, max compression
+gzip compressed data, was "TestingBm_123-0.0.4.tar", last modified: Mon May 15 10:44:54 2023, max compression
```

## Comparing `TestingBm_123-0.0.3.tar` & `TestingBm_123-0.0.4.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:25.017149 TestingBm_123-0.0.3/
--rw-rw-rw-   0        0        0      313 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:24.851164 TestingBm_123-0.0.3/.github/
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:24.896157 TestingBm_123-0.0.3/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      538 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      526 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:24.914154 TestingBm_123-0.0.3/.github/workflows/
--rw-rw-rw-   0        0        0     2125 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/workflows/docs-build.yml
--rw-rw-rw-   0        0        0     1041 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1076 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0     1032 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1586 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/workflows/ubuntu.yml
--rw-rw-rw-   0        0        0      962 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.github/workflows/windows.yml
--rw-rw-rw-   0        0        0     1310 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/.gitignore
--rw-rw-rw-   0        0        0     1092 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      129 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1129 2023-05-15 10:29:25.017149 TestingBm_123-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:24.968148 TestingBm_123-0.0.3/TestingBm_123/
--rw-rw-rw-   0        0        0      171 2023-05-15 10:26:11.000000 TestingBm_123-0.0.3/TestingBm_123/TestingBm_123.py
--rw-rw-rw-   0        0        0      172 2023-05-15 10:29:14.000000 TestingBm_123-0.0.3/TestingBm_123/__init__.py
--rw-rw-rw-   0        0        0      196 2023-05-15 09:28:57.000000 TestingBm_123-0.0.3/TestingBm_123/common.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:24.981149 TestingBm_123-0.0.3/TestingBm_123.egg-info/
--rw-rw-rw-   0        0        0     1129 2023-05-15 10:29:24.000000 TestingBm_123-0.0.3/TestingBm_123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      930 2023-05-15 10:29:24.000000 TestingBm_123-0.0.3/TestingBm_123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 10:29:24.000000 TestingBm_123-0.0.3/TestingBm_123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:48:48.000000 TestingBm_123-0.0.3/TestingBm_123.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-05-15 10:29:24.000000 TestingBm_123-0.0.3/TestingBm_123.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:25.002153 TestingBm_123-0.0.3/docs/
--rw-rw-rw-   0        0        0       60 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/TestingBm_123.md
--rw-rw-rw-   0        0        0       96 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/changelog.md
--rw-rw-rw-   0        0        0       43 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/common.md
--rw-rw-rw-   0        0        0     3314 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/contributing.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:25.004150 TestingBm_123-0.0.3/docs/examples/
--rw-rw-rw-   0        0        0      309 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/examples/intro.ipynb
--rw-rw-rw-   0        0        0        7 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/faq.md
--rw-rw-rw-   0        0        0      293 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/index.md
--rw-rw-rw-   0        0        0      617 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:25.006150 TestingBm_123-0.0.3/docs/overrides/
--rw-rw-rw-   0        0        0      285 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/overrides/main.html
--rw-rw-rw-   0        0        0       81 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/docs/usage.md
--rw-rw-rw-   0        0        0     2225 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/mkdocs.yml
--rw-rw-rw-   0        0        0        0 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       99 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/requirements_dev.txt
--rw-rw-rw-   0        0        0      371 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/requirements_docs.txt
--rw-rw-rw-   0        0        0      421 2023-05-15 10:29:25.019151 TestingBm_123-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1753 2023-05-15 10:29:19.000000 TestingBm_123-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:25.014155 TestingBm_123-0.0.3/tests/
--rw-rw-rw-   0        0        0       44 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0      438 2023-05-15 09:14:16.000000 TestingBm_123-0.0.3/tests/test_TestingBm_123.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.588286 TestingBm_123-0.0.4/
+-rw-rw-rw-   0        0        0      313 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.300181 TestingBm_123-0.0.4/.github/
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.345224 TestingBm_123-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      538 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      526 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      459 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.360293 TestingBm_123-0.0.4/.github/workflows/
+-rw-rw-rw-   0        0        0     2125 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/workflows/docs-build.yml
+-rw-rw-rw-   0        0        0     1041 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1076 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0     1032 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1586 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/workflows/ubuntu.yml
+-rw-rw-rw-   0        0        0      962 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.github/workflows/windows.yml
+-rw-rw-rw-   0        0        0     1310 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/.gitignore
+-rw-rw-rw-   0        0        0     1092 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1129 2023-05-15 10:44:54.588286 TestingBm_123-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.453288 TestingBm_123-0.0.4/TestingBm_123/
+-rw-rw-rw-   0        0        0      164 2023-05-15 10:43:25.000000 TestingBm_123-0.0.4/TestingBm_123/TestingBm_123.py
+-rw-rw-rw-   0        0        0      172 2023-05-15 10:44:13.000000 TestingBm_123-0.0.4/TestingBm_123/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-05-15 10:43:49.000000 TestingBm_123-0.0.4/TestingBm_123/common.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.508321 TestingBm_123-0.0.4/TestingBm_123.egg-info/
+-rw-rw-rw-   0        0        0     1129 2023-05-15 10:44:53.000000 TestingBm_123-0.0.4/TestingBm_123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      948 2023-05-15 10:44:54.000000 TestingBm_123-0.0.4/TestingBm_123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 10:44:53.000000 TestingBm_123-0.0.4/TestingBm_123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 09:48:48.000000 TestingBm_123-0.0.4/TestingBm_123.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-05-15 10:44:53.000000 TestingBm_123-0.0.4/TestingBm_123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.530292 TestingBm_123-0.0.4/docs/
+-rw-rw-rw-   0        0        0       60 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/TestingBm_123.md
+-rw-rw-rw-   0        0        0       96 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/changelog.md
+-rw-rw-rw-   0        0        0       43 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/common.md
+-rw-rw-rw-   0        0        0     3314 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.532287 TestingBm_123-0.0.4/docs/examples/
+-rw-rw-rw-   0        0        0      309 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/examples/intro.ipynb
+-rw-rw-rw-   0        0        0        7 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/faq.md
+-rw-rw-rw-   0        0        0      293 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/index.md
+-rw-rw-rw-   0        0        0      617 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.534291 TestingBm_123-0.0.4/docs/overrides/
+-rw-rw-rw-   0        0        0      285 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/overrides/main.html
+-rw-rw-rw-   0        0        0       81 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/docs/usage.md
+-rw-rw-rw-   0        0        0     2225 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/mkdocs.yml
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.536287 TestingBm_123-0.0.4/my_utils/
+-rw-rw-rw-   0        0        0      104 2023-05-15 10:43:20.000000 TestingBm_123-0.0.4/my_utils/utils.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       99 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/requirements_dev.txt
+-rw-rw-rw-   0        0        0      371 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/requirements_docs.txt
+-rw-rw-rw-   0        0        0      421 2023-05-15 10:44:54.592294 TestingBm_123-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1753 2023-05-15 10:43:57.000000 TestingBm_123-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:44:54.585286 TestingBm_123-0.0.4/tests/
+-rw-rw-rw-   0        0        0       44 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      438 2023-05-15 09:14:16.000000 TestingBm_123-0.0.4/tests/test_TestingBm_123.py
```

### Comparing `TestingBm_123-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `TestingBm_123-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/.github/ISSUE_TEMPLATE/config.yml` & `TestingBm_123-0.0.4/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/.github/workflows/docs-build.yml` & `TestingBm_123-0.0.4/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/.github/workflows/docs.yml` & `TestingBm_123-0.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/.github/workflows/macos.yml` & `TestingBm_123-0.0.4/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/.github/workflows/pypi.yml` & `TestingBm_123-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/.github/workflows/ubuntu.yml` & `TestingBm_123-0.0.4/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/.github/workflows/windows.yml` & `TestingBm_123-0.0.4/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/.gitignore` & `TestingBm_123-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/LICENSE` & `TestingBm_123-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/PKG-INFO` & `TestingBm_123-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestingBm_123
-Version: 0.0.3
+Version: 0.0.4
 Summary: testing bm
 Home-page: https://github.com/youssefamroo/TestingBm_123
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: TestingBm_123
 Classifier: Intended Audience :: Developers
```

### Comparing `TestingBm_123-0.0.3/TestingBm_123.egg-info/PKG-INFO` & `TestingBm_123-0.0.4/TestingBm_123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestingBm-123
-Version: 0.0.3
+Version: 0.0.4
 Summary: testing bm
 Home-page: https://github.com/youssefamroo/TestingBm_123
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: TestingBm_123
 Classifier: Intended Audience :: Developers
```

### Comparing `TestingBm_123-0.0.3/TestingBm_123.egg-info/SOURCES.txt` & `TestingBm_123-0.0.4/TestingBm_123.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,9 +32,10 @@
 docs/contributing.md
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/usage.md
 docs/examples/intro.ipynb
 docs/overrides/main.html
+my_utils/utils.py
 tests/__init__.py
 tests/test_TestingBm_123.py
```

### Comparing `TestingBm_123-0.0.3/docs/contributing.md` & `TestingBm_123-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/docs/installation.md` & `TestingBm_123-0.0.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/mkdocs.yml` & `TestingBm_123-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `TestingBm_123-0.0.3/setup.py` & `TestingBm_123-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='TestingBm_123',
     name='TestingBm_123',
     packages=find_packages(include=['TestingBm_123', 'TestingBm_123.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/youssefamroo/TestingBm_123',
-    version='0.0.3',
+    version='0.0.4',
     zip_safe=False,
 )
```

