# Comparing `tmp/evacuator-1.0.2.tar.gz` & `tmp/evacuator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evacuator-1.0.2.tar", last modified: Mon Feb 27 11:42:43 2023, max compression
+gzip compressed data, was "evacuator-1.0.3.tar", last modified: Mon May 15 14:57:41 2023, max compression
```

## Comparing `evacuator-1.0.2.tar` & `evacuator-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:42:43.427599 evacuator-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-27 11:42:36.000000 evacuator-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-27 11:42:43.427599 evacuator-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-02-27 11:42:36.000000 evacuator-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:42:43.423599 evacuator-1.0.2/evacuator/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-27 11:42:36.000000 evacuator-1.0.2/evacuator/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-27 11:42:36.000000 evacuator-1.0.2/evacuator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-02-27 11:42:36.000000 evacuator-1.0.2/evacuator/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-27 11:42:36.000000 evacuator-1.0.2/evacuator/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-02-27 11:42:36.000000 evacuator-1.0.2/evacuator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:42:43.427599 evacuator-1.0.2/evacuator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-27 11:42:43.000000 evacuator-1.0.2/evacuator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-27 11:42:43.000000 evacuator-1.0.2/evacuator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 11:42:43.000000 evacuator-1.0.2/evacuator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 11:42:43.000000 evacuator-1.0.2/evacuator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-27 11:42:43.000000 evacuator-1.0.2/evacuator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-27 11:42:36.000000 evacuator-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-02-27 11:42:43.427599 evacuator-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-02-27 11:42:36.000000 evacuator-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:57:41.109541 evacuator-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-15 14:57:36.000000 evacuator-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-15 14:57:36.000000 evacuator-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-15 14:57:41.109541 evacuator-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-15 14:57:36.000000 evacuator-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:57:41.109541 evacuator-1.0.3/evacuator/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 14:57:36.000000 evacuator-1.0.3/evacuator/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-15 14:57:36.000000 evacuator-1.0.3/evacuator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-15 14:57:36.000000 evacuator-1.0.3/evacuator/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-15 14:57:36.000000 evacuator-1.0.3/evacuator/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:57:36.000000 evacuator-1.0.3/evacuator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-15 14:57:36.000000 evacuator-1.0.3/evacuator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:57:41.109541 evacuator-1.0.3/evacuator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-15 14:57:41.000000 evacuator-1.0.3/evacuator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 14:57:41.000000 evacuator-1.0.3/evacuator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:57:41.000000 evacuator-1.0.3/evacuator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:57:41.000000 evacuator-1.0.3/evacuator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 14:57:41.000000 evacuator-1.0.3/evacuator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-15 14:57:36.000000 evacuator-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-15 14:57:41.113541 evacuator-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-15 14:57:36.000000 evacuator-1.0.3/setup.py
```

### Comparing `evacuator-1.0.2/PKG-INFO` & `evacuator-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: evacuator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Catch an exception and exit with an exit code
 Home-page: https://github.com/MobileTeleSystems/evacuator
 Author: ONEtools Team
 Author-email: onetools@mts.ru
 License: Apache License 2.0
-Project-URL: Documentation, https://evacuator.readthedocs.io/en/stable/
+Project-URL: Documentation, https://evacuator.readthedocs.io
 Project-URL: Source, https://github.com/MobileTeleSystems/evacuator
 Project-URL: CI/CD, https://github.com/MobileTeleSystems/evacuator/actions
 Project-URL: Tracker, https://github.com/MobileTeleSystems/evacuator/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 
 .. title
 
 Evacuator
 =========
 
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/evacuator
 .. |PyPI| image:: https://img.shields.io/pypi/v/evacuator
     :target: https://pypi.org/project/evacuator/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/evacuator.svg
     :target: https://github.com/MobileTeleSystems/evacuator/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/evacuator.svg
     :target: https://badge.fury.io/py/evacuator
-.. |ReadTheDocs| image:: https://img.shields.io/readthedocs/evacuator.svg
-    :target: https://evacuator.readthedocs.io
 .. |Build Status| image:: https://github.com/MobileTeleSystems/evacuator/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/evacuator/actions
 .. |Documentation| image:: https://readthedocs.org/projects/evacuator/badge/?version=stable
     :target: https://evacuator.readthedocs.io/en/stable/
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/evacuator/branch/develop/graph/badge.svg?token=CM6AQWY65P
     :target: https://codecov.io/gh/MobileTeleSystems/evacuator
```

### Comparing `evacuator-1.0.2/README.rst` & `evacuator-1.0.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 Evacuator
 =========
 
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/evacuator
 .. |PyPI| image:: https://img.shields.io/pypi/v/evacuator
     :target: https://pypi.org/project/evacuator/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/evacuator.svg
     :target: https://github.com/MobileTeleSystems/evacuator/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/evacuator.svg
     :target: https://badge.fury.io/py/evacuator
