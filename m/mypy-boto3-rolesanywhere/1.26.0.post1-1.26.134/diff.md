# Comparing `tmp/mypy-boto3-rolesanywhere-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-rolesanywhere-1.26.134.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rolesanywhere-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:55 2022, max compression
+gzip compressed data, was "mypy-boto3-rolesanywhere-1.26.134.tar", last modified: Mon May 15 20:22:58 2023, max compression
```

## Comparing `mypy-boto3-rolesanywhere-1.26.0.post1.tar` & `mypy-boto3-rolesanywhere-1.26.134.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.056845 mypy-boto3-rolesanywhere-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14604 2022-11-01 21:43:55.048845 mypy-boto3-rolesanywhere-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13136 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.036845 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18966 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    18929 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7896 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7894 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5078 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5072 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    12331 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12318 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.048845 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14604 2022-11-01 21:43:54.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-11-01 21:43:54.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:54.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:54.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:54.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:54.000000 mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:55.056845 mypy-boto3-rolesanywhere-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-11-01 21:40:09.000000 mypy-boto3-rolesanywhere-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-05-15 20:22:42.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/setup.py
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/LICENSE` & `mypy-boto3-rolesanywhere-1.26.134/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/PKG-INFO` & `mypy-boto3-rolesanywhere-1.26.134/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.134
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.26.134 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
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
 
 <a id="mypy-boto3-rolesanywhere"></a>
 
 # mypy-boto3-rolesanywhere
 
 [![PyPI - mypy-boto3-rolesanywhere](https://img.shields.io/pypi/v/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.26.134](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,14 +310,16 @@
 
 ```python
 from mypy_boto3_rolesanywhere.literals import (
     ListCrlsPaginatorName,
     ListProfilesPaginatorName,
     ListSubjectsPaginatorName,
     ListTrustAnchorsPaginatorName,
+    NotificationChannelType,
+    NotificationEventType,
     TrustAnchorTypeType,
     IAMRolesAnywhereServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -332,51 +335,58 @@
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
+    NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
     PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    NotificationSettingDetailTypeDef,
+    NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
     ListRequestListCrlsPaginateTypeDef,
     ListRequestListProfilesPaginateTypeDef,
     ListRequestListSubjectsPaginateTypeDef,
     ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
+    ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
+    PutNotificationSettingsResponseTypeDef,
+    ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
@@ -384,42 +394,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/README.md` & `mypy-boto3-rolesanywhere-1.26.134/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rolesanywhere"></a>
 
 # mypy-boto3-rolesanywhere
 
 [![PyPI - mypy-boto3-rolesanywhere](https://img.shields.io/pypi/v/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.26.134](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -278,14 +278,16 @@
 
 ```python
 from mypy_boto3_rolesanywhere.literals import (
     ListCrlsPaginatorName,
     ListProfilesPaginatorName,
     ListSubjectsPaginatorName,
     ListTrustAnchorsPaginatorName,
+    NotificationChannelType,
+    NotificationEventType,
     TrustAnchorTypeType,
     IAMRolesAnywhereServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -301,51 +303,58 @@
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
+    NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
     PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    NotificationSettingDetailTypeDef,
+    NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
     ListRequestListCrlsPaginateTypeDef,
     ListRequestListProfilesPaginateTypeDef,
     ListRequestListSubjectsPaginateTypeDef,
     ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
+    ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
+    PutNotificationSettingsResponseTypeDef,
+    ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
@@ -353,42 +362,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/__init__.py` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/__init__.pyi` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/__main__.py` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAMRolesAnywhere 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.IAMRolesAnywhere 1.26.134\nVersion:         1.26.134\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.134")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/client.py` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 from .type_defs import (
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSubjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustAnchorsResponseTypeDef,
+    NotificationSettingKeyTypeDef,
+    NotificationSettingTypeDef,
     ProfileDetailResponseTypeDef,
+    PutNotificationSettingsResponseTypeDef,
+    ResetNotificationSettingsResponseTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     TagTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -106,30 +110,33 @@
         enabled: bool = ...,
         managedPolicyArns: Sequence[str] = ...,
         requireInstanceProperties: bool = ...,
         sessionPolicy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> ProfileDetailResponseTypeDef:
         """
-        Creates a profile.
+        Creates a *profile*, a list of the roles that Roles Anywhere service is trusted
+        to assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#create_profile)
         """
 
     def create_trust_anchor(
         self,
         *,
         name: str,
         source: SourceTypeDef,
         enabled: bool = ...,
+        notificationSettings: Sequence[NotificationSettingTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> TrustAnchorDetailResponseTypeDef:
         """
-        Creates a trust anchor.
+        Creates a trust anchor to establish trust between IAM Roles Anywhere and your
+        certificate authority (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_trust_anchor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#create_trust_anchor)
         """
 
     def delete_crl(self, *, crlId: str) -> CrlDetailResponseTypeDef:
         """
@@ -185,17 +192,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.enable_crl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#enable_crl)
         """
 
     def enable_profile(self, *, profileId: str) -> ProfileDetailResponseTypeDef:
         """
-        Enables the roles in a profile to receive session credentials in
-        [CreateSession](https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html)_
-        .
+        Enables temporary credential requests for a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.enable_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#enable_profile)
         """
 
     def enable_trust_anchor(self, *, trustAnchorId: str) -> TrustAnchorDetailResponseTypeDef:
         """
@@ -233,15 +238,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.get_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#get_profile)
         """
 
     def get_subject(self, *, subjectId: str) -> SubjectDetailResponseTypeDef:
         """
-        Gets a Subject.
+        Gets a *subject*, which associates a certificate identity with authentication
+        attempts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.get_subject)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#get_subject)
         """
 
     def get_trust_anchor(self, *, trustAnchorId: str) -> TrustAnchorDetailResponseTypeDef:
         """
@@ -265,15 +271,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.import_crl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#import_crl)
         """
 
     def list_crls(self, *, nextToken: str = ..., pageSize: int = ...) -> ListCrlsResponseTypeDef:
         """
-        Lists all Crls in the authenticated account and Amazon Web Services Region.
+        Lists all certificate revocation lists (CRL) in the authenticated account and
+        Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.list_crls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#list_crls)
         """
 
     def list_profiles(
         self, *, nextToken: str = ..., pageSize: int = ...
@@ -310,14 +317,37 @@
         Lists the trust anchors in the authenticated account and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.list_trust_anchors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#list_trust_anchors)
         """
 
+    def put_notification_settings(
+        self, *, notificationSettings: Sequence[NotificationSettingTypeDef], trustAnchorId: str
+    ) -> PutNotificationSettingsResponseTypeDef:
+        """
+        Attaches a list of *notification settings* to a trust anchor.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.put_notification_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#put_notification_settings)
+        """
+
+    def reset_notification_settings(
+        self,
+        *,
+        notificationSettingKeys: Sequence[NotificationSettingKeyTypeDef],
+        trustAnchorId: str
+    ) -> ResetNotificationSettingsResponseTypeDef:
+        """
+        Resets the *custom notification setting* to IAM Roles Anywhere default setting.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.reset_notification_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#reset_notification_settings)
+        """
+
     def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Attaches tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#tag_resource)
         """
@@ -351,26 +381,26 @@
         durationSeconds: int = ...,
         managedPolicyArns: Sequence[str] = ...,
         name: str = ...,
         roleArns: Sequence[str] = ...,
         sessionPolicy: str = ...
     ) -> ProfileDetailResponseTypeDef:
         """
-        Updates the profile.
+        Updates a *profile*, a list of the roles that IAM Roles Anywhere service is
+        trusted to assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#update_profile)
         """
 
     def update_trust_anchor(
         self, *, trustAnchorId: str, name: str = ..., source: SourceTypeDef = ...
     ) -> TrustAnchorDetailResponseTypeDef:
         """
-        Updates the trust anchor.You establish trust between IAM Roles Anywhere and your
-        certificate authority (CA) by configuring a trust anchor.
+        Updates a trust anchor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_trust_anchor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#update_trust_anchor)
         """
 
     @overload
     def get_paginator(self, operation_name: Literal["list_crls"]) -> ListCrlsPaginator:
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/client.pyi` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 from .type_defs import (
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSubjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustAnchorsResponseTypeDef,
+    NotificationSettingKeyTypeDef,
+    NotificationSettingTypeDef,
     ProfileDetailResponseTypeDef,
+    PutNotificationSettingsResponseTypeDef,
+    ResetNotificationSettingsResponseTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     TagTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -99,29 +103,32 @@
         enabled: bool = ...,
         managedPolicyArns: Sequence[str] = ...,
         requireInstanceProperties: bool = ...,
         sessionPolicy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> ProfileDetailResponseTypeDef:
         """
-        Creates a profile.
+        Creates a *profile*, a list of the roles that Roles Anywhere service is trusted
+        to assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#create_profile)
         """
     def create_trust_anchor(
         self,
         *,
         name: str,
         source: SourceTypeDef,
         enabled: bool = ...,
+        notificationSettings: Sequence[NotificationSettingTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> TrustAnchorDetailResponseTypeDef:
         """
-        Creates a trust anchor.
+        Creates a trust anchor to establish trust between IAM Roles Anywhere and your
+        certificate authority (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_trust_anchor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#create_trust_anchor)
         """
     def delete_crl(self, *, crlId: str) -> CrlDetailResponseTypeDef:
         """
         Deletes a certificate revocation list (CRL).
@@ -169,17 +176,15 @@
         Enables a certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.enable_crl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#enable_crl)
         """
     def enable_profile(self, *, profileId: str) -> ProfileDetailResponseTypeDef:
         """
-        Enables the roles in a profile to receive session credentials in
-        [CreateSession](https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html)_
-        .
+        Enables temporary credential requests for a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.enable_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#enable_profile)
         """
     def enable_trust_anchor(self, *, trustAnchorId: str) -> TrustAnchorDetailResponseTypeDef:
         """
         Enables a trust anchor.
@@ -212,15 +217,16 @@
         Gets a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.get_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#get_profile)
         """
     def get_subject(self, *, subjectId: str) -> SubjectDetailResponseTypeDef:
         """
-        Gets a Subject.
+        Gets a *subject*, which associates a certificate identity with authentication
+        attempts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.get_subject)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#get_subject)
         """
     def get_trust_anchor(self, *, trustAnchorId: str) -> TrustAnchorDetailResponseTypeDef:
         """
         Gets a trust anchor.
@@ -241,15 +247,16 @@
         Imports the certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.import_crl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#import_crl)
         """
     def list_crls(self, *, nextToken: str = ..., pageSize: int = ...) -> ListCrlsResponseTypeDef:
         """
-        Lists all Crls in the authenticated account and Amazon Web Services Region.
+        Lists all certificate revocation lists (CRL) in the authenticated account and
+        Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.list_crls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#list_crls)
         """
     def list_profiles(
         self, *, nextToken: str = ..., pageSize: int = ...
     ) -> ListProfilesResponseTypeDef:
@@ -281,14 +288,35 @@
         """
         Lists the trust anchors in the authenticated account and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.list_trust_anchors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#list_trust_anchors)
         """
+    def put_notification_settings(
+        self, *, notificationSettings: Sequence[NotificationSettingTypeDef], trustAnchorId: str
+    ) -> PutNotificationSettingsResponseTypeDef:
+        """
+        Attaches a list of *notification settings* to a trust anchor.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.put_notification_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#put_notification_settings)
+        """
+    def reset_notification_settings(
+        self,
+        *,
+        notificationSettingKeys: Sequence[NotificationSettingKeyTypeDef],
+        trustAnchorId: str
+    ) -> ResetNotificationSettingsResponseTypeDef:
+        """
+        Resets the *custom notification setting* to IAM Roles Anywhere default setting.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.reset_notification_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#reset_notification_settings)
+        """
     def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Attaches tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#tag_resource)
         """
@@ -319,25 +347,25 @@
         durationSeconds: int = ...,
         managedPolicyArns: Sequence[str] = ...,
         name: str = ...,
         roleArns: Sequence[str] = ...,
         sessionPolicy: str = ...
     ) -> ProfileDetailResponseTypeDef:
         """
-        Updates the profile.
+        Updates a *profile*, a list of the roles that IAM Roles Anywhere service is
+        trusted to assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#update_profile)
         """
     def update_trust_anchor(
         self, *, trustAnchorId: str, name: str = ..., source: SourceTypeDef = ...
     ) -> TrustAnchorDetailResponseTypeDef:
         """
-        Updates the trust anchor.You establish trust between IAM Roles Anywhere and your
-        certificate authority (CA) by configuring a trust anchor.
+        Updates a trust anchor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_trust_anchor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#update_trust_anchor)
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_crls"]) -> ListCrlsPaginator:
         """
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/literals.py` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/literals.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -14,33 +14,35 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListCrlsPaginatorName",
     "ListProfilesPaginatorName",
     "ListSubjectsPaginatorName",
     "ListTrustAnchorsPaginatorName",
+    "NotificationChannelType",
+    "NotificationEventType",
     "TrustAnchorTypeType",
     "IAMRolesAnywhereServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListCrlsPaginatorName = Literal["list_crls"]
 ListProfilesPaginatorName = Literal["list_profiles"]
 ListSubjectsPaginatorName = Literal["list_subjects"]
 ListTrustAnchorsPaginatorName = Literal["list_trust_anchors"]
+NotificationChannelType = Literal["ALL"]
+NotificationEventType = Literal["CA_CERTIFICATE_EXPIRY", "END_ENTITY_CERTIFICATE_EXPIRY"]
 TrustAnchorTypeType = Literal["AWS_ACM_PCA", "CERTIFICATE_BUNDLE", "SELF_SIGNED_REPOSITORY"]
 IAMRolesAnywhereServiceName = Literal["rolesanywhere"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -59,14 +61,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -76,27 +79,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
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
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -125,14 +132,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -177,51 +185,57 @@
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
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
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
@@ -253,28 +267,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -283,14 +302,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -301,55 +321,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
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
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/literals.pyi` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,31 +14,37 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListCrlsPaginatorName",
     "ListProfilesPaginatorName",
     "ListSubjectsPaginatorName",
     "ListTrustAnchorsPaginatorName",
+    "NotificationChannelType",
+    "NotificationEventType",
     "TrustAnchorTypeType",
     "IAMRolesAnywhereServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ListCrlsPaginatorName = Literal["list_crls"]
 ListProfilesPaginatorName = Literal["list_profiles"]
 ListSubjectsPaginatorName = Literal["list_subjects"]
 ListTrustAnchorsPaginatorName = Literal["list_trust_anchors"]
+NotificationChannelType = Literal["ALL"]
+NotificationEventType = Literal["CA_CERTIFICATE_EXPIRY", "END_ENTITY_CERTIFICATE_EXPIRY"]
 TrustAnchorTypeType = Literal["AWS_ACM_PCA", "CERTIFICATE_BUNDLE", "SELF_SIGNED_REPOSITORY"]
 IAMRolesAnywhereServiceName = Literal["rolesanywhere"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -57,14 +63,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -74,27 +81,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
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
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -123,14 +134,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -175,51 +187,57 @@
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
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
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
@@ -251,28 +269,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -281,14 +304,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -299,55 +323,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
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
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/paginator.py` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/paginator.pyi` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/type_defs.py` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,72 +13,106 @@
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
-from .literals import TrustAnchorTypeType
+from .literals import NotificationEventType, TrustAnchorTypeType
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
+    "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
     "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
     "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "NotificationSettingDetailTypeDef",
+    "NotificationSettingKeyTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
     "ListRequestListCrlsPaginateTypeDef",
     "ListRequestListProfilesPaginateTypeDef",
     "ListRequestListSubjectsPaginateTypeDef",
     "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
+    "ResetNotificationSettingsRequestRequestTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
+    "PutNotificationSettingsResponseTypeDef",
+    "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+_RequiredNotificationSettingTypeDef = TypedDict(
+    "_RequiredNotificationSettingTypeDef",
+    {
+        "enabled": bool,
+        "event": NotificationEventType,
+    },
+)
+_OptionalNotificationSettingTypeDef = TypedDict(
+    "_OptionalNotificationSettingTypeDef",
+    {
+        "channel": Literal["ALL"],
+        "threshold": int,
+    },
+    total=False,
+)
+
+
+class NotificationSettingTypeDef(
+    _RequiredNotificationSettingTypeDef, _OptionalNotificationSettingTypeDef
+):
+    pass
+
+
 CredentialSummaryTypeDef = TypedDict(
     "CredentialSummaryTypeDef",
     {
         "enabled": bool,
         "failed": bool,
         "issuer": str,
         "seenAt": datetime,
@@ -179,14 +213,59 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+_RequiredNotificationSettingDetailTypeDef = TypedDict(
+    "_RequiredNotificationSettingDetailTypeDef",
+    {
+        "enabled": bool,
+        "event": NotificationEventType,
+    },
+)
+_OptionalNotificationSettingDetailTypeDef = TypedDict(
+    "_OptionalNotificationSettingDetailTypeDef",
+    {
+        "channel": Literal["ALL"],
+        "configuredBy": str,
+        "threshold": int,
+    },
+    total=False,
+)
+
+
+class NotificationSettingDetailTypeDef(
+    _RequiredNotificationSettingDetailTypeDef, _OptionalNotificationSettingDetailTypeDef
+):
+    pass
+
+
+_RequiredNotificationSettingKeyTypeDef = TypedDict(
+    "_RequiredNotificationSettingKeyTypeDef",
+    {
+        "event": NotificationEventType,
+    },
+)
+_OptionalNotificationSettingKeyTypeDef = TypedDict(
+    "_OptionalNotificationSettingKeyTypeDef",
+    {
+        "channel": Literal["ALL"],
+    },
+    total=False,
+)
+
+
+class NotificationSettingKeyTypeDef(
+    _RequiredNotificationSettingKeyTypeDef, _OptionalNotificationSettingKeyTypeDef
+):
+    pass
+
+
 ScalarCrlRequestRequestTypeDef = TypedDict(
     "ScalarCrlRequestRequestTypeDef",
     {
         "crlId": str,
     },
 )
 
@@ -330,14 +409,22 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+PutNotificationSettingsRequestRequestTypeDef = TypedDict(
+    "PutNotificationSettingsRequestRequestTypeDef",
+    {
+        "notificationSettings": Sequence[NotificationSettingTypeDef],
+        "trustAnchorId": str,
+    },
+)
+
 CrlDetailResponseTypeDef = TypedDict(
     "CrlDetailResponseTypeDef",
     {
         "crl": CrlDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -433,14 +520,22 @@
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
+    "ResetNotificationSettingsRequestRequestTypeDef",
+    {
+        "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
+        "trustAnchorId": str,
+    },
+)
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "sourceData": SourceDataTypeDef,
         "sourceType": TrustAnchorTypeType,
     },
     total=False,
@@ -461,14 +556,15 @@
         "source": SourceTypeDef,
     },
 )
 _OptionalCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrustAnchorRequestRequestTypeDef",
     {
         "enabled": bool,
+        "notificationSettings": Sequence[NotificationSettingTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateTrustAnchorRequestRequestTypeDef(
@@ -479,14 +575,15 @@
 
 TrustAnchorDetailTypeDef = TypedDict(
     "TrustAnchorDetailTypeDef",
     {
         "createdAt": datetime,
         "enabled": bool,
         "name": str,
+        "notificationSettings": List[NotificationSettingDetailTypeDef],
         "source": SourceTypeDef,
         "trustAnchorArn": str,
         "trustAnchorId": str,
         "updatedAt": datetime,
     },
     total=False,
 )
@@ -518,14 +615,30 @@
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutNotificationSettingsResponseTypeDef = TypedDict(
+    "PutNotificationSettingsResponseTypeDef",
+    {
+        "trustAnchor": TrustAnchorDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResetNotificationSettingsResponseTypeDef = TypedDict(
+    "ResetNotificationSettingsResponseTypeDef",
+    {
+        "trustAnchor": TrustAnchorDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TrustAnchorDetailResponseTypeDef = TypedDict(
     "TrustAnchorDetailResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere/type_defs.pyi` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -13,71 +13,103 @@
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
-from .literals import TrustAnchorTypeType
+from .literals import NotificationEventType, TrustAnchorTypeType
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
+    "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
     "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
     "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "NotificationSettingDetailTypeDef",
+    "NotificationSettingKeyTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
     "ListRequestListCrlsPaginateTypeDef",
     "ListRequestListProfilesPaginateTypeDef",
     "ListRequestListSubjectsPaginateTypeDef",
     "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
+    "ResetNotificationSettingsRequestRequestTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
+    "PutNotificationSettingsResponseTypeDef",
+    "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+_RequiredNotificationSettingTypeDef = TypedDict(
+    "_RequiredNotificationSettingTypeDef",
+    {
+        "enabled": bool,
+        "event": NotificationEventType,
+    },
+)
+_OptionalNotificationSettingTypeDef = TypedDict(
+    "_OptionalNotificationSettingTypeDef",
+    {
+        "channel": Literal["ALL"],
+        "threshold": int,
+    },
+    total=False,
+)
+
+class NotificationSettingTypeDef(
+    _RequiredNotificationSettingTypeDef, _OptionalNotificationSettingTypeDef
+):
+    pass
+
 CredentialSummaryTypeDef = TypedDict(
     "CredentialSummaryTypeDef",
     {
         "enabled": bool,
         "failed": bool,
         "issuer": str,
         "seenAt": datetime,
@@ -178,14 +210,55 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+_RequiredNotificationSettingDetailTypeDef = TypedDict(
+    "_RequiredNotificationSettingDetailTypeDef",
+    {
+        "enabled": bool,
+        "event": NotificationEventType,
+    },
+)
+_OptionalNotificationSettingDetailTypeDef = TypedDict(
+    "_OptionalNotificationSettingDetailTypeDef",
+    {
+        "channel": Literal["ALL"],
+        "configuredBy": str,
+        "threshold": int,
+    },
+    total=False,
+)
+
+class NotificationSettingDetailTypeDef(
+    _RequiredNotificationSettingDetailTypeDef, _OptionalNotificationSettingDetailTypeDef
+):
+    pass
+
+_RequiredNotificationSettingKeyTypeDef = TypedDict(
+    "_RequiredNotificationSettingKeyTypeDef",
+    {
+        "event": NotificationEventType,
+    },
+)
+_OptionalNotificationSettingKeyTypeDef = TypedDict(
+    "_OptionalNotificationSettingKeyTypeDef",
+    {
+        "channel": Literal["ALL"],
+    },
+    total=False,
+)
+
+class NotificationSettingKeyTypeDef(
+    _RequiredNotificationSettingKeyTypeDef, _OptionalNotificationSettingKeyTypeDef
+):
+    pass
+
 ScalarCrlRequestRequestTypeDef = TypedDict(
     "ScalarCrlRequestRequestTypeDef",
     {
         "crlId": str,
     },
 )
 
@@ -321,14 +394,22 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+PutNotificationSettingsRequestRequestTypeDef = TypedDict(
+    "PutNotificationSettingsRequestRequestTypeDef",
+    {
+        "notificationSettings": Sequence[NotificationSettingTypeDef],
+        "trustAnchorId": str,
+    },
+)
+
 CrlDetailResponseTypeDef = TypedDict(
     "CrlDetailResponseTypeDef",
     {
         "crl": CrlDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -424,14 +505,22 @@
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
+    "ResetNotificationSettingsRequestRequestTypeDef",
+    {
+        "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
+        "trustAnchorId": str,
+    },
+)
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "sourceData": SourceDataTypeDef,
         "sourceType": TrustAnchorTypeType,
     },
     total=False,
@@ -452,14 +541,15 @@
         "source": SourceTypeDef,
     },
 )
 _OptionalCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrustAnchorRequestRequestTypeDef",
     {
         "enabled": bool,
+        "notificationSettings": Sequence[NotificationSettingTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateTrustAnchorRequestRequestTypeDef(
     _RequiredCreateTrustAnchorRequestRequestTypeDef, _OptionalCreateTrustAnchorRequestRequestTypeDef
@@ -468,14 +558,15 @@
 
 TrustAnchorDetailTypeDef = TypedDict(
     "TrustAnchorDetailTypeDef",
     {
         "createdAt": datetime,
         "enabled": bool,
         "name": str,
+        "notificationSettings": List[NotificationSettingDetailTypeDef],
         "source": SourceTypeDef,
         "trustAnchorArn": str,
         "trustAnchorId": str,
         "updatedAt": datetime,
     },
     total=False,
 )
@@ -505,14 +596,30 @@
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutNotificationSettingsResponseTypeDef = TypedDict(
+    "PutNotificationSettingsResponseTypeDef",
+    {
+        "trustAnchor": TrustAnchorDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResetNotificationSettingsResponseTypeDef = TypedDict(
+    "ResetNotificationSettingsResponseTypeDef",
+    {
+        "trustAnchor": TrustAnchorDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TrustAnchorDetailResponseTypeDef = TypedDict(
     "TrustAnchorDetailResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/PKG-INFO` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.134
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.26.134 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
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
 
 <a id="mypy-boto3-rolesanywhere"></a>
 
 # mypy-boto3-rolesanywhere
 
 [![PyPI - mypy-boto3-rolesanywhere](https://img.shields.io/pypi/v/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.26.134](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,14 +310,16 @@
 
 ```python
 from mypy_boto3_rolesanywhere.literals import (
     ListCrlsPaginatorName,
     ListProfilesPaginatorName,
     ListSubjectsPaginatorName,
     ListTrustAnchorsPaginatorName,
+    NotificationChannelType,
+    NotificationEventType,
     TrustAnchorTypeType,
     IAMRolesAnywhereServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -332,51 +335,58 @@
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
+    NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
     PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    NotificationSettingDetailTypeDef,
+    NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
     ListRequestListCrlsPaginateTypeDef,
     ListRequestListProfilesPaginateTypeDef,
     ListRequestListSubjectsPaginateTypeDef,
     ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
+    ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
+    PutNotificationSettingsResponseTypeDef,
+    ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
@@ -384,42 +394,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt` & `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.0.post1/setup.py` & `mypy-boto3-rolesanywhere-1.26.134/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-rolesanywhere.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rolesanywhere",
-    version="1.26.0.post1",
+    version="1.26.134",
     packages=["mypy_boto3_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAMRolesAnywhere 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.IAMRolesAnywhere 1.26.134 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords="boto3 rolesanywhere type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_rolesanywhere": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_rolesanywhere": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

