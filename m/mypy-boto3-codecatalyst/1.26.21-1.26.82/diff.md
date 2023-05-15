# Comparing `tmp/mypy-boto3-codecatalyst-1.26.21.tar.gz` & `tmp/mypy-boto3-codecatalyst-1.26.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecatalyst-1.26.21.tar", last modified: Thu Dec  1 20:25:43 2022, max compression
+gzip compressed data, was "mypy-boto3-codecatalyst-1.26.82.tar", last modified: Wed Mar  1 20:27:29 2023, max compression
```

## Comparing `mypy-boto3-codecatalyst-1.26.21.tar` & `mypy-boto3-codecatalyst-1.26.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.978805 mypy-boto3-codecatalyst-1.26.21/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    17082 2022-12-01 20:25:43.978805 mypy-boto3-codecatalyst-1.26.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    15625 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.978805 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1925 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      928 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22245 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    22207 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8811 2022-12-01 20:25:24.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     8809 2022-12-01 20:25:24.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     9026 2022-12-01 20:25:24.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     9017 2022-12-01 20:25:24.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    31844 2022-12-01 20:25:24.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    31785 2022-12-01 20:25:24.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.978805 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17082 2022-12-01 20:25:43.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      775 2022-12-01 20:25:43.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:25:43.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:25:43.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-01 20:25:43.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2022-12-01 20:25:43.000000 mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 20:25:43.978805 mypy-boto3-codecatalyst-1.26.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2022-12-01 20:25:23.000000 mypy-boto3-codecatalyst-1.26.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22862 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22823 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32475 2023-03-01 20:27:18.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-03-01 20:27:18.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/setup.py
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/LICENSE` & `mypy-boto3-codecatalyst-1.26.82/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.26.21/PKG-INFO` & `mypy-boto3-codecatalyst-1.26.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.26.21
-Summary: Type annotations for boto3.CodeCatalyst 1.26.21 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.82
+Summary: Type annotations for boto3.CodeCatalyst 1.26.82 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,26 +389,28 @@
     ListSourceRepositoriesItemTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
+    StopDevEnvironmentSessionRequestRequestTypeDef,
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     ListAccessTokensResponseTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/README.md` & `mypy-boto3-codecatalyst-1.26.82/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,26 +357,28 @@
     ListSourceRepositoriesItemTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
+    StopDevEnvironmentSessionRequestRequestTypeDef,
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     ListAccessTokensResponseTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/__init__.py` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/__init__.pyi` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/__main__.py` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCatalyst 1.26.21\nVersion:         1.26.21\nBuilder"
-        " version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.CodeCatalyst 1.26.82\nVersion:         1.26.82\nBuilder"
+        " version: 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.21")
+    print("1.26.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/client.py` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     ListSpacesResponseTypeDef,
     PersistentStorageConfigurationTypeDef,
     ProjectListFilterTypeDef,
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionResponseTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -400,14 +401,24 @@
         """
         Pauses a specified Dev Environment and places it in a non-running state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.stop_dev_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#stop_dev_environment)
         """
 
+    def stop_dev_environment_session(
+        self, *, spaceName: str, projectName: str, id: str, sessionId: str
+    ) -> StopDevEnvironmentSessionResponseTypeDef:
+        """
+        Stops a session for a specified Dev Environment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.stop_dev_environment_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#stop_dev_environment_session)
+        """
+
     def update_dev_environment(
         self,
         *,
         spaceName: str,
         projectName: str,
         id: str,
         alias: str = ...,
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/client.pyi` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     ListSpacesResponseTypeDef,
     PersistentStorageConfigurationTypeDef,
     ProjectListFilterTypeDef,
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionResponseTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -370,14 +371,23 @@
     ) -> StopDevEnvironmentResponseTypeDef:
         """
         Pauses a specified Dev Environment and places it in a non-running state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.stop_dev_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#stop_dev_environment)
         """
+    def stop_dev_environment_session(
+        self, *, spaceName: str, projectName: str, id: str, sessionId: str
+    ) -> StopDevEnvironmentSessionResponseTypeDef:
+        """
+        Stops a session for a specified Dev Environment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.stop_dev_environment_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#stop_dev_environment_session)
+        """
     def update_dev_environment(
         self,
         *,
         spaceName: str,
         projectName: str,
         id: str,
         alias: str = ...,
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/literals.py` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,24 +99,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -202,14 +204,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -224,30 +227,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -333,14 +339,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -374,14 +381,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/literals.pyi` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -97,24 +97,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -200,14 +202,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -222,30 +225,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -331,14 +337,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -372,14 +379,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/paginator.py` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/paginator.pyi` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/type_defs.py` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,26 +69,28 @@
     "ListSourceRepositoriesItemTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
     "CreateAccessTokenResponseTypeDef",
     "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchResponseTypeDef",
     "DeleteDevEnvironmentResponseTypeDef",
     "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsResponseTypeDef",
     "GetSpaceResponseTypeDef",
     "GetSubscriptionResponseTypeDef",
     "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentSessionResponseTypeDef",
     "VerifySessionResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
@@ -654,20 +656,31 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+    },
+)
+
 CreateAccessTokenResponseTypeDef = TypedDict(
     "CreateAccessTokenResponseTypeDef",
     {
         "secret": str,
         "name": str,
         "expiresTime": datetime,
+        "accessTokenId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDevEnvironmentResponseTypeDef = TypedDict(
     "CreateDevEnvironmentResponseTypeDef",
     {
@@ -776,14 +789,25 @@
         "projectName": str,
         "id": str,
         "status": DevEnvironmentStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StopDevEnvironmentSessionResponseTypeDef = TypedDict(
+    "StopDevEnvironmentSessionResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst/type_defs.pyi` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,26 +68,28 @@
     "ListSourceRepositoriesItemTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
     "CreateAccessTokenResponseTypeDef",
     "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchResponseTypeDef",
     "DeleteDevEnvironmentResponseTypeDef",
     "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsResponseTypeDef",
     "GetSpaceResponseTypeDef",
     "GetSubscriptionResponseTypeDef",
     "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentSessionResponseTypeDef",
     "VerifySessionResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
@@ -621,20 +623,31 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+    },
+)
+
 CreateAccessTokenResponseTypeDef = TypedDict(
     "CreateAccessTokenResponseTypeDef",
     {
         "secret": str,
         "name": str,
         "expiresTime": datetime,
+        "accessTokenId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDevEnvironmentResponseTypeDef = TypedDict(
     "CreateDevEnvironmentResponseTypeDef",
     {
@@ -743,14 +756,25 @@
         "projectName": str,
         "id": str,
         "status": DevEnvironmentStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StopDevEnvironmentSessionResponseTypeDef = TypedDict(
+    "StopDevEnvironmentSessionResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/PKG-INFO` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.26.21
-Summary: Type annotations for boto3.CodeCatalyst 1.26.21 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.82
+Summary: Type annotations for boto3.CodeCatalyst 1.26.82 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,26 +389,28 @@
     ListSourceRepositoriesItemTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
+    StopDevEnvironmentSessionRequestRequestTypeDef,
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     ListAccessTokensResponseTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.26.21/mypy_boto3_codecatalyst.egg-info/SOURCES.txt` & `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.26.21/setup.py` & `mypy-boto3-codecatalyst-1.26.82/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-codecatalyst",
-    version="1.26.21",
+    version="1.26.82",
     packages=["mypy_boto3_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCatalyst 1.26.21 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.CodeCatalyst 1.26.82 service generated with mypy-boto3-builder"
+        " 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 codecatalyst type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codecatalyst": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codecatalyst": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