-.. |ReadTheDocs| image:: https://img.shields.io/readthedocs/evacuator.svg
-    :target: https://evacuator.readthedocs.io
 .. |Build Status| image:: https://github.com/MobileTeleSystems/evacuator/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/evacuator/actions
 .. |Documentation| image:: https://readthedocs.org/projects/evacuator/badge/?version=stable
     :target: https://evacuator.readthedocs.io/en/stable/
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/evacuator/branch/develop/graph/badge.svg?token=CM6AQWY65P
     :target: https://codecov.io/gh/MobileTeleSystems/evacuator
```

### Comparing `evacuator-1.0.2/evacuator/__init__.py` & `evacuator-1.0.3/evacuator/__init__.py`

 * *Files identical despite different names*

### Comparing `evacuator-1.0.2/evacuator/core.py` & `evacuator-1.0.3/evacuator/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,9 +119,9 @@
 
     def __exit__(self, exc_type, exc_value, _traceback):
         if exc_type is not None and issubclass(exc_type, self.exception):
             self._handle()
 
     def _handle(self) -> NoReturn:
         logger.exception("Caught an exception")
-        logger.exception("Die with exit code %s", self.exit_code, exc_info=False)  # noqa: WPS323
+        logger.exception("Die with exit code %s", self.exit_code, exc_info=False)
         sys.exit(self.exit_code)
```

### Comparing `evacuator-1.0.2/evacuator/exception.py` & `evacuator-1.0.3/evacuator/exception.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 
 class NeedEvacuation(RuntimeError):
-    pass  # noqa: WPS604 WPS420
+    pass
```

### Comparing `evacuator-1.0.2/evacuator/version.py` & `evacuator-1.0.3/evacuator/version.py`

 * *Files identical despite different names*

### Comparing `evacuator-1.0.2/evacuator.egg-info/PKG-INFO` & `evacuator-1.0.3/evacuator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: evacuator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Catch an exception and exit with an exit code
 Home-page: https://github.com/MobileTeleSystems/evacuator
 Author: ONEtools Team
 Author-email: onetools@mts.ru
 License: Apache License 2.0
-Project-URL: Documentation, https://evacuator.readthedocs.io/en/stable/
+Project-URL: Documentation, https://evacuator.readthedocs.io
 Project-URL: Source, https://github.com/MobileTeleSystems/evacuator
 Project-URL: CI/CD, https://github.com/MobileTeleSystems/evacuator/actions
 Project-URL: Tracker, https://github.com/MobileTeleSystems/evacuator/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 
 .. title
 
 Evacuator
 =========
 
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/evacuator
 .. |PyPI| image:: https://img.shields.io/pypi/v/evacuator
     :target: https://pypi.org/project/evacuator/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/evacuator.svg
     :target: https://github.com/MobileTeleSystems/evacuator/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/evacuator.svg
     :target: https://badge.fury.io/py/evacuator
-.. |ReadTheDocs| image:: https://img.shields.io/readthedocs/evacuator.svg
-    :target: https://evacuator.readthedocs.io
 .. |Build Status| image:: https://github.com/MobileTeleSystems/evacuator/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/evacuator/actions
 .. |Documentation| image:: https://readthedocs.org/projects/evacuator/badge/?version=stable
     :target: https://evacuator.readthedocs.io/en/stable/
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/evacuator/branch/develop/graph/badge.svg?token=CM6AQWY65P
     :target: https://codecov.io/gh/MobileTeleSystems/evacuator
```

### Comparing `evacuator-1.0.2/setup.py` & `evacuator-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def get_version():
     if os.getenv("GITHUB_REF_TYPE", "branch") == "tag":
         return os.environ["GITHUB_REF_NAME"]
 
     version_file = here / "evacuator" / "VERSION"
-    version = version_file.read_text().strip()  # noqa: WPS410
+    version = version_file.read_text().strip()
 
     build_num = os.environ.get("GITHUB_RUN_ID", "0")
     branch_name = os.environ.get("GITHUB_REF_NAME", "")
 
     if not branch_name:
         return version
 
@@ -28,15 +28,15 @@
     version=get_version(),
     description="Catch an exception and exit with an exit code",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="Apache License 2.0",
     license_files=("LICENSE.txt",),
     url="https://github.com/MobileTeleSystems/evacuator",
-    packages=find_packages(),
+    packages=find_packages(exclude=["docs", "docs.*", "tests", "tests.*"]),
     author="ONEtools Team",
     author_email="onetools@mts.ru",
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
@@ -45,13 +45,13 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
     project_urls={
-        "Documentation": "https://evacuator.readthedocs.io/en/stable/",
+        "Documentation": "https://evacuator.readthedocs.io",
         "Source": "https://github.com/MobileTeleSystems/evacuator",
         "CI/CD": "https://github.com/MobileTeleSystems/evacuator/actions",
         "Tracker": "https://github.com/MobileTeleSystems/evacuator/issues",
     },
 )
```

