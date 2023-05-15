# Comparing `tmp/pycallrail-0.9.0.0.tar.gz` & `tmp/pycallrail-0.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycallrail-0.9.0.0.tar", last modified: Thu May  4 14:35:18 2023, max compression
+gzip compressed data, was "pycallrail-0.9.0.1.tar", last modified: Mon May 15 07:19:38 2023, max compression
```

## Comparing `pycallrail-0.9.0.0.tar` & `pycallrail-0.9.0.1.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:35:18.647394 pycallrail-0.9.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-04 14:35:18.647394 pycallrail-0.9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:35:18.639393 pycallrail-0.9.0.0/pycallrail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:35:18.643394 pycallrail-0.9.0.0/pycallrail/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/pycallrail/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/pycallrail/objects/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/pycallrail/objects/calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/pycallrail/objects/companies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/pycallrail/objects/form_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/pycallrail/objects/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/pycallrail/objects/textmessages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:35:18.643394 pycallrail-0.9.0.0/pycallrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-04 14:35:18.000000 pycallrail-0.9.0.0/pycallrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-04 14:35:18.000000 pycallrail-0.9.0.0/pycallrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:35:18.000000 pycallrail-0.9.0.0/pycallrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-04 14:35:18.000000 pycallrail-0.9.0.0/pycallrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 14:35:18.000000 pycallrail-0.9.0.0/pycallrail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:35:18.647394 pycallrail-0.9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:35:18.647394 pycallrail-0.9.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    17983 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_companies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_formsubmissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-05-04 14:35:04.000000 pycallrail-0.9.0.0/tests/test_textmessages.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.863575 pycallrail-0.9.0.1/
+-rw-rw-rw-   0        0        0     1100 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/LICENSE
+-rw-rw-rw-   0        0        0       61 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3263 2023-05-15 07:19:38.862495 pycallrail-0.9.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.807327 pycallrail-0.9.0.1/pycallrail/
+-rw-rw-rw-   0        0        0     1039 2023-05-15 07:19:22.000000 pycallrail-0.9.0.1/pycallrail/__init__.py
+-rw-rw-rw-   0        0        0      251 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/base.py
+-rw-rw-rw-   0        0        0    12252 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/callrail.py
+-rw-rw-rw-   0        0        0      148 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/errors.py
+-rw-rw-rw-   0        0        0      550 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/helpers.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/mixins.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.841345 pycallrail-0.9.0.1/pycallrail/objects/
+-rw-rw-rw-   0        0        0        0 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/__init__.py
+-rw-rw-rw-   0        0        0    18844 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/accounts.py
+-rw-rw-rw-   0        0        0     7114 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/calls.py
+-rw-rw-rw-   0        0        0     3504 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/companies.py
+-rw-rw-rw-   0        0        0     4271 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/form_submissions.py
+-rw-rw-rw-   0        0        0     3487 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/tags.py
+-rw-rw-rw-   0        0        0     3844 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/textmessages.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.827322 pycallrail-0.9.0.1/pycallrail.egg-info/
+-rw-rw-rw-   0        0        0     3263 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      281 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       75 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 07:19:38.863575 pycallrail-0.9.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2667 2023-05-15 07:12:37.000000 pycallrail-0.9.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.861097 pycallrail-0.9.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-21 03:45:56.000000 pycallrail-0.9.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-05-04 01:12:26.000000 pycallrail-0.9.0.1/tests/cfg.py
+-rw-rw-rw-   0        0        0    18215 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_account.py
+-rw-rw-rw-   0        0        0     8894 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_apiclient.py
+-rw-rw-rw-   0        0        0    18436 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_call.py
+-rw-rw-rw-   0        0        0     5238 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_companies.py
+-rw-rw-rw-   0        0        0    14850 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_formsubmissions.py
+-rw-rw-rw-   0        0        0     2785 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     3121 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_integration.py
+-rw-rw-rw-   0        0        0     4983 2023-05-04 14:18:46.000000 pycallrail-0.9.0.1/tests/test_tags.py
+-rw-rw-rw-   0        0        0     8376 2023-05-04 14:18:46.000000 pycallrail-0.9.0.1/tests/test_textmessages.py
```

### Comparing `pycallrail-0.9.0.0/LICENSE` & `pycallrail-0.9.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
```

### Comparing `pycallrail-0.9.0.0/PKG-INFO` & `pycallrail-0.9.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-Metadata-Version: 2.1
-Name: pycallrail
-Version: 0.9.0.0
-Summary: An unofficial Python wrapper for the CallRail API
-Home-page: https://github.com/predictive-data-lab/pycallrail
-Author: Engineering @ Predictive Data Lab
-License: MIT
-Project-URL: Documentation, https://pycallrail.readthedocs.io/en/latest/
-Project-URL: Issue Tracker, https://github.com/predictive-data-lab/pycallrail/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Communications
-Requires-Python: >=3.8.0
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
-pycallrail
-==========
-
-.. image:: https://img.shields.io/pypi/v/pycallrail.svg
-   :target: https://pypi.python.org/pypi/pycallrail
-   :alt: PyPI version info
-.. image:: https://img.shields.io/pypi/pyversions/pycallrail.svg
-   :target: https://pypi.python.org/pypi/pycallrail.py
-   :alt: PyPI supported Python versions
-.. image:: https://github.com/predictive-data-lab/pycallrail/actions/workflows/test.yml/badge.svg
-   :target: https://github.com/predictive-data-lab/pycallrail/commits/main
-   :alt: GitHub Actions build status
-.. image:: https://codecov.io/gh/predictive-data-lab/pycallrail/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/predictive-data-lab/pycallrail
-   :alt: Codecov coverage report
-.. image:: https://readthedocs.org/projects/pycallrail/badge/?version=latest
-   :target: https://pycallrail.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-
-Python wrapper for the CallRail API.
-
-Description
------------
-
-This library provides a Python intefrace for interacting with the Callrail API.
-It allows for CRUD operations on objects and resources within your CallRail account and to integrate
-with your own applications.
-
-Installation
-------------
-Install from PyPI using pip, a package manager for Python.
-
-.. code:: sh
-
-   # Linux/macOS
-   python3 -m pip install pycallrail
-
-   # Windows
-   py -3 -m pip install pycallrail
-
-Requirements & Dependencies
----------------------------
-- Python 3.6+
-- requests
-- ujson
-- python-dateutil
-- typeguard
-
-Usage
------
-
-.. code:: py
-
-   import pycallrail.callrail as clrl
-
-   # init the api client
-
-   api = clrl.CallRail('your_api_key')
-
-   # list accounts associated with your api key
-   accounts = api.list_accounts(# optional kwargs, more info on supported kwargs at endpoint docs)
-
-   # list calls associated with your account
-   calls = accounts[0].list_calls(# optional kwargs, more info on supported kwargs at endpoint docs)
-
-   print(calls[0].id) # prints the id of the first call in the list
-
-   # >>> 123456789
-
-Links & Contact
----------------
-
-- `Documentation <https://pycallrail.readthedocs.io/en/latest/>`_
-- `Questions <mailto:engineering@predictivedatalab.com>`_
+Metadata-Version: 2.1
+Name: pycallrail
+Version: 0.9.0.1
+Summary: An unofficial Python wrapper for the CallRail API
+Home-page: https://github.com/predictive-data-lab/pycallrail
+Author: Engineering @ Predictive Data Lab
+License: MIT
+Project-URL: Documentation, https://pycallrail.readthedocs.io/en/latest/
+Project-URL: Issue Tracker, https://github.com/predictive-data-lab/pycallrail/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Communications
+Requires-Python: >=3.8.0
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+pycallrail
+==========
+
+.. image:: https://img.shields.io/pypi/v/pycallrail.svg
+   :target: https://pypi.python.org/pypi/pycallrail
+   :alt: PyPI version info
+.. image:: https://img.shields.io/pypi/pyversions/pycallrail.svg
+   :target: https://pypi.python.org/pypi/pycallrail.py
+   :alt: PyPI supported Python versions
+.. image:: https://github.com/predictive-data-lab/pycallrail/actions/workflows/test.yml/badge.svg
+   :target: https://github.com/predictive-data-lab/pycallrail/commits/main
+   :alt: GitHub Actions build status
+.. image:: https://codecov.io/gh/predictive-data-lab/pycallrail/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/predictive-data-lab/pycallrail
+   :alt: Codecov coverage report
+.. image:: https://readthedocs.org/projects/pycallrail/badge/?version=latest
+   :target: https://pycallrail.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+Python wrapper for the CallRail API.
+
+Description
+-----------
+
+This library provides a Python intefrace for interacting with the Callrail API.
+It allows for CRUD operations on objects and resources within your CallRail account and to integrate
+with your own applications.
+
+Installation
+------------
+Install from PyPI using pip, a package manager for Python.
+
+.. code:: sh
+
+   # Linux/macOS
+   python3 -m pip install pycallrail
+
+   # Windows
+   py -3 -m pip install pycallrail
+
+Requirements & Dependencies
+---------------------------
+- Python 3.6+
+- requests
+- ujson
+- python-dateutil
+- typeguard
+
+Usage
+-----
+
+.. code:: py
+
+   import pycallrail.callrail as clrl
+
+   # init the api client
+
+   api = clrl.CallRail('your_api_key')
+
+   # list accounts associated with your api key
+   accounts = api.list_accounts(# optional kwargs, more info on supported kwargs at endpoint docs)
+
+   # list calls associated with your account
+   calls = accounts[0].list_calls(# optional kwargs, more info on supported kwargs at endpoint docs)
+
+   print(calls[0].id) # prints the id of the first call in the list
+
+   # >>> 123456789
+
+Links & Contact
+---------------
+
+- `Documentation <https://pycallrail.readthedocs.io/en/latest/>`_
+- `Questions <mailto:engineering@predictivedatalab.com>`_
```

### Comparing `pycallrail-0.9.0.0/README.rst` & `pycallrail-0.9.0.1/README.rst`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-pycallrail
-==========
-
-.. image:: https://img.shields.io/pypi/v/pycallrail.svg
-   :target: https://pypi.python.org/pypi/pycallrail
-   :alt: PyPI version info
-.. image:: https://img.shields.io/pypi/pyversions/pycallrail.svg
-   :target: https://pypi.python.org/pypi/pycallrail.py
-   :alt: PyPI supported Python versions
-.. image:: https://github.com/predictive-data-lab/pycallrail/actions/workflows/test.yml/badge.svg
-   :target: https://github.com/predictive-data-lab/pycallrail/commits/main
-   :alt: GitHub Actions build status
-.. image:: https://codecov.io/gh/predictive-data-lab/pycallrail/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/predictive-data-lab/pycallrail
-   :alt: Codecov coverage report
-.. image:: https://readthedocs.org/projects/pycallrail/badge/?version=latest
-   :target: https://pycallrail.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-
-Python wrapper for the CallRail API.
-
-Description
------------
-
-This library provides a Python intefrace for interacting with the Callrail API.
-It allows for CRUD operations on objects and resources within your CallRail account and to integrate
-with your own applications.
-
-Installation
-------------
-Install from PyPI using pip, a package manager for Python.
-
-.. code:: sh
-
-   # Linux/macOS
-   python3 -m pip install pycallrail
-
-   # Windows
-   py -3 -m pip install pycallrail
-
-Requirements & Dependencies
----------------------------
-- Python 3.6+
-- requests
-- ujson
-- python-dateutil
-- typeguard
-
-Usage
------
-
-.. code:: py
-
-   import pycallrail.callrail as clrl
-
-   # init the api client
-
-   api = clrl.CallRail('your_api_key')
-
-   # list accounts associated with your api key
-   accounts = api.list_accounts(# optional kwargs, more info on supported kwargs at endpoint docs)
-
-   # list calls associated with your account
-   calls = accounts[0].list_calls(# optional kwargs, more info on supported kwargs at endpoint docs)
-
-   print(calls[0].id) # prints the id of the first call in the list
-
-   # >>> 123456789
-
-Links & Contact
----------------
-
-- `Documentation <https://pycallrail.readthedocs.io/en/latest/>`_
+pycallrail
+==========
+
+.. image:: https://img.shields.io/pypi/v/pycallrail.svg
+   :target: https://pypi.python.org/pypi/pycallrail
+   :alt: PyPI version info
+.. image:: https://img.shields.io/pypi/pyversions/pycallrail.svg
+   :target: https://pypi.python.org/pypi/pycallrail.py
+   :alt: PyPI supported Python versions
+.. image:: https://github.com/predictive-data-lab/pycallrail/actions/workflows/test.yml/badge.svg
+   :target: https://github.com/predictive-data-lab/pycallrail/commits/main
+   :alt: GitHub Actions build status
+.. image:: https://codecov.io/gh/predictive-data-lab/pycallrail/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/predictive-data-lab/pycallrail
+   :alt: Codecov coverage report
+.. image:: https://readthedocs.org/projects/pycallrail/badge/?version=latest
+   :target: https://pycallrail.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+Python wrapper for the CallRail API.
+
+Description
+-----------
+
+This library provides a Python intefrace for interacting with the Callrail API.
+It allows for CRUD operations on objects and resources within your CallRail account and to integrate
+with your own applications.
+
+Installation
+------------
+Install from PyPI using pip, a package manager for Python.
+
+.. code:: sh
+
+   # Linux/macOS
+   python3 -m pip install pycallrail
+
+   # Windows
+   py -3 -m pip install pycallrail
+
+Requirements & Dependencies
+---------------------------
+- Python 3.6+
+- requests
+- ujson
+- python-dateutil
+- typeguard
+
+Usage
+-----
+
+.. code:: py
+
+   import pycallrail.callrail as clrl
+
+   # init the api client
+
+   api = clrl.CallRail('your_api_key')
+
+   # list accounts associated with your api key
+   accounts = api.list_accounts(# optional kwargs, more info on supported kwargs at endpoint docs)
+
+   # list calls associated with your account
+   calls = accounts[0].list_calls(# optional kwargs, more info on supported kwargs at endpoint docs)
+
+   print(calls[0].id) # prints the id of the first call in the list
+
+   # >>> 123456789
+
+Links & Contact
+---------------
+
+- `Documentation <https://pycallrail.readthedocs.io/en/latest/>`_
 - `Questions <mailto:engineering@predictivedatalab.com>`_
```

### Comparing `pycallrail-0.9.0.0/pycallrail/objects/accounts.py` & `pycallrail-0.9.0.1/pycallrail/objects/accounts.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,588 +1,588 @@
-from __future__ import annotations
-
-import datetime as dt
-from dateutil import parser as dateparser
-import pycallrail.base as base
-import pycallrail.callrail as crl
-import pycallrail.objects.calls as calls
-import pycallrail.objects.tags as tags
-import pycallrail.objects.companies as companies
-import pycallrail.objects.form_submissions as forms
-import pycallrail.objects.textmessages as messages
-import typing
-import logging
-
-class Account(base.CallRailBase):
-    """
-    Represents a CallRail Account. Class should preferably not be instantiated directly.
-
-    More information: https://apidocs.callrail.com/#accounts
-    """
-
-    id: str
-    name: str
-    outbound_recording_enabled: bool
-    hipaa_account: bool
-
-    # Optional User Requested Fields
-    numeric_id: typing.Optional[int]
-
-    def __init__(
-            self,
-            api_client: crl.CallRail,
-            id: str,
-            name: str,
-            outbound_recording_enabled: bool,
-            hipaa_account: bool,
-            numeric_id: typing.Optional[int] = None
-    ) -> None:
-        super(Account, self).__init__()
-        self.api_client: crl.CallRail = api_client
-        self.id = id
-        self.name = name
-        self.outbound_recording_enabled = outbound_recording_enabled
-        self.hipaa_account = hipaa_account
-
-        if numeric_id:
-            self.numeric_id = numeric_id
-
-    @classmethod
-    def from_json(
-        cls,
-        api_client: crl.CallRail,
-        json_data: typing.Dict[str, typing.Any]
-    ) -> Account:
-        """
-        Deserialize JSON data into an Account object.
-        
-        :api_client: CallRail API object
-        :json_data: JSON data
-        """
-
-        account = Account(
-            api_client=api_client,
-            id=json_data['id'],
-            name=json_data['name'],
-            outbound_recording_enabled=json_data['outbound_recording_enabled'],
-            hipaa_account=json_data['hipaa_account']
-        )
-
-        if 'numeric_id' in json_data:
-            account.numeric_id = json_data['numeric_id']
-
-        return account
-    
-    #########################
-    # Calls
-    #########################
-
-    def list_calls(
-            self,
-            **kwargs
-        ) -> typing.Union[typing.List[calls.Call], None]:
-        """
-        List all calls associated with this account.
-
-        Keyword args acceptable include: Pagination Type, Sorting, Filtering, Field Selection, and Searching.
-        Defaults to relative pagination.
-        
-        More info: https://apidocs.callrail.com/#listing-all-calls
-        """
-
-        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
-
-        sorting = kwargs.get('sorting', None)
-        filtering = kwargs.get('filtering', None)
-        searching = kwargs.get('searching', None)
-        fields = kwargs.get('fields', None)
-
-        params = {}
-
-        if sorting:
-            params['sorting'] = sorting
-        if filtering:
-            params['filtering'] = filtering
-        if searching:
-            params['searching'] = searching
-        if fields:
-            params['fields'] = fields
-
-        if calls_response := typing.cast(
-            typing.Union[typing.List[typing.Dict[str, typing.Any]], None],
-            self.api_client._get(
-                endpoint=f'a/{self.id}',
-                response_data_key='calls',
-                path='calls.json',
-                params=params or None,
-                pagination_type=pagination_type,
-            ),
-        ):
-            return [calls.Call.from_json(self.api_client, self.id, call) for call in calls_response]
-        else:
-            return None
-
-    def get_call(
-        self,
-        call_id: str,
-        fields: typing.Optional[typing.MutableMapping[str, typing.Union[str, typing.Any]]] = None
-    ) -> calls.Call:
-        """
-        Retrieve a single call by ID.
-        
-        Field selection is supported by this method.
-        
-        More info: https://apidocs.callrail.com/#retrieving-a-single-call
-        """
-
-        if fields:
-            data = self.api_client._get(
-                endpoint=f'a/{self.id}',
-                path=f'calls/{call_id}.json',
-                params=fields
-            )
-        else:
-            data = self.api_client._get(
-                endpoint=f'a/{self.id}',
-                path=f'calls/{call_id}.json'
-            )
-
-        return calls.Call.from_json(
-            self.api_client, 
-            self.id, 
-            typing.cast(typing.Dict[str, typing.Any], data)
-        )
-    
-    def create_call(
-            self,
-            caller_id: int,
-            customer_phone_number: str,
-            business_phone_number: str,
-            recording_enabled: typing.Optional[bool] = None,
-            outbound_greeting_recording_url: typing.Optional[str] = None,
-            outbound_greeting_text: typing.Optional[str] = None,
-            agent_id: typing.Optional[str] = None
-    ) -> calls.Call:
-        """
-        Create a new call.
-        
-        This method is rate limited. There is no functionality to currently check for rate limits. Be careful!
-        More info: https://apidocs.callrail.com/#creating-an-outbound-phone-call
-        """
-
-        logging.warning('This method is rate limited. There is no functionality to currently check for rate limits. Be careful!')
-
-        body = {
-            'caller_id': caller_id,
-            'customer_phone_number': customer_phone_number,
-            'business_phone_number': business_phone_number
-        }
-
-        
-
-        if recording_enabled:
-            body['recording_enabled'] = recording_enabled
-        if outbound_greeting_recording_url:
-            body['outbound_greeting_recording_url'] = outbound_greeting_recording_url
-        if outbound_greeting_text:
-            body['outbound_greeting_text'] = outbound_greeting_text
-        if agent_id:
-            body['agent_id'] = agent_id
-        
-        data = self.api_client._post(
-            endpoint=f'a/{self.id}',
-            path='calls.json',
-            data=body
-        )
-
-        return calls.Call.from_json(
-            self.api_client,
-            self.id,
-            typing.cast(typing.Dict[str, typing.Any], data)
-        )
-    
-    #########################
-    # Tags
-    #########################
-
-    def list_tags(
-            self,
-            **kwargs
-    ) -> typing.Union[typing.List[tags.Tag], None]:
-        """
-        This endpoint returns a paginated array of tags within the target account.
-
-        More info: https://apidocs.callrail.com/#retrieving-all-tags
-        """
-
-        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
-
-        sorting = kwargs.get('sorting', None)
-
-        params = {}
-
-        if sorting:
-            params['sorting'] = sorting
-
-        if tags_response := typing.cast(
-            typing.List[typing.Dict[str, typing.Any]],
-            self.api_client._get(
-                endpoint=f'a/{self.id}',
-                response_data_key='tags',
-                path='tags.json',
-                params=params or None,
-                pagination_type=pagination_type,
-            )
-        ):
-            return [tags.Tag.from_json(self.api_client, self.id, tag) for tag in tags_response]
-
-        else:
-            return None
-        
-    def create_tag(
-            self,
-            name: str,
-            company_id: typing.Optional[str] = None,
-            color: typing.Optional[str] = None,
-            tag_level: typing.Optional[str] = None
-    ) -> tags.Tag:
-        """
-        Create a new tag.
-        
-        More info: https://apidocs.callrail.com/#creating-a-tag
-        """
-
-        # some validation before sending the request
-        if not name:
-            raise ValueError('name is required')
-
-        if tag_level == 'company' and not company_id:
-            raise ValueError('company_id is required if tag_level is company or not "account"')
-
-        body = {
-            'name': name
-        }
-
-        if company_id:
-            body['company_id'] = company_id
-        if color:
-            body['color'] = color
-        if tag_level:
-            body['tag_level'] = tag_level
-
-        data = self.api_client._post(
-            endpoint=f'a/{self.id}',
-            path='tags.json',
-            data=body
-        )
-
-        return tags.Tag.from_json(
-            self.api_client,
-            self.id,
-            typing.cast(typing.Dict[str, typing.Any], data)
-        )
-    
-    #########################
-    # Companies
-    #########################
-
-    def list_companies(
-            self,
-            **kwargs
-    ) -> typing.Union[typing.List[companies.Company], None]:
-        """
-        List all companies under account scope.
-
-        More info: https://apidocs.callrail.com/#creating-a-company
-        """
-
-        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
-
-        sorting = kwargs.get('sorting', None)
-        filtering: typing.Dict[str, typing.Any] = typing.cast(typing.Dict[str, typing.Any], kwargs.get('filtering', None))
-        searching = kwargs.get('searching', None)
-
-        if filtering:
-            # only filtering field supported is status, raise a ValueError if there is a other field
-            for k,v in filtering.items():
-                if k != 'status':
-                    raise ValueError(f'filtering field {k} is not supported')
-
-        params = {}
-
-        if sorting:
-            params['sorting'] = sorting
-        if filtering:
-            params['filtering'] = filtering
-        if searching:
-            params['searching'] = searching
-
-        if companies_response := typing.cast(
-            typing.List[typing.Dict[str, typing.Any]],
-            self.api_client._get(
-                endpoint=f'a/{self.id}',
-                response_data_key='companies',
-                path='companies.json',
-                params=params or None,
-                pagination_type=pagination_type,
-        )):
-            return [companies.Company.from_json(self.api_client, self.id, company) for company in companies_response]
-        else:
-            return None
-        
-    def get_company(
-            self,
-            company_id: str,
-            fields: typing.Optional[typing.MutableMapping[str, str]] = None
-    ) -> companies.Company:
-        """
-        Get a company.
-        
-        More info: https://apidocs.callrail.com/#retrieving-a-single-company
-        """
-
-        if fields:
-            data = self.api_client._get(
-                endpoint=f'a/{self.id}',
-                path=f'companies/{company_id}.json',
-                params=fields
-            )
-        else:
-            data = self.api_client._get(
-                endpoint=f'a/{self.id}',
-                path=f'companies/{company_id}.json'
-            )
-
-        return companies.Company.from_json(
-            self.api_client,
-            self.id,
-            typing.cast(typing.Dict[str, typing.Any], data)
-        )
-    
-    def create_company(
-            self,
-            name: str,
-            time_zone: typing.Optional[str] = None
-    ) -> companies.Company:
-        """
-        Create a new company.
-        
-        More info: https://apidocs.callrail.com/#creating-a-company
-        """
-
-        body = {
-            'name': name
-        }
-
-        if time_zone:
-            body['time_zone'] = time_zone
-
-        data = self.api_client._post(
-            endpoint=f'a/{self.id}',
-            path='companies.json',
-            data=body
-        )
-
-        return companies.Company.from_json(
-            self.api_client,
-            self.id,
-            typing.cast(typing.Dict[str, typing.Any], data)
-        )
-
-    #########################
-    # Form Submissions
-    #########################
-
-    def list_form_submissions(
-            self,
-            **kwargs
-    ) -> typing.Union[typing.List[forms.FormSubmission], None]:
-        """
-        List form submissions.
-
-        More information: https://apidocs.callrail.com/#listing-all-form-submissions
-        """
-
-        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
-
-        sorting = kwargs.get('sorting', None)
-        filtering = kwargs.get('filtering', None)
-        fields = kwargs.get('fields', None)
-
-        params = {}
-
-        if sorting:
-            params['sorting'] = sorting
-        if filtering:
-            params['filtering'] = filtering
-        if fields:
-            params['fields'] = fields
-
-        if forms_response := typing.cast(
-            typing.List[typing.Dict[str, typing.Any]],
-            self.api_client._get(
-                endpoint=f'a/{self.id}',
-                response_data_key='form_submissions',
-                path='form_submissions.json',
-                params=params or None,
-                pagination_type=pagination_type,
-            )
-        ):
-            return [forms.FormSubmission.from_json(self.api_client, self.id, submission) for submission in forms_response]
-        else:
-            logging.warning('No form submissions found')
-            return None
-        
-    def create_form_submission(
-            self,
-            company_id: str,
-            referrer: str,
-            referring_url: str,
-            landing_page_url: str,
-            form_url: str,
-            form_data: typing.Dict[str, typing.Any]
-    ) -> forms.FormSubmission:
-        """
-        Create a Form Submission.
-        
-        More information: https://apidocs.callrail.com/#creating-a-form-submission
-        """
-        body = {
-            'company_id': company_id,
-            'referrer': referrer,
-            'referring_url': referring_url,
-            'landing_page_url': landing_page_url,
-            'form_url': form_url,
-            'form_data': form_data
-        }
-
-        data = self.api_client._post(
-            endpoint=f'a/{self.id}',
-            path='form_submissions.json',
-            data=body
-        )
-
-        return forms.FormSubmission.from_json(
-            self.api_client,
-            self.id,
-            typing.cast(typing.Dict[str, typing.Any], data)
-        )
-    
-    #########################
-    # Text Messages
-    #########################
-
-    def list_text_message_conversations(
-            self,
-            **kwargs
-    ) -> typing.Union[typing.List[messages.TextMessageConversation], None]:
-        """
-        List all text message conversations.
-        More information: https://apidocs.callrail.com/#listing-all-conversations
-        """
-        
-        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
-
-        sorting = kwargs.get('sorting', None)
-        filtering = kwargs.get('filtering', None)
-        searching = kwargs.get('searching', None)
-        fields = kwargs.get('fields', None)
-
-        params = {}
-
-        if sorting:
-            params['sorting'] = sorting
-        if filtering:
-            params['filtering'] = filtering
-        if searching:
-            params['searching'] = searching
-        if fields:
-            params['fields'] = fields
-
-
-        if text_messages_response := typing.cast(
-            typing.List[typing.Dict[str, typing.Any]],
-            self.api_client._get(
-                endpoint=f'a/{self.id}',
-                response_data_key='conversations',
-                path='text-messages.json',
-                params=params or None,
-                pagination_type=pagination_type,
-            )
-        ):
-            return [messages.TextMessageConversation.from_json(self.api_client, self.id, message) for message in text_messages_response]
-        else:
-            logging.warning('No text messages found')
-            return None
-        
-    def get_text_message_conversation(
-            self,
-            conversation_id: str,
-            fields: typing.Optional[typing.MutableMapping[str, str]] = None
-    ) -> messages.TextMessageConversation:
-        """
-        Retrieve a single text message conversation.
-        More information: https://apidocs.callrail.com/#retrieving-a-single-text-conversation
-        """
-
-        if fields:
-            data = self.api_client._get(
-                endpoint=f'a/{self.id}',
-                path=f'text-messages/{conversation_id}.json',
-                params=fields
-            )
-        else:
-            data = self.api_client._get(
-                endpoint=f'a/{self.id}',
-                path=f'text-messages/{conversation_id}.json'
-            )
-        
-        return messages.TextMessageConversation.from_json(
-            self.api_client,
-            self.id,
-            typing.cast(typing.Dict[str, typing.Any], data)
-        )
-        
-    def send_text(
-            self,
-            company_id: str,
-            customer_phone_number: str,
-            content: str,
-            tracking_number: typing.Optional[typing.Union[str, int]] = None
-    ) -> messages.TextMessageConversation:
-        """
-        Send a text message.
-        More information: https://apidocs.callrail.com/#sending-a-text-message
-
-        Automated messaging is strictly prohibited by CallRail. This functionality is only for
-        use in person to person communication. For example, this method can be used when building a customer service
-        portal initiated by a agent. 
-
-        Predictive Data Lab is not to be held responsible for any misuse of this method.
-        """
-        logging.warning('Sending a text message requires approval from CallRail')
-        logging.warning('Endpoint is rate limited! Be careful!')
-        logging.warning('Automated messaging is not allowed. Please use this only for use in person to person communication')
-
-        body = {
-            'company_id': company_id,
-            'customer_phone_number': customer_phone_number,
-            'content': content
-        }
-
-        if tracking_number:
-            body['tracking_number'] = tracking_number # type: ignore
-
-        if len(content) >= 140:
-            raise ValueError('Content must be less than 140 characters')
-        
-        data = self.api_client._post(
-            endpoint=f'a/{self.id}',
-            path='text-messages.json',
-            data=body
-        )
-
-        return messages.TextMessageConversation.from_json(
-            self.api_client,
-            self.id,
-            typing.cast(typing.Dict[str, typing.Any], data)
+from __future__ import annotations
+
+import datetime as dt
+from dateutil import parser as dateparser
+import pycallrail.base as base
+import pycallrail.callrail as crl
+import pycallrail.objects.calls as calls
+import pycallrail.objects.tags as tags
+import pycallrail.objects.companies as companies
+import pycallrail.objects.form_submissions as forms
+import pycallrail.objects.textmessages as messages
+import typing
+import logging
+
+class Account(base.CallRailBase):
+    """
+    Represents a CallRail Account. Class should preferably not be instantiated directly.
+
+    More information: https://apidocs.callrail.com/#accounts
+    """
+
+    id: str
+    name: str
+    outbound_recording_enabled: bool
+    hipaa_account: bool
+
+    # Optional User Requested Fields
+    numeric_id: typing.Optional[int]
+
+    def __init__(
+            self,
+            api_client: crl.CallRail,
+            id: str,
+            name: str,
+            outbound_recording_enabled: bool,
+            hipaa_account: bool,
+            numeric_id: typing.Optional[int] = None
+    ) -> None:
+        super(Account, self).__init__()
+        self.api_client: crl.CallRail = api_client
+        self.id = id
+        self.name = name
+        self.outbound_recording_enabled = outbound_recording_enabled
+        self.hipaa_account = hipaa_account
+
+        if numeric_id:
+            self.numeric_id = numeric_id
+
+    @classmethod
+    def from_json(
+        cls,
+        api_client: crl.CallRail,
+        json_data: typing.Dict[str, typing.Any]
+    ) -> Account:
+        """
+        Deserialize JSON data into an Account object.
+        
+        :api_client: CallRail API object
+        :json_data: JSON data
+        """
+
+        account = Account(
+            api_client=api_client,
+            id=json_data['id'],
+            name=json_data['name'],
+            outbound_recording_enabled=json_data['outbound_recording_enabled'],
+            hipaa_account=json_data['hipaa_account']
+        )
+
+        if 'numeric_id' in json_data:
+            account.numeric_id = json_data['numeric_id']
+
+        return account
+    
+    #########################
+    # Calls
+    #########################
+
+    def list_calls(
+            self,
+            **kwargs
+        ) -> typing.Union[typing.List[calls.Call], None]:
+        """
+        List all calls associated with this account.
+
+        Keyword args acceptable include: Pagination Type, Sorting, Filtering, Field Selection, and Searching.
+        Defaults to relative pagination.
+        
+        More info: https://apidocs.callrail.com/#listing-all-calls
+        """
+
+        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
+
+        sorting = kwargs.get('sorting', None)
+        filtering = kwargs.get('filtering', None)
+        searching = kwargs.get('searching', None)
+        fields = kwargs.get('fields', None)
+
+        params = {}
+
+        if sorting:
+            params['sorting'] = sorting
+        if filtering:
+            params['filtering'] = filtering
+        if searching:
+            params['searching'] = searching
+        if fields:
+            params['fields'] = fields
+
+        if calls_response := typing.cast(
+            typing.Union[typing.List[typing.Dict[str, typing.Any]], None],
+            self.api_client._get(
+                endpoint=f'a/{self.id}',
+                response_data_key='calls',
+                path='calls.json',
+                params=params or None,
+                pagination_type=pagination_type,
+            ),
+        ):
+            return [calls.Call.from_json(self.api_client, self.id, call) for call in calls_response]
+        else:
+            return None
+
+    def get_call(
+        self,
+        call_id: str,
+        fields: typing.Optional[typing.MutableMapping[str, typing.Union[str, typing.Any]]] = None
+    ) -> calls.Call:
+        """
+        Retrieve a single call by ID.
+        
+        Field selection is supported by this method.
+        
+        More info: https://apidocs.callrail.com/#retrieving-a-single-call
+        """
+
+        if fields:
+            data = self.api_client._get(
+                endpoint=f'a/{self.id}',
+                path=f'calls/{call_id}.json',
+                params=fields
+            )
+        else:
+            data = self.api_client._get(
+                endpoint=f'a/{self.id}',
+                path=f'calls/{call_id}.json'
+            )
+
+        return calls.Call.from_json(
+            self.api_client, 
+            self.id, 
+            typing.cast(typing.Dict[str, typing.Any], data)
+        )
+    
+    def create_call(
+            self,
+            caller_id: int,
+            customer_phone_number: str,
+            business_phone_number: str,
+            recording_enabled: typing.Optional[bool] = None,
+            outbound_greeting_recording_url: typing.Optional[str] = None,
+            outbound_greeting_text: typing.Optional[str] = None,
+            agent_id: typing.Optional[str] = None
+    ) -> calls.Call:
+        """
+        Create a new call.
+        
+        This method is rate limited. There is no functionality to currently check for rate limits. Be careful!
+        More info: https://apidocs.callrail.com/#creating-an-outbound-phone-call
+        """
+
+        logging.warning('This method is rate limited. There is no functionality to currently check for rate limits. Be careful!')
+
+        body = {
+            'caller_id': caller_id,
+            'customer_phone_number': customer_phone_number,
+            'business_phone_number': business_phone_number
+        }
+
+        
+
+        if recording_enabled:
+            body['recording_enabled'] = recording_enabled
+        if outbound_greeting_recording_url:
+            body['outbound_greeting_recording_url'] = outbound_greeting_recording_url
+        if outbound_greeting_text:
+            body['outbound_greeting_text'] = outbound_greeting_text
+        if agent_id:
+            body['agent_id'] = agent_id
+        
+        data = self.api_client._post(
+            endpoint=f'a/{self.id}',
+            path='calls.json',
+            data=body
+        )
+
+        return calls.Call.from_json(
+            self.api_client,
+            self.id,
+            typing.cast(typing.Dict[str, typing.Any], data)
+        )
+    
+    #########################
+    # Tags
+    #########################
+
+    def list_tags(
+            self,
+            **kwargs
+    ) -> typing.Union[typing.List[tags.Tag], None]:
+        """
+        This endpoint returns a paginated array of tags within the target account.
+
+        More info: https://apidocs.callrail.com/#retrieving-all-tags
+        """
+
+        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
+
+        sorting = kwargs.get('sorting', None)
+
+        params = {}
+
+        if sorting:
+            params['sorting'] = sorting
+
+        if tags_response := typing.cast(
+            typing.List[typing.Dict[str, typing.Any]],
+            self.api_client._get(
+                endpoint=f'a/{self.id}',
+                response_data_key='tags',
+                path='tags.json',
+                params=params or None,
+                pagination_type=pagination_type,
+            )
+        ):
+            return [tags.Tag.from_json(self.api_client, self.id, tag) for tag in tags_response]
+
+        else:
+            return None
+        
+    def create_tag(
+            self,
+            name: str,
+            company_id: typing.Optional[str] = None,
+            color: typing.Optional[str] = None,
+            tag_level: typing.Optional[str] = None
+    ) -> tags.Tag:
+        """
+        Create a new tag.
+        
+        More info: https://apidocs.callrail.com/#creating-a-tag
+        """
+
+        # some validation before sending the request
+        if not name:
+            raise ValueError('name is required')
+
+        if tag_level == 'company' and not company_id:
+            raise ValueError('company_id is required if tag_level is company or not "account"')
+
+        body = {
+            'name': name
+        }
+
+        if company_id:
+            body['company_id'] = company_id
+        if color:
+            body['color'] = color
+        if tag_level:
+            body['tag_level'] = tag_level
+
+        data = self.api_client._post(
+            endpoint=f'a/{self.id}',
+            path='tags.json',
+            data=body
+        )
+
+        return tags.Tag.from_json(
+            self.api_client,
+            self.id,
+            typing.cast(typing.Dict[str, typing.Any], data)
+        )
+    
+    #########################
+    # Companies
+    #########################
+
+    def list_companies(
+            self,
+            **kwargs
+    ) -> typing.Union[typing.List[companies.Company], None]:
+        """
+        List all companies under account scope.
+
+        More info: https://apidocs.callrail.com/#creating-a-company
+        """
+
+        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
+
+        sorting = kwargs.get('sorting', None)
+        filtering: typing.Dict[str, typing.Any] = typing.cast(typing.Dict[str, typing.Any], kwargs.get('filtering', None))
+        searching = kwargs.get('searching', None)
+
+        if filtering:
+            # only filtering field supported is status, raise a ValueError if there is a other field
+            for k,v in filtering.items():
+                if k != 'status':
+                    raise ValueError(f'filtering field {k} is not supported')
+
+        params = {}
+
+        if sorting:
+            params['sorting'] = sorting
+        if filtering:
+            params['filtering'] = filtering
+        if searching:
+            params['searching'] = searching
+
+        if companies_response := typing.cast(
+            typing.List[typing.Dict[str, typing.Any]],
+            self.api_client._get(
+                endpoint=f'a/{self.id}',
+                response_data_key='companies',
+                path='companies.json',
+                params=params or None,
+                pagination_type=pagination_type,
+        )):
+            return [companies.Company.from_json(self.api_client, self.id, company) for company in companies_response]
+        else:
+            return None
+        
+    def get_company(
+            self,
+            company_id: str,
+            fields: typing.Optional[typing.MutableMapping[str, str]] = None
+    ) -> companies.Company:
+        """
+        Get a company.
+        
+        More info: https://apidocs.callrail.com/#retrieving-a-single-company
+        """
+
+        if fields:
+            data = self.api_client._get(
+                endpoint=f'a/{self.id}',
+                path=f'companies/{company_id}.json',
+                params=fields
+            )
+        else:
+            data = self.api_client._get(
+                endpoint=f'a/{self.id}',
+                path=f'companies/{company_id}.json'
+            )
+
+        return companies.Company.from_json(
+            self.api_client,
+            self.id,
+            typing.cast(typing.Dict[str, typing.Any], data)
+        )
+    
+    def create_company(
+            self,
+            name: str,
+            time_zone: typing.Optional[str] = None
+    ) -> companies.Company:
+        """
+        Create a new company.
+        
+        More info: https://apidocs.callrail.com/#creating-a-company
+        """
+
+        body = {
+            'name': name
+        }
+
+        if time_zone:
+            body['time_zone'] = time_zone
+
+        data = self.api_client._post(
+            endpoint=f'a/{self.id}',
+            path='companies.json',
+            data=body
+        )
+
+        return companies.Company.from_json(
+            self.api_client,
+            self.id,
+            typing.cast(typing.Dict[str, typing.Any], data)
+        )
+
+    #########################
+    # Form Submissions
+    #########################
+
+    def list_form_submissions(
+            self,
+            **kwargs
+    ) -> typing.Union[typing.List[forms.FormSubmission], None]:
+        """
+        List form submissions.
+
+        More information: https://apidocs.callrail.com/#listing-all-form-submissions
+        """
+
+        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
+
+        sorting = kwargs.get('sorting', None)
+        filtering = kwargs.get('filtering', None)
+        fields = kwargs.get('fields', None)
+
+        params = {}
+
+        if sorting:
+            params['sorting'] = sorting
+        if filtering:
+            params['filtering'] = filtering
+        if fields:
+            params['fields'] = fields
+
+        if forms_response := typing.cast(
+            typing.List[typing.Dict[str, typing.Any]],
+            self.api_client._get(
+                endpoint=f'a/{self.id}',
+                response_data_key='form_submissions',
+                path='form_submissions.json',
+                params=params or None,
+                pagination_type=pagination_type,
+            )
+        ):
+            return [forms.FormSubmission.from_json(self.api_client, self.id, submission) for submission in forms_response]
+        else:
+            logging.warning('No form submissions found')
+            return None
+        
+    def create_form_submission(
+            self,
+            company_id: str,
+            referrer: str,
+            referring_url: str,
+            landing_page_url: str,
+            form_url: str,
+            form_data: typing.Dict[str, typing.Any]
+    ) -> forms.FormSubmission:
+        """
+        Create a Form Submission.
+        
+        More information: https://apidocs.callrail.com/#creating-a-form-submission
+        """
+        body = {
+            'company_id': company_id,
+            'referrer': referrer,
+            'referring_url': referring_url,
+            'landing_page_url': landing_page_url,
+            'form_url': form_url,
+            'form_data': form_data
+        }
+
+        data = self.api_client._post(
+            endpoint=f'a/{self.id}',
+            path='form_submissions.json',
+            data=body
+        )
+
+        return forms.FormSubmission.from_json(
+            self.api_client,
+            self.id,
+            typing.cast(typing.Dict[str, typing.Any], data)
+        )
+    
+    #########################
+    # Text Messages
+    #########################
+
+    def list_text_message_conversations(
+            self,
+            **kwargs
+    ) -> typing.Union[typing.List[messages.TextMessageConversation], None]:
+        """
+        List all text message conversations.
+        More information: https://apidocs.callrail.com/#listing-all-conversations
+        """
+        
+        pagination_type: str = kwargs.get('pagination_type', 'RELATIVE')
+
+        sorting = kwargs.get('sorting', None)
+        filtering = kwargs.get('filtering', None)
+        searching = kwargs.get('searching', None)
+        fields = kwargs.get('fields', None)
+
+        params = {}
+
+        if sorting:
+            params['sorting'] = sorting
+        if filtering:
+            params['filtering'] = filtering
+        if searching:
+            params['searching'] = searching
+        if fields:
+            params['fields'] = fields
+
+
+        if text_messages_response := typing.cast(
+            typing.List[typing.Dict[str, typing.Any]],
+            self.api_client._get(
+                endpoint=f'a/{self.id}',
+                response_data_key='conversations',
+                path='text-messages.json',
+                params=params or None,
+                pagination_type=pagination_type,
+            )
+        ):
+            return [messages.TextMessageConversation.from_json(self.api_client, self.id, message) for message in text_messages_response]
+        else:
+            logging.warning('No text messages found')
+            return None
+        
+    def get_text_message_conversation(
+            self,
+            conversation_id: str,
+            fields: typing.Optional[typing.MutableMapping[str, str]] = None
+    ) -> messages.TextMessageConversation:
+        """
+        Retrieve a single text message conversation.
+        More information: https://apidocs.callrail.com/#retrieving-a-single-text-conversation
+        """
+
+        if fields:
+            data = self.api_client._get(
+                endpoint=f'a/{self.id}',
+                path=f'text-messages/{conversation_id}.json',
+                params=fields
+            )
+        else:
+            data = self.api_client._get(
+                endpoint=f'a/{self.id}',
+                path=f'text-messages/{conversation_id}.json'
+            )
+        
+        return messages.TextMessageConversation.from_json(
+            self.api_client,
+            self.id,
+            typing.cast(typing.Dict[str, typing.Any], data)
+        )
+        
+    def send_text(
+            self,
+            company_id: str,
+            customer_phone_number: str,
+            content: str,
+            tracking_number: typing.Optional[typing.Union[str, int]] = None
+    ) -> messages.TextMessageConversation:
+        """
+        Send a text message.
+        More information: https://apidocs.callrail.com/#sending-a-text-message
+
+        Automated messaging is strictly prohibited by CallRail. This functionality is only for
+        use in person to person communication. For example, this method can be used when building a customer service
+        portal initiated by a agent. 
+
+        Predictive Data Lab is not to be held responsible for any misuse of this method.
+        """
+        logging.warning('Sending a text message requires approval from CallRail')
+        logging.warning('Endpoint is rate limited! Be careful!')
+        logging.warning('Automated messaging is not allowed. Please use this only for use in person to person communication')
+
+        body = {
+            'company_id': company_id,
+            'customer_phone_number': customer_phone_number,
+            'content': content
+        }
+
+        if tracking_number:
+            body['tracking_number'] = tracking_number # type: ignore
+
+        if len(content) >= 140:
+            raise ValueError('Content must be less than 140 characters')
+        
+        data = self.api_client._post(
+            endpoint=f'a/{self.id}',
+            path='text-messages.json',
+            data=body
+        )
+
+        return messages.TextMessageConversation.from_json(
+            self.api_client,
+            self.id,
+            typing.cast(typing.Dict[str, typing.Any], data)
         )
```

### Comparing `pycallrail-0.9.0.0/pycallrail/objects/calls.py` & `pycallrail-0.9.0.1/pycallrail/objects/calls.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-from __future__ import annotations
-
-import datetime as dt
-from dateutil import parser as dateparser
-import pycallrail.base as base
-import pycallrail.callrail as crl
-import typing
-import typing_extensions
-import requests
-
-
-class Call(base.CallRailBase):
-    """
-    Represents a CallRail call.
-    
-    More information: https://apidocs.callrail.com/#calls
-    """
-
-    # These fields are always returned by the API
-    answered: bool
-    business_phone_number: typing.Optional[str]
-    customer_city: str
-    customer_country: str
-    customer_name: str
-    customer_phone_number: str
-    customer_state: str
-    direction: str
-    duration: int
-    id: str
-    recording: typing.Optional[str]
-    recording_duration: typing.Optional[str]
-    recording_player: typing.Optional[str]
-    start_time: dt.datetime
-    tracking_phone_number: str
-    voicemail: bool
-    
-    # User Requested Fields
-    call_type: typing.Optional[str]
-    company_id: typing.Optional[str]
-    company_name: typing.Optional[str]
-    company_time_zone: typing.Optional[str]
-    created_at: typing.Optional[str]
-    device_type: typing.Optional[str]
-    first_call: typing.Optional[bool]
-    formatted_call_type: typing.Optional[str]
-    formatted_customer_location: typing.Optional[str]
-    formatted_business_phone_number: typing.Optional[str]
-    formatted_customer_name: typing.Optional[str]
-    prior_calls: typing.Optional[int]
-    formatted_customer_name_or_phone_number: typing.Optional[str]
-    formatted_customer_phone_number: typing.Optional[str]
-    formatted_duration: typing.Optional[str]
-    formatted_tracking_phone_number: typing.Optional[str]
-    formatted_tracking_source: typing.Optional[str]
-    formatted_value: typing.Optional[str]
-    good_lead_call_id: typing.Optional[int]
-    good_lead_call_time: typing.Optional[str]
-    lead_status: typing.Optional[str]
-    note: typing.Optional[str]
-    source: typing.Optional[str]
-    source_name: typing.Optional[str]
-    tags: typing.Optional[typing.List[typing.Any]]
-    total_calls: typing.Optional[int]
-    value: typing.Optional[str]
-    waveforms: typing.Optional[typing.List[typing.Any]]
-    tracker_id: typing.Optional[str]
-    speaker_percent: typing.Optional[typing.Dict[str, typing.Any]]
-    keywords: typing.Optional[str]
-    medium: typing.Optional[str]
-    campaign: typing.Optional[str]
-    referring_url: typing.Optional[str]
-    landing_page_url: typing.Optional[str]
-    last_requested_url: typing.Optional[str]
-    referrer_domain: typing.Optional[str]
-    utm_source: typing.Optional[str]
-    utm_medium: typing.Optional[str]
-    utm_term: typing.Optional[str]
-    utm_content: typing.Optional[str]
-    utm_campaign: typing.Optional[str]
-    utma: typing.Optional[str]
-    utmb: typing.Optional[str]
-    utmc: typing.Optional[str]
-    utmv: typing.Optional[str]
-    utmz: typing.Optional[str]
-    ga: typing.Optional[str]
-    gclid: typing.Optional[str]
-    fbclid: typing.Optional[str]
-    msclkid: typing.Optional[str]
-    milestones: typing.Optional[typing.Any]
-    timeline_url: typing.Optional[str]
-    keywords_spotted: typing.Optional[typing.List[typing.Any]]
-    call_highlights: typing.Optional[typing.List[typing.Any]]
-    agent_email: typing.Optional[str]
-    keypad_entries: typing.Optional[typing.MutableMapping[str, typing.Any]]
-
-
-    def __init__(
-            self,
-            api_client: crl.CallRail,
-            account_id: str,
-            **kwargs
-    ) -> None:
-        super(Call, self).__init__()
-        self.api_client: crl.CallRail = api_client
-        self.account_id: str = account_id
-
-        for key, value in kwargs.items():
-            if key not in self.__class__.__annotations__.keys():
-                raise AttributeError(f'{key} is not a valid attribute for {self.__class__.__name__}.')
-            else:
-                setattr(self, key, value)
-    
-    @classmethod
-    def from_json(
-        cls,
-        api_client: crl.CallRail,
-        account_id: str,
-        json_data: typing.Dict[str, typing.Any]
-    ) -> Call:
-        """
-        Deserialize JSON data to a Call object.
-        
-        :param api_client: The CallRail API client.
-        :param json_data: The JSON data to deserialize.
-        """
-
-        # first lets convert the start_time to a datetime
-        json_data['start_time'] = dateparser.parse(json_data['start_time'])
-
-        return cls(api_client, account_id, **json_data)
-    
-    
-    def update(
-            self, 
-            tags: typing.Optional[typing.List[typing.Any]] = None,
-            note: typing.Optional[str] = None,
-            value: typing.Optional[str] = None,
-            lead_status: typing.Optional[str] = None,
-            append_tags: typing.Optional[bool] = None,
-            customer_name: typing.Optional[str] = None,
-            spam: typing.Optional[bool] = None
-        ) -> None:
-        """
-        Update a Call object.
-        More information: https://apidocs.callrail.com/#updating-a-call
-        """
-        # update the attributes
-        if append_tags and tags and hasattr(self, 'tags'):
-            self.tags.extend(tags) # type: ignore
-        else:
-            self.tags = tags
-        if note:
-            self.note = note
-        if value:
-            self.value = value
-        if lead_status:
-            self.lead_status = lead_status
-        if customer_name:
-            self.customer_name = customer_name
-        if spam:
-            self.spam = spam
-
-        # form the request body
-        body: typing.Dict[str, typing.Any] = {
-            'tags': tags,
-            'note': note,
-            'value': value,
-            'lead_status': lead_status,
-            'append_tags': append_tags,
-            'customer_name': customer_name,
-            'spam': spam
-        }
-
-        # send the request
-        response_data: typing.Dict[str, typing.Any] = typing.cast(
-            typing.Dict[str, typing.Any], 
-            self.api_client._put(
-                endpoint = f'a/{self.account_id}',
-                path=f'calls/{self.id}.json',
-                data=body
-            )
-        )
-
-        # update the attributes
-        for key, value in response_data.items():
-            # raise an error if the attribute doesn't exist
-            if key not in self.__class__.__annotations__.keys():
-                raise AttributeError(f'{key} is not a valid attribute for {self.__class__.__name__}.')
-            else:
-                setattr(self, key, value)
-        
-        
-        
-
-    def get_recording(self) -> typing.Union[bytes, None]:
-        """
-        Get the recording of the call.
-        More information: https://apidocs.callrail.com/#get-the-recording-of-the-call
-
-        If no recording exists, None is returned.
-        """
-        if self.recording:
-            with self.api_client.session.get(url=self.recording) as response:
-                return response.content
-        else:
+from __future__ import annotations
+
+import datetime as dt
+from dateutil import parser as dateparser
+import pycallrail.base as base
+import pycallrail.callrail as crl
+import typing
+import typing_extensions
+import requests
+
+
+class Call(base.CallRailBase):
+    """
+    Represents a CallRail call.
+    
+    More information: https://apidocs.callrail.com/#calls
+    """
+
+    # These fields are always returned by the API
+    answered: bool
+    business_phone_number: typing.Optional[str]
+    customer_city: str
+    customer_country: str
+    customer_name: str
+    customer_phone_number: str
+    customer_state: str
+    direction: str
+    duration: int
+    id: str
+    recording: typing.Optional[str]
+    recording_duration: typing.Optional[str]
+    recording_player: typing.Optional[str]
+    start_time: dt.datetime
+    tracking_phone_number: str
+    voicemail: bool
+    
+    # User Requested Fields
+    call_type: typing.Optional[str]
+    company_id: typing.Optional[str]
+    company_name: typing.Optional[str]
+    company_time_zone: typing.Optional[str]
+    created_at: typing.Optional[str]
+    device_type: typing.Optional[str]
+    first_call: typing.Optional[bool]
+    formatted_call_type: typing.Optional[str]
+    formatted_customer_location: typing.Optional[str]
+    formatted_business_phone_number: typing.Optional[str]
+    formatted_customer_name: typing.Optional[str]
+    prior_calls: typing.Optional[int]
+    formatted_customer_name_or_phone_number: typing.Optional[str]
+    formatted_customer_phone_number: typing.Optional[str]
+    formatted_duration: typing.Optional[str]
+    formatted_tracking_phone_number: typing.Optional[str]
+    formatted_tracking_source: typing.Optional[str]
+    formatted_value: typing.Optional[str]
+    good_lead_call_id: typing.Optional[int]
+    good_lead_call_time: typing.Optional[str]
+    lead_status: typing.Optional[str]
+    note: typing.Optional[str]
+    source: typing.Optional[str]
+    source_name: typing.Optional[str]
+    tags: typing.Optional[typing.List[typing.Any]]
+    total_calls: typing.Optional[int]
+    value: typing.Optional[str]
+    waveforms: typing.Optional[typing.List[typing.Any]]
+    tracker_id: typing.Optional[str]
+    speaker_percent: typing.Optional[typing.Dict[str, typing.Any]]
+    keywords: typing.Optional[str]
+    medium: typing.Optional[str]
+    campaign: typing.Optional[str]
+    referring_url: typing.Optional[str]
+    landing_page_url: typing.Optional[str]
+    last_requested_url: typing.Optional[str]
+    referrer_domain: typing.Optional[str]
+    utm_source: typing.Optional[str]
+    utm_medium: typing.Optional[str]
+    utm_term: typing.Optional[str]
+    utm_content: typing.Optional[str]
+    utm_campaign: typing.Optional[str]
+    utma: typing.Optional[str]
+    utmb: typing.Optional[str]
+    utmc: typing.Optional[str]
+    utmv: typing.Optional[str]
+    utmz: typing.Optional[str]
+    ga: typing.Optional[str]
+    gclid: typing.Optional[str]
+    fbclid: typing.Optional[str]
+    msclkid: typing.Optional[str]
+    milestones: typing.Optional[typing.Any]
+    timeline_url: typing.Optional[str]
+    keywords_spotted: typing.Optional[typing.List[typing.Any]]
+    call_highlights: typing.Optional[typing.List[typing.Any]]
+    agent_email: typing.Optional[str]
+    keypad_entries: typing.Optional[typing.MutableMapping[str, typing.Any]]
+
+
+    def __init__(
+            self,
+            api_client: crl.CallRail,
+            account_id: str,
+            **kwargs
+    ) -> None:
+        super(Call, self).__init__()
+        self.api_client: crl.CallRail = api_client
+        self.account_id: str = account_id
+
+        for key, value in kwargs.items():
+            if key not in self.__class__.__annotations__.keys():
+                raise AttributeError(f'{key} is not a valid attribute for {self.__class__.__name__}.')
+            else:
+                setattr(self, key, value)
+    
+    @classmethod
+    def from_json(
+        cls,
+        api_client: crl.CallRail,
+        account_id: str,
+        json_data: typing.Dict[str, typing.Any]
+    ) -> Call:
+        """
+        Deserialize JSON data to a Call object.
+        
+        :param api_client: The CallRail API client.
+        :param json_data: The JSON data to deserialize.
+        """
+
+        # first lets convert the start_time to a datetime
+        json_data['start_time'] = dateparser.parse(json_data['start_time'])
+
+        return cls(api_client, account_id, **json_data)
+    
+    
+    def update(
+            self, 
+            tags: typing.Optional[typing.List[typing.Any]] = None,
+            note: typing.Optional[str] = None,
+            value: typing.Optional[str] = None,
+            lead_status: typing.Optional[str] = None,
+            append_tags: typing.Optional[bool] = None,
+            customer_name: typing.Optional[str] = None,
+            spam: typing.Optional[bool] = None
+        ) -> None:
+        """
+        Update a Call object.
+        More information: https://apidocs.callrail.com/#updating-a-call
+        """
+        # update the attributes
+        if append_tags and tags and hasattr(self, 'tags'):
+            self.tags.extend(tags) # type: ignore
+        else:
+            self.tags = tags
+        if note:
+            self.note = note
+        if value:
+            self.value = value
+        if lead_status:
+            self.lead_status = lead_status
+        if customer_name:
+            self.customer_name = customer_name
+        if spam:
+            self.spam = spam
+
+        # form the request body
+        body: typing.Dict[str, typing.Any] = {
+            'tags': tags,
+            'note': note,
+            'value': value,
+            'lead_status': lead_status,
+            'append_tags': append_tags,
+            'customer_name': customer_name,
+            'spam': spam
+        }
+
+        # send the request
+        response_data: typing.Dict[str, typing.Any] = typing.cast(
+            typing.Dict[str, typing.Any], 
+            self.api_client._put(
+                endpoint = f'a/{self.account_id}',
+                path=f'calls/{self.id}.json',
+                data=body
+            )
+        )
+
+        # update the attributes
+        for key, value in response_data.items():
+            # raise an error if the attribute doesn't exist
+            if key not in self.__class__.__annotations__.keys():
+                raise AttributeError(f'{key} is not a valid attribute for {self.__class__.__name__}.')
+            else:
+                setattr(self, key, value)
+        
+        
+        
+
+    def get_recording(self) -> typing.Union[bytes, None]:
+        """
+        Get the recording of the call.
+        More information: https://apidocs.callrail.com/#get-the-recording-of-the-call
+
+        If no recording exists, None is returned.
+        """
+        if self.recording:
+            with self.api_client.session.get(url=self.recording) as response:
+                return response.content
+        else:
             return None
```

### Comparing `pycallrail-0.9.0.0/pycallrail/objects/form_submissions.py` & `pycallrail-0.9.0.1/pycallrail/objects/form_submissions.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from __future__ import annotations
-
-import datetime as dt
-from dateutil import parser as dateparser
-import pycallrail.base as base
-import pycallrail.callrail as crl
-import typing
-import typing_extensions
-import requests
-
-
-class FormSubmission(base.CallRailBase):
-    """
-    Represents a form submission.
-
-    More info: https://apidocs.callrail.com/#form-submissions
-    """
-
-    # These fields are always returned by the API
-    id: str
-    company_id: str
-    person_id: str
-    form_data: typing.Dict[str, typing.Any]
-    form_url: str
-    landing_page_url: str
-    referrer: str
-    referring_url: str
-    submitted_at: dt.datetime
-    first_form: bool
-    customer_phone_number: str
-    customer_name: str
-    formatted_customer_phone_number: str
-    formatted_customer_name: str
-    source: str
-    keywords: str
-    campaign: str
-    medium: str
-
-    # User Requested Fields
-    lead_status: typing.Optional[str]
-    value: typing.Optional[typing.Union[int, float]]
-    note: typing.Optional[str]
-    tags: typing.Optional[typing.List[typing.Any]]
-    utm_source: typing.Optional[str]
-    utm_campaign: typing.Optional[str]
-    form_name: typing.Optional[str]
-    timeline_url: typing.Optional[str]
-    milestones: typing.Optional[typing.Any]
-
-    def __init__(
-        self,
-        api_client: crl.CallRail,
-        account_id: str,
-        **kwargs
-    ) -> None:
-        super(FormSubmission, self).__init__()
-        self.api_client: crl.CallRail = api_client
-        self.account_id: str = account_id
-
-        for k,v in kwargs.items():
-            if k not in self.__class__.__annotations__.keys():
-                raise AttributeError(f'{k} is not a valid attribute for {self.__class__.__name__}')
-            else:
-                setattr(self, k, v)
-
-    @classmethod
-    def from_json(
-        cls,
-        api_client: crl.CallRail,
-        account_id: str,
-        json_data: typing.Dict[str, typing.Any]
-    ) -> FormSubmission:
-        """
-        Deserializes a FormSubmission from JSON.
-
-        :param api_client: The CallRail API client
-        :param json_data: The JSON data to deserialize
-        :param account_id: The CallRail account ID
-        :return: The FormSubmission object
-        """
-        json_data['submitted_at'] = dateparser.parse(json_data['submitted_at'])
-        
-        return cls(
-            api_client=api_client,
-            account_id=account_id,
-            **json_data
-        )
-        
-    def update(
-        self,
-        tags: typing.Optional[typing.List[typing.Any]] = None,
-        note: typing.Optional[str] = None,
-        value: typing.Optional[typing.Union[int, float]] = None,
-        lead_status: typing.Optional[str] = None,
-        append_tags: typing.Optional[bool] = None
-    ) -> None:
-        """
-        Update a Form Submission.
-        More information: https://apidocs.callrail.com/#updating-a-form-submission
-        """
-
-        # update the attributes
-        if append_tags and tags and hasattr(self, 'tags'):
-            self.tags.extend(tags) # type: ignore
-        elif tags:
-            self.tags = tags
-        if note:
-            self.note = note
-        if value:
-            self.value = value
-        if lead_status:
-            self.lead_status = lead_status
-
-        # form the request
-        body: typing.Dict[str, typing.Any] = {
-            'tags': tags,
-            'note': note,
-            'value': value,
-            'lead_status': lead_status
-        }
-
-        # send the request
-        response: typing.Dict[str, typing.Any] = typing.cast(
-            typing.Dict[str, typing.Any],
-            self.api_client._put(
-                endpoint=f'a/{self.account_id}',
-                path=f'form_submissions/{self.id}.json',
-                data=body
-            )
-        )
-
-        # update the object
-        for k,v in response.items():
-            # raise an error if the attribute is not found
-            if k not in self.__class__.__annotations__.keys():
-                raise AttributeError(f'{k} is not a valid attribute for {self.__class__.__name__}')
-            else:
-                setattr(self, k, v)
-
+from __future__ import annotations
+
+import datetime as dt
+from dateutil import parser as dateparser
+import pycallrail.base as base
+import pycallrail.callrail as crl
+import typing
+import typing_extensions
+import requests
+
+
+class FormSubmission(base.CallRailBase):
+    """
+    Represents a form submission.
+
+    More info: https://apidocs.callrail.com/#form-submissions
+    """
+
+    # These fields are always returned by the API
+    id: str
+    company_id: str
+    person_id: str
+    form_data: typing.Dict[str, typing.Any]
+    form_url: str
+    landing_page_url: str
+    referrer: str
+    referring_url: str
+    submitted_at: dt.datetime
+    first_form: bool
+    customer_phone_number: str
+    customer_name: str
+    formatted_customer_phone_number: str
+    formatted_customer_name: str
+    source: str
+    keywords: str
+    campaign: str
+    medium: str
+
+    # User Requested Fields
+    lead_status: typing.Optional[str]
+    value: typing.Optional[typing.Union[int, float]]
+    note: typing.Optional[str]
+    tags: typing.Optional[typing.List[typing.Any]]
+    utm_source: typing.Optional[str]
+    utm_campaign: typing.Optional[str]
+    form_name: typing.Optional[str]
+    timeline_url: typing.Optional[str]
+    milestones: typing.Optional[typing.Any]
+
+    def __init__(
+        self,
+        api_client: crl.CallRail,
+        account_id: str,
+        **kwargs
+    ) -> None:
+        super(FormSubmission, self).__init__()
+        self.api_client: crl.CallRail = api_client
+        self.account_id: str = account_id
+
+        for k,v in kwargs.items():
+            if k not in self.__class__.__annotations__.keys():
+                raise AttributeError(f'{k} is not a valid attribute for {self.__class__.__name__}')
+            else:
+                setattr(self, k, v)
+
+    @classmethod
+    def from_json(
+        cls,
+        api_client: crl.CallRail,
+        account_id: str,
+        json_data: typing.Dict[str, typing.Any]
+    ) -> FormSubmission:
+        """
+        Deserializes a FormSubmission from JSON.
+
+        :param api_client: The CallRail API client
+        :param json_data: The JSON data to deserialize
+        :param account_id: The CallRail account ID
+        :return: The FormSubmission object
+        """
+        json_data['submitted_at'] = dateparser.parse(json_data['submitted_at'])
+        
+        return cls(
+            api_client=api_client,
+            account_id=account_id,
+            **json_data
+        )
+        
+    def update(
+        self,
+        tags: typing.Optional[typing.List[typing.Any]] = None,
+        note: typing.Optional[str] = None,
+        value: typing.Optional[typing.Union[int, float]] = None,
+        lead_status: typing.Optional[str] = None,
+        append_tags: typing.Optional[bool] = None
+    ) -> None:
+        """
+        Update a Form Submission.
+        More information: https://apidocs.callrail.com/#updating-a-form-submission
+        """
+
+        # update the attributes
+        if append_tags and tags and hasattr(self, 'tags'):
+            self.tags.extend(tags) # type: ignore
+        elif tags:
+            self.tags = tags
+        if note:
+            self.note = note
+        if value:
+            self.value = value
+        if lead_status:
+            self.lead_status = lead_status
+
+        # form the request
+        body: typing.Dict[str, typing.Any] = {
+            'tags': tags,
+            'note': note,
+            'value': value,
+            'lead_status': lead_status
+        }
+
+        # send the request
+        response: typing.Dict[str, typing.Any] = typing.cast(
+            typing.Dict[str, typing.Any],
+            self.api_client._put(
+                endpoint=f'a/{self.account_id}',
+                path=f'form_submissions/{self.id}.json',
+                data=body
+            )
+        )
+
+        # update the object
+        for k,v in response.items():
+            # raise an error if the attribute is not found
+            if k not in self.__class__.__annotations__.keys():
+                raise AttributeError(f'{k} is not a valid attribute for {self.__class__.__name__}')
+            else:
+                setattr(self, k, v)
+
```

### Comparing `pycallrail-0.9.0.0/pycallrail/objects/tags.py` & `pycallrail-0.9.0.1/pycallrail/objects/tags.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-from __future__ import annotations
-
-import datetime as dt
-from dateutil import parser as dateparser
-import pycallrail.base as base
-import pycallrail.callrail as crl
-import typing
-import logging
-import typeguard
-
-@typeguard.typechecked
-class Tag(base.CallRailBase):
-    """
-    Represents a Tag.
-
-    More information: https://apidocs.callrail.com/#tags
-    """
-
-    id: typing.Union[int, str]
-    name: str
-    tag_level: str
-    color: str
-    background_color: str
-    company_id: str
-    status: str
-    created_at: dt.datetime
-
-    def __init__(
-        self,
-        api_client: crl.CallRail,
-        account_id: str,
-        id: typing.Union[int, str],
-        name: str,
-        tag_level: str,
-        color: str,
-        background_color: str,
-        company_id: str,
-        status: str,
-        created_at: dt.datetime
-    ) -> None:
-        super(Tag, self).__init__()
-        self.api_client: crl.CallRail = api_client
-        self.account_id = account_id
-        self.id = id
-        self.name = name    
-        self.tag_level = tag_level
-        self.color = color
-        self.background_color = background_color
-        self.company_id = company_id
-        self.status = status
-        self.created_at = created_at
-
-    @classmethod
-    def from_json(
-        cls,
-        api_client: crl.CallRail,
-        account_id: str,
-        json_data: typing.Dict[str, typing.Any]
-    ) -> Tag:
-        """
-        Deserialize JSON data to a Tag object.
-        """
-        json_data['created_at'] = dateparser.parse(json_data['created_at'])
-
-        return cls(
-            api_client=api_client,
-            account_id=account_id,
-            id=json_data['id'],
-            name=json_data['name'],
-            tag_level=json_data['tag_level'],
-            color=json_data['color'],
-            background_color=json_data['background_color'],
-            company_id=json_data['company_id'],
-            status=json_data['status'],
-            created_at=json_data['created_at']
-        )
-    
-    def update(
-            self,
-            name: typing.Optional[str] = None,
-            color: typing.Optional[str] = None,
-            disabled: typing.Optional[typing.Union[str, bool]] = None
-    ) -> None:
-        """
-        Updates the Tag.
-        """
-        if name:
-            self.name = name
-        if color:
-            self.color = color
-        if disabled == 'true' or disabled == True:
-            self.disabled = True
-
-        body: typing.Dict[str, typing.Any] = {
-            'name': name,
-            'color': color,
-            'disabled': disabled
-        }
-
-        response: typing.Dict[str, typing.Any] = typing.cast(
-            typing.Dict[str, typing.Any],
-            self.api_client._put(
-                endpoint=f'a/{self.account_id}',
-                path=f'tags/{self.id}.json',
-                data=body
-            )
-        )
-
-        for key, value in response.items():
-            if key not in self.__class__.__annotations__.keys():
-                raise AttributeError(f'{key} is not a valid attribute for {self.__class__.__name__}')
-            else:
-                setattr(self, key, value)
-    
-    def delete(self) -> None:
-        """
-        Deletes the Tag.
-        """
-        self.api_client._delete(
-            endpoint=f'a/{self.account_id}',
-            path=f'tags/{self.id}.json'
-        )
-
+from __future__ import annotations
+
+import datetime as dt
+from dateutil import parser as dateparser
+import pycallrail.base as base
+import pycallrail.callrail as crl
+import typing
+import logging
+import typeguard
+
+@typeguard.typechecked
+class Tag(base.CallRailBase):
+    """
+    Represents a Tag.
+
+    More information: https://apidocs.callrail.com/#tags
+    """
+
+    id: typing.Union[int, str]
+    name: str
+    tag_level: str
+    color: str
+    background_color: str
+    company_id: str
+    status: str
+    created_at: dt.datetime
+
+    def __init__(
+        self,
+        api_client: crl.CallRail,
+        account_id: str,
+        id: typing.Union[int, str],
+        name: str,
+        tag_level: str,
+        color: str,
+        background_color: str,
+        company_id: str,
+        status: str,
+        created_at: dt.datetime
+    ) -> None:
+        super(Tag, self).__init__()
+        self.api_client: crl.CallRail = api_client
+        self.account_id = account_id
+        self.id = id
+        self.name = name    
+        self.tag_level = tag_level
+        self.color = color
+        self.background_color = background_color
+        self.company_id = company_id
+        self.status = status
+        self.created_at = created_at
+
+    @classmethod
+    def from_json(
+        cls,
+        api_client: crl.CallRail,
+        account_id: str,
+        json_data: typing.Dict[str, typing.Any]
+    ) -> Tag:
+        """
+        Deserialize JSON data to a Tag object.
+        """
+        json_data['created_at'] = dateparser.parse(json_data['created_at'])
+
+        return cls(
+            api_client=api_client,
+            account_id=account_id,
+            id=json_data['id'],
+            name=json_data['name'],
+            tag_level=json_data['tag_level'],
+            color=json_data['color'],
+            background_color=json_data['background_color'],
+            company_id=json_data['company_id'],
+            status=json_data['status'],
+            created_at=json_data['created_at']
+        )
+    
+    def update(
+            self,
+            name: typing.Optional[str] = None,
+            color: typing.Optional[str] = None,
+            disabled: typing.Optional[typing.Union[str, bool]] = None
+    ) -> None:
+        """
+        Updates the Tag.
+        """
+        if name:
+            self.name = name
+        if color:
+            self.color = color
+        if disabled == 'true' or disabled == True:
+            self.disabled = True
+
+        body: typing.Dict[str, typing.Any] = {
+            'name': name,
+            'color': color,
+            'disabled': disabled
+        }
+
+        response: typing.Dict[str, typing.Any] = typing.cast(
+            typing.Dict[str, typing.Any],
+            self.api_client._put(
+                endpoint=f'a/{self.account_id}',
+                path=f'tags/{self.id}.json',
+                data=body
+            )
+        )
+
+        for key, value in response.items():
+            if key not in self.__class__.__annotations__.keys():
+                raise AttributeError(f'{key} is not a valid attribute for {self.__class__.__name__}')
+            else:
+                setattr(self, key, value)
+    
+    def delete(self) -> None:
+        """
+        Deletes the Tag.
+        """
+        self.api_client._delete(
+            endpoint=f'a/{self.account_id}',
+            path=f'tags/{self.id}.json'
+        )
+
```

### Comparing `pycallrail-0.9.0.0/pycallrail.egg-info/PKG-INFO` & `pycallrail-0.9.0.1/pycallrail.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-Metadata-Version: 2.1
-Name: pycallrail
-Version: 0.9.0.0
-Summary: An unofficial Python wrapper for the CallRail API
-Home-page: https://github.com/predictive-data-lab/pycallrail
-Author: Engineering @ Predictive Data Lab
-License: MIT
-Project-URL: Documentation, https://pycallrail.readthedocs.io/en/latest/
-Project-URL: Issue Tracker, https://github.com/predictive-data-lab/pycallrail/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Communications
-Requires-Python: >=3.8.0
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
-pycallrail
-==========
-
-.. image:: https://img.shields.io/pypi/v/pycallrail.svg
-   :target: https://pypi.python.org/pypi/pycallrail
-   :alt: PyPI version info
-.. image:: https://img.shields.io/pypi/pyversions/pycallrail.svg
-   :target: https://pypi.python.org/pypi/pycallrail.py
-   :alt: PyPI supported Python versions
-.. image:: https://github.com/predictive-data-lab/pycallrail/actions/workflows/test.yml/badge.svg
-   :target: https://github.com/predictive-data-lab/pycallrail/commits/main
-   :alt: GitHub Actions build status
-.. image:: https://codecov.io/gh/predictive-data-lab/pycallrail/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/predictive-data-lab/pycallrail
-   :alt: Codecov coverage report
-.. image:: https://readthedocs.org/projects/pycallrail/badge/?version=latest
-   :target: https://pycallrail.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-
-Python wrapper for the CallRail API.
-
-Description
------------
-
-This library provides a Python intefrace for interacting with the Callrail API.
-It allows for CRUD operations on objects and resources within your CallRail account and to integrate
-with your own applications.
-
-Installation
-------------
-Install from PyPI using pip, a package manager for Python.
-
-.. code:: sh
-
-   # Linux/macOS
-   python3 -m pip install pycallrail
-
-   # Windows
-   py -3 -m pip install pycallrail
-
-Requirements & Dependencies
----------------------------
-- Python 3.6+
-- requests
-- ujson
-- python-dateutil
-- typeguard
-
-Usage
------
-
-.. code:: py
-
-   import pycallrail.callrail as clrl
-
-   # init the api client
-
-   api = clrl.CallRail('your_api_key')
-
-   # list accounts associated with your api key
-   accounts = api.list_accounts(# optional kwargs, more info on supported kwargs at endpoint docs)
-
-   # list calls associated with your account
-   calls = accounts[0].list_calls(# optional kwargs, more info on supported kwargs at endpoint docs)
-
-   print(calls[0].id) # prints the id of the first call in the list
-
-   # >>> 123456789
-
-Links & Contact
----------------
-
-- `Documentation <https://pycallrail.readthedocs.io/en/latest/>`_
-- `Questions <mailto:engineering@predictivedatalab.com>`_
+Metadata-Version: 2.1
+Name: pycallrail
+Version: 0.9.0.1
+Summary: An unofficial Python wrapper for the CallRail API
+Home-page: https://github.com/predictive-data-lab/pycallrail
+Author: Engineering @ Predictive Data Lab
+License: MIT
+Project-URL: Documentation, https://pycallrail.readthedocs.io/en/latest/
+Project-URL: Issue Tracker, https://github.com/predictive-data-lab/pycallrail/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Communications
+Requires-Python: >=3.8.0
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+pycallrail
+==========
+
+.. image:: https://img.shields.io/pypi/v/pycallrail.svg
+   :target: https://pypi.python.org/pypi/pycallrail
+   :alt: PyPI version info
+.. image:: https://img.shields.io/pypi/pyversions/pycallrail.svg
+   :target: https://pypi.python.org/pypi/pycallrail.py
+   :alt: PyPI supported Python versions
+.. image:: https://github.com/predictive-data-lab/pycallrail/actions/workflows/test.yml/badge.svg
+   :target: https://github.com/predictive-data-lab/pycallrail/commits/main
+   :alt: GitHub Actions build status
+.. image:: https://codecov.io/gh/predictive-data-lab/pycallrail/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/predictive-data-lab/pycallrail
+   :alt: Codecov coverage report
+.. image:: https://readthedocs.org/projects/pycallrail/badge/?version=latest
+   :target: https://pycallrail.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+Python wrapper for the CallRail API.
+
+Description
+-----------
+
+This library provides a Python intefrace for interacting with the Callrail API.
+It allows for CRUD operations on objects and resources within your CallRail account and to integrate
+with your own applications.
+
+Installation
+------------
+Install from PyPI using pip, a package manager for Python.
+
+.. code:: sh
+
+   # Linux/macOS
+   python3 -m pip install pycallrail
+
+   # Windows
+   py -3 -m pip install pycallrail
+
+Requirements & Dependencies
+---------------------------
+- Python 3.6+
+- requests
+- ujson
+- python-dateutil
+- typeguard
+
+Usage
+-----
+
+.. code:: py
+
+   import pycallrail.callrail as clrl
+
+   # init the api client
+
+   api = clrl.CallRail('your_api_key')
+
+   # list accounts associated with your api key
+   accounts = api.list_accounts(# optional kwargs, more info on supported kwargs at endpoint docs)
+
+   # list calls associated with your account
+   calls = accounts[0].list_calls(# optional kwargs, more info on supported kwargs at endpoint docs)
+
+   print(calls[0].id) # prints the id of the first call in the list
+
+   # >>> 123456789
+
+Links & Contact
+---------------
+
+- `Documentation <https://pycallrail.readthedocs.io/en/latest/>`_
+- `Questions <mailto:engineering@predictivedatalab.com>`_
```

### Comparing `pycallrail-0.9.0.0/pycallrail.egg-info/SOURCES.txt` & `pycallrail-0.9.0.1/pycallrail.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
 setup.py
+pycallrail/__init__.py
+pycallrail/base.py
+pycallrail/callrail.py
+pycallrail/errors.py
+pycallrail/helpers.py
+pycallrail/mixins.py
 pycallrail.egg-info/PKG-INFO
 pycallrail.egg-info/SOURCES.txt
 pycallrail.egg-info/dependency_links.txt
 pycallrail.egg-info/requires.txt
 pycallrail.egg-info/top_level.txt
 pycallrail/objects/__init__.py
 pycallrail/objects/accounts.py
 pycallrail/objects/calls.py
 pycallrail/objects/companies.py
 pycallrail/objects/form_submissions.py
 pycallrail/objects/tags.py
 pycallrail/objects/textmessages.py
+tests/__init__.py
+tests/cfg.py
 tests/test_account.py
 tests/test_apiclient.py
 tests/test_call.py
 tests/test_companies.py
 tests/test_formsubmissions.py
 tests/test_helpers.py
 tests/test_integration.py
```

### Comparing `pycallrail-0.9.0.0/tests/test_apiclient.py` & `pycallrail-0.9.0.1/tests/test_apiclient.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-import pytest
-import pytest_mock
-import requests_mock
-import requests
-
-from pycallrail.callrail import CallRail
-from pycallrail.objects.accounts import Account
-import typing
-
-
-
-
-# Tests that list_accounts method returns a list of Account objects. 
-def test_list_accounts_happy_path(requests_mock: requests_mock.Mocker) -> None:
-    # Setup
-    api_key = 'test_api_key'
-    api_client = CallRail(api_key=api_key)
-    mock_response: typing.Dict[str, typing.Any] = {
-        "page": 1,
-        "per_page": 100,
-        "total_pages": 1,
-        "total_records": 2,
-        "accounts": [
-            {
-                "id": "ACC8154748ae6bd4e278a7cddd38a662f4f",
-                "name": "Last Mile Metrics",
-                "outbound_recording_enabled": True,
-                "hipaa_account": False
-            },
-            {
-                "id": "ACC8154748ae6bd4e278a7cddd38a662d4d",
-                "name": "CallRail",
-                "outbound_recording_enabled": True,
-                "hipaa_account": False
-            }
-        ]   
-    }
-    
-    requests_mock.get('https://api.callrail.com/v3/a.json', json=mock_response)
-
-    # Execution
-    accounts: typing.List[Account] = api_client.list_accounts()
-
-    # Assertion
-    assert len(accounts) == 2
-    assert accounts[0].id == 'ACC8154748ae6bd4e278a7cddd38a662f4f'
-    assert accounts[1].id == 'ACC8154748ae6bd4e278a7cddd38a662d4d'
-    assert accounts[0].name == 'Last Mile Metrics'
-    assert accounts[1].name == 'CallRail'
-    assert accounts[0].outbound_recording_enabled == True
-    assert accounts[1].outbound_recording_enabled == True
-    assert accounts[0].hipaa_account == False
-    assert accounts[1].hipaa_account == False
-
-# Tests that get_account returns an Account object. 
-def test_get_account_happy_path(requests_mock: requests_mock.Mocker) -> None:
-    # Setup
-    api_key = 'test_api_key'
-    api_client = CallRail(api_key=api_key)
-    mock_response: typing.Dict[str, typing.Any] = {
-        "id": "ACC8154748ae6bd4e278a7cddd38a662f4f",
-        "name": "Last Mile Metrics",
-        "outbound_recording_enabled": True,
-        "hipaa_account": False
-    }
-    
-    requests_mock.get('https://api.callrail.com/v3/a/ACC8154748ae6bd4e278a7cddd38a662f4f.json', json=mock_response)
-
-    # Execution
-    account: Account = api_client.get_account(account_id='ACC8154748ae6bd4e278a7cddd38a662f4f')
-
-    # Assertion
-    assert account.id == 'ACC8154748ae6bd4e278a7cddd38a662f4f'
-    assert account.name == 'Last Mile Metrics'
-    assert account.outbound_recording_enabled == True
-    assert account.hipaa_account == False
-
-# Tests that _post handles missing response_data_key. 
-def test__post_edge_case(requests_mock: requests_mock.Mocker) -> None:
-    # Setup
-    api_key = 'test_api_key'
-    cr = CallRail(api_key=api_key)
-    data_post: typing.Dict[str, typing.Any] = {
-        "caller_id": "+17703334455",
-        "business_phone_number": "+14045556666",
-        "customer_phone_number": "+14044442233",
-        "recording_enabled": True,
-        "outbound_greeting_recording_url": "http://www.test.com/greeting.mp3",
-        "outbound_greeting_text": "These are not the droids you are looking for."
-    }
-
-    mock_response: typing.Dict[str, typing.Any] = {
-        "answered": None,
-        "business_phone_number": "+19044567899",
-        "customer_city": "Atlanta",
-        "customer_country": "US",
-        "customer_name": None,
-        "customer_phone_number": "+14703444700",
-        "customer_state": "GA",
-        "direction": "outbound",
-        "duration": None,
-        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
-        "recording": None,
-        "recording_duration": None,
-        "start_time": "2017-02-22T15:02:24.916-05:00",
-        "tracking_phone_number": "+19044567899",
-        "voicemail": False
-    }
-    
-    requests_mock.post('https://api.callrail.com/v3/a/12345/calls.json', json=mock_response)
-
-    # Execution
-    response: typing.Dict[str, typing.Any] = typing.cast(
-        typing.Dict[str, typing.Any], cr._post(endpoint='a/12345', path='calls.json', data=data_post))
-
-    # Assertion
-    assert response == mock_response
-
-# Tests that _relative_paginator handles pagination correctly. 
-def test__relative_paginator_edge_case(requests_mock: requests_mock.Mocker) -> None:
-    # Setup
-    api_key = 'test_api_key'
-    cr = CallRail(api_key=api_key)
-    mock_response_1: typing.Dict[str, typing.Any] = {
-        'accounts': [
-            {
-                'id': '1',
-                'name': 'Test Account 1',
-                'outbound_recording_enabled': True,
-                'hipaa_account': False
-            }
-        ],
-        'has_next_page': True,
-        'next_page': 'https://api.callrail.com/v3/a.json?page=2'
-    }
-    mock_response_2: typing.Dict[str, typing.Any] = {
-        'accounts': [
-            {
-                'id': '2',
-                'name': 'Test Account 2',
-                'outbound_recording_enabled': False,
-                'hipaa_account': True
-            }
-        ],
-        'has_next_page': False
-    }
-    requests_mock.get('https://api.callrail.com/v3/a.json', json=mock_response_1)
-    requests_mock.get('https://api.callrail.com/v3/a.json?page=2', json=mock_response_2)
-
-    # Execution
-    response: typing.List[typing.Dict[str, typing.Any]] = cr._relative_paginator(
-        response=requests.get('https://api.callrail.com/v3/a.json'), response_data_key='accounts')
-
-    # Assertion
-    assert len(response) == 2
-    assert response[0]['id'] == '1'
-    assert response[1]['id'] == '2'
-
-# Tests handling of invalid API responses. 
-def test_list_accounts_general_behavior(requests_mock: requests_mock.Mocker):
-    # Setup
-    api_key = 'test_api_key'
-    cr = CallRail(api_key=api_key)
-    mock_response: typing.Dict[str, str] = {
-        'error': 'Invalid API key'
-    }
-    requests_mock.get('https://api.callrail.com/v3/a.json', json=mock_response, status_code=401)
-
-    # Execution and Assertion
-    with pytest.raises(requests.exceptions.HTTPError):
-        cr.list_accounts()
-
-    # Tests that _get correctly handles query string parameters. 
-def test__get_happy_path(requests_mock: requests_mock.Mocker):
-    # Setup
-    api_key = 'test_api_key'
-    cr = CallRail(api_key=api_key)
-    mock_response: typing.Dict[str, typing.Any] = {
-        "page": 1,
-        "per_page": 100,
-        "total_pages": 1,
-        "total_records": 2,
-        "accounts": [
-            {
-                "id": "ACC8154748ae6bd4e278a7cddd38a662f4f",
-                "name": "Last Mile Metrics",
-                "outbound_recording_enabled": True,
-                "hipaa_account": False
-            },
-            {
-                "id": "ACC8154748ae6bd4e278a7cddd38a662d4d",
-                "name": "CallRail",
-                "outbound_recording_enabled": True,
-                "hipaa_account": False
-            }
-        ]   
-    }
-
-    requests_mock.get('https://api.callrail.com/v3/a.json?sorting=name', json=mock_response)
-
-    # Execution
-    response = cr._get(endpoint='a.json', response_data_key='accounts', params={'sorting': 'name'})
-
-    # Assertion
-    assert response == mock_response['accounts']
-
-# Tests that _post handles missing response_data_key.  
-def test__post_happy_path(requests_mock: requests_mock.Mocker) -> None:
-    # Setup
-    api_key = 'test_api_key'
-    cr = CallRail(api_key=api_key)
-    mock_response = {
-        'data': {
-            'id': 1,
-            'name': 'Test Account',
-            'outbound_recording_enabled': True,
-            'hipaa_account': False
-        }
-    }
-
-    requests_mock.post('https://api.callrail.com/v3/test_endpoint', json=mock_response)
-
-    # Test
-    response = cr._post(endpoint='test_endpoint', response_data_key='data')
-
-    # Assert
-    assert response == mock_response['data']
-    assert requests_mock.last_request.headers['Authorization'] == f'Token token="{api_key}"'
-
-# Tests handling of API errors and exceptions.  
-def test_get_account_general_behavior(requests_mock: requests_mock.Mocker) -> None:
-    # Test handling of API errors and exceptions in get_account method
-    account_id = '123'
-    url = f'https://api.callrail.com/v3/a/{account_id}.json'
-    requests_mock.get(url, status_code=404)
-
-    callrail = CallRail(api_key='test')
-    with pytest.raises(requests.exceptions.HTTPError):
-        callrail.get_account(account_id=account_id)
-
-# Tests handling of unexpected input parameters in CallRail constructor.  
-def test_CallRail_constructor_general_behavior() -> None:
-    # Test handling of unexpected input parameters in CallRail constructor
-    with pytest.raises(TypeError):
+import pytest
+import pytest_mock
+import requests_mock
+import requests
+
+from pycallrail.callrail import CallRail
+from pycallrail.objects.accounts import Account
+import typing
+
+
+
+
+# Tests that list_accounts method returns a list of Account objects. 
+def test_list_accounts_happy_path(requests_mock: requests_mock.Mocker) -> None:
+    # Setup
+    api_key = 'test_api_key'
+    api_client = CallRail(api_key=api_key)
+    mock_response: typing.Dict[str, typing.Any] = {
+        "page": 1,
+        "per_page": 100,
+        "total_pages": 1,
+        "total_records": 2,
+        "accounts": [
+            {
+                "id": "ACC8154748ae6bd4e278a7cddd38a662f4f",
+                "name": "Last Mile Metrics",
+                "outbound_recording_enabled": True,
+                "hipaa_account": False
+            },
+            {
+                "id": "ACC8154748ae6bd4e278a7cddd38a662d4d",
+                "name": "CallRail",
+                "outbound_recording_enabled": True,
+                "hipaa_account": False
+            }
+        ]   
+    }
+    
+    requests_mock.get('https://api.callrail.com/v3/a.json', json=mock_response)
+
+    # Execution
+    accounts: typing.List[Account] = api_client.list_accounts()
+
+    # Assertion
+    assert len(accounts) == 2
+    assert accounts[0].id == 'ACC8154748ae6bd4e278a7cddd38a662f4f'
+    assert accounts[1].id == 'ACC8154748ae6bd4e278a7cddd38a662d4d'
+    assert accounts[0].name == 'Last Mile Metrics'
+    assert accounts[1].name == 'CallRail'
+    assert accounts[0].outbound_recording_enabled == True
+    assert accounts[1].outbound_recording_enabled == True
+    assert accounts[0].hipaa_account == False
+    assert accounts[1].hipaa_account == False
+
+# Tests that get_account returns an Account object. 
+def test_get_account_happy_path(requests_mock: requests_mock.Mocker) -> None:
+    # Setup
+    api_key = 'test_api_key'
+    api_client = CallRail(api_key=api_key)
+    mock_response: typing.Dict[str, typing.Any] = {
+        "id": "ACC8154748ae6bd4e278a7cddd38a662f4f",
+        "name": "Last Mile Metrics",
+        "outbound_recording_enabled": True,
+        "hipaa_account": False
+    }
+    
+    requests_mock.get('https://api.callrail.com/v3/a/ACC8154748ae6bd4e278a7cddd38a662f4f.json', json=mock_response)
+
+    # Execution
+    account: Account = api_client.get_account(account_id='ACC8154748ae6bd4e278a7cddd38a662f4f')
+
+    # Assertion
+    assert account.id == 'ACC8154748ae6bd4e278a7cddd38a662f4f'
+    assert account.name == 'Last Mile Metrics'
+    assert account.outbound_recording_enabled == True
+    assert account.hipaa_account == False
+
+# Tests that _post handles missing response_data_key. 
+def test__post_edge_case(requests_mock: requests_mock.Mocker) -> None:
+    # Setup
+    api_key = 'test_api_key'
+    cr = CallRail(api_key=api_key)
+    data_post: typing.Dict[str, typing.Any] = {
+        "caller_id": "+17703334455",
+        "business_phone_number": "+14045556666",
+        "customer_phone_number": "+14044442233",
+        "recording_enabled": True,
+        "outbound_greeting_recording_url": "http://www.test.com/greeting.mp3",
+        "outbound_greeting_text": "These are not the droids you are looking for."
+    }
+
+    mock_response: typing.Dict[str, typing.Any] = {
+        "answered": None,
+        "business_phone_number": "+19044567899",
+        "customer_city": "Atlanta",
+        "customer_country": "US",
+        "customer_name": None,
+        "customer_phone_number": "+14703444700",
+        "customer_state": "GA",
+        "direction": "outbound",
+        "duration": None,
+        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
+        "recording": None,
+        "recording_duration": None,
+        "start_time": "2017-02-22T15:02:24.916-05:00",
+        "tracking_phone_number": "+19044567899",
+        "voicemail": False
+    }
+    
+    requests_mock.post('https://api.callrail.com/v3/a/12345/calls.json', json=mock_response)
+
+    # Execution
+    response: typing.Dict[str, typing.Any] = typing.cast(
+        typing.Dict[str, typing.Any], cr._post(endpoint='a/12345', path='calls.json', data=data_post))
+
+    # Assertion
+    assert response == mock_response
+
+# Tests that _relative_paginator handles pagination correctly. 
+def test__relative_paginator_edge_case(requests_mock: requests_mock.Mocker) -> None:
+    # Setup
+    api_key = 'test_api_key'
+    cr = CallRail(api_key=api_key)
+    mock_response_1: typing.Dict[str, typing.Any] = {
+        'accounts': [
+            {
+                'id': '1',
+                'name': 'Test Account 1',
+                'outbound_recording_enabled': True,
+                'hipaa_account': False
+            }
+        ],
+        'has_next_page': True,
+        'next_page': 'https://api.callrail.com/v3/a.json?page=2'
+    }
+    mock_response_2: typing.Dict[str, typing.Any] = {
+        'accounts': [
+            {
+                'id': '2',
+                'name': 'Test Account 2',
+                'outbound_recording_enabled': False,
+                'hipaa_account': True
+            }
+        ],
+        'has_next_page': False
+    }
+    requests_mock.get('https://api.callrail.com/v3/a.json', json=mock_response_1)
+    requests_mock.get('https://api.callrail.com/v3/a.json?page=2', json=mock_response_2)
+
+    # Execution
+    response: typing.List[typing.Dict[str, typing.Any]] = cr._relative_paginator(
+        response=requests.get('https://api.callrail.com/v3/a.json'), response_data_key='accounts')
+
+    # Assertion
+    assert len(response) == 2
+    assert response[0]['id'] == '1'
+    assert response[1]['id'] == '2'
+
+# Tests handling of invalid API responses. 
+def test_list_accounts_general_behavior(requests_mock: requests_mock.Mocker):
+    # Setup
+    api_key = 'test_api_key'
+    cr = CallRail(api_key=api_key)
+    mock_response: typing.Dict[str, str] = {
+        'error': 'Invalid API key'
+    }
+    requests_mock.get('https://api.callrail.com/v3/a.json', json=mock_response, status_code=401)
+
+    # Execution and Assertion
+    with pytest.raises(requests.exceptions.HTTPError):
+        cr.list_accounts()
+
+    # Tests that _get correctly handles query string parameters. 
+def test__get_happy_path(requests_mock: requests_mock.Mocker):
+    # Setup
+    api_key = 'test_api_key'
+    cr = CallRail(api_key=api_key)
+    mock_response: typing.Dict[str, typing.Any] = {
+        "page": 1,
+        "per_page": 100,
+        "total_pages": 1,
+        "total_records": 2,
+        "accounts": [
+            {
+                "id": "ACC8154748ae6bd4e278a7cddd38a662f4f",
+                "name": "Last Mile Metrics",
+                "outbound_recording_enabled": True,
+                "hipaa_account": False
+            },
+            {
+                "id": "ACC8154748ae6bd4e278a7cddd38a662d4d",
+                "name": "CallRail",
+                "outbound_recording_enabled": True,
+                "hipaa_account": False
+            }
+        ]   
+    }
+
+    requests_mock.get('https://api.callrail.com/v3/a.json?sorting=name', json=mock_response)
+
+    # Execution
+    response = cr._get(endpoint='a.json', response_data_key='accounts', params={'sorting': 'name'})
+
+    # Assertion
+    assert response == mock_response['accounts']
+
+# Tests that _post handles missing response_data_key.  
+def test__post_happy_path(requests_mock: requests_mock.Mocker) -> None:
+    # Setup
+    api_key = 'test_api_key'
+    cr = CallRail(api_key=api_key)
+    mock_response = {
+        'data': {
+            'id': 1,
+            'name': 'Test Account',
+            'outbound_recording_enabled': True,
+            'hipaa_account': False
+        }
+    }
+
+    requests_mock.post('https://api.callrail.com/v3/test_endpoint', json=mock_response)
+
+    # Test
+    response = cr._post(endpoint='test_endpoint', response_data_key='data')
+
+    # Assert
+    assert response == mock_response['data']
+    assert requests_mock.last_request.headers['Authorization'] == f'Token token="{api_key}"'
+
+# Tests handling of API errors and exceptions.  
+def test_get_account_general_behavior(requests_mock: requests_mock.Mocker) -> None:
+    # Test handling of API errors and exceptions in get_account method
+    account_id = '123'
+    url = f'https://api.callrail.com/v3/a/{account_id}.json'
+    requests_mock.get(url, status_code=404)
+
+    callrail = CallRail(api_key='test')
+    with pytest.raises(requests.exceptions.HTTPError):
+        callrail.get_account(account_id=account_id)
+
+# Tests handling of unexpected input parameters in CallRail constructor.  
+def test_CallRail_constructor_general_behavior() -> None:
+    # Test handling of unexpected input parameters in CallRail constructor
+    with pytest.raises(TypeError):
         CallRail(api_key='test', invalid_param=True)
```

### Comparing `pycallrail-0.9.0.0/tests/test_call.py` & `pycallrail-0.9.0.1/tests/test_call.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,454 +1,454 @@
-import pytest
-import pytest_mock
-import requests_mock
-import requests
-
-from pycallrail.callrail import CallRail
-from pycallrail.objects.calls import Call
-import typing
-import logging
-import datetime as dt
-
-# Tests that a Call object can be created with valid arguments. 
-def test_create_call_with_valid_arguments(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    call_data: typing.Dict[str, typing.Any] =  {
-        "answered": False,
-        "business_phone_number": None,
-        "customer_city": "New York City",
-        "customer_country": "US",
-        "customer_name": "Jimmy Pesto, Sr.",
-        "customer_phone_number": "+13036231131",
-        "customer_state": "NY",
-        "direction": "inbound",
-        "duration": 4,
-        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
-        "recording": "https://api.callrail.com/v3/a/227799611/calls/111222333/recording.json",
-        "recording_duration": "27",
-        "recording_player": "https://app.callrail.com/calls/111222333/recording?access_key=3b91eb7f7cc08a4d01ed",
-        "start_time": "2017-01-24T11:27:48.119-05:00",
-        "tracking_phone_number": "+13038163491",
-        "voicemail": False,
-        "agent_email": "gil@televised.com"
-    }
-
-    # Act
-    call = Call(api_client, account_id, **call_data)
-
-    # Assert
-    assert call.answered == call_data['answered']
-    assert call.customer_city == call_data['customer_city']
-    assert call.customer_country == call_data['customer_country']
-    assert call.customer_name == call_data['customer_name']
-    assert call.customer_phone_number == call_data['customer_phone_number']
-    assert call.customer_state == call_data['customer_state']
-    assert call.direction == call_data['direction']
-    assert call.duration == call_data['duration']
-    assert call.id == call_data['id']
-    assert call.start_time == call_data['start_time']
-    assert call.tracking_phone_number == call_data['tracking_phone_number']
-    assert call.voicemail == call_data['voicemail']
-
-# Tests that a Call object can be created with valid arguments. 
-def test_call_creation_two_instances(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    call_data: typing.Dict[str, typing.Any] =  {
-        "answered": False,
-        "business_phone_number": None,
-        "customer_city": "New York City",
-        "customer_country": "US",
-        "customer_name": "Jimmy Pesto, Sr.",
-        "customer_phone_number": "+13036231131",
-        "customer_state": "NY",
-        "direction": "inbound",
-        "duration": 4,
-        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
-        "recording": "https://api.callrail.com/v3/a/227799611/calls/111222333/recording.json",
-        "recording_duration": "27",
-        "recording_player": "https://app.callrail.com/calls/111222333/recording?access_key=3b91eb7f7cc08a4d01ed",
-        "start_time": "2017-01-24T11:27:48.119-05:00",
-        "tracking_phone_number": "+13038163491",
-        "voicemail": False,
-        "agent_email": "gil@televised.com"
-    }
-
-    # Act
-    call = Call(api_client, account_id, **call_data)
-
-    call_data_2: typing.Dict[str, typing.Any] =  {
-        "answered": True,
-        "business_phone_number": None,
-        "customer_city": "Toronto",
-        "customer_country": "CA",
-        "customer_name": "Jimmy Pesto, Sr.",
-        "customer_phone_number": "+13036231131",
-        "customer_state": "NY",
-        "direction": "inbound",
-        "duration": 4,
-        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
-        "recording": "https://api.callrail.com/v3/a/227799611/calls/111222333/recording.json",
-        "recording_duration": "27",
-        "recording_player": "https://app.callrail.com/calls/111222333/recording?access_key=3b91eb7f7cc08a4d01ed",
-        "start_time": "2017-01-24T11:27:48.119-05:00",
-        "tracking_phone_number": "+13038163491",
-        "voicemail": False,
-        "agent_email": "gil@televised.com"
-    }
-
-    call_2 = Call(api_client, account_id, **call_data_2)
-
-    # Assert
-    assert call.answered == call_data['answered']
-    assert call.customer_city == call_data['customer_city']
-    assert call.customer_country == call_data['customer_country']
-    assert call.customer_name == call_data['customer_name']
-    assert call.customer_phone_number == call_data['customer_phone_number']
-    assert call.customer_state == call_data['customer_state']
-    assert call.direction == call_data['direction']
-    assert call.duration == call_data['duration']
-    assert call.id == call_data['id']
-    assert call.start_time == call_data['start_time']
-    assert call.tracking_phone_number == call_data['tracking_phone_number']
-    assert call.voicemail == call_data['voicemail']
-
-    assert call_2.answered == call_data_2['answered']
-    assert call_2.customer_city == call_data_2['customer_city']
-    assert call_2.customer_country == call_data_2['customer_country']
-
-# Tests that a Call object can be updated with valid arguments. 
-def test_update_call_with_valid_arguments(requests_mock: requests_mock.Mocker) -> None:
-    # Arrange
-    api_client = CallRail(api_key='123')
-    account_id = '123'
-    
-    call_data =  {
-        "answered": False,
-        "business_phone_number": None,
-        "customer_city": "Denver",
-        "customer_country": "US",
-        "customer_name": "James Smith",
-        "customer_phone_number": "+13036231131",
-        "customer_state": "CO",
-        "direction": "inbound",
-        "duration": 4,
-        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
-        "recording": "https://api.callrail.com/v3/a/227799611/calls/213472384/recording.json",
-        "recording_duration": "27",
-        "start_time": "2017-01-24T11:27:48.119-05:00",
-        "tracking_phone_number": "+13038163491",
-        "voicemail": False
-    }
-
-    call = Call(api_client, account_id, **call_data)
-
-    update_data = {
-        "note": "Call customer back tomorrow",
-        "tags": ["New Client"],
-        "lead_status": "good_lead",
-        "value": "$1.00",
-        "append_tags": True,
-        "customer_name": "James Smith"
-    }
-
-    # Act
-    requests_mock.put(
-        url=f'https://api.callrail.com/v3/a/{account_id}/calls/{call.id}.json',
-        json= call_data 
-    )
-
-
-    call.update(
-        tags = update_data['tags'], 
-        note = update_data['note'], 
-        value = update_data['value'], 
-        append_tags = update_data['append_tags'], 
-        customer_name = update_data['customer_name'])
-
-    # Assert
-    assert call.tags == update_data['tags']
-    assert call.note == update_data['note']
-    assert call.value == update_data['value']
-    assert call.customer_name == update_data['customer_name']
-
-# Tests that a Call object cannot be created with missing or invalid required arguments. 
-def test_create_call_with_invalid_arguments(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    call_data = {
-        "answered": False,
-        "business_phone_number": None,
-        "customer_city": "Denver",
-        "customer_country": "US",
-        "customer_name": "James Smith",
-        "customer_phone_number": "+13036231131",
-        "customer_state": "CO",
-        "direction": "inbound",
-        "duration": 4,
-        "recording": "https://api.callrail.com/v3/a/227799611/calls/213472384/recording.json",
-        "recording_duration": "27",
-        "start_time": "2017-01-24T11:27:48.119-05:00",
-        "tracking_phone_number": "+13038163491",
-        "invalid_argument": True
-    } 
-
-    # Act & Assert
-    with pytest.raises(AttributeError):
-        Call(api_client, account_id, **call_data)
-
-def test_update_call_with_invalid_arguments(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    call_data = {
-        "answered": False,
-        "business_phone_number": None,
-        "customer_city": "Denver",
-        "customer_country": "US",
-        "customer_name": "James Smith",
-        "customer_phone_number": "+13036231131",
-        "customer_state": "CO",
-        "direction": "inbound",
-        "duration": 4,
-        "recording": "https://api.callrail.com/v3/a/227799611/calls/213472384/recording.json",
-        "recording_duration": "27",
-        "start_time": "2017-01-24T11:27:48.119-05:00",
-        "tracking_phone_number": "+13038163491"
-    }
-
-    call = Call(api_client, account_id, **call_data)
-
-    with pytest.raises(Exception):
-        call.update(invalid_argument = True)
-
-# Tests that the recording of a call can be retrieved with a valid recording URL. 
-def test_get_recording_with_valid_recording_url(requests_mock: requests_mock.Mocker) -> None:
-    # Arrange
-    api_client = CallRail(api_key='123')
-    account_id = '123'
-    call_data = {
-        'answered': True,
-        'customer_city': 'New York',
-        'customer_country': 'USA',
-        'customer_name': 'John Doe',
-        'customer_phone_number': '123-456-7890',
-        'customer_state': 'NY',
-        'direction': 'inbound',
-        'duration': 60,
-        'id': '456',
-        'start_time': '2017-01-24T11:27:48.119-05:00',
-        'tracking_phone_number': '987-654-3210',
-        'voicemail': False,
-        'recording': 'http://example.com/recording.mp3'
-    }
-    call = Call(api_client, account_id, **call_data)
-    recording_content = b'This is a recording'
-
-    # Mock the response from the recording URL
-    requests_mock.get(
-        url='http://example.com/recording.mp3',
-        content=recording_content
-    )
-
-    # Act
-    recording = call.get_recording()
-
-    # Assert
-    assert recording == recording_content
-
-# Tests that None is returned when attempting to retrieve the recording of a call with no recording URL. 
-def test_get_recording_with_no_recording_url(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    call_data = {
-        'answered': True,
-        'customer_city': 'New York',
-        'customer_country': 'USA',
-        'customer_name': 'John Doe',
-        'customer_phone_number': '123-456-7890',
-        'customer_state': 'NY',
-        'direction': 'inbound',
-        'duration': 60,
-        'id': '456',
-        'start_time': '2017-01-24T11:27:48.119-05:00',
-        'tracking_phone_number': '987-654-3210',
-        'voicemail': False,
-        'recording': None
-    }
-    call = Call(api_client, account_id, **call_data)
-
-    # Act
-    recording = call.get_recording()
-
-    # Assert
-    assert recording is None
-
-# Tests that JSON data can be successfully deserialized to a Call object.  
-def test_deserialize_json_data_to_call_object(mocker: pytest_mock.MockerFixture) -> None:
-    # Setup
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    json_data = {
-        'answered': True,
-        'business_phone_number': '555-555-5555',
-        'customer_city': 'New York',
-        'customer_country': 'USA',
-        'customer_name': 'John Doe',
-        'customer_phone_number': '555-555-5555',
-        'customer_state': 'NY',
-        'direction': 'inbound',
-        'duration': 60,
-        'id': '456',
-        'recording': 'http://example.com/recording.mp3',
-        'recording_duration': '00:01:00',
-        'recording_player': 'http://example.com/recording_player.mp3',
-        'start_time': '2022-01-01T00:00:00Z',
-        'tracking_phone_number': '555-555-5555',
-        'voicemail': False,
-        'call_type': 'sales',
-        'company_id': '789',
-        'company_name': 'Acme Inc.',
-        'company_time_zone': 'America/New_York',
-        'created_at': '2022-01-01T00:00:00Z',
-        'device_type': 'mobile',
-        'first_call': True,
-        'formatted_call_type': 'Sales Call',
-        'formatted_customer_location': 'New York, NY, USA',
-        'formatted_business_phone_number': '(555) 555-5555',
-        'formatted_customer_name': 'John Doe',
-        'prior_calls': 2,
-        'formatted_customer_name_or_phone_number': '(555) 555-5555',
-        'formatted_customer_phone_number': '(555) 555-5555',
-        'formatted_duration': '1m 0s',
-        'formatted_tracking_phone_number': '(555) 555-5555',
-        'formatted_tracking_source': 'Google Ads',
-        'formatted_value': '$100',
-        'good_lead_call_id': 123,
-        'good_lead_call_time': '2022-01-01T00:00:00Z',
-        'lead_status': 'qualified',
-        'note': 'This was a good call.',
-        'source': 'google',
-        'source_name': 'Google Ads',
-        'tags': ['tag1', 'tag2'],
-        'total_calls': 10,
-        'value': 100,
-        'waveforms': [{'time': 0, 'value': 0}, {'time': 1, 'value': 1}],
-        'tracker_id': 'abc123',
-        'speaker_percent': {'speaker1': 50, 'speaker2': 50},
-        'keywords': 'important keywords',
-        'medium': 'cpc',
-        'campaign': 'campaign1',
-        'referring_url': 'http://example.com/referrer',
-        'landing_page_url': 'http://example.com/landing',
-        'last_requested_url': 'http://example.com/requested',
-        'referrer_domain': 'example.com',
-        'utm_source': 'google',
-        'utm_medium': 'cpc',
-        'utm_term': 'term1',
-        'utm_content': 'content1',
-        'utm_campaign': 'campaign1',
-        'utma': '123456789.1234567890.1234567890.1234567890.1',
-        'utmb': '123456789.1.10.1234567890',
-        'utmc': '',
-        'utmv': '',
-        'utmz': '',
-        'ga': '',
-        'gclid': '',
-        'fbclid': '',
-        'msclkid': '',
-        'milestones': {'milestone1': '2022-01-01T00:00:00Z', 'milestone2': '2022-01-01T00:01:00Z'},
-        'timeline_url': 'http://example.com/timeline',
-        'keywords_spotted': ['keyword1', 'keyword2'],
-        'call_highlights': [{'start_time': '2022-01-01T00:00:00Z', 'end_time': '2022-01-01T00:01:00Z', 'text': 'highlighted text'}],
-        'agent_email': 'johndoe@example.com',
-        'keypad_entries': {'1': 2, '2': 3}
-    }
-
-    # Exercise
-    call = Call.from_json(api_client, account_id, json_data)
-
-    # Verify
-    assert isinstance(call, Call)
-    assert call.answered == True
-    assert call.business_phone_number == '555-555-5555'
-    assert call.customer_city == 'New York'
-    assert call.customer_country == 'USA'
-    assert call.customer_name == 'John Doe'
-    assert call.customer_phone_number == '555-555-5555'
-    assert call.customer_state == 'NY'
-    assert call.direction == 'inbound'
-    assert call.duration == 60
-    assert call.id == '456'
-    assert call.recording == 'http://example.com/recording.mp3'
-    assert call.recording_duration == '00:01:00'
-    assert call.recording_player == 'http://example.com/recording_player.mp3'
-    assert isinstance(call.start_time, dt.datetime)
-    assert call.start_time.isoformat() == '2022-01-01T00:00:00+00:00'
-    assert call.tracking_phone_number == '555-555-5555'
-    assert call.voicemail == False
-    assert call.call_type == 'sales'
-    assert call.company_id == '789'
-    assert call.company_name == 'Acme Inc.'
-    assert call.company_time_zone == 'America/New_York'
-    assert call.created_at == '2022-01-01T00:00:00Z'
-    assert call.device_type == 'mobile'
-    assert call.first_call == True
-    assert call.formatted_call_type == 'Sales Call'
-    assert call.formatted_customer_location == 'New York, NY, USA'
-    assert call.formatted_business_phone_number == '(555) 555-5555'
-    assert call.formatted_customer_name == 'John Doe'
-    assert call.prior_calls == 2
-    assert call.formatted_customer_name_or_phone_number == '(555) 555-5555'
-    assert call.formatted_customer_phone_number == '(555) 555-5555'
-    assert call.formatted_duration == '1m 0s'
-    assert call.formatted_tracking_phone_number == '(555) 555-5555'
-    assert call.formatted_tracking_source == 'Google Ads'
-    assert call.formatted_value == '$100'
-    assert call.good_lead_call_id == 123
-    assert call.good_lead_call_time == '2022-01-01T00:00:00Z'
-    assert call.lead_status == 'qualified'
-    assert call.note == 'This was a good call.'
-    assert call.source == 'google'
-    assert call.source_name == 'Google Ads'
-    assert call.tags == ['tag1', 'tag2']
-    assert call.total_calls == 10
-    assert call.value == 100
-    assert isinstance(call.waveforms, list)
-    assert call.waveforms == [{'time': 0, 'value': 0}, {'time': 1, 'value': 1}]
-    assert call.tracker_id == 'abc123'
-    assert call.speaker_percent == {'speaker1': 50, 'speaker2': 50}
-    assert call.keywords == 'important keywords'
-    assert call.medium == 'cpc'
-    assert call.campaign == 'campaign1'
-    assert call.referring_url == 'http://example.com/referrer'
-    assert call.landing_page_url == 'http://example.com/landing'
-    assert call.last_requested_url == 'http://example.com/requested'
-    assert call.referrer_domain == 'example.com'
-    assert call.utm_source == 'google'
-    assert call.utm_medium == 'cpc'
-    assert call.utm_term == 'term1'
-    assert call.utm_content == 'content1'
-    assert call.utm_campaign == 'campaign1'
-    assert call.utma == '123456789.1234567890.1234567890.1234567890.1'
-    assert call.utmb == '123456789.1.10.1234567890'
-    assert call.utmc == ''
-    assert call.utmv == ''
-    assert call.utmz == ''
-    assert call.ga == ''
-    assert call.gclid == ''
-    assert call.fbclid == ''
-    assert call.msclkid == ''
-    assert isinstance(call.milestones, dict)
-    assert call.milestones == {'milestone1': '2022-01-01T00:00:00Z', 'milestone2': '2022-01-01T00:01:00Z'}
-    assert call.timeline_url == 'http://example.com/timeline'
-    assert call.keywords_spotted == ['keyword1', 'keyword2']
-    assert isinstance(call.call_highlights, list)
-    assert call.call_highlights == [{'start_time': '2022-01-01T00:00:00Z', 'end_time': '2022-01-01T00:01:00Z', 'text': 'highlighted text'}]
-    assert call.agent_email == 'johndoe@example.com'
-    assert isinstance(call.keypad_entries, dict)
+import pytest
+import pytest_mock
+import requests_mock
+import requests
+
+from pycallrail.callrail import CallRail
+from pycallrail.objects.calls import Call
+import typing
+import logging
+import datetime as dt
+
+# Tests that a Call object can be created with valid arguments. 
+def test_create_call_with_valid_arguments(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    call_data: typing.Dict[str, typing.Any] =  {
+        "answered": False,
+        "business_phone_number": None,
+        "customer_city": "New York City",
+        "customer_country": "US",
+        "customer_name": "Jimmy Pesto, Sr.",
+        "customer_phone_number": "+13036231131",
+        "customer_state": "NY",
+        "direction": "inbound",
+        "duration": 4,
+        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
+        "recording": "https://api.callrail.com/v3/a/227799611/calls/111222333/recording.json",
+        "recording_duration": "27",
+        "recording_player": "https://app.callrail.com/calls/111222333/recording?access_key=3b91eb7f7cc08a4d01ed",
+        "start_time": "2017-01-24T11:27:48.119-05:00",
+        "tracking_phone_number": "+13038163491",
+        "voicemail": False,
+        "agent_email": "gil@televised.com"
+    }
+
+    # Act
+    call = Call(api_client, account_id, **call_data)
+
+    # Assert
+    assert call.answered == call_data['answered']
+    assert call.customer_city == call_data['customer_city']
+    assert call.customer_country == call_data['customer_country']
+    assert call.customer_name == call_data['customer_name']
+    assert call.customer_phone_number == call_data['customer_phone_number']
+    assert call.customer_state == call_data['customer_state']
+    assert call.direction == call_data['direction']
+    assert call.duration == call_data['duration']
+    assert call.id == call_data['id']
+    assert call.start_time == call_data['start_time']
+    assert call.tracking_phone_number == call_data['tracking_phone_number']
+    assert call.voicemail == call_data['voicemail']
+
+# Tests that a Call object can be created with valid arguments. 
+def test_call_creation_two_instances(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    call_data: typing.Dict[str, typing.Any] =  {
+        "answered": False,
+        "business_phone_number": None,
+        "customer_city": "New York City",
+        "customer_country": "US",
+        "customer_name": "Jimmy Pesto, Sr.",
+        "customer_phone_number": "+13036231131",
+        "customer_state": "NY",
+        "direction": "inbound",
+        "duration": 4,
+        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
+        "recording": "https://api.callrail.com/v3/a/227799611/calls/111222333/recording.json",
+        "recording_duration": "27",
+        "recording_player": "https://app.callrail.com/calls/111222333/recording?access_key=3b91eb7f7cc08a4d01ed",
+        "start_time": "2017-01-24T11:27:48.119-05:00",
+        "tracking_phone_number": "+13038163491",
+        "voicemail": False,
+        "agent_email": "gil@televised.com"
+    }
+
+    # Act
+    call = Call(api_client, account_id, **call_data)
+
+    call_data_2: typing.Dict[str, typing.Any] =  {
+        "answered": True,
+        "business_phone_number": None,
+        "customer_city": "Toronto",
+        "customer_country": "CA",
+        "customer_name": "Jimmy Pesto, Sr.",
+        "customer_phone_number": "+13036231131",
+        "customer_state": "NY",
+        "direction": "inbound",
+        "duration": 4,
+        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
+        "recording": "https://api.callrail.com/v3/a/227799611/calls/111222333/recording.json",
+        "recording_duration": "27",
+        "recording_player": "https://app.callrail.com/calls/111222333/recording?access_key=3b91eb7f7cc08a4d01ed",
+        "start_time": "2017-01-24T11:27:48.119-05:00",
+        "tracking_phone_number": "+13038163491",
+        "voicemail": False,
+        "agent_email": "gil@televised.com"
+    }
+
+    call_2 = Call(api_client, account_id, **call_data_2)
+
+    # Assert
+    assert call.answered == call_data['answered']
+    assert call.customer_city == call_data['customer_city']
+    assert call.customer_country == call_data['customer_country']
+    assert call.customer_name == call_data['customer_name']
+    assert call.customer_phone_number == call_data['customer_phone_number']
+    assert call.customer_state == call_data['customer_state']
+    assert call.direction == call_data['direction']
+    assert call.duration == call_data['duration']
+    assert call.id == call_data['id']
+    assert call.start_time == call_data['start_time']
+    assert call.tracking_phone_number == call_data['tracking_phone_number']
+    assert call.voicemail == call_data['voicemail']
+
+    assert call_2.answered == call_data_2['answered']
+    assert call_2.customer_city == call_data_2['customer_city']
+    assert call_2.customer_country == call_data_2['customer_country']
+
+# Tests that a Call object can be updated with valid arguments. 
+def test_update_call_with_valid_arguments(requests_mock: requests_mock.Mocker) -> None:
+    # Arrange
+    api_client = CallRail(api_key='123')
+    account_id = '123'
+    
+    call_data =  {
+        "answered": False,
+        "business_phone_number": None,
+        "customer_city": "Denver",
+        "customer_country": "US",
+        "customer_name": "James Smith",
+        "customer_phone_number": "+13036231131",
+        "customer_state": "CO",
+        "direction": "inbound",
+        "duration": 4,
+        "id": "CAL8154748ae6bd4e278a7cddd38a662f4f",
+        "recording": "https://api.callrail.com/v3/a/227799611/calls/213472384/recording.json",
+        "recording_duration": "27",
+        "start_time": "2017-01-24T11:27:48.119-05:00",
+        "tracking_phone_number": "+13038163491",
+        "voicemail": False
+    }
+
+    call = Call(api_client, account_id, **call_data)
+
+    update_data = {
+        "note": "Call customer back tomorrow",
+        "tags": ["New Client"],
+        "lead_status": "good_lead",
+        "value": "$1.00",
+        "append_tags": True,
+        "customer_name": "James Smith"
+    }
+
+    # Act
+    requests_mock.put(
+        url=f'https://api.callrail.com/v3/a/{account_id}/calls/{call.id}.json',
+        json= call_data 
+    )
+
+
+    call.update(
+        tags = update_data['tags'], 
+        note = update_data['note'], 
+        value = update_data['value'], 
+        append_tags = update_data['append_tags'], 
+        customer_name = update_data['customer_name'])
+
+    # Assert
+    assert call.tags == update_data['tags']
+    assert call.note == update_data['note']
+    assert call.value == update_data['value']
+    assert call.customer_name == update_data['customer_name']
+
+# Tests that a Call object cannot be created with missing or invalid required arguments. 
+def test_create_call_with_invalid_arguments(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    call_data = {
+        "answered": False,
+        "business_phone_number": None,
+        "customer_city": "Denver",
+        "customer_country": "US",
+        "customer_name": "James Smith",
+        "customer_phone_number": "+13036231131",
+        "customer_state": "CO",
+        "direction": "inbound",
+        "duration": 4,
+        "recording": "https://api.callrail.com/v3/a/227799611/calls/213472384/recording.json",
+        "recording_duration": "27",
+        "start_time": "2017-01-24T11:27:48.119-05:00",
+        "tracking_phone_number": "+13038163491",
+        "invalid_argument": True
+    } 
+
+    # Act & Assert
+    with pytest.raises(AttributeError):
+        Call(api_client, account_id, **call_data)
+
+def test_update_call_with_invalid_arguments(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    call_data = {
+        "answered": False,
+        "business_phone_number": None,
+        "customer_city": "Denver",
+        "customer_country": "US",
+        "customer_name": "James Smith",
+        "customer_phone_number": "+13036231131",
+        "customer_state": "CO",
+        "direction": "inbound",
+        "duration": 4,
+        "recording": "https://api.callrail.com/v3/a/227799611/calls/213472384/recording.json",
+        "recording_duration": "27",
+        "start_time": "2017-01-24T11:27:48.119-05:00",
+        "tracking_phone_number": "+13038163491"
+    }
+
+    call = Call(api_client, account_id, **call_data)
+
+    with pytest.raises(Exception):
+        call.update(invalid_argument = True)
+
+# Tests that the recording of a call can be retrieved with a valid recording URL. 
+def test_get_recording_with_valid_recording_url(requests_mock: requests_mock.Mocker) -> None:
+    # Arrange
+    api_client = CallRail(api_key='123')
+    account_id = '123'
+    call_data = {
+        'answered': True,
+        'customer_city': 'New York',
+        'customer_country': 'USA',
+        'customer_name': 'John Doe',
+        'customer_phone_number': '123-456-7890',
+        'customer_state': 'NY',
+        'direction': 'inbound',
+        'duration': 60,
+        'id': '456',
+        'start_time': '2017-01-24T11:27:48.119-05:00',
+        'tracking_phone_number': '987-654-3210',
+        'voicemail': False,
+        'recording': 'http://example.com/recording.mp3'
+    }
+    call = Call(api_client, account_id, **call_data)
+    recording_content = b'This is a recording'
+
+    # Mock the response from the recording URL
+    requests_mock.get(
+        url='http://example.com/recording.mp3',
+        content=recording_content
+    )
+
+    # Act
+    recording = call.get_recording()
+
+    # Assert
+    assert recording == recording_content
+
+# Tests that None is returned when attempting to retrieve the recording of a call with no recording URL. 
+def test_get_recording_with_no_recording_url(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    call_data = {
+        'answered': True,
+        'customer_city': 'New York',
+        'customer_country': 'USA',
+        'customer_name': 'John Doe',
+        'customer_phone_number': '123-456-7890',
+        'customer_state': 'NY',
+        'direction': 'inbound',
+        'duration': 60,
+        'id': '456',
+        'start_time': '2017-01-24T11:27:48.119-05:00',
+        'tracking_phone_number': '987-654-3210',
+        'voicemail': False,
+        'recording': None
+    }
+    call = Call(api_client, account_id, **call_data)
+
+    # Act
+    recording = call.get_recording()
+
+    # Assert
+    assert recording is None
+
+# Tests that JSON data can be successfully deserialized to a Call object.  
+def test_deserialize_json_data_to_call_object(mocker: pytest_mock.MockerFixture) -> None:
+    # Setup
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    json_data = {
+        'answered': True,
+        'business_phone_number': '555-555-5555',
+        'customer_city': 'New York',
+        'customer_country': 'USA',
+        'customer_name': 'John Doe',
+        'customer_phone_number': '555-555-5555',
+        'customer_state': 'NY',
+        'direction': 'inbound',
+        'duration': 60,
+        'id': '456',
+        'recording': 'http://example.com/recording.mp3',
+        'recording_duration': '00:01:00',
+        'recording_player': 'http://example.com/recording_player.mp3',
+        'start_time': '2022-01-01T00:00:00Z',
+        'tracking_phone_number': '555-555-5555',
+        'voicemail': False,
+        'call_type': 'sales',
+        'company_id': '789',
+        'company_name': 'Acme Inc.',
+        'company_time_zone': 'America/New_York',
+        'created_at': '2022-01-01T00:00:00Z',
+        'device_type': 'mobile',
+        'first_call': True,
+        'formatted_call_type': 'Sales Call',
+        'formatted_customer_location': 'New York, NY, USA',
+        'formatted_business_phone_number': '(555) 555-5555',
+        'formatted_customer_name': 'John Doe',
+        'prior_calls': 2,
+        'formatted_customer_name_or_phone_number': '(555) 555-5555',
+        'formatted_customer_phone_number': '(555) 555-5555',
+        'formatted_duration': '1m 0s',
+        'formatted_tracking_phone_number': '(555) 555-5555',
+        'formatted_tracking_source': 'Google Ads',
+        'formatted_value': '$100',
+        'good_lead_call_id': 123,
+        'good_lead_call_time': '2022-01-01T00:00:00Z',
+        'lead_status': 'qualified',
+        'note': 'This was a good call.',
+        'source': 'google',
+        'source_name': 'Google Ads',
+        'tags': ['tag1', 'tag2'],
+        'total_calls': 10,
+        'value': 100,
+        'waveforms': [{'time': 0, 'value': 0}, {'time': 1, 'value': 1}],
+        'tracker_id': 'abc123',
+        'speaker_percent': {'speaker1': 50, 'speaker2': 50},
+        'keywords': 'important keywords',
+        'medium': 'cpc',
+        'campaign': 'campaign1',
+        'referring_url': 'http://example.com/referrer',
+        'landing_page_url': 'http://example.com/landing',
+        'last_requested_url': 'http://example.com/requested',
+        'referrer_domain': 'example.com',
+        'utm_source': 'google',
+        'utm_medium': 'cpc',
+        'utm_term': 'term1',
+        'utm_content': 'content1',
+        'utm_campaign': 'campaign1',
+        'utma': '123456789.1234567890.1234567890.1234567890.1',
+        'utmb': '123456789.1.10.1234567890',
+        'utmc': '',
+        'utmv': '',
+        'utmz': '',
+        'ga': '',
+        'gclid': '',
+        'fbclid': '',
+        'msclkid': '',
+        'milestones': {'milestone1': '2022-01-01T00:00:00Z', 'milestone2': '2022-01-01T00:01:00Z'},
+        'timeline_url': 'http://example.com/timeline',
+        'keywords_spotted': ['keyword1', 'keyword2'],
+        'call_highlights': [{'start_time': '2022-01-01T00:00:00Z', 'end_time': '2022-01-01T00:01:00Z', 'text': 'highlighted text'}],
+        'agent_email': 'johndoe@example.com',
+        'keypad_entries': {'1': 2, '2': 3}
+    }
+
+    # Exercise
+    call = Call.from_json(api_client, account_id, json_data)
+
+    # Verify
+    assert isinstance(call, Call)
+    assert call.answered == True
+    assert call.business_phone_number == '555-555-5555'
+    assert call.customer_city == 'New York'
+    assert call.customer_country == 'USA'
+    assert call.customer_name == 'John Doe'
+    assert call.customer_phone_number == '555-555-5555'
+    assert call.customer_state == 'NY'
+    assert call.direction == 'inbound'
+    assert call.duration == 60
+    assert call.id == '456'
+    assert call.recording == 'http://example.com/recording.mp3'
+    assert call.recording_duration == '00:01:00'
+    assert call.recording_player == 'http://example.com/recording_player.mp3'
+    assert isinstance(call.start_time, dt.datetime)
+    assert call.start_time.isoformat() == '2022-01-01T00:00:00+00:00'
+    assert call.tracking_phone_number == '555-555-5555'
+    assert call.voicemail == False
+    assert call.call_type == 'sales'
+    assert call.company_id == '789'
+    assert call.company_name == 'Acme Inc.'
+    assert call.company_time_zone == 'America/New_York'
+    assert call.created_at == '2022-01-01T00:00:00Z'
+    assert call.device_type == 'mobile'
+    assert call.first_call == True
+    assert call.formatted_call_type == 'Sales Call'
+    assert call.formatted_customer_location == 'New York, NY, USA'
+    assert call.formatted_business_phone_number == '(555) 555-5555'
+    assert call.formatted_customer_name == 'John Doe'
+    assert call.prior_calls == 2
+    assert call.formatted_customer_name_or_phone_number == '(555) 555-5555'
+    assert call.formatted_customer_phone_number == '(555) 555-5555'
+    assert call.formatted_duration == '1m 0s'
+    assert call.formatted_tracking_phone_number == '(555) 555-5555'
+    assert call.formatted_tracking_source == 'Google Ads'
+    assert call.formatted_value == '$100'
+    assert call.good_lead_call_id == 123
+    assert call.good_lead_call_time == '2022-01-01T00:00:00Z'
+    assert call.lead_status == 'qualified'
+    assert call.note == 'This was a good call.'
+    assert call.source == 'google'
+    assert call.source_name == 'Google Ads'
+    assert call.tags == ['tag1', 'tag2']
+    assert call.total_calls == 10
+    assert call.value == 100
+    assert isinstance(call.waveforms, list)
+    assert call.waveforms == [{'time': 0, 'value': 0}, {'time': 1, 'value': 1}]
+    assert call.tracker_id == 'abc123'
+    assert call.speaker_percent == {'speaker1': 50, 'speaker2': 50}
+    assert call.keywords == 'important keywords'
+    assert call.medium == 'cpc'
+    assert call.campaign == 'campaign1'
+    assert call.referring_url == 'http://example.com/referrer'
+    assert call.landing_page_url == 'http://example.com/landing'
+    assert call.last_requested_url == 'http://example.com/requested'
+    assert call.referrer_domain == 'example.com'
+    assert call.utm_source == 'google'
+    assert call.utm_medium == 'cpc'
+    assert call.utm_term == 'term1'
+    assert call.utm_content == 'content1'
+    assert call.utm_campaign == 'campaign1'
+    assert call.utma == '123456789.1234567890.1234567890.1234567890.1'
+    assert call.utmb == '123456789.1.10.1234567890'
+    assert call.utmc == ''
+    assert call.utmv == ''
+    assert call.utmz == ''
+    assert call.ga == ''
+    assert call.gclid == ''
+    assert call.fbclid == ''
+    assert call.msclkid == ''
+    assert isinstance(call.milestones, dict)
+    assert call.milestones == {'milestone1': '2022-01-01T00:00:00Z', 'milestone2': '2022-01-01T00:01:00Z'}
+    assert call.timeline_url == 'http://example.com/timeline'
+    assert call.keywords_spotted == ['keyword1', 'keyword2']
+    assert isinstance(call.call_highlights, list)
+    assert call.call_highlights == [{'start_time': '2022-01-01T00:00:00Z', 'end_time': '2022-01-01T00:01:00Z', 'text': 'highlighted text'}]
+    assert call.agent_email == 'johndoe@example.com'
+    assert isinstance(call.keypad_entries, dict)
     assert call.keypad_entries == {'1': 2, '2': 3}
```

### Comparing `pycallrail-0.9.0.0/tests/test_companies.py` & `pycallrail-0.9.0.1/tests/test_companies.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-import pytest
-import pytest_mock
-import requests_mock
-import requests
-
-from pycallrail.callrail import CallRail
-from pycallrail.objects.companies import Company
-import typing
-import logging
-import datetime as dt
-
-# Tests creating a Company object with valid parameters. 
-def test_create_company_valid_params(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    company_data = {
-        "id": "COM8154748ae6bd4e278a7cddd38a662f4f",
-        "name": "Widget Shop",
-        "status": "active",
-        "time_zone": "America/New_York",
-        "created_at": "2017-01-26T22:58:04.184Z",
-        "disabled_at": None,
-        "dni_active": None,
-        "script_url": "//cdn.callrail.com/companies/279054151/a74c824140d67442debd/12/swap.js",
-        "callscribe_enabled": False,
-        "lead_scoring_enabled": False,
-        "swap_exclude_jquery": None,
-        "swap_ppc_override": None,
-        "swap_landing_override": None,
-        "swap_cookie_duration": 365,
-        "callscore_enabled": False,
-        "keyword_spotting_enabled": False
-    }
-
-    # Act
-    company = Company(api_client, account_id, **company_data)
-
-    # Assert
-    assert company.id == company_data['id']
-    assert company.name == company_data['name']
-    assert company.status == company_data['status']
-    assert company.time_zone == company_data['time_zone']
-    assert company.created_at == company_data['created_at']
-    assert company.disabled_at == company_data['disabled_at']
-    assert company.dni_active == company_data['dni_active']
-    assert company.script_url == company_data['script_url']
-    assert company.callscore_enabled == company_data['callscore_enabled']
-    assert company.lead_scoring_enabled == company_data['lead_scoring_enabled']
-    assert company.swap_exclude_jquery == company_data['swap_exclude_jquery']
-    assert company.swap_ppc_override == company_data['swap_ppc_override']
-    assert company.swap_landing_override == company_data['swap_landing_override']
-    assert company.swap_cookie_duration == company_data['swap_cookie_duration']
-    assert company.callscribe_enabled == company_data['callscribe_enabled']
-    assert company.keyword_spotting_enabled == company_data['keyword_spotting_enabled']
-
-# Tests updating a Company object with valid parameters. 
-def test_update_company_valid_params(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    company_data = {
-        "id": "COM8154748ae6bd4e278a7cddd38a662f4f",
-        "name": "Widget Shop",
-        "status": "active",
-        "time_zone": "America/New_York",
-        "created_at": "2017-01-26T22:58:04.184Z",
-        "disabled_at": None,
-        "dni_active": None,
-        "script_url": "//cdn.callrail.com/companies/279054151/a74c824140d67442debd/12/swap.js",
-        "callscribe_enabled": False,
-        "lead_scoring_enabled": False,
-        "swap_exclude_jquery": None,
-        "swap_ppc_override": None,
-        "swap_landing_override": None,
-        "swap_cookie_duration": 365,
-        "callscore_enabled": False,
-        "keyword_spotting_enabled": False
-    }
-    company = Company(api_client, account_id, **company_data)
-
-    updated_name = 'Updated Company Name'
-
-    # Act
-    company.update(name=updated_name)
-
-    # Assert
-    assert company.name == updated_name
-
-# Tests creating a Company object with missing parameters. 
-def test_create_company_missing_params(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    # Act and Assert
-    with pytest.raises(TypeError):
-        Company(api_client, account_id)
-
-# Tests creating a Company object with invalid parameters. 
-def test_create_company_invalid_params(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock()
-    account_id = '123'
-
-    # Act and Assert
-    with pytest.raises(AttributeError):
-        Company(api_client, account_id, invalid_param='invalid')
-
-# Tests deleting a Company object successfully. 
-def test_delete_company(mocker: pytest_mock.MockerFixture):
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    company_data = {
-        'id': '456',
-        'name': 'Test Company',
-        'status': 'active',
-        'time_zone': 'America/New_York',
-        'created_at': dt.datetime.now(),
-        'disabled_at': None,
-        'dni_active': False,
-        'script_url': 'https://example.com/script.js',
-        'callscore_enabled': True,
-        'lead_scoring_enabled': False,
-        'swap_exclude_jquery': None,
-        'swap_ppc_override': None,
-        'swap_landing_override': None,
-        'swap_cookie_duration': None,
-        'callscribe_enabled': True,
-        'keyword_spotting_enabled': None,
-        'form_capture': True
-    }
-    company = Company(api_client, account_id, **company_data)
-
-    # Act
-    company.delete()
-
-    # Assert
+import pytest
+import pytest_mock
+import requests_mock
+import requests
+
+from pycallrail.callrail import CallRail
+from pycallrail.objects.companies import Company
+import typing
+import logging
+import datetime as dt
+
+# Tests creating a Company object with valid parameters. 
+def test_create_company_valid_params(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    company_data = {
+        "id": "COM8154748ae6bd4e278a7cddd38a662f4f",
+        "name": "Widget Shop",
+        "status": "active",
+        "time_zone": "America/New_York",
+        "created_at": "2017-01-26T22:58:04.184Z",
+        "disabled_at": None,
+        "dni_active": None,
+        "script_url": "//cdn.callrail.com/companies/279054151/a74c824140d67442debd/12/swap.js",
+        "callscribe_enabled": False,
+        "lead_scoring_enabled": False,
+        "swap_exclude_jquery": None,
+        "swap_ppc_override": None,
+        "swap_landing_override": None,
+        "swap_cookie_duration": 365,
+        "callscore_enabled": False,
+        "keyword_spotting_enabled": False
+    }
+
+    # Act
+    company = Company(api_client, account_id, **company_data)
+
+    # Assert
+    assert company.id == company_data['id']
+    assert company.name == company_data['name']
+    assert company.status == company_data['status']
+    assert company.time_zone == company_data['time_zone']
+    assert company.created_at == company_data['created_at']
+    assert company.disabled_at == company_data['disabled_at']
+    assert company.dni_active == company_data['dni_active']
+    assert company.script_url == company_data['script_url']
+    assert company.callscore_enabled == company_data['callscore_enabled']
+    assert company.lead_scoring_enabled == company_data['lead_scoring_enabled']
+    assert company.swap_exclude_jquery == company_data['swap_exclude_jquery']
+    assert company.swap_ppc_override == company_data['swap_ppc_override']
+    assert company.swap_landing_override == company_data['swap_landing_override']
+    assert company.swap_cookie_duration == company_data['swap_cookie_duration']
+    assert company.callscribe_enabled == company_data['callscribe_enabled']
+    assert company.keyword_spotting_enabled == company_data['keyword_spotting_enabled']
+
+# Tests updating a Company object with valid parameters. 
+def test_update_company_valid_params(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    company_data = {
+        "id": "COM8154748ae6bd4e278a7cddd38a662f4f",
+        "name": "Widget Shop",
+        "status": "active",
+        "time_zone": "America/New_York",
+        "created_at": "2017-01-26T22:58:04.184Z",
+        "disabled_at": None,
+        "dni_active": None,
+        "script_url": "//cdn.callrail.com/companies/279054151/a74c824140d67442debd/12/swap.js",
+        "callscribe_enabled": False,
+        "lead_scoring_enabled": False,
+        "swap_exclude_jquery": None,
+        "swap_ppc_override": None,
+        "swap_landing_override": None,
+        "swap_cookie_duration": 365,
+        "callscore_enabled": False,
+        "keyword_spotting_enabled": False
+    }
+    company = Company(api_client, account_id, **company_data)
+
+    updated_name = 'Updated Company Name'
+
+    # Act
+    company.update(name=updated_name)
+
+    # Assert
+    assert company.name == updated_name
+
+# Tests creating a Company object with missing parameters. 
+def test_create_company_missing_params(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    # Act and Assert
+    with pytest.raises(TypeError):
+        Company(api_client, account_id)
+
+# Tests creating a Company object with invalid parameters. 
+def test_create_company_invalid_params(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock()
+    account_id = '123'
+
+    # Act and Assert
+    with pytest.raises(AttributeError):
+        Company(api_client, account_id, invalid_param='invalid')
+
+# Tests deleting a Company object successfully. 
+def test_delete_company(mocker: pytest_mock.MockerFixture):
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    company_data = {
+        'id': '456',
+        'name': 'Test Company',
+        'status': 'active',
+        'time_zone': 'America/New_York',
+        'created_at': dt.datetime.now(),
+        'disabled_at': None,
+        'dni_active': False,
+        'script_url': 'https://example.com/script.js',
+        'callscore_enabled': True,
+        'lead_scoring_enabled': False,
+        'swap_exclude_jquery': None,
+        'swap_ppc_override': None,
+        'swap_landing_override': None,
+        'swap_cookie_duration': None,
+        'callscribe_enabled': True,
+        'keyword_spotting_enabled': None,
+        'form_capture': True
+    }
+    company = Company(api_client, account_id, **company_data)
+
+    # Act
+    company.delete()
+
+    # Assert
     api_client._delete.assert_called_once_with(endpoint=f'/a/{account_id}', path=f'/companies/{company.id}.json')
```

### Comparing `pycallrail-0.9.0.0/tests/test_helpers.py` & `pycallrail-0.9.0.1/tests/test_helpers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import pytest
-import pytest_mock
-import typing
-from pycallrail.helpers import build_url
-
-# Tests that the function returns a valid URL string when base_url and endpoint are valid strings. 
-def test_happy_path_build_url() -> None:
-    # Arrange
-    base_url = "https://api.callrail.com/v3/"
-    endpoint = "a.json"
-    expected_url = "https://api.callrail.com/v3/a.json"
-
-    # Act
-    actual_url: str = build_url(base_url, endpoint)
-
-    # Assert
-    assert actual_url == expected_url
-
-# Tests that the function handles an empty string for base_url or endpoint. 
-def test_edge_case_empty_strings() -> None:
-    # Arrange
-    base_url: typing.Literal[''] = ""
-    endpoint = "/api/v1/users"
-    expected_url = "/api/v1/users"
-
-    # Act
-    actual_url: str = build_url(base_url, endpoint)
-
-    # Assert
-    assert actual_url == expected_url
-
-# Tests that the function handles a path that starts with a leading slash. 
-def test_edge_case_leading_slash() -> None:
-    # Arrange
-    base_url = "https://www.example.com"
-    endpoint = "/api/v1/users"
-    path = "/profile"
-    expected_url = "https://www.example.com/api/v1/users/profile"
-
-    # Act
-    actual_url: str = build_url(base_url, endpoint, path)
-
-    # Assert
-    assert actual_url == expected_url
-
-# Tests that the function handles query parameters in the URL. 
-def test_general_behavior_query_parameters() -> None:
-    # Arrange
-    base_url = "https://www.example.com"
-    endpoint = "/api/v1/users"
-    query_params: dict[str, str] = {"sort": "name", "filter": "active"}
-    expected_url = "https://www.example.com/api/v1/users?sort=name&filter=active"
-
-    # Act
-    actual_url: str = build_url(base_url, endpoint, None)
-    actual_url += "?" + "&".join([f"{k}={v}" for k, v in query_params.items()])
-
-    # Assert
-    assert actual_url == expected_url
-
-# Tests that the function handles trailing slashes correctly for endpoint and path. 
-def test_edge_case_trailing_slashes() -> None:
-    # Arrange
-    base_url = "https://www.example.com/"
-    endpoint = "/api/v1/users/"
-    path = "/profile/"
-    expected_url = "https://www.example.com/api/v1/users/profile/"
-
-    # Act
-    actual_url: str = build_url(base_url, endpoint, path)
-
-    # Assert
-    assert actual_url == expected_url
-
-# Tests that the function handles special characters in the URL. 
-def test_general_behavior_special_characters() -> None:
-    # Arrange
-    base_url = "https://www.example.com"
-    endpoint = "/api/v1/users"
-    path = "/profile?name=John&age=30"
-    expected_url = "https://www.example.com/api/v1/users/profile?name=John&age=30"
-
-    # Act
-    actual_url: str = build_url(base_url, endpoint, path)
-
-    # Assert
+import pytest
+import pytest_mock
+import typing
+from pycallrail.helpers import build_url
+
+# Tests that the function returns a valid URL string when base_url and endpoint are valid strings. 
+def test_happy_path_build_url() -> None:
+    # Arrange
+    base_url = "https://api.callrail.com/v3/"
+    endpoint = "a.json"
+    expected_url = "https://api.callrail.com/v3/a.json"
+
+    # Act
+    actual_url: str = build_url(base_url, endpoint)
+
+    # Assert
+    assert actual_url == expected_url
+
+# Tests that the function handles an empty string for base_url or endpoint. 
+def test_edge_case_empty_strings() -> None:
+    # Arrange
+    base_url: typing.Literal[''] = ""
+    endpoint = "/api/v1/users"
+    expected_url = "/api/v1/users"
+
+    # Act
+    actual_url: str = build_url(base_url, endpoint)
+
+    # Assert
+    assert actual_url == expected_url
+
+# Tests that the function handles a path that starts with a leading slash. 
+def test_edge_case_leading_slash() -> None:
+    # Arrange
+    base_url = "https://www.example.com"
+    endpoint = "/api/v1/users"
+    path = "/profile"
+    expected_url = "https://www.example.com/api/v1/users/profile"
+
+    # Act
+    actual_url: str = build_url(base_url, endpoint, path)
+
+    # Assert
+    assert actual_url == expected_url
+
+# Tests that the function handles query parameters in the URL. 
+def test_general_behavior_query_parameters() -> None:
+    # Arrange
+    base_url = "https://www.example.com"
+    endpoint = "/api/v1/users"
+    query_params: dict[str, str] = {"sort": "name", "filter": "active"}
+    expected_url = "https://www.example.com/api/v1/users?sort=name&filter=active"
+
+    # Act
+    actual_url: str = build_url(base_url, endpoint, None)
+    actual_url += "?" + "&".join([f"{k}={v}" for k, v in query_params.items()])
+
+    # Assert
+    assert actual_url == expected_url
+
+# Tests that the function handles trailing slashes correctly for endpoint and path. 
+def test_edge_case_trailing_slashes() -> None:
+    # Arrange
+    base_url = "https://www.example.com/"
+    endpoint = "/api/v1/users/"
+    path = "/profile/"
+    expected_url = "https://www.example.com/api/v1/users/profile/"
+
+    # Act
+    actual_url: str = build_url(base_url, endpoint, path)
+
+    # Assert
+    assert actual_url == expected_url
+
+# Tests that the function handles special characters in the URL. 
+def test_general_behavior_special_characters() -> None:
+    # Arrange
+    base_url = "https://www.example.com"
+    endpoint = "/api/v1/users"
+    path = "/profile?name=John&age=30"
+    expected_url = "https://www.example.com/api/v1/users/profile?name=John&age=30"
+
+    # Act
+    actual_url: str = build_url(base_url, endpoint, path)
+
+    # Assert
     assert actual_url == expected_url
```

### Comparing `pycallrail-0.9.0.0/tests/test_integration.py` & `pycallrail-0.9.0.1/tests/test_integration.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import pytest
-import pytest_mock
-
-import os
-import typing
-from pycallrail.callrail import CallRail
-from pycallrail.objects.accounts import Account
-from pycallrail.objects.calls import Call
-from pycallrail.objects.companies import Company
-from pycallrail.objects.form_submissions import FormSubmission
-from pycallrail.objects.textmessages import TextMessageConversation
-import logging
-
-
-@pytest.fixture(scope='module')
-def callrail() -> typing.Generator[CallRail, None, None]:
-    if os.getenv('CALLRAIL_API_KEY'):
-        api_key: str = os.getenv('CALLRAIL_API_KEY')
-    else:
-        from . import cfg
-        api_key = cfg.CALLRAIL_API_KEY
-
-    yield CallRail(api_key)
-
-@pytest.mark.integration
-def test_list_accounts(callrail: CallRail) -> None:
-    
-    accounts = callrail.list_accounts()
-
-
-    assert isinstance(accounts, list)
-    assert isinstance(accounts[0], Account)
-    
-    # assert there are attributes in the response
-    assert hasattr(accounts[0], 'id')
-    assert hasattr(accounts[0], 'name')
-
-@pytest.mark.integration
-def test_list_calls(callrail: CallRail) -> None:
-
-    accounts: typing.List[Account] = callrail.list_accounts()
-    account: Account = accounts[0]
-
-    calls: typing.List[Call] = account.list_calls()
-
-    assert isinstance(calls, list)
-    assert isinstance(calls[0], Call)
-
-    # assert there are attributes in the response
-    assert hasattr(calls[0], 'id')
-    assert hasattr(calls[0], 'account_id')
-
-
-@pytest.mark.integration
-def test_list_companies(callrail: CallRail) -> None:
-
-    accounts = callrail.list_accounts()
-    account: Account = accounts[0]
-    
-    companies: typing.List[Account] = account.list_companies()
-
-    assert isinstance(companies, list)
-    assert isinstance(companies[0], Company)
-
-    # assert there are attributes in the response
-    assert hasattr(companies[0], 'id')
-    assert hasattr(companies[0], 'name')
-
-@pytest.mark.integration
-def test_formsubmission(callrail: CallRail) -> None:
-
-    accounts = callrail.list_accounts()
-    account: Account = accounts[0]
-    
-    form_submissions: typing.List[FormSubmission] = account.list_form_submissions()
-    
-    assert isinstance(form_submissions, list)
-    assert isinstance(form_submissions[0], FormSubmission)
-    
-    # assert there are attributes in the response
-    assert hasattr(form_submissions[0], 'id')
-    assert hasattr(form_submissions[0], 'account_id')
-    assert hasattr(form_submissions[0], 'form_data')
-
-@pytest.mark.integration
-def test_list_text_messages(callrail: CallRail) -> None:
-
-    accounts = callrail.list_accounts()
-    account: Account = accounts[0]
-    
-    text_messages: typing.List[TextMessageConversation] = account.list_text_message_conversations()
-    
-    assert isinstance(text_messages, list)
-    assert isinstance(text_messages[0], TextMessageConversation)
-    
-    # assert there are attributes in the response
-    assert hasattr(text_messages[0], 'id')
-    assert hasattr(text_messages[0], 'account_id')
+import pytest
+import pytest_mock
+
+import os
+import typing
+from pycallrail.callrail import CallRail
+from pycallrail.objects.accounts import Account
+from pycallrail.objects.calls import Call
+from pycallrail.objects.companies import Company
+from pycallrail.objects.form_submissions import FormSubmission
+from pycallrail.objects.textmessages import TextMessageConversation
+import logging
+
+
+@pytest.fixture(scope='module')
+def callrail() -> typing.Generator[CallRail, None, None]:
+    if os.getenv('CALLRAIL_API_KEY'):
+        api_key: str = os.getenv('CALLRAIL_API_KEY')
+    else:
+        from . import cfg
+        api_key = cfg.CALLRAIL_API_KEY
+
+    yield CallRail(api_key)
+
+@pytest.mark.integration
+def test_list_accounts(callrail: CallRail) -> None:
+    
+    accounts = callrail.list_accounts()
+
+
+    assert isinstance(accounts, list)
+    assert isinstance(accounts[0], Account)
+    
+    # assert there are attributes in the response
+    assert hasattr(accounts[0], 'id')
+    assert hasattr(accounts[0], 'name')
+
+@pytest.mark.integration
+def test_list_calls(callrail: CallRail) -> None:
+
+    accounts: typing.List[Account] = callrail.list_accounts()
+    account: Account = accounts[0]
+
+    calls: typing.List[Call] = account.list_calls()
+
+    assert isinstance(calls, list)
+    assert isinstance(calls[0], Call)
+
+    # assert there are attributes in the response
+    assert hasattr(calls[0], 'id')
+    assert hasattr(calls[0], 'account_id')
+
+
+@pytest.mark.integration
+def test_list_companies(callrail: CallRail) -> None:
+
+    accounts = callrail.list_accounts()
+    account: Account = accounts[0]
+    
+    companies: typing.List[Account] = account.list_companies()
+
+    assert isinstance(companies, list)
+    assert isinstance(companies[0], Company)
+
+    # assert there are attributes in the response
+    assert hasattr(companies[0], 'id')
+    assert hasattr(companies[0], 'name')
+
+@pytest.mark.integration
+def test_formsubmission(callrail: CallRail) -> None:
+
+    accounts = callrail.list_accounts()
+    account: Account = accounts[0]
+    
+    form_submissions: typing.List[FormSubmission] = account.list_form_submissions()
+    
+    assert isinstance(form_submissions, list)
+    assert isinstance(form_submissions[0], FormSubmission)
+    
+    # assert there are attributes in the response
+    assert hasattr(form_submissions[0], 'id')
+    assert hasattr(form_submissions[0], 'account_id')
+    assert hasattr(form_submissions[0], 'form_data')
+
+@pytest.mark.integration
+def test_list_text_messages(callrail: CallRail) -> None:
+
+    accounts = callrail.list_accounts()
+    account: Account = accounts[0]
+    
+    text_messages: typing.List[TextMessageConversation] = account.list_text_message_conversations()
+    
+    assert isinstance(text_messages, list)
+    assert isinstance(text_messages[0], TextMessageConversation)
+    
+    # assert there are attributes in the response
+    assert hasattr(text_messages[0], 'id')
+    assert hasattr(text_messages[0], 'account_id')
     assert hasattr(text_messages[0], 'recent_messages')
```

### Comparing `pycallrail-0.9.0.0/tests/test_tags.py` & `pycallrail-0.9.0.1/tests/test_tags.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import pytest
-import pytest_mock
-import requests_mock
-import requests
-
-from pycallrail.callrail import CallRail
-from pycallrail.objects.tags import Tag
-import typing
-import logging
-import datetime as dt
-import typeguard
-
-# Tests creating a Tag object with valid input parameters. 
-def test_create_tag_valid_input(mocker: pytest_mock.MockerFixture):
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    
-    account_id = "123ABC"
-
-    json_data: typing.Dict[str, typing.Any] = {
-        "id": 1234569,
-        "name": "Existing Customer",
-        "tag_level": "company",
-        "color": "gray1",
-        "background_color": "gray1",
-        "company_id": "COM8154748ae6bd4e278a7cddd38a662f4f",
-        "status": "enabled",
-        "created_at": "2014-06-06T12:11:02.964-04:00"
-    }
-
-    api_client._post.return_value = json_data
-
-    # Act
-    tag = Tag.from_json(api_client, account_id, json_data)
-
-    # Assert
-    assert tag.id == json_data["id"]
-    assert tag.name == json_data["name"]
-    assert tag.tag_level == json_data["tag_level"]
-    assert tag.color == json_data["color"]
-    assert tag.background_color == json_data["background_color"]
-    assert tag.company_id == json_data["company_id"]
-    assert tag.status ==   json_data["status"]
-    assert tag.created_at == json_data["created_at"]
-    assert isinstance(tag.created_at, dt.datetime)
-
-# Tests updating a Tag object with valid input parameters. 
-def test_update_tag_valid_input(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-
-    account_id = '123ABC'
-    id = 1234569
-    name = 'Existing Customer - Old Name'
-    tag_level = 'company'
-    color = 'gray2'
-    background_color = 'gray1'
-    company_id = 'COM8154748ae6bd4e278a7cddd38a662f4f'
-    status = 'enabled'
-    created_at: dt.datetime = dt.datetime.now()
-
-    update_data: typing.Dict[str, str] = {
-           "name": "Existing Customer",
-           "color": "gray1"
-    }
-
-    json_data: typing.Dict[str, str] = {
-        "id": "1234569",
-        "name": "Existing Customer",
-        "tag_level": "company",
-        "color": "gray1",
-        "background_color": "gray1",
-        "company_id": "COM8154748ae6bd4e278a7cddd38a662f4f",
-        "status": "enabled",
-        "created_at": "2014-06-06T12:11:02.964-04:00"
-    }
-
-    api_client._put.return_value = json_data
-
-    tag = Tag(api_client, account_id, id, name, tag_level, color, background_color, company_id, status, created_at)
-
-    # Act
-    tag.update(name=update_data["name"], color=update_data["color"])
-
-    # Assert
-    assert tag.name == update_data["name"]
-    assert tag.color == update_data["color"]
-    
-# Tests creating a Tag object with invalid input parameters. 
-def test_create_tag_invalid_input(mocker: pytest_mock.MockerFixture) -> None:
-    # Arrange
-    api_client = mocker.Mock(spec=CallRail)
-    account_id = '123'
-    id = 1
-    name = None
-    tag_level = 'company'
-    color = '#FFFFFF'
-    background_color = '#000000'
-    company_id = '456'
-    status = 'active'
-    created_at: dt.datetime = dt.datetime.now()
-
-    json_data: typing.Dict[str, typing.Any] = {
-        'id': id,
-        'name': name,
-        'tag_level': tag_level,
-        'color': color,
-        'background_color': background_color,
-        'company_id': company_id,
-        'status': status,
-        'created_at': created_at.isoformat()
-    }
-
-    api_client._post.return_value = json_data
-
-    # Act and Assert
-    with pytest.raises(typeguard.TypeCheckError):
-        Tag.from_json(api_client, account_id, json_data)
-
-# Tests deleting a Tag object. 
-def test_delete_tag(mocker: pytest_mock.MockerFixture):
-    # Arrange
-    api_client = mocker.Mock()
-    account_id = '123'
-    id = 1
-    name = 'Test Tag'
-    tag_level = 'company'
-    color = '#FFFFFF'
-    background_color = '#000000'
-    company_id = '456'
-    status = 'active'
-    created_at: dt.datetime = dt.datetime.now()
-
-    tag = Tag(api_client, account_id, id, name, tag_level, color, background_color, company_id, status, created_at)
-
-    # Act
-    tag.delete()
-
-    # Assert
-    api_client._delete.assert_called_once_with(endpoint=f'a/{account_id}', path=f'tags/{id}.json')
-
-# Tests deleting a non-existent Tag object. 
-def test_delete_nonexistent_tag(mocker: pytest_mock.MockerFixture):
-    # Arrange
-    api_client = mocker.Mock()
-    account_id = '123'
-    id = 1
-    name = 'Test Tag'
-    tag_level = 'company'
-    color = '#FFFFFF'
-    background_color = '#000000'
-    company_id = '456'
-    status = 'active'
-    created_at = dt.datetime.now()
-
-    tag = Tag(api_client, account_id, id, name, tag_level, color, background_color, company_id, status, created_at)
-
-    api_client._delete.side_effect = Exception('Tag not found')
-
-    # Act and Assert
-    with pytest.raises(Exception):
+import pytest
+import pytest_mock
+import requests_mock
+import requests
+
+from pycallrail.callrail import CallRail
+from pycallrail.objects.tags import Tag
+import typing
+import logging
+import datetime as dt
+import typeguard
+
+# Tests creating a Tag object with valid input parameters. 
+def test_create_tag_valid_input(mocker: pytest_mock.MockerFixture):
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    
+    account_id = "123ABC"
+
+    json_data: typing.Dict[str, typing.Any] = {
+        "id": 1234569,
+        "name": "Existing Customer",
+        "tag_level": "company",
+        "color": "gray1",
+        "background_color": "gray1",
+        "company_id": "COM8154748ae6bd4e278a7cddd38a662f4f",
+        "status": "enabled",
+        "created_at": "2014-06-06T12:11:02.964-04:00"
+    }
+
+    api_client._post.return_value = json_data
+
+    # Act
+    tag = Tag.from_json(api_client, account_id, json_data)
+
+    # Assert
+    assert tag.id == json_data["id"]
+    assert tag.name == json_data["name"]
+    assert tag.tag_level == json_data["tag_level"]
+    assert tag.color == json_data["color"]
+    assert tag.background_color == json_data["background_color"]
+    assert tag.company_id == json_data["company_id"]
+    assert tag.status ==   json_data["status"]
+    assert tag.created_at == json_data["created_at"]
+    assert isinstance(tag.created_at, dt.datetime)
+
+# Tests updating a Tag object with valid input parameters. 
+def test_update_tag_valid_input(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+
+    account_id = '123ABC'
+    id = 1234569
+    name = 'Existing Customer - Old Name'
+    tag_level = 'company'
+    color = 'gray2'
+    background_color = 'gray1'
+    company_id = 'COM8154748ae6bd4e278a7cddd38a662f4f'
+    status = 'enabled'
+    created_at: dt.datetime = dt.datetime.now()
+
+    update_data: typing.Dict[str, str] = {
+           "name": "Existing Customer",
+           "color": "gray1"
+    }
+
+    json_data: typing.Dict[str, str] = {
+        "id": "1234569",
+        "name": "Existing Customer",
+        "tag_level": "company",
+        "color": "gray1",
+        "background_color": "gray1",
+        "company_id": "COM8154748ae6bd4e278a7cddd38a662f4f",
+        "status": "enabled",
+        "created_at": "2014-06-06T12:11:02.964-04:00"
+    }
+
+    api_client._put.return_value = json_data
+
+    tag = Tag(api_client, account_id, id, name, tag_level, color, background_color, company_id, status, created_at)
+
+    # Act
+    tag.update(name=update_data["name"], color=update_data["color"])
+
+    # Assert
+    assert tag.name == update_data["name"]
+    assert tag.color == update_data["color"]
+    
+# Tests creating a Tag object with invalid input parameters. 
+def test_create_tag_invalid_input(mocker: pytest_mock.MockerFixture) -> None:
+    # Arrange
+    api_client = mocker.Mock(spec=CallRail)
+    account_id = '123'
+    id = 1
+    name = None
+    tag_level = 'company'
+    color = '#FFFFFF'
+    background_color = '#000000'
+    company_id = '456'
+    status = 'active'
+    created_at: dt.datetime = dt.datetime.now()
+
+    json_data: typing.Dict[str, typing.Any] = {
+        'id': id,
+        'name': name,
+        'tag_level': tag_level,
+        'color': color,
+        'background_color': background_color,
+        'company_id': company_id,
+        'status': status,
+        'created_at': created_at.isoformat()
+    }
+
+    api_client._post.return_value = json_data
+
+    # Act and Assert
+    with pytest.raises(typeguard.TypeCheckError):
+        Tag.from_json(api_client, account_id, json_data)
+
+# Tests deleting a Tag object. 
+def test_delete_tag(mocker: pytest_mock.MockerFixture):
+    # Arrange
+    api_client = mocker.Mock()
+    account_id = '123'
+    id = 1
+    name = 'Test Tag'
+    tag_level = 'company'
+    color = '#FFFFFF'
+    background_color = '#000000'
+    company_id = '456'
+    status = 'active'
+    created_at: dt.datetime = dt.datetime.now()
+
+    tag = Tag(api_client, account_id, id, name, tag_level, color, background_color, company_id, status, created_at)
+
+    # Act
+    tag.delete()
+
+    # Assert
+    api_client._delete.assert_called_once_with(endpoint=f'a/{account_id}', path=f'tags/{id}.json')
+
+# Tests deleting a non-existent Tag object. 
+def test_delete_nonexistent_tag(mocker: pytest_mock.MockerFixture):
+    # Arrange
+    api_client = mocker.Mock()
+    account_id = '123'
+    id = 1
+    name = 'Test Tag'
+    tag_level = 'company'
+    color = '#FFFFFF'
+    background_color = '#000000'
+    company_id = '456'
+    status = 'active'
+    created_at = dt.datetime.now()
+
+    tag = Tag(api_client, account_id, id, name, tag_level, color, background_color, company_id, status, created_at)
+
+    api_client._delete.side_effect = Exception('Tag not found')
+
+    # Act and Assert
+    with pytest.raises(Exception):
         tag.delete()
```

### Comparing `pycallrail-0.9.0.0/tests/test_textmessages.py` & `pycallrail-0.9.0.1/tests/test_textmessages.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-import pytest
-import pytest_mock
-import requests_mock
-import requests
-
-from pycallrail.callrail import CallRail
-from pycallrail.objects.textmessages import TextMessage, TextMessageConversation
-import typing
-import logging
-import datetime as dt
-import typeguard
-import dataclasses
-
-# Tests that a TextMessage object can be created with valid parameters. 
-def test_creating_valid_text_message() -> None:
-    direction = "outgoing"
-    content = "Hello, this is a test message."
-    created_at: dt.datetime = dt.datetime.now()
-    text_message = TextMessage(direction=direction, content=content, created_at=created_at)
-    assert text_message.direction == direction
-    assert text_message.content == content
-    assert text_message.created_at == created_at
-
-# Tests that a TextMessage object cannot be created with empty string parameters. 
-def test_empty_string_parameters() -> None:
-    with pytest.raises(ValueError):
-        direction = ""
-        content = "Hello, this is a test message."
-        created_at: dt.datetime = dt.datetime.now()
-        TextMessage(direction=direction, content=content, created_at=created_at)
-
-# Tests that a TextMessage object cannot be created with an invalid datetime format. 
-def test_invalid_datetime_format() -> None:
-    with pytest.raises(ValueError):
-        direction = "outgpomg"
-        content = "Hello, this is a test message."
-        created_at = "2022-13-01 12:00:00"
-        TextMessage(direction=direction, content=content, created_at=created_at)
-
-# Tests that accessing the id attribute of a TextMessage object that has not been set returns None. 
-def test_accessing_unset_id_attribute() -> None:
-    text_message = TextMessage(
-        direction="outgoing", 
-        content="Hello, this is a test message.", 
-        created_at=dt.datetime.now())
-    assert text_message.id is None
-
-# Tests archiving a TextMessageConversation. 
-def test_archive_conversation(mocker: pytest_mock.MockerFixture) -> None:
-    # Happy path test for archiving a TextMessageConversation
-    api_client = CallRail('test_key')
-    account_id = 'test_account'
-    conversation_id = 'test_conversation'
-    conversation_data: typing.Dict[str, str] = {
-        'id': conversation_id,
-        'state': 'active'
-    }
-    conversation = TextMessageConversation(api_client, account_id, **conversation_data)
-
-    # Mock the _put method of the api_client to simulate a successful archive request
-    mocker.patch.object(api_client, '_put', return_value=None)
-
-    conversation.archive()
-
-    assert conversation.state == 'archived'
-
-# Tests creating a TextMessageConversation object with valid arguments. 
-def test_create_text_message_conversation_valid_args() -> None:
-    # Happy path test for creating a TextMessageConversation with valid arguments
-    api_client = CallRail('test_key')
-    account_id = 'test_account'
-    conversation_data: typing.Dict[str, typing.Any] = {
-        'id': 'test_conversation',
-        'company_id': 'test_company',
-        'initial_tracker_id': 'test_initial_tracker',
-        'current_tracker_id': 'test_current_tracker',
-        'customer_name': 'John Doe',
-        'customer_phone_number': '+1234567890',
-        'initial_tracking_number': '+0987654321',
-        'current_tracking_number': '+1234567890',
-        'last_message_at': dt.datetime.now(),
-        'state': 'active',
-        'company_time_zone': 'UTC',
-        'formatted_customer_phone_number': '(123) 456-7890',
-        'formatted_initial_tracking_number': '(098) 765-4321',
-        'formatted_current_tracking_number': '(123) 456-7890',
-        'formatted_customer_name': 'Doe, John',
-        'recent_messages': []
-    }
-
-    conversation = TextMessageConversation(api_client, account_id, **conversation_data)
-
-    assert conversation.id == conversation_data['id']
-    assert conversation.customer_name == conversation_data['customer_name']
-    assert conversation.recent_messages == conversation_data['recent_messages']
-
-
-# Tests deserializing JSON data into a TextMessageConversation object with missing or invalid fields. 
-def test_deserialize_json_missing_fields() -> None:
-    # Edge case test for deserializing JSON data into a TextMessageConversation with missing or invalid fields
-    api_client = CallRail('test_key')
-    account_id = 'test_account'
-    json_data = {
-        # Missing id field
-        'company_id': 'test_company',
-        'initial_tracker_id': 'test_initial_tracker',
-        'current_tracker_id': 'test_current_tracker',
-        'customer_name': 'John Doe',
-        'customer_phone_number': '+1234567890',
-        'initial_tracking_number': '+0987654321',
-        'current_tracking_number': '+1234567890',
-        'last_message_at': dt.datetime.now().isoformat(),
-        'state': 'active',
-        'company_time_zone': 'UTC',
-        'formatted_customer_phone_number': '(123) 456-7890',
-        'formatted_initial_tracking_number': '(098) 765-4321',
-        'formatted_current_tracking_number': '(123) 456-7890',
-        'formatted_customer_name': 'Doe, John',
-        'recent_messages': []
-    }
-
-    with pytest.raises(KeyError):
-        TextMessageConversation.from_json(api_client, account_id, json_data)
-
-# Tests deserializing JSON data into a TextMessageConversation object with valid data. 
-def test_deserialize_json_valid_data() -> None:
-    # Happy path test for deserializing JSON data into a TextMessageConversation with valid data
-    api_client = CallRail('test_key')
-    account_id = 'test_account'
-    json_data = {
-        'id': 'test_conversation',
-        'company_id': 'test_company',
-        'initial_tracker_id': 'test_initial_tracker',
-        'current_tracker_id': 'test_current_tracker',
-        'customer_name': 'John Doe',
-        'customer_phone_number': '+1234567890',
-        'initial_tracking_number': '+0987654321',
-        'current_tracking_number': '+1234567890',
-        'last_message_at': '2022-01-01T00:00:00Z',
-        'state': 'active',
-        'company_time_zone': 'UTC',
-        'formatted_customer_phone_number': '(123) 456-7890',
-        'formatted_initial_tracking_number': '(098) 765-4321',
-        'formatted_current_tracking_number': '(123) 456-7890',
-        'formatted_customer_name': 'Doe, John',
-        'recent_messages': [
-            {
-                'direction': 'incoming',
-                'content': 'Hello',
-                'created_at': '2022-01-01T00:00:00Z'
-            },
-            {
-                'direction': 'outgoing',
-                'content': 'Hi there',
-                'created_at': '2022-01-01T00:01:00Z'
-            }
-        ]
-    }
-
-    conversation = TextMessageConversation.from_json(api_client, account_id, json_data)
-
-    assert conversation.id == json_data['id']
-    assert conversation.customer_name == json_data['customer_name']
-    assert len(conversation.recent_messages) == len(json_data['recent_messages'])
-
-# Tests accessing attributes of a TextMessageConversation object. 
-def test_access_attributes() -> None:
-    # Happy path test for accessing attributes of a TextMessageConversation object
-    api_client = CallRail('test_key')
-    account_id = 'test_account'
-    conversation_data = {
-        'id': 'test_conversation',
-        'company_id': 'test_company',
-        'initial_tracker_id': 'test_initial_tracker',
-        'current_tracker_id': 'test_current_tracker',
-        'customer_name': 'John Doe',
-        'customer_phone_number': '+1234567890',
-        'initial_tracking_number': '+0987654321',
-        'current_tracking_number': '+1234567890',
-        'last_message_at': dt.datetime.now(),
-        'state': 'active',
-        'company_time_zone': 'UTC',
-        'formatted_customer_phone_number': '(123) 456-7890',
-        'formatted_initial_tracking_number': '(098) 765-4321',
-        'formatted_current_tracking_number': '(123) 456-7890',
-        'formatted_customer_name': 'Doe, John',
-        'recent_messages': []
-    }
-
-    conversation = TextMessageConversation(api_client, account_id, **conversation_data)
-
-    assert conversation.id == conversation_data['id']
-    assert conversation.customer_name == conversation_data['customer_name']
+import pytest
+import pytest_mock
+import requests_mock
+import requests
+
+from pycallrail.callrail import CallRail
+from pycallrail.objects.textmessages import TextMessage, TextMessageConversation
+import typing
+import logging
+import datetime as dt
+import typeguard
+import dataclasses
+
+# Tests that a TextMessage object can be created with valid parameters. 
+def test_creating_valid_text_message() -> None:
+    direction = "outgoing"
+    content = "Hello, this is a test message."
+    created_at: dt.datetime = dt.datetime.now()
+    text_message = TextMessage(direction=direction, content=content, created_at=created_at)
+    assert text_message.direction == direction
+    assert text_message.content == content
+    assert text_message.created_at == created_at
+
+# Tests that a TextMessage object cannot be created with empty string parameters. 
+def test_empty_string_parameters() -> None:
+    with pytest.raises(ValueError):
+        direction = ""
+        content = "Hello, this is a test message."
+        created_at: dt.datetime = dt.datetime.now()
+        TextMessage(direction=direction, content=content, created_at=created_at)
+
+# Tests that a TextMessage object cannot be created with an invalid datetime format. 
+def test_invalid_datetime_format() -> None:
+    with pytest.raises(ValueError):
+        direction = "outgpomg"
+        content = "Hello, this is a test message."
+        created_at = "2022-13-01 12:00:00"
+        TextMessage(direction=direction, content=content, created_at=created_at)
+
+# Tests that accessing the id attribute of a TextMessage object that has not been set returns None. 
+def test_accessing_unset_id_attribute() -> None:
+    text_message = TextMessage(
+        direction="outgoing", 
+        content="Hello, this is a test message.", 
+        created_at=dt.datetime.now())
+    assert text_message.id is None
+
+# Tests archiving a TextMessageConversation. 
+def test_archive_conversation(mocker: pytest_mock.MockerFixture) -> None:
+    # Happy path test for archiving a TextMessageConversation
+    api_client = CallRail('test_key')
+    account_id = 'test_account'
+    conversation_id = 'test_conversation'
+    conversation_data: typing.Dict[str, str] = {
+        'id': conversation_id,
+        'state': 'active'
+    }
+    conversation = TextMessageConversation(api_client, account_id, **conversation_data)
+
+    # Mock the _put method of the api_client to simulate a successful archive request
+    mocker.patch.object(api_client, '_put', return_value=None)
+
+    conversation.archive()
+
+    assert conversation.state == 'archived'
+
+# Tests creating a TextMessageConversation object with valid arguments. 
+def test_create_text_message_conversation_valid_args() -> None:
+    # Happy path test for creating a TextMessageConversation with valid arguments
+    api_client = CallRail('test_key')
+    account_id = 'test_account'
+    conversation_data: typing.Dict[str, typing.Any] = {
+        'id': 'test_conversation',
+        'company_id': 'test_company',
+        'initial_tracker_id': 'test_initial_tracker',
+        'current_tracker_id': 'test_current_tracker',
+        'customer_name': 'John Doe',
+        'customer_phone_number': '+1234567890',
+        'initial_tracking_number': '+0987654321',
+        'current_tracking_number': '+1234567890',
+        'last_message_at': dt.datetime.now(),
+        'state': 'active',
+        'company_time_zone': 'UTC',
+        'formatted_customer_phone_number': '(123) 456-7890',
+        'formatted_initial_tracking_number': '(098) 765-4321',
+        'formatted_current_tracking_number': '(123) 456-7890',
+        'formatted_customer_name': 'Doe, John',
+        'recent_messages': []
+    }
+
+    conversation = TextMessageConversation(api_client, account_id, **conversation_data)
+
+    assert conversation.id == conversation_data['id']
+    assert conversation.customer_name == conversation_data['customer_name']
+    assert conversation.recent_messages == conversation_data['recent_messages']
+
+
+# Tests deserializing JSON data into a TextMessageConversation object with missing or invalid fields. 
+def test_deserialize_json_missing_fields() -> None:
+    # Edge case test for deserializing JSON data into a TextMessageConversation with missing or invalid fields
+    api_client = CallRail('test_key')
+    account_id = 'test_account'
+    json_data = {
+        # Missing id field
+        'company_id': 'test_company',
+        'initial_tracker_id': 'test_initial_tracker',
+        'current_tracker_id': 'test_current_tracker',
+        'customer_name': 'John Doe',
+        'customer_phone_number': '+1234567890',
+        'initial_tracking_number': '+0987654321',
+        'current_tracking_number': '+1234567890',
+        'last_message_at': dt.datetime.now().isoformat(),
+        'state': 'active',
+        'company_time_zone': 'UTC',
+        'formatted_customer_phone_number': '(123) 456-7890',
+        'formatted_initial_tracking_number': '(098) 765-4321',
+        'formatted_current_tracking_number': '(123) 456-7890',
+        'formatted_customer_name': 'Doe, John',
+        'recent_messages': []
+    }
+
+    with pytest.raises(KeyError):
+        TextMessageConversation.from_json(api_client, account_id, json_data)
+
+# Tests deserializing JSON data into a TextMessageConversation object with valid data. 
+def test_deserialize_json_valid_data() -> None:
+    # Happy path test for deserializing JSON data into a TextMessageConversation with valid data
+    api_client = CallRail('test_key')
+    account_id = 'test_account'
+    json_data = {
+        'id': 'test_conversation',
+        'company_id': 'test_company',
+        'initial_tracker_id': 'test_initial_tracker',
+        'current_tracker_id': 'test_current_tracker',
+        'customer_name': 'John Doe',
+        'customer_phone_number': '+1234567890',
+        'initial_tracking_number': '+0987654321',
+        'current_tracking_number': '+1234567890',
+        'last_message_at': '2022-01-01T00:00:00Z',
+        'state': 'active',
+        'company_time_zone': 'UTC',
+        'formatted_customer_phone_number': '(123) 456-7890',
+        'formatted_initial_tracking_number': '(098) 765-4321',
+        'formatted_current_tracking_number': '(123) 456-7890',
+        'formatted_customer_name': 'Doe, John',
+        'recent_messages': [
+            {
+                'direction': 'incoming',
+                'content': 'Hello',
+                'created_at': '2022-01-01T00:00:00Z'
+            },
+            {
+                'direction': 'outgoing',
+                'content': 'Hi there',
+                'created_at': '2022-01-01T00:01:00Z'
+            }
+        ]
+    }
+
+    conversation = TextMessageConversation.from_json(api_client, account_id, json_data)
+
+    assert conversation.id == json_data['id']
+    assert conversation.customer_name == json_data['customer_name']
+    assert len(conversation.recent_messages) == len(json_data['recent_messages'])
+
+# Tests accessing attributes of a TextMessageConversation object. 
+def test_access_attributes() -> None:
+    # Happy path test for accessing attributes of a TextMessageConversation object
+    api_client = CallRail('test_key')
+    account_id = 'test_account'
+    conversation_data = {
+        'id': 'test_conversation',
+        'company_id': 'test_company',
+        'initial_tracker_id': 'test_initial_tracker',
+        'current_tracker_id': 'test_current_tracker',
+        'customer_name': 'John Doe',
+        'customer_phone_number': '+1234567890',
+        'initial_tracking_number': '+0987654321',
+        'current_tracking_number': '+1234567890',
+        'last_message_at': dt.datetime.now(),
+        'state': 'active',
+        'company_time_zone': 'UTC',
+        'formatted_customer_phone_number': '(123) 456-7890',
+        'formatted_initial_tracking_number': '(098) 765-4321',
+        'formatted_current_tracking_number': '(123) 456-7890',
+        'formatted_customer_name': 'Doe, John',
+        'recent_messages': []
+    }
+
+    conversation = TextMessageConversation(api_client, account_id, **conversation_data)
+
+    assert conversation.id == conversation_data['id']
+    assert conversation.customer_name == conversation_data['customer_name']
     assert conversation.recent_messages == conversation_data['recent_messages']
```

