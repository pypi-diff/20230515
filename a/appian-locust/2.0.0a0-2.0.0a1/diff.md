# Comparing `tmp/appian-locust-2.0.0a0.tar.gz` & `tmp/appian-locust-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0a0.tar", last modified: Mon May 15 15:39:54 2023, max compression
+gzip compressed data, was "dist/appian-locust-2.0.0a1.tar", last modified: Mon May 15 17:19:45 2023, max compression
```

## Comparing `appian-locust-2.0.0a0.tar` & `appian-locust-2.0.0a1.tar`

### file list

```diff
@@ -1,53 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:39:54.842062 appian-locust-2.0.0a0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5403 2023-05-15 15:39:54.842062 appian-locust-2.0.0a0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4829 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:39:54.840062 appian-locust-2.0.0a0/appian_locust/
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9541 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2479 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_design.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_feature_toggle_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_grid_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    53252 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)     5171 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_locust_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7765 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_portals.py
--rw-rw-rw-   0 root         (0) root         (0)    16297 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_records.py
--rw-rw-rw-   0 root         (0) root         (0)     7380 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_records_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7185 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_save_request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    10948 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_sites.py
--rw-rw-rw-   0 root         (0) root         (0)     4514 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_task_opener.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/_ui_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/actions_info.py
--rw-rw-rw-   0 root         (0) root         (0)    14485 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/appianclient.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/application_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/design_object_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/design_object_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/design_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/feature_flag.py
--rw-rw-rw-   0 root         (0) root         (0)    16278 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     1431 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/loadDriverUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     2749 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/news_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1941 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/record_list_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/record_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/records_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1472 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/reports_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1364 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/site_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/tasks_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/tempo_navigator.py
--rw-rw-rw-   0 root         (0) root         (0)    73573 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/uiform.py
--rw-rw-rw-   0 root         (0) root         (0)    13955 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/appian_locust/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:39:54.842062 appian-locust-2.0.0a0/appian_locust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5403 2023-05-15 15:39:54.000000 appian-locust-2.0.0a0/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1403 2023-05-15 15:39:54.000000 appian-locust-2.0.0a0/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 15:39:54.000000 appian-locust-2.0.0a0/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-15 15:39:54.000000 appian-locust-2.0.0a0/appian_locust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-15 15:39:54.000000 appian-locust-2.0.0a0/appian_locust.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-15 15:39:54.843062 appian-locust-2.0.0a0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-15 15:39:43.000000 appian-locust-2.0.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5264 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4670 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/appian_locust/
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10382 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_app_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3978 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_design.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_feature_flag.py
+-rw-rw-rw-   0 root         (0) root         (0)     5878 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_feature_toggle_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7905 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_grid_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    54901 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5170 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_locust_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7709 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)    21546 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_save_request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12661 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_sites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_task_opener.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/_ui_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)    16727 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/appianclient.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15963 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1185 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/loadDriverUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     6674 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/records_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    77531 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/appian_locust/uiform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/appian_locust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5264 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      968 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/appian_locust.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-15 17:19:45.000000 appian-locust-2.0.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-15 17:19:35.000000 appian-locust-2.0.0a1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `appian-locust-2.0.0a0/LICENSE` & `appian-locust-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a0/PKG-INFO` & `appian-locust-2.0.0a1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -57,28 +58,14 @@
 
 1. Install appian-locust using `pip`, for more comprehensive projects we recommend using `pipenv`.
 
 .. code-block:: bash
 
       pip install appian-locust
 
-
-If using ``pipenv``, simply start from the following ``Pipfile``:
-
-.. code-block:: toml
-
-    [packages]
-    appian-locust = {version = "*"}
-
-    [requires]
-    python_version = "3.10"
-
-    [pipenv]
-    allow_prereleases = true
-
 2. Configure your test to point at the Appian instance you will be using.
 You can use example file provided in this repository `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_:
 
 - Set ``host_address`` to the address of your Appian instance.
 - In ``auth``, specify the username and password of the user account to use.
 
 .. code-block:: json
@@ -98,45 +85,53 @@
     locust -f example_locustfile.py -u 1 -t 60 --headless
 
 If everything is set up correctly, you should start to see output from the load test reporting results. This should run for 60 seconds and end with a summary report of the results.
 
 * For more examples of different site interactions, see the ``example_*.py`` files included in this repository.
 * For more in-depth information about the test library, see the rest of this documentation.
 
-Build from source
-----------------------
-Clone the repository:
+Troubleshooting
+----------------
+* **"Failed to establish a new connection: [Errno 8] nodename nor servname provided, or not known"**
 
-.. code-block:: bash
+  * check that ``host_address`` is specified correctly in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
 
-    git clone -o prod git@gitlab.com:appian-oss/appian-locust.git
+* **"Login unsuccessful, no multipart cookie found...make sure credentials are correct"**
 
+  * check that `auth` specifies a valid username and password combination for the site you're testing on in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
 
-Install the library globally:
+* **"General request and response debugging"**
 
-.. code-block:: bash
+  * Add ``self.appian.interactor.record_mode = True`` to your ``AppianTaskSet`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
 
-    pip install -e appian-locust
+.. quick_start-inclusion-end-do-not-remove
 
+.. contrib-inclusion-begin-do-not-remove
 
-If you’re using a virtualenv or a dependency management tool (e.g. ``pipenv``), you can do the same type of install, but you will want to be in the context of the virtualenv (i.e. source the virtualenv), and you’ll need to pass the path to the repository you cloned.
+********************
+Contributing
+********************
 
-Note: It’s highly recommended that you use a virtual environment when installing python artifacts. You can follow the instructions `here <https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/>`__ to install virtualenv and pip.
+* Read and agree to our `Contributing Policy <https://gitlab.com/appian-oss/appian-locust/-/blob/master/CONTRIBUTING>`__
+* Fork the `appian-locust <https://gitlab.com/appian-oss/appian-locust>`__ repository
+* Make any desired changes to python files, etc.
+* Commit changes and push to your fork
+* Make a merge request to the upstream fork
 
-If you have issues installing, make sure you have the proper prerequisites installed for Locust and its dependencies.
-If you're having trouble on Windows, check `here <https://github.com/locustio/locust/issues/1208#issuecomment-569693439>`__
+To test changes
+-----------------
+In any test-implementation repo where you use appian-locust, change the following (assuming you're using a ``Pipfile``)
 
-Troubleshooting
-----------------
-* **"Failed to establish a new connection: [Errno 8] nodename nor servname provided, or not known"**
+.. code-block:: python
 
-  * check that ``host_address`` is specified correctly in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+    appian-locust = {path="../appian-locust", editable=true}
 
-* **"Login unsuccessful, no multipart cookie found...make sure credentials are correct"**
+**NOTE** The path above assumes appian-locust is checked out locally, hence we can use a relative directory path.
 
-  * check that `auth` specifies a valid username and password combination for the site you're testing on in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+And run ``pipenv install --skip-lock`` to allow you to use a local version of appian-locust
+without recreating the lock file. However, remember to use a lock file in your test-implementation repo.
 
-* **"General request and response debugging"**
+Now you can test your changes as you normally would.
+
+.. contrib-inclusion-end-do-not-remove
 
-  * Add ``self.appian.interactor.record_mode = True`` to your ``AppianTaskSet`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
 
-.. quick_start-inclusion-end-do-not-remove
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `appian-locust-2.0.0a0/README.rst` & `appian-locust-2.0.0a1/appian_locust.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: appian-locust
+Version: 2.0.0a1
+Summary: Tools and functions to make testing Appian with Locust easier
+Home-page: https://gitlab.com/appian-oss/appian-locust
+Author: Appian Performance & Reliability Engineering Squad
+License: Apache 2.0
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 5 - Production/Stable
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 .. what_is_appian_locust-inclusion-begin-do-not-remove
 
 #######################################
 What is Appian Locust?
 #######################################
 
 Appian Locust is a wrapper library around `Locust <https://locust.io>`__ for load testing Appian.
@@ -42,28 +58,14 @@
 
 1. Install appian-locust using `pip`, for more comprehensive projects we recommend using `pipenv`.
 
 .. code-block:: bash
 
       pip install appian-locust
 
-
-If using ``pipenv``, simply start from the following ``Pipfile``:
-
-.. code-block:: toml
-
-    [packages]
-    appian-locust = {version = "*"}
-
-    [requires]
-    python_version = "3.10"
-
-    [pipenv]
-    allow_prereleases = true
-
 2. Configure your test to point at the Appian instance you will be using.
 You can use example file provided in this repository `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_:
 
 - Set ``host_address`` to the address of your Appian instance.
 - In ``auth``, specify the username and password of the user account to use.
 
 .. code-block:: json
@@ -83,45 +85,53 @@
     locust -f example_locustfile.py -u 1 -t 60 --headless
 
 If everything is set up correctly, you should start to see output from the load test reporting results. This should run for 60 seconds and end with a summary report of the results.
 
 * For more examples of different site interactions, see the ``example_*.py`` files included in this repository.
 * For more in-depth information about the test library, see the rest of this documentation.
 
-Build from source
-----------------------
-Clone the repository:
+Troubleshooting
+----------------
+* **"Failed to establish a new connection: [Errno 8] nodename nor servname provided, or not known"**
 
-.. code-block:: bash
+  * check that ``host_address`` is specified correctly in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
 
-    git clone -o prod git@gitlab.com:appian-oss/appian-locust.git
+* **"Login unsuccessful, no multipart cookie found...make sure credentials are correct"**
+
+  * check that `auth` specifies a valid username and password combination for the site you're testing on in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
 
+* **"General request and response debugging"**
 
-Install the library globally:
+  * Add ``self.appian.interactor.record_mode = True`` to your ``AppianTaskSet`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
 
-.. code-block:: bash
+.. quick_start-inclusion-end-do-not-remove
 
-    pip install -e appian-locust
+.. contrib-inclusion-begin-do-not-remove
 
+********************
+Contributing
+********************
 
-If you’re using a virtualenv or a dependency management tool (e.g. ``pipenv``), you can do the same type of install, but you will want to be in the context of the virtualenv (i.e. source the virtualenv), and you’ll need to pass the path to the repository you cloned.
+* Read and agree to our `Contributing Policy <https://gitlab.com/appian-oss/appian-locust/-/blob/master/CONTRIBUTING>`__
+* Fork the `appian-locust <https://gitlab.com/appian-oss/appian-locust>`__ repository
+* Make any desired changes to python files, etc.
+* Commit changes and push to your fork
+* Make a merge request to the upstream fork
 
-Note: It’s highly recommended that you use a virtual environment when installing python artifacts. You can follow the instructions `here <https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/>`__ to install virtualenv and pip.
+To test changes
+-----------------
+In any test-implementation repo where you use appian-locust, change the following (assuming you're using a ``Pipfile``)
 
-If you have issues installing, make sure you have the proper prerequisites installed for Locust and its dependencies.
-If you're having trouble on Windows, check `here <https://github.com/locustio/locust/issues/1208#issuecomment-569693439>`__
+.. code-block:: python
 
-Troubleshooting
-----------------
-* **"Failed to establish a new connection: [Errno 8] nodename nor servname provided, or not known"**
+    appian-locust = {path="../appian-locust", editable=true}
 
-  * check that ``host_address`` is specified correctly in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+**NOTE** The path above assumes appian-locust is checked out locally, hence we can use a relative directory path.
 
-* **"Login unsuccessful, no multipart cookie found...make sure credentials are correct"**
+And run ``pipenv install --skip-lock`` to allow you to use a local version of appian-locust
+without recreating the lock file. However, remember to use a lock file in your test-implementation repo.
 
-  * check that `auth` specifies a valid username and password combination for the site you're testing on in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+Now you can test your changes as you normally would.
 
-* **"General request and response debugging"**
+.. contrib-inclusion-end-do-not-remove
 
-  * Add ``self.appian.interactor.record_mode = True`` to your ``AppianTaskSet`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
 
-.. quick_start-inclusion-end-do-not-remove
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_actions.py` & `appian-locust-2.0.0a1/appian_locust/_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict
+from urllib.parse import urlparse
 
 from requests.models import Response
 
 from . import logger
 from ._base import _Base
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error
@@ -33,20 +34,14 @@
         """
         self.interactor = interactor
 
         # When Get All functions called, these variables will be used to cache the values
         self._actions: Dict[str, Any] = dict()
         self._errors: int = 0
 
-    def get_errors_count(self) -> int:
-        return self._errors
-
-    def clear_actions_cache(self) -> None:
-        self._actions = dict()
-
     def get_actions_interface(self, locust_request_label: str = "Actions") -> Dict[str, Any]:
         uri = self.interactor.host + ACTIONS_INTERFACE_PATH
         headers = self.interactor.setup_sail_headers()
         resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Interface')
         return resp.json()
 
     def get_actions_nav(self, locust_request_label: str = "Actions") -> Dict[str, Any]:
@@ -60,15 +55,15 @@
 
     def get_actions_feed(self, locust_request_label: str = "Actions.Feed") -> Dict[str, Any]:
         uri = self.interactor.host + ACTIONS_FEED_PATH
         headers = self.interactor.setup_feed_headers()
         resp = self.interactor.get_page(uri, headers, locust_request_label)
         return resp.json()
 
-    def get_all(self, search_string: Optional[str] = None, locust_request_label: str = "Actions") -> Dict[str, Any]:
+    def get_all(self, search_string: str = None, locust_request_label: str = "Actions") -> Dict[str, Any]:
         """
         Retrieves all the available "actions" and associated metadata from "Appian-Tempo-Actions"
 
         Note: All the retrieved data about actions is stored in the private variable self._actions
 
         Returns (dict): List of actions and associated metadata
 
@@ -112,15 +107,15 @@
 
     def get_action(self, action_name: str, exact_match: bool = False) -> Dict[str, Any]:
         """
         Get the information about specific action by name.
 
         Args:
             action_name (str): Name of the action
-            exact_match (bool): Should action name match exactly or to be partial match. Default : False
+            exact_match (bool): Should action name match exactly or to be partial match. Default : True
 
         Returns (dict): Specific Action's info
 
         Raises: In case of action is not found in the system, it throws an "Exception"
 
         Example:
             If full name of action is known, with the opaque ID,
@@ -135,70 +130,92 @@
         """
         _, current_action = super().get(self._actions, action_name, exact_match)
         if not current_action:
             raise (Exception("There is no action with name {} in the system under test (Exact match = {})".format(
                 action_name, exact_match)))
         return current_action
 
-    def fetch_action_json(self, action_name: str, exact_match: bool = False, label: str = "") -> Dict[str, Any]:
+    def visit(self, action_name: str, exact_match: bool = False, label: str = "") -> Dict[str, Any]:
         """
         This function calls the API for the specific action to get its "form" data
 
         Args:
             action_name (str): Name of the action to be called. Name of the action will be in the below pattern.
                          "displayLabel::opaquqId"
-            exact_match (bool, optional): Should action name match exactly or to be partial match. Default : False
+            exact_match (bool, optional): Should action name match exactly or to be partial match. Default : True
 
         Returns (dict): Response of actions's Get UI call in dictionary
 
         Examples:
 
             If the full name of the action is known, with the opaque ID,
 
-            >>> self.appian.action.fetch_action_json("action_name:igB0K7YxC0UQ2Fhx4hicRw...", exact_match=True)
+            >>> self.appian.action.visit("action_name:igB0K7YxC0UQ2Fhx4hicRw...", exact_match=True)
 
             If only the display name is known, or part of the display name
 
-            >>> self.appian.action.fetch_action_json("action_name")
-            >>> self.appian.action.fetch_action_json("actio")
+            >>> self.appian.action.visit("action_name")
+            >>> self.appian.action.visit("actio")
 
         """
+
         action_under_test = self.get_action(action_name, exact_match)
 
         headers = self.interactor.setup_request_headers(action_under_test[KEY_FORM_HREF])
         headers["Accept"] = "application/vnd.appian.tv.ui+json"
         headers["Content-Type"] = "text/plain;charset=UTF-8"
 
         if not label:
             label = 'Actions.GetUi.' + format_label(action_name, "::", 0)
 
         resp = self.interactor.get_page(
             action_under_test[KEY_FORM_HREF],
             headers=headers,
             label=label,
         )
-        resp_json = resp.json()
+        return resp.json()
+
+    def visit_and_get_form(self, action_name: str, exact_match: bool = False, locust_request_label: str = "") -> SailUiForm:
+        """
+        Gets the action by name and returns the corresponding SailUiForm to interact with
+
+        If the action is activity chained, this will attempt to start the process and retrieve the chained SAIL form.
+
+        Args:
+            action_name (str): Name of the action
+            exact_match (bool): Should action name match exactly or to be partial match. Default : True
+            locust_request_label (str, optional): label to be used within locust
+
+        Returns: SailUiForm
+        """
+        initial_action_resp: dict = self.get_action(action_name, exact_match)
+        form_url = urlparse(initial_action_resp[KEY_FORM_HREF]).path
+        action_key = format_label(action_name, "::", 0)
+        label = locust_request_label or f'Actions.GetUi.{action_key}'
+        form_json: dict = self.visit(action_name, exact_match, label=label)
+
         # Check to see if we're in an activity chained form, and if so, make post call
-        if resp_json.get('empty') == 'true':
-            activity_chained_form_resp: Response = self.start_action(action_name, skip_design_call=True, exact_match=exact_match)
-            activity_chained_form_resp.raise_for_status()
-            resp_json = activity_chained_form_resp.json()
+        if form_json.get('empty') == 'true':
+            resp: Response = self.start_action(action_name, exact_match=exact_match)
+            resp.raise_for_status()
+            form_json = resp.json()
 
-        return resp_json
+        breadcrumb = locust_request_label or f'Actions.SailUi.{action_key}'
+        return SailUiForm(self.interactor, form_json, form_url, breadcrumb=breadcrumb)
 
     def start_action(self, action_name: str, skip_design_call: bool = False, exact_match: bool = False) -> Response:
         """
         Perform the post operation on action's API to start specific action.
         Actions that do not have a UI can be called directly without using "GET" to retrieve the UI.
         this is controlled by the optional skip_design_call parameter
 
         Args:
             action_name(str): Name of the action
             skip_design_call(bool, optional): to skip the "GET" call for the action's UI. Default : False
-            exact_match (bool, optional): Should action name match exactly or to be partial match. Default : False
+            exact_match (bool, optional): Should action name match exactly or to be partial match. Default : True
 
         Returns: NONE
 
         Example:
 
             >>> self.appian.action.start_action("action_name")
 
@@ -206,15 +223,15 @@
         action_under_test = self.get_action(action_name, exact_match)
 
         if not skip_design_call:
             # Note: Actions which do not have a UI component this call is
             # not required to kick off processes. This request causes a call
             # to design to retrieve the UI, meaning this it will cause more K
             # activity, but it does not kick off processes on the exec engines.
-            self.fetch_action_json(action_name)
+            self.visit(action_name)
 
         headers = self.interactor.setup_sail_headers()
         headers["Origin"] = self.interactor.host
 
         del headers["X-Atom-Content-Type"]
         headers["X-Client-Mode"] = "TEMPO"
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_base.py` & `appian-locust-2.0.0a1/appian_locust/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from .helper import list_filter
 from . import logger
-from typing import Any, Optional
+from typing import Any
 
 
 log = logger.getLogger(__name__)
 
 
 class _Base():
     """
     Base class for classes ``_Actions``, ``_News``, ``_Records``, ``_Reports``, ``_Tasks``, ``Sites``
     """
 
-    def get_all(self, search_string: Optional[str] = None, locust_request_label: str = "") -> Any:
+    def get_all(self, search_string: str = None, locust_request_label: str = "") -> Any:
         """
         Common Get All function prototype that is overwritten by subclasses.
         Created only to conform to Mypy validation.
         """
         return None
 
-    def get(self, items_in_dict: dict, item_name: str, exact_match: bool = True, ignore_retry: bool = False, search_string: Optional[str] = None) -> tuple:
+    def get(self, items_in_dict: dict, item_name: str, exact_match: bool = True, ignore_retry: bool = False, search_string: str = None) -> tuple:
         """
         Common Get function to get the specific component from dictionary of items. If item is not found, it calls
         get_all function to update itself and retry.
 
         Warning: Internal function, should never be called directly.
 
         Args:
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.0a1/appian_locust/_feature_toggle_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
-from typing import Any, Dict, Tuple, Optional, Generator, Callable
+from typing import Any, Dict, List, Tuple
 
 from locust.clients import HttpSession
 
-from .feature_flag import FeatureFlag
+from ._feature_flag import FeatureFlag
 from ._interactor import _Interactor
 from ._locust_error_handler import test_response_for_error
 from .logger import getLogger
 
 log = getLogger(__name__)
 
 
@@ -26,36 +26,37 @@
         flag_str = _get_javascript_and_find_feature_flag(session,
                                                          script_uri)
         if flag_str:
             return _get_feature_flags_from_regex_match(flag_str)
         raise Exception(f"Could not find flag string within uri {script_uri}")
 
 
-def _get_javascript_uri(interactor: _Interactor, headers: Optional[Dict[str, Any]] = None) -> Any:
+def _get_javascript_uri(interactor: _Interactor, headers: Dict[str, Any] = None) -> Any:
     """
     Gets the URI for the javascript file that contains the Feature Toggles
     """
 
     news_uri = interactor.replace_base_path_if_appropriate("/suite/sites")
     response = interactor.get_page(
         uri=news_uri, headers=headers, label="Login.Feature_Toggles.GetSites"
     )
     tempo_text = response.text
-
-    for regex in __get_javascript_uri_regex():
+    relative_regex = r'<script src="(.*\/tempo\/ui\/sail-client\/sites-.*?.js)'
+    cloud_regex = r'<script src="(https://web-assets.appiancloud.com/.*\/tempo\/ui\/sail-client\/sites-.*?.js)'
+    for regex in [relative_regex, cloud_regex]:
         script_regex = interactor.replace_base_path_if_appropriate(regex)
         uri_match = re.search(script_regex, tempo_text)
         if uri_match:
             script_uri = uri_match.groups()[0]
             return script_uri
-        log.info(f"Could not find feature toggle uri using regex {regex}")
+        log.info(f"Could not find feature toggle uri using regex {relative_regex}")
     return None
 
 
-def _get_javascript_and_find_feature_flag(client: HttpSession, script_uri: str, headers: Optional[Dict[str, Any]] = None) -> Any:
+def _get_javascript_and_find_feature_flag(client: HttpSession, script_uri: str, headers: Dict[str, Any] = None) -> Any:
     """
     Read through minified javascript for feature flags
     """
     flag_str = None
     # Since this is a large request, read incrementally
     with client.get(
             script_uri,
@@ -72,15 +73,19 @@
         var RAW_DEFAULT_FEATURE_FLAGS=5802956083228348;
         var RAW_DEFAULT_FEATURE_FLAGS=jsbi__WEBPACK_IMPORTED_MODULE_10__["default"].BigInt("0b110100100111011100000111111111111111001110111010111100");
         """
         for chunk in res.iter_content(8192, decode_unicode=True):
             if flag_str:
                 # Not reading the whole stream will throw errors, so continue reading once found
                 continue
-            for script_regex in __get_javascript_feature_flag_regex():
+            script_regexes = [
+                r'RAW_DEFAULT_FEATURE_FLAGS=(0x\w+|\d+);',
+                r'RAW_DEFAULT_FEATURE_FLAGS=jsbi__WEBPACK_IMPORTED_MODULE_\d+__\["default"\].BigInt\("(0b[01]+)"\);',
+            ]
+            for script_regex in script_regexes:
                 js_match = re.search(script_regex, prev_chunk + chunk)
                 if js_match:
                     flag_str = js_match.groups()[0]
             prev_chunk = chunk
     return flag_str
 
 
@@ -106,27 +111,27 @@
 
 def _truncate_flag_extended(flag_extended: int) -> int:
     # This mask is a max int that will truncate the extended features to the size of an integer.
     old_flag_mask = 2147483647
     return flag_extended & old_flag_mask
 
 
-def _create_override_flag_mask(flags_to_override: Callable[[], Generator[FeatureFlag, None, None]]) -> int:
+def _create_override_flag_mask(flags_to_override: List[FeatureFlag]) -> int:
     """
     Given a list of flag enums from FeatureFlag, this will set that flag to 1 to override the default feature set.
     returns flag mask reflecting all the flags combined.
     """
     flags = 0
-    for flag in flags_to_override():
+    for flag in flags_to_override:
         if isinstance(flag, FeatureFlag):
             flags |= (1 << flag.value)
     return flags
 
 
-def override_default_feature_flags(interactor: _Interactor, flags_to_override: Callable[[], Generator[FeatureFlag, None, None]]) -> None:
+def override_default_flags(interactor: _Interactor, flags_to_override: List[FeatureFlag]) -> None:
     """
     Given a list of flag enums from FeatureFlag, override_default_flags gets the flag mask to
     set all of the flags to true, and it overrides the current feature flag extended value to
     set these flags to true.
     """
     override_flags_mask = _create_override_flag_mask(flags_to_override)
     feature_flag_with_override = int(interactor.client.feature_flag_extended, 16) | override_flags_mask
@@ -135,22 +140,8 @@
     interactor.client.feature_flag = _to_hex_str(old_flag)
 
 
 def set_mobile_feature_flags(interactor: _Interactor) -> None:
     """
     This overrides the feature flags to tell the service that the request is coming from a mobile device.
     """
-    override_default_feature_flags(interactor, __get_mobile_feature_flag_overrides)
-
-
-def __get_mobile_feature_flag_overrides() -> Generator[FeatureFlag, None, None]:
-    yield FeatureFlag.RECORD_LIST_FEED_ITEM_DTO
-
-
-def __get_javascript_uri_regex() -> Generator[str, None, None]:
-    yield r'<script src="(.*\/tempo\/ui\/sail-client\/sites-.*?.js)'
-    yield r'<script src="(https://web-assets.appiancloud.com/.*\/tempo\/ui\/sail-client\/sites-.*?.js)'
-
-
-def __get_javascript_feature_flag_regex() -> Generator[str, None, None]:
-    yield r'RAW_DEFAULT_FEATURE_FLAGS=(0x\w+|\d+);'
-    yield r'RAW_DEFAULT_FEATURE_FLAGS=jsbi__WEBPACK_IMPORTED_MODULE_\d+__\["default"\].BigInt\("(0b[01]+)"\);'
+    override_default_flags(interactor, [FeatureFlag.RECORD_LIST_FEED_ITEM_DTO])
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_grid_interactor.py` & `appian-locust-2.0.0a1/appian_locust/_grid_interactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List
 
-from .helper import extract_values_multiple_key_values, find_component_by_label_and_type_dict
+from .exceptions import ComponentNotFoundException
+
+from .helper import extract_values, extract_values_multiple_key_values, find_component_by_attribute_in_dict, find_component_by_label_and_type_dict
 
 from . import logger
 
 log = logger.getLogger(__name__)
 
 
 class GridInteractor:
@@ -28,15 +30,15 @@
         grids = extract_values_multiple_key_values(form, '#t', ["PagingGridLayout", "GridField"])
         if not grids:
             raise Exception("No grids found in form")
         if len(grids) < index:
             raise Exception(f"Index {index} out of range, only found {len(grids)} grid(s) in form")
         return grids[index]
 
-    def find_grid_by_label_or_index(self, form: Dict[str, Any], label: Optional[str] = None, index: Optional[int] = None) -> Dict[str, Any]:
+    def find_grid_by_label_or_index(self, form: Dict[str, Any], label: str = None, index: int = None) -> Dict[str, Any]:
         if label:
             grid = self.find_grid_by_label(label, form)
         elif index is not None:  # 0 is a valid index
             grid = self.find_grid_by_index(index, form)
         else:
             raise Exception("Either an index or a label must be passed")
         return grid
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_interactor.py` & `appian-locust-2.0.0a1/appian_locust/_interactor.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,67 +11,69 @@
 from requests import Response
 
 from . import logger
 from ._locust_error_handler import log_locust_error, test_response_for_error
 from ._save_request_builder import save_builder
 from .exceptions import BadCredentialsException, MissingCsrfTokenException, ComponentNotFoundException
 from .helper import find_component_by_attribute_in_dict, get_username
-from ._records_helper import get_url_stub_from_record_list_post_request_url
+from .records_helper import get_url_stub_from_record_list_post_request_url
 
 log = logger.getLogger(__name__)
 
 # TODO: Consider breaking this class up into smaller pieces
 
 
 RECORD_PATH = "recorded_responses"
 
 
 class _Interactor:
-    def __init__(self, session: HttpSession, host: str, portals_mode: bool = False) -> None:
+    def __init__(self, session: HttpSession, host: str, portals_mode: bool = False, request_timeout: int = 300) -> None:
         """
         Class that represents interactions with the UI and Appian system
         If you want to record all requests made, you can set the record_mode attribute
         on the client, see the mock_client.py in the tests directory as an example
 
         >>> setattr(self.client, 'record_mode', True)
 
         Args:
             session: Locust session/client object
             host (str): Host URL inherited from subclass to conform with Mypy standards
             portals_mode (bool): Set to true if attempting to connect to a portals site
+            request_timeout (int): time in seconds after which requests initiated by the Interactor should time out
         """
         self.client = session
         self.host = host
         self.record_mode = True if hasattr(self.client, "record_mode") else False
         self.datatype_cache = DataTypeCache()
         self.user_agent = ""
         self.portals_mode = portals_mode
         self.url_pattern_version = 0
+        self.__request_timeout = request_timeout
         # Set to default as desktop request.
         self.set_user_agent_to_desktop()
 
     # GENERIC UTILITY METHODS
     def set_user_agent_to_desktop(self) -> None:
         self.user_agent = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/61.0.3163.100 Safari/537.36"
 
     def set_user_agent_to_mobile(self) -> None:
         self.user_agent = "AppianAndroid/20.2 (Google AOSP on IA Emulator, 9; Build 0-SNAPSHOT; AppianPhone)"
 
-    def setup_request_headers(self, uri: Optional[str] = None) -> dict:
+    def setup_request_headers(self, uri: str = None) -> dict:
         """
         Generates standard headers for session
 
         Args:
             uri (str): URI to be assigned as the Referer
 
         Returns (dict): headers
 
         Examples:
 
-            >>> self.appian._interactor.setup_request_headers()
+            >>> self.appian.interactor.setup_request_headers()
         """
 
         uri = uri if uri is not None else self.host
         headers = {
             "Accept": "application/atom+json,application/json",
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en_US",
@@ -119,56 +121,57 @@
 
     def replace_base_path_if_appropriate(self, uri: str) -> str:
         if hasattr(self.client, "base_path_override") and self.client.base_path_override and \
                 self.client.base_path_override != '/suite':
             return uri.replace('/suite', self.client.base_path_override, 1)
         return uri
 
-    def post_page(self, uri: str, payload: Any = {}, headers: Optional[Dict[str, Any]] = None, label: Optional[str] = None,
-                  files: Optional[dict] = None, check_login: bool = True) -> Response:
+    def post_page(self, uri: str, payload: Any = {}, headers: Dict[str, Any] = None, label: str = None,
+                  files: dict = None, check_login: bool = True) -> Response:
         """
         Given a uri, executes POST request and returns response
 
         Args:
             uri: API URI to be called
             payload: Body of the API request. Can be either JSON or text input to allow for different payload types.
             headers: header for the REST API Call
             label: the label to be displayed by locust
 
         Returns: Json response of post operation
 
         """
+
         if headers is None:
             headers = self.setup_sail_headers()
 
         uri = self.replace_base_path_if_appropriate(uri)
         username = "No-auth User" if self.portals_mode else get_username(self.auth)
         if files:  # When a file is specified, don't send any data in the 'data' field
             post_payload = None
         elif isinstance(payload, dict):
             post_payload = json.dumps(payload).encode()
         elif isinstance(payload, str):
             post_payload = payload.encode()
         else:
             log_locust_error(Exception("Cannot POST a payload that is not of type dict or string"))
             sys.exit(1)
-        with self.client.post(uri, data=post_payload, headers=headers, timeout=60, name=label, files=files,
+        with self.client.post(uri, data=post_payload, headers=headers, timeout=self.__request_timeout, name=label, files=files,
                               catch_response=True) as resp:  # type: ResponseContextManager
             try:
                 test_response_for_error(resp, uri, raise_error=check_login, username=username)
             except Exception as e:
                 raise e
             else:
                 if check_login:
                     resp.raise_for_status()
             if self.record_mode:
                 self.write_response_to_lib_folder(label, resp)
             return resp
 
-    def login(self, auth: Optional[list] = None, retry: bool = True, check_login: bool = True) -> Tuple[HttpSession, Response]:
+    def login(self, auth: list = None, retry: bool = True, check_login: bool = True) -> Tuple[HttpSession, Response]:
         if auth is not None:
             self.auth = auth
         """
         Login to Appian Tempo using given auth
 
         Args:
             auth: list containing 2 elements. username and password
@@ -232,15 +235,15 @@
             self.login()
         elif not resp.ok:
             # Check login page actually returns a csrf token
             login_page_resp = self.get_page('/suite/', label="Login.LoadUi", check_login=False)
             if login_page_resp.ok and '__appianCsrfToken' in login_page_resp.cookies:
                 self.login()
 
-    def get_page(self, uri: str, headers: Optional[Dict[str, Any]] = None, label: Optional[str] = None,
+    def get_page(self, uri: str, headers: Optional[Dict[str, Any]] = None, label: str = None,
                  check_login: bool = True) -> Response:
         """
         Given a uri, executes GET request and returns response
 
         Args:
             uri: API URI to be called
             headers: header for the REST API Call
@@ -255,47 +258,47 @@
             else:
                 headers = self.setup_request_headers(uri)
         kwargs: Dict[str, Any] = {'name': label, 'catch_response': True}
 
         uri = self.replace_base_path_if_appropriate(uri)
         if headers is not None:
             kwargs['headers'] = headers
-            kwargs['timeout'] = 60
+            kwargs['timeout'] = self.__request_timeout
         with self.client.get(uri, **kwargs) as resp:  # type: ResponseContextManager
             if check_login and not self.portals_mode:
                 self.check_login(resp)
             if not self.portals_mode:
                 username = get_username(self.auth)
                 test_response_for_error(resp, uri, raise_error=check_login, username=username)
             if self.record_mode:
                 self.write_response_to_lib_folder(label, resp)
             return resp
 
-    def get_webapi(self, uri: str, headers: Optional[Dict[str, Any]] = None, label: Optional[str] = None,
+    def get_webapi(self, uri: str, headers: Dict[str, Any] = None, label: str = None,
                    queryparameters: Dict[str, Any] = {}) -> Response:
         """
         Same as ``get_page``. Additionally it accepts the query parameter to add query parameter while running "GET" operation
         Args:
             uri: API URI to be called
             headers: header for the REST API Call
             label: the label to be displayed by locust
             queryparameters: Queries/Filters
 
         Returns: Json response of GET operation
 
         To set custom headers
 
-        >>> headers = self.appian._interactor.setup_request_headers()
+        >>> headers = self.appian.interactor.setup_request_headers()
         ... headers['Is-Admin'] = 'true'
-        ... self.appian._interactor.get_webapi('/suite/webapi/headers', headers=headers)
+        ... self.appian.interactor.get_webapi('/suite/webapi/headers', headers=headers)
 
         To set custom query parameters
 
         >>> params = {'age': 5, 'start-date': '10-05-2020'}
-        ... self.appian._interactor.get_webapi('/suite/webapi/query', queryparameters=params)
+        ... self.appian.interactor.get_webapi('/suite/webapi/query', queryparameters=params)
         """
         querystring = []
         for k, v in queryparameters.items():
             querystring.append("{}={}".format(k, v))
 
         uri += "?" + "&".join(querystring)
         resp = self.get_page(uri, headers=headers, label=label)
@@ -357,15 +360,15 @@
                     req_str_file.write(body)
         with open(proposed_response_file_name, 'w') as resp_text_file:
             resp_text_file.write(response.text)
         if 'X-Trace-Id' in response.headers:
             log.info(cleaned_label + ' | X-Trace-Id: ' + response.headers['X-Trace-Id'])
 
     def click_record_link(self, get_url: str, component: Dict[str, Any], context: Dict[str, Any],
-                          label: Optional[str] = None, headers: Optional[Dict[str, Any]] = None, locust_label: str = "") -> Dict[str, Any]:
+                          label: str = None, headers: Dict[str, Any] = None, locust_label: str = "") -> Dict[str, Any]:
         '''
         Use this function to interact specifically with record links, which represent links to new sail forms.
         Args:
             get_url: the url (not including the host and domain) to navigate to
             component: the JSON code for the RecordLink
             context: the Sail context parsed from the json response
             label: the label to be displayed by locust for this action
@@ -435,15 +438,15 @@
         resp = self.get_page(
             self.host + record_link_url, headers=headers, label=locust_label
         )
         return resp.json()
 
     def click_start_process_link(self, component: Dict[str, Any], process_model_opaque_id: str,
                                  cache_key: str, site_name: str, page_name: str, is_mobile: bool = False,
-                                 locust_request_label: Optional[str] = None) -> Dict[str, Any]:
+                                 locust_request_label: str = None) -> Dict[str, Any]:
         '''
         Use this function to interact with start process links, which start a process and return the
         start form.
         Args:
             component: the JSON representing the Start Process Link
             process_model_opaque_id: opaque id for the process model of the Start Process Link
             cache_key: cachekey for the start process link
@@ -511,16 +514,16 @@
             else:
                 return json_response
         return resp.json()
 
     # COMPONENT RELATED METHODS
 
     def click_component(self, post_url: str, component: Dict[str, Any], context: Dict[str, Any],
-                        uuid: str, label: Optional[str] = None, headers: Optional[Dict[str, Any]] = None,
-                        client_mode: Optional[str] = None) -> Dict[str, Any]:
+                        uuid: str, label: str = None, headers: Dict[str, Any] = None,
+                        client_mode: str = None) -> Dict[str, Any]:
         '''
             Calls the post operation to click certain SAIL components such as Buttons and Dynamic Links
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 component: the JSON code for the desired component
                 context: the Sail context parsed from the json response
@@ -540,24 +543,24 @@
             .context(context) \
             .uuid(uuid) \
             .build()
 
         locust_label = label or f'Click \'{component["label"]}\' Component'
 
         resp = self.post_page(
-            self.host + post_url, payload=payload, label=locust_label
+            self.host + post_url, payload=payload, label=locust_label, headers=headers
         )
         return resp.json()
 
     # Aliases for click_component to preserve backwards compatibiltiy and increase readability
     click_button = click_component
     click_link = click_component
 
     def send_dropdown_update(self, post_url: str, dropdown: Dict[str, Any], context: Dict[str, Any],
-                             uuid: str, index: int, label: Optional[str] = None, url_stub: Optional[str] = None) -> Dict[str, Any]:
+                             uuid: str, index: int, label: str = None, url_stub: str = None) -> Dict[str, Any]:
         '''
             Calls the post operation to send an update to a dropdown
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 dropdown: the JSON code for the desired dropdown
                 context: the Sail context parsed from the json response
@@ -587,15 +590,15 @@
 
         resp = self.post_page(
             self.host + post_url, payload=payload, label=locust_label
         )
         return resp.json()
 
     def send_multiple_dropdown_update(self, post_url: str, multi_dropdown: Dict[str, Any], context: Dict[str, Any],
-                                      uuid: str, index: List[int], label: Optional[str] = None, url_stub: Optional[str] = None) -> Dict[str, Any]:
+                                      uuid: str, index: List[int], label: str = None, url_stub: str = None) -> Dict[str, Any]:
         '''
             Calls the post operation to send an update to a multiple dropdown
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 dropdown: the JSON code for the desired dropdown
                 context: the Sail context parsed from the json response
@@ -647,15 +650,15 @@
             .context(context) \
             .uuid(uuid) \
             .build()
 
         return payload
 
     def fill_textfield(self, post_url: str, text_field: Dict[str, Any], text: str,
-                       context: Dict[str, Any], uuid: str, label: Optional[str] = None) -> Dict[str, Any]:
+                       context: Dict[str, Any], uuid: str, label: str = None) -> Dict[str, Any]:
         """
         Fill a TextField with the given text
         Args:
             post_url: the url (not including the host and domain) to post to
             text_field: the text field component returned from find_component_by_attribute_in_dict
             text: the text to fill into the text field
             context: the Sail context parsed from the json response
@@ -677,15 +680,15 @@
 
         resp = self.post_page(
             self.host + post_url, payload=payload, label=locust_label
         )
         return resp.json()
 
     def fill_pickerfield_text(self, post_url: str, picker_field: Dict[str, Any], text: str,
-                              context: Dict[str, Any], uuid: str, label: Optional[str] = None) -> Dict[str, Any]:
+                              context: Dict[str, Any], uuid: str, label: str = None) -> Dict[str, Any]:
         """
         Fill a Picker field with the given text and randomly select one of the suggested item
         Args:
             post_url: the url (not including the host and domain) to post to
             picker_field: the picker field component returned from find_component_by_attribute_in_dict
             text: the text to fill into the picker field
             context: the SAIL context parsed from the json response
@@ -711,15 +714,15 @@
 
         resp = self.post_page(
             self.host + post_url, payload=payload, label=locust_label
         )
         return resp.json()
 
     def select_pickerfield_suggestion(self, post_url: str, picker_field: Dict[str, Any], selection: Dict[str, Any],
-                                      context: Dict[str, Any], uuid: str, label: Optional[str] = None) -> Dict[str, Any]:
+                                      context: Dict[str, Any], uuid: str, label: str = None) -> Dict[str, Any]:
         """
         Select a Picker field from available selections
         Args:
             post_url: the url (not including the host and domain) to post to
             picker_field: the text field component returned from find_component_by_attribute_in_dict
             selection: the suggested item to select for the picker field
             context: the SAIL context parsed from the json response
@@ -749,15 +752,15 @@
         resp = self.post_page(
             self.host + post_url, payload=payload, label=locust_label
         )
         return resp.json()
 
     def select_checkbox_item(self, post_url: str, checkbox: Dict[str, Any],
                              context: Dict[str, Any], uuid: str, indices: list,
-                             context_label: Optional[str] = None) -> Dict[str, Any]:
+                             context_label: str = None) -> Dict[str, Any]:
         '''
             Calls the post operation to send an update to a checkbox to check all appropriate boxes
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 checkbox: the JSON representing the desired checkbox
                 context: the Sail context parsed from the json response
@@ -832,15 +835,15 @@
 
         resp = self.post_page(
             self.host + post_url, payload=payload, label=locust_label
         )
         return resp.json()
 
     def select_radio_button(self, post_url: str, buttons: Dict[str, Any], context: Dict[str, Any],
-                            uuid: str, index: int, context_label: Optional[str] = None) -> Dict[str, Any]:
+                            uuid: str, index: int, context_label: str = None) -> Dict[str, Any]:
         '''
             Calls the post operation to send an update to a radio button to select the appropriate button
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 buttons: the JSON representing the desired radio button field
                 context: the Sail context parsed from the json response
@@ -894,15 +897,15 @@
                 "id": id
             },
             "extension": dummy_data["extension"]
         }
 
     def upload_document_to_field(self, post_url: str, upload_field: Dict[str, Any],
                                  context: Dict[str, Any], uuid: str, doc_id: Union[int, List[int]],
-                                 locust_label: Optional[str] = None, client_mode: str = 'DESIGN') -> Dict[str, Any]:
+                                 locust_label: str = None, client_mode: str = 'DESIGN') -> Dict[str, Any]:
         '''
             Calls the post operation to send an update to a upload_field to upload a document or list thereof.
             Requires a previously uploaded document id or ids
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 upload_field: the JSON representing the desired checkbox
@@ -944,15 +947,15 @@
         resp = self.post_page(
             self.host + post_url, payload=payload, headers=headers, label=locust_label
         )
         return resp.json()
 
     def update_date_field(self, post_url: str, date_field_component: Dict[str, Any],
                           date_input: date, context: Dict[str, Any], uuid: str,
-                          locust_label: Optional[str] = None) -> Dict[str, Any]:
+                          locust_label: str = None) -> Dict[str, Any]:
         '''
             Calls the post operation to update a date field
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 date_field_component: the JSON representing the date field component
                 date_input: date field to convert to proper text format
@@ -981,15 +984,15 @@
         resp = self.post_page(
             self.host + post_url, payload=payload, headers=headers, label=locust_label
         )
         return resp.json()
 
     def update_datetime_field(self, post_url: str, datetime_field: Dict[str, Any],
                               datetime_input: datetime, context: Dict[str, Any], uuid: str,
-                              locust_label: Optional[str] = None) -> Dict[str, Any]:
+                              locust_label: str = None) -> Dict[str, Any]:
         '''
             Calls the post operation to update a date field
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 datetime_field: the JSON representing the datetime field to edit
                 datetime_input: datetime field to convert to the proper text format
@@ -1020,15 +1023,15 @@
             self.host + post_url, payload=payload, headers=headers, label=locust_label
         )
         return resp.json()
 
     def update_grid_from_sail_form(self, post_url: str,
                                    grid_component: Dict[str, Any], new_grid_save_value: Dict[str, Any],
                                    context: Dict[str, Any], uuid: str,
-                                   context_label: Optional[str] = None) -> Dict[str, Any]:
+                                   context_label: str = None) -> Dict[str, Any]:
         """
             Calls the post operation to send a grid update
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 grid_component: the JSON dict representing the grid to update
                 context: the Sail context parsed from the json response
@@ -1050,15 +1053,15 @@
             self.host + post_url, payload=payload, label=locust_label
         )
         return resp.json()
 
     def interact_with_record_grid(self, post_url: str,
                                   grid_component: Dict[str, Any],
                                   context: Dict[str, Any], uuid: str,
-                                  context_label: Optional[str] = None) -> Dict[str, Any]:
+                                  context_label: str = None) -> Dict[str, Any]:
         """
             Calls the post operation to send a record grid update
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 grid_component: the JSON dict representing the grid to update
                 context: the Sail context parsed from the json response
@@ -1080,15 +1083,15 @@
             self.host + post_url, payload=payload, label=locust_label
         )
         resp.raise_for_status()
         return resp.json()
 
     def refresh_after_record_action(self, post_url: str, record_action_component: Dict[str, Any],
                                     record_action_trigger_component: Dict[str, Any],
-                                    context: Dict[str, Any], uuid: str, label: Optional[str] = None) -> Dict[str, Any]:
+                                    context: Dict[str, Any], uuid: str, label: str = None) -> Dict[str, Any]:
         """
             Calls the post operation to refresh a form after completion of a record action
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 record_action_component: the JSON representing the relevant record action component
                 record_action_trigger_component: the JSON representing the form's record action trigger component
@@ -1122,15 +1125,15 @@
 
         resp = self.post_page(
             self.host + post_url, payload=record_action_payload, label=label
         )
         return resp.json()
 
     def click_record_search_button(self, post_url: str, component: Dict[str, Any], context: Dict[str, Any],
-                                   uuid: str, label: Optional[str] = None) -> Dict[str, Any]:
+                                   uuid: str, label: str = None) -> Dict[str, Any]:
         """
             Calls the post operation to click a record search button
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 component: the JSON code for the desired SearchBoxWidget component
                 context: the Sail context parsed from the json response
@@ -1168,15 +1171,15 @@
 
         resp = self.post_page(
             self.host + post_url, payload=payload, label=locust_label
         )
         return resp.json()
 
     def click_generic_element(self, post_url: str, component: Dict[str, Any], context: Dict[str, Any], uuid: str,
-                              new_value: Dict[str, Any], label: Optional[str] = None) -> Dict[str, Any]:
+                              new_value: Dict[str, Any], label: str = None) -> Dict[str, Any]:
         """
             Calls the post operation to click on a generic element
 
             Args:
                 post_url: the url (not including the host and domain) to post to
                 component: the JSON code for the component
                 context: the Sail context parsed from the json response
@@ -1197,14 +1200,53 @@
         locust_label = label or "ClickElement"
 
         resp = self.post_page(
             self.host + post_url, payload=payload, label=locust_label
         )
         return resp.json()
 
+    def launch_query_editor(self, post_url: str, editor_component: Dict[str, Any],
+                            context: Dict[str, Any], uuid: str, expr: str, label: str = None) -> Dict[str, Any]:
+        """
+            Calls the post operation to click on the LaunchVQD button in the toolbar for the ExpressionEditorWidget.
+            This will launch the query editor with the provided expression.
+
+            Args:
+                post_url: the url (not including the host and domain) to post to
+                editor_component: the JSON code for the expression editor component
+                context: the Sail context parsed from the json response
+                uuid: the uuid parsed from the json response
+                expr: expression in the expression editor
+                label: the label to be displayed by locust for this action
+
+            Returns: the response of post operation as json
+
+        """
+        launchVQD_action = "LaunchVQD"
+
+        new_value = {
+            "#t": "Dictionary",
+            "#v": {
+                "actionType": launchVQD_action,
+                "hasMatchingBracketError": False,
+                "launchOrigin": "toolbarButton",
+                "queryFnType": "queryRecordType",
+                "queryFnStartIndex": 0,
+                "queryFnEndIndex": len(expr),
+                "value": {
+                    "#t": "Text",
+                    "#v": expr
+                }
+            }
+        }
+
+        locust_label = label or f'Click \'{launchVQD_action}\' Expression Editor Widget Button'
+
+        return self.click_generic_element(post_url=post_url, component=editor_component, context=context, uuid=uuid, new_value=new_value, label=locust_label)
+
 
 class DataTypeCache(object):
     def __init__(self) -> None:
         """
         This class provides a structure to handle data type cache
         """
         self._cached_datatype: Set[str] = set()
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.0a1/appian_locust/_locust_error_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 
     Returns:
         None
 
     Example (Returns a HTTP 500 error):
 
     .. code-block:: python
-
       username = 'admin'
       uri = 'https://httpbin.org/status/500'
       with self.client.get(uri) as resp:
         test_response_for_error(resp, uri, username)
     """
     try:
         if not resp or not resp.ok:
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_news.py` & `appian-locust-2.0.0a1/appian_locust/_news.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Tuple, Optional
+from typing import Any, Dict, Tuple
 
 from appian_locust import logger
 from appian_locust._base import _Base
 from appian_locust._interactor import _Interactor
 from appian_locust._locust_error_handler import log_locust_error
 
 log = logger.getLogger(__name__)
@@ -27,17 +27,17 @@
         """
         self.interactor = interactor
 
         # When Get All functions called, these variables will be used to cache the values
         self._news: Dict[str, Any] = dict()
         self._errors: int = 0
 
-    def get_all(self, search_string: Optional[str] = None, locust_request_label: str = "") -> Dict[str, Any]:
+    def get_all(self, search_string: str = None, locust_request_label: str = "") -> Dict[str, Any]:
         """
-        Retrieves all the available "news" and associated metadata from "Appian-Tempo-News"
+        Retrieves all the available "news" and assgit ociated metadata from "Appian-Tempo-News"
 
         Note: All the retrieved data about news is stored in the private variable self._news
 
         Args:
             search_string(str, optional): results will be filtered based on the search string.
 
         Returns (dict): List of news and associated metadata
@@ -74,15 +74,15 @@
                 log_locust_error(e, error_desc="Corrupt News Error", location=uri, raise_error=False)
         self._errors = error_key_count
 
         if len(self._news) == 0:
             log.warning(f"News search failed for keyword: '{search_string}'")
         return self._news
 
-    def get_news(self, news_name: str, exact_match: bool = True, search_string: Optional[str] = None) -> Dict[str, Any]:
+    def get_news(self, news_name: str, exact_match: bool = True, search_string: str = None) -> Dict[str, Any]:
         """
         Get the information about specific news by name.
 
         Args:
             news_name (str): name of the news entry
             exact_match (bool, optional): Should news name match exactly or to be partial match. Default : True
             search_string (str, optional): results will be filtered based on the search string.
@@ -104,15 +104,15 @@
         _, current_news = super().get(self._news, news_name,
                                       exact_match=exact_match, search_string=search_string)
         if not current_news:
             raise (Exception("There is no news with name {} in the system under test (Exact match = {})".format(
                 news_name, exact_match)))
         return current_news
 
-    def visit(self, news_name: str, exact_match: bool = True, search_string: Optional[str] = None) -> None:
+    def visit(self, news_name: str, exact_match: bool = True, search_string: str = None) -> None:
         """
         This function calls the nav API for the specific news item and its related records if any
 
         Args:
             news_name (str): Name of the news entry to be called
             exact_match (bool, optional): Should news name match exactly or to be partial match. Default : True
             search_string (str, optional): results will be filtered based on the search string.
@@ -132,15 +132,15 @@
         """
         current_news, headers = self._visit_internal(news_name, exact_match, search_string)
         for link in current_news['links']:
             if link['rel'] == "related-records-properties":
                 if str(link['href']).strip() != "":
                     self.interactor.get_page(link['href'], headers, label="News.LoadEntry." + news_name)
 
-    def visit_news_entry(self, news_name: str, exact_match: bool = True, search_string: Optional[str] = None) -> Tuple:
+    def visit_news_entry(self, news_name: str, exact_match: bool = True, search_string: str = None) -> Tuple:
         """
         This function simulates navigating to a single entry in the ui. There are two parts to navigating to a
         news entry: navigating to the view and getting the news entry's feed.
 
         Args:
             news_name (str): Name of the news entry to be called
             exact_match (bool, optional): Should news name match exactly or to be partial match. Default : True
@@ -167,15 +167,15 @@
                     view_status_code = self.interactor.get_page(link['href'], headers).status_code
             elif link['rel'] == 'edit':
                 if str(link['href']).strip() != "":
                     feed_status_code = self.interactor.get_page(link['href'], headers).status_code
 
         return (view_status_code, feed_status_code)
 
-    def _visit_internal(self, news_name: str, exact_match: bool = True, search_string: Optional[str] = None) -> Tuple:
+    def _visit_internal(self, news_name: str, exact_match: bool = True, search_string: str = None) -> Tuple:
         current_news = self.get_news(news_name, exact_match, search_string)
         headers = self.interactor.setup_request_headers()
 
         # Nav
         nav_uri = NEWS_NAV_PATH[0]
         if self.interactor.url_pattern_version == 1:
             nav_uri += "p."
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_records.py` & `appian-locust-2.0.0a1/appian_locust/_records.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import json
 import random
-from typing import Any, Dict, Tuple, Optional
+from typing import Any, Dict, Tuple
 from urllib.parse import quote
 
 import requests
 
 from appian_locust import logger
 
 from ._base import _Base
 from ._interactor import _Interactor
-from ._records_helper import (get_all_records_from_json,
-                              get_all_record_types_from_json, get_records_from_json_by_column)
+from .helper import format_label
+from .records_helper import (get_all_records_from_json,
+                             get_record_summary_view_response, get_records_from_json_by_column)
+from .uiform import SailUiForm
 from ._locust_error_handler import log_locust_error
 
 log = logger.getLogger(__name__)
 
 RECORDS_ALL_PATH = "/suite/rest/a/applications/latest/app/records/view/all"
 RECORDS_INTERFACE_PATH = "/suite/rest/a/sites/latest/D6JMim/pages/records/interface"
 RECORDS_NAV_PATH = ["/suite/rest/a/sites/latest/D6JMim/page/", "records", "/nav"]
@@ -54,15 +56,15 @@
         if self.interactor.url_pattern_version == 1:
             uri += "p."
         uri += RECORDS_NAV_PATH[1] + RECORDS_NAV_PATH[2]
         headers = self.interactor.setup_sail_headers()
         resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Nav')
         return resp.json()
 
-    def get_all(self, search_string: Optional[str] = None, locust_request_label: str = "Records") -> Dict[str, Any]:
+    def get_all(self, search_string: str = None, locust_request_label: str = "Records") -> Dict[str, Any]:
         """
         Retrieves all available "records types" and "records" and associated metadata from "Appian-Tempo-Records"
 
         Note: All the retrieved data about record types and records is stored in the private variables
         self._record_types and self._records respectively
 
         Returns (dict): List of records and associated metadata
@@ -70,14 +72,17 @@
         try:
             self.get_records_interface(locust_request_label=locust_request_label)
             self.get_records_nav(locust_request_label=locust_request_label)
         except Exception as e:
             log_locust_error(e, error_desc="Response Error", raise_error=False)
 
         if search_string:
+            # If using exact_match=True, then a unique identifier is require to be appended, which must be removed for the search
+            search_string = search_string.split("::")[0]
+
             # Format search string to be compatible with URLs
             search_string = quote(search_string)
 
         self.get_all_record_types(locust_request_label=locust_request_label)
         for record_type in self._record_types:
             try:
                 self.get_all_records_of_record_type(record_type, search_string=search_string)
@@ -89,87 +94,88 @@
 
     def get_all_record_types(self, locust_request_label: str = "Records") -> Dict[str, Any]:
         """
         Navigate to Tempo Records Tab and load all metadata for associated list of record types into cache.
 
         Returns (dict): List of record types and associated metadata
         """
-
-        json_response = self.fetch_all_records_json(locust_request_label)
-
-        self._record_types = get_all_record_types_from_json(json_response)
-        for title in self._record_types.keys():
-            self._records[title] = dict()
-
-        return self._record_types
-
-    def fetch_all_records_json(self, locust_request_label: str = "Records") -> Dict[str, Any]:
         uri = RECORDS_ALL_PATH
+        self._record_types = dict()
 
         headers = self.interactor.setup_request_headers()
         headers['X-Appian-Features-Extended'] = 'e4bc'
         headers["Accept"] = "application/vnd.appian.tv.ui+json"
         response = self.interactor.get_page(uri=uri, headers=headers, label=locust_request_label)
+        json_response = response.json()
         if not(self._is_response_good(response.text)):
             raise(Exception("Unexpected response on Get call of All Records"))
-        return response.json()
 
-    def get_all_records_of_record_type(self, record_type: str, column_index: Optional[int] = None, search_string: Optional[str] = None) -> Dict[str, Any]:
+        for current_record_type in json_response["ui"]["contents"][0]["feedItems"]:
+            title = current_record_type['title'].strip()
+            self._record_types[title] = current_record_type
+            self._records[title] = dict()
+
+        return self._record_types
+
+    def get_all_records_of_record_type(self, record_type: str, column_index: int = None, search_string: str = None) -> Dict[str, Any]:
         """
         Navigate to the desired record type and load all metadata for the associated list of record views into cache.
 
         Args:
             record_type (str): Name of record type for which we want to enumerate the record instances.
             column_index (int, optional): Column index to only fetch record links from a specific column, starts at 0.
 
         Returns (dict): List of records and associated metadata
 
         Examples:
 
             >>> self.appian.records.get_all_records_of_record_type("record_type_name")
         """
 
-        json_response = self._record_type_list_request(record_type, search_string=search_string)
+        json_response, _ = self._record_type_list_request(record_type, search_string=search_string)
 
         if column_index is not None:
             self._records[record_type], self._errors = get_records_from_json_by_column(json_response, column_index)
         else:
             self._records[record_type], self._errors = get_all_records_from_json(json_response)
 
         return self._records
 
-    def get_all_records_of_record_type_mobile(self, record_type: str, search_string: Optional[str] = None) -> Dict[str, Any]:
+    def get_all_records_of_record_type_mobile(self, record_type: str, search_string: str = None) -> Dict[str, Any]:
         """
         Retrieves all the available "records" for the given record type for a mobile device.
 
         Todo: Partial match functionality is not yet implemented
 
         Returns (dict): List of records and associated metadata
 
         Examples:
 
             >>> self.appian.records.get_all_records_of_record_type_mobile("record_type_name")
         """
-        json_response = self._record_type_list_request(record_type, is_mobile=True, search_string=search_string)
+        json_response, _ = self._record_type_list_request(record_type, is_mobile=True, search_string=search_string)
 
         self._records[record_type], self._errors = get_all_records_from_json(json_response)
 
         return self._records
 
-    def get_all_mobile(self, search_string: Optional[str] = None) -> Dict[str, Any]:
+    def get_all_mobile(self, search_string: str = None) -> Dict[str, Any]:
         """
         Retrieves all available "records types" and "records" and associated metadata from "Appian-Tempo-Records"
 
         Note: All the retrieved data about record types and records is stored in the private variables
         self._record_types and self._records respectively
 
         Returns (dict): List of records and associated metadata
         """
 
         if search_string:
+            # If using exact_match=True, then a unique identifier is require to be appended, which must be removed for the search
+            search_string = search_string.split("::")[0]
+
             # Format search string to be compatible with URLs
             search_string = quote(search_string)
 
         self.get_all_record_types()
         for record_type in self._record_types:
             self.get_all_records_of_record_type_mobile(record_type, search_string=search_string)
         return self._records
@@ -228,28 +234,28 @@
 
         """
         _, current_record_type = super().get(self._record_types, record_type, exact_match)
         if not current_record_type:
             raise Exception(f"There is no record type with name {record_type} in the system under test (Exact match = {exact_match})")
         return current_record_type
 
-    def visit_record_instance(self, record_type: str = "", record_name: str = "", view_url_stub: str = "", exact_match: bool = True, locust_request_label: str = "") -> Dict[str, Any]:
+    def visit_record_instance(self, record_type: str = "", record_name: str = "", view_url_stub: str = "", exact_match: bool = True, locust_request_label: str = "") -> Tuple[Dict[str, Any], str]:
         """
         This function calls the API for the specific record view/instance to get its response data.
 
         Note: This function is meant to only traverse to Record forms, not to interact with them. For that, use visit_record_instance_and_get_form()
 
         Args:
             record_type (str): Record Type Name. If not specified, a random record type will be selected.
             record_name (str): Name of the record to be called. If not specified, a random record will be selected.
             view_url_stub (str, optional): page/tab to be visited in the record. If not specified, "summary" dashboard will be selected.
             exact_match (bool, optional): Should record type and record name matched exactly as it is or partial match.
             locust_request_label(str,optional): Label used to identify the request for locust statistics
 
-        Returns (dict): Responses of Record's Get UI call in a dictionary
+        Returns (tuple): Responses of Record's Get UI call in a dictionary and the request URI as a string.
 
         Examples:
 
             If full name of record type and record is known,
 
             >>> self.appian.records.visit_record_instance("record_type_name", "record_name", "summary")
 
@@ -265,16 +271,14 @@
 
             >>> self.appian.records.visit_record_instance("record_type_name")
 
         """
 
         if not record_name:
             record_type, record_name = self._get_random_record_instance(record_type)
-            # remove id from record name
-            record_name = record_name.split("::")[0]
 
         if not record_type:
             raise Exception("If record_name parameter is specified, record_type must also be included")
 
         current_record = self.fetch_record_instance(record_type, record_name, exact_match)
 
         headers = self.interactor.setup_feed_headers()
@@ -286,20 +290,20 @@
         if not view_url_stub:
             dashboard_val = current_record.get("dashboard")
             view_url_stub = dashboard_val if dashboard_val else "summary"
 
         locust_label = locust_request_label or f'Records.{record_type}.{record_label}.{view_url_stub}'
         uri = f"{RECORD_VIEW_PATH[0]}{tempo_site_url_stub}{RECORD_VIEW_PATH[1]}{opaque_id}{RECORD_VIEW_PATH[2]}{view_url_stub}"
         resp = self.interactor.get_page(uri=uri, headers=headers, label=locust_label)
-        return resp.json()
+        return resp.json(), uri
 
     # Alias for the above function to allow backwards compatability
     visit = visit_record_instance
 
-    def visit_record_type(self, record_type: str = "", exact_match: bool = True, is_mobile: bool = False) -> Dict[str, Any]:
+    def visit_record_type(self, record_type: str = "", exact_match: bool = True, is_mobile: bool = False) -> Tuple[Dict[str, Any], str]:
         """
         Navigate into desired record type and retrieve all metadata for associated list of record views.
 
         Returns (dict): List of records and associated metadata
 
         Examples:
 
@@ -312,15 +316,107 @@
 
         # If no record_type is specified, a random one will be assigned
         if not record_type:
             record_type = self._get_random_record_type()
 
         return self._record_type_list_request(record_type, is_mobile=is_mobile)
 
-    # ----- Private Functions ----- #
+    def visit_record_instance_and_get_feed_form(self, record_type: str = "", record_name: str = "", exact_match: bool = True) -> SailUiForm:
+        """
+        This function calls the API for the specific record view/instance and returns a SAILUiForm object for "feed" response.
+        The returned SailUiForm object can then be used to get header response by using calling get_record_header_form(). The header form
+        should have related actions available to interact with.
+
+        Args:
+            record_type (str): Record Type Name. If not specified, a random record type will be selected.
+            record_name (str): Name of the record to be called. If not specified, a random record will be selected.
+            exact_match (bool, optional): Should record type and record name matched exactly as it is or partial match.
+
+        Returns: Custom SailUiForm object that can interact with Appian forms. Use this object to fill textfields, click links/buttons, etc...
+        """
+        # view_url_stub does not matter in case of feed response for a record instance. Feed Response for each tab on an record instance is the same
+        # no matter which dashboard is selected.
+        form_json, form_uri = self.visit_record_instance(record_type, record_name, view_url_stub="summary", exact_match=exact_match)
+        breadcrumb = f'Records.{record_type}.{record_name}.Feed'
+        return SailUiForm(self.interactor, form_json, form_uri, breadcrumb=breadcrumb)
+
+    def visit_record_instance_and_get_form(self, record_type: str = "", record_name: str = "", view_url_stub: str = "", exact_match: bool = False) -> SailUiForm:
+        """
+        This function calls the API for the specific record view/instance and returns a SAIL form object that Locust users can interact with.
+
+        Note: Since this function is enabled for interactions, it has a higher runtime than visit_record_instance()
+
+        Args:
+            record_type (str): Record Type Name. If not specified, a random record type will be selected.
+            record_name (str): Name of the record to be called. If not specified, a random record will be selected.
+            view_url_stub (str, optional): page/tab to be visited in the record. If not specified, "summary" dashboard will be selected.
+            exact_match (bool, optional): Should record type and record name matched exactly as it is or partial match.
+
+        Returns: Custom SailUiForm object that can interact with Appian forms. Use this object to fill textfields, click links/buttons, etc...
+
+        Examples:
+
+            If full name of record type and record is known,
+
+            >>> self.appian.records.visit_and_get_form("record_type_name", "record_name", "summary")
+
+            If only partial name is known,
+
+            >>> self.appian.records.visit_and_get_form("record_type_name", "record_name", "summary", exact_match=False)
+
+            If random record is desired,
+
+            >>> self.appian.records.visit_and_get_form()
+
+            If random record of a specific record type is desired,
+
+            >>> self.appian.records.visit_and_get_form("record_type_name")
+        """
+
+        form_json, form_uri = self.visit_record_instance(record_type, record_name, view_url_stub=view_url_stub, exact_match=exact_match)
+        # SAIL Code for the Record Summary View is embedded within the response.
+        embedded_record_resp = get_record_summary_view_response(form_json)
+        breadcrumb = f'Records.{record_type}.{format_label(record_name, "::", 0)}.SailUi'
+        return SailUiForm(self.interactor, json.loads(embedded_record_resp), form_uri, breadcrumb=breadcrumb)
+
+    visit_and_get_form = visit_record_instance_and_get_form
+
+    def visit_record_type_and_get_form(self, record_type: str = "", exact_match: bool = False, is_mobile: bool = False) -> SailUiForm:
+        """
+        This function calls the API for the specific record typew and returns a SAIL form object that Locust users can interact with.
+
+        Note: Since this function is enabled for interactions, it has a higher runtime than visit_record_type()
+
+        Args:
+            record_type (str): Record Type Name. If not specified, a random record type will be selected.
+            exact_match (bool, optional): Should record type and record name matched exactly as it is or partial match.
+
+        Returns: Custom SailUiForm object that can interact with Appian forms. Use this object to fill textfields, click links/buttons, etc...
+
+        Examples:
+
+            If the full name of record type is known,
+
+            >>> self.appian.records.visit_record_type_and_get_form("record_type_name")
+
+            If only partial name is known,
+
+            >>> self.appian.records.visit_record_type_and_get_form("record_type_name", exact_match=False)
+
+            If random record type is desired,
+
+            >>> self.appian.records.visit_record_type_and_get_form()
+        """
+        if not self._records or not self._record_types:
+            self.get_all()
+        form_json, form_uri = self.visit_record_type(record_type, exact_match=exact_match, is_mobile=is_mobile)
+        breadcrumb = f'Records.{record_type}.SailUi'
+        return SailUiForm(self.interactor, form_json, form_uri, breadcrumb=breadcrumb)
+
+        # ----- Private Functions ----- #
 
     def _is_response_good(self, response_text: str) -> bool:
         return ('"rel":"x-web-bookmark"' in response_text or '"#t":"CardLayout"' in response_text)
 
     def _get_random_record_instance(self, record_type: str = "") -> Tuple[str, str]:
         if not self._records or not self._record_types:
             self.get_all()
@@ -330,37 +426,34 @@
         return record_type, record_name
 
     def _get_random_record_type(self) -> str:
         if not self._records or not self._record_types:
             self.get_all()
         return random.choice(list(self._records.keys()))
 
-    def _record_type_list_request(self, record_type: str, is_mobile: bool = False, search_string: Optional[str] = None) -> Dict[str, Any]:
+    def _record_type_list_request(self, record_type: str, is_mobile: bool = False, search_string: str = None) -> Tuple[Dict[str, Any], str]:
         if record_type not in self._record_types:
             raise Exception(f"There is no record type with name {record_type} in the system under test")
         record_type_component = self._record_types[record_type]
         record_type_url_stub = record_type_component['link']['value']['urlstub']
-        return self.fetch_record_type_json(record_type_url_stub, is_mobile, search_string, f"Records.{record_type}")
 
-    def fetch_record_type_json(self, record_type_url_stub: str, is_mobile: bool = False, search_string: Optional[str] = None, label: Optional[str] = None) -> Dict[str, Any]:
-        if not label:
-            label = f"Records.{record_type_url_stub}"
         if is_mobile:
             uri = self._get_mobile_records_uri(record_type_url_stub)
         else:
             uri = f"{RECORD_TYPE_VIEW_PATH}{record_type_url_stub}"
             if search_string:
                 uri = f"{uri}?searchTerm={search_string}"
+        label = f"Records.{record_type}"
         headers = self.interactor.setup_request_headers()
         headers["Accept"] = "application/vnd.appian.tv.ui+json"
         response = self.interactor.get_page(uri=uri, headers=headers, label=label)
         json_response = response.json()
 
-        return json_response
+        return json_response, uri
 
-    def _get_mobile_records_uri(self, record_type_url_stub: str, search_string: Optional[str] = None) -> str:
+    def _get_mobile_records_uri(self, record_type_url_stub: str, search_string: str = None) -> str:
         if not record_type_url_stub:
             raise Exception("Mobile records uri must have a unique stub provided.")
         uri = f"{RECORDS_MOBILE_PATH}{record_type_url_stub}"
         if search_string:
             return f"{uri}/search/{search_string}"
         return f"{uri}/view/all"
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_records_helper.py` & `appian-locust-2.0.0a1/appian_locust/records_helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,14 @@
-import json
 from typing import Any, Dict, Tuple, Optional
 
 from ._locust_error_handler import log_locust_error
 from .helper import extract_values, find_component_by_attribute_in_dict
 from re import match
 
 
-def get_all_record_types_from_json(json_response: Dict[str, Any]) -> Dict[str, Any]:
-    response = dict()
-    for current_record_type in json_response["ui"]["contents"][0]["feedItems"]:
-        title = current_record_type['title'].strip()
-        response[title] = current_record_type
-    return response
-
-
 def get_all_records_from_json(json_response: Dict[str, Any]) -> Tuple[Dict[str, Any], int]:
     is_grid = _is_grid(json_response)
     records = {}
     error_key_string = "ERROR::"
     error_key_count = 0
     if is_grid:
         all_record_items = extract_values(json_response, "#t", "RecordLink")
@@ -29,26 +20,23 @@
                 key = label + "::" + opaque_id
                 records[key] = record_item
             except Exception as e:
                 error_key_count += 1
                 records[error_key_string + str(error_key_count)] = {}
                 log_locust_error(e, error_desc="Corrupt Record Error")
     else:
-        all_items = extract_values(json_response, "#t", "LinkedItem")
-        label_extractor = _get_linkedItem_label
-        if len(all_items) == 0:
-            all_items = extract_values(json_response, "#t", "FeedItemLayout")
-            label_extractor = _get_feedItemLayout_label
-        for current_item in all_items:
+        all_linked_items = extract_values(json_response, "#t", "LinkedItem")
+        for current_item in all_linked_items:
             record_link_raw = extract_values(current_item, "#t", "RecordLink")
             if len(record_link_raw) > 0:
+                label_raw = extract_values(current_item["values"], "#t", "string")
                 record_item = record_link_raw[0]
                 try:
                     opaque_id = record_item["_recordRef"]
-                    label = label_extractor(current_item)
+                    label = label_raw[0]["#v"]
                     record_item["label"] = label
                     key = label + "::" + opaque_id
                     records[key] = record_item
                 except Exception as e:
                     error_key_count += 1
                     records[error_key_string + str(error_key_count)] = {}
                     log_locust_error(e, error_desc="Corrupt Record Error", raise_error=False)
@@ -86,39 +74,39 @@
             else:
                 error_key_count += 1
                 log_locust_error(e=Exception('No record links found.'))
 
     return records, error_key_count
 
 
-def get_record_summary_view_response(form_json: Dict[str, Any]) -> Dict[str, Any]:
+def get_record_summary_view_response(form_json: Dict[str, Any]) -> str:
     """
         This returns the contents of "x-embedded-summary" from Record Instance's Feed response
     """
     # SAIL Code for the Record Summary View is embedded within the response.
     record_summary_response = find_component_by_attribute_in_dict("name", "x-embedded-summary", form_json).get("children")
     if not record_summary_response or len(record_summary_response) < 1:
         log_locust_error(Exception("Parser was not able to find embedded SAIL code within JSON response for the requested Record Instance."),
                          raise_error=True
                          )
-    return json.loads(record_summary_response[0])
+    return record_summary_response[0]
 
 
-def get_record_header_response(form_json: Dict[str, Any]) -> Dict[str, Any]:
+def get_record_header_response(form_json: Dict[str, Any]) -> str:
     """
         This returns the contents of "x-embedded-header" from Record Instance's Feed response.
         Header response is needed in cases like clicking on a related action.
     """
     # SAIL Code for the Record Header is embedded within the response.
     record_header_response = find_component_by_attribute_in_dict("name", "x-embedded-header", form_json).get("children")
     if not record_header_response or len(record_header_response) < 1:
         log_locust_error(Exception("Parser was not able to find embedded SAIL code within JSON response for the requested Record Instance."),
                          raise_error=True
                          )
-    return json.loads(record_header_response[0])
+    return record_header_response[0]
 
 
 def _is_grid(res_dict_var: Dict[str, Any]) -> bool:
     return any([len(extract_values(res_dict_var, "testLabel", "recordGrid")) != 0,
                 len(extract_values(res_dict_var, "testLabel", "recordGridInstances")) != 0])
 
 
@@ -149,15 +137,7 @@
 
         Returns: The url stub if post_url matches a record instance list url, otherwise None
     """
     record_url_match = None
     if post_url:
         record_url_match = match(r'[\S]+\/pages\/records\/recordType\/([\w]+)', post_url)
     return record_url_match.groups()[0] if record_url_match else None
-
-
-def _get_linkedItem_label(item: Dict[str, Any]) -> str:
-    return extract_values(item["values"], "#t", "string")[0]["#v"]
-
-
-def _get_feedItemLayout_label(item: Dict[str, Any]) -> str:
-    return item["title"]
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_reports.py` & `appian-locust-2.0.0a1/appian_locust/_reports.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 from urllib.parse import quote
 
 from ._base import _Base
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error, test_response_for_error
 from .helper import format_label
 from .uiform import SailUiForm
 
-ALL_REPORTS_URI = "/suite/rest/a/uicontainer/latest/reports"
 REPORTS_INTERFACE_PATH = "/suite/rest/a/sites/latest/D6JMim/pages/reports/interface"
 REPORTS_LINK_PATH = ["/suite/rest/a/sites/latest/D6JMim/pages/reports/report/", "/reportlink"]
 REPORTS_NAV_PATH = ["/suite/rest/a/sites/latest/D6JMim/page/", "reports", "/nav"]
 
 
 class _Reports(_Base):
     def __init__(self, interactor: _Interactor) -> None:
@@ -29,21 +28,14 @@
         """
         self.interactor = interactor
 
         # When Get All functions called, these variables will be used to cache the values
         self._reports: Dict[str, Any] = dict()
         self._errors: int = 0
 
-    def get_report_form_uri(self, report_name: str, exact_match: bool = True) -> str:
-        report_resp: dict = self.get_report(report_name, exact_match)
-        report_url_stub = report_resp['links'][1]['href'].rsplit(
-            '/', 1)[1]
-        uri = f"{REPORTS_LINK_PATH[0]}{report_url_stub}{REPORTS_LINK_PATH[1]}"
-        return uri
-
     def get_reports_interface(self, locust_request_label: str = "Reports") -> Dict[str, Any]:
         uri = self.interactor.host + REPORTS_INTERFACE_PATH
         headers = self.interactor.setup_sail_headers()
         resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Interface')
         return resp.json()
 
     def get_reports_nav(self, locust_request_label: str = "Reports") -> Dict[str, Any]:
@@ -51,15 +43,15 @@
         if self.interactor.url_pattern_version == 1:
             uri += "p."
         uri += REPORTS_NAV_PATH[1] + REPORTS_NAV_PATH[2]
         headers = self.interactor.setup_sail_headers()
         resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Nav')
         return resp.json()
 
-    def get_all(self, search_string: Optional[str] = None, locust_request_label: str = "Reports.Feed") -> Dict[str, Any]:
+    def get_all(self, search_string: str = None, locust_request_label: str = "Reports.Feed") -> Dict[str, Any]:
         """
         Retrieves all the available "reports" and associated metadata from "Appian-Tempo-Reports"
 
         Note: All the retrieved data about reports is stored in the private variable self._reports
 
         Returns (dict): List of reports and associated metadata
 
@@ -70,16 +62,19 @@
         """
         try:
             self.get_reports_interface(locust_request_label=locust_request_label)
             self.get_reports_nav(locust_request_label=locust_request_label)
         except Exception as e:
             log_locust_error(e, error_desc="Response Error", raise_error=False)
 
-        uri = ALL_REPORTS_URI
+        uri = "/suite/rest/a/uicontainer/latest/reports"
         if search_string:
+            # If using exact_match=True, then a unique identifier is require to be appended, which must be removed for the search
+            search_string = search_string.split("::")[0]
+
             # Format search string to be compatible with URLs
             search_string = quote(search_string)
             uri = f"{uri}?q={search_string}"
 
         self._reports = dict()
         error_key_string = "ERROR::"
         error_key_count = 0
@@ -130,44 +125,57 @@
         if not current_report:
             _, current_report = super().get(self._reports, report_name, exact_match, search_string=report_name)
         if not current_report:
             raise (Exception("There is no report with name {} in the system under test (Exact match = {})".format(
                 report_name, exact_match)))
         return current_report
 
-    def fetch_report_json(self, report_name: str, exact_match: bool = True) -> Dict[str, Any]:
+    def visit(self, report_name: str, exact_match: bool = True) -> Dict[str, Any]:
         """
         This function calls the API for the specific report to get its "form" data
 
         Args:
             report_name (str): Name of the report to be called.
             exact_match (bool, optional): Should report name match exactly or to be partial match. Default : True
 
         Returns (dict): Response of report's Get UI call in dictionary
 
         Examples:
 
             If full name of report is known,
 
-            >>> self.appian.reports.fetch_report_json("report_name")
+            >>> self.appian.reports.visit("report_name")
 
             If only partial name is known,
 
-            >>> self.appian.reports.fetch_report_json("report_name", exact_match=False)
+            >>> self.appian.reports.visit("report_name", exact_match=False)
 
         """
-        form_uri = self.get_report_form_uri(report_name, exact_match)
+
+        report_under_test = self.get_report(report_name, exact_match)
+
         headers = self.interactor.setup_request_headers()
         headers["Accept"] = "application/vnd.appian.tv.ui+json"
 
         # navigation request
         uri = REPORTS_NAV_PATH[0]
         if self.interactor.url_pattern_version == 1:
             uri += "p."
         uri += REPORTS_NAV_PATH[1] + REPORTS_NAV_PATH[2]
         label = "Reports.Nav." + format_label(report_name, "::", 0)
         self.interactor.get_page(uri=uri, headers=headers, label=label)  # report request
+        report_url_stub = report_under_test['links'][1]['href'].rsplit('/', 1)[1]
+        uri = f"{REPORTS_LINK_PATH[0]}{report_url_stub}{REPORTS_LINK_PATH[1]}"
         label = "Reports.GetUi." + format_label(report_name, "::", 0)
-        resp = self.interactor.get_page(uri=form_uri, headers=headers, label=label)
+        resp = self.interactor.get_page(uri=uri, headers=headers, label=label)
         test_response_for_error(resp)
         resp.raise_for_status()
         return resp.json()
+
+    def visit_and_get_form(self, report_name: str, exact_match: bool = True) -> SailUiForm:
+        report_resp: dict = self.get_report(report_name, exact_match)
+        report_url_stub = report_resp['links'][1]['href'].rsplit(
+            '/', 1)[1]
+        form_uri = f"{REPORTS_LINK_PATH[0]}{report_url_stub}{REPORTS_LINK_PATH[1]}"
+        form_json = self.visit(report_name, exact_match)
+        breadcrumb = f'Reports.SailUi.{format_label(report_name, "::", 0)}'
+        return SailUiForm(self.interactor, form_json, form_uri, breadcrumb=breadcrumb)
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_save_request_builder.py` & `appian-locust-2.0.0a1/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a0/appian_locust/_sites.py` & `appian-locust-2.0.0a1/appian_locust/_sites.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import enum
 import json
 import random
-from typing import Any, Dict, List, Union, Optional
+from typing import Any, Dict, List, Union
 
 from requests import Response
 
 from . import logger
 from ._base import _Base
 from ._interactor import _Interactor
 from ._news import NEWS_NAV_PATH
 from .helper import extract_values, format_label
-from ._records_helper import (get_all_records_from_json,
-                              get_record_summary_view_response)
+from .records_helper import (get_all_records_from_json,
+                             get_record_summary_view_response)
 from .uiform import SailUiForm
 
 log = logger.getLogger(__name__)
 
 SITES_NAV_PATH = ["/suite/rest/a/sites/latest/", "/page/", "/nav"]
 SITES_PAGE_PATH = ["/suite/rest/a/sites/latest/", "/pages/", "/"]
 
@@ -37,78 +37,112 @@
 
         """
         self.interactor = interactor
 
         self._sites: Dict[str, Site] = {}
         self._sites_records: Dict[str, Dict[str, Any]] = {}
 
-    def fetch_site_tab_json(self, site_name: str, page_name: str) -> Dict[str, Any]:
+    def navigate_to_tab(self, site_name: str, page_name: str) -> Response:
         """
         Navigates to a site page, either a record, action or report.
 
         Args:
             site_name: Site Url stub
             page_name: Page Url stub
 
         Returns: Response of report/action/record
         """
+        if site_name not in self._sites:
+            self.get_site_data_by_site_name(site_name)
+
+        if site_name not in self._sites:
+            raise SiteNotFoundException(f"The site with name '{site_name}' could not be found")
+        site: Site = self._sites[site_name]
+        if page_name not in [page.page_name for page in site.pages.values()]:
+            raise PageNotFoundException(f"The site with name '{site_name}' does not contain the page {page_name}")
+        page = site.pages[page_name]
+        page_type = page.page_type.value
 
-        page_type = self.get_site_page_type(site_name, page_name).value
         headers = self._setup_headers_with_sail_json()
 
         base_path = f"{SITES_NAV_PATH[0]}{site_name}{SITES_NAV_PATH[1]}"
         if self.interactor.url_pattern_version == 1:
             base_path += f"p.{page_name}"
         else:
             base_path += f"{page_name}"
         base_path += SITES_NAV_PATH[2]
         self.interactor.get_page(base_path, headers=headers, label=f"Sites.{site_name}.{page_name}.Nav")
         base_path = f"{SITES_PAGE_PATH[0]}{site_name}{SITES_PAGE_PATH[1]}{page_name}{SITES_PAGE_PATH[2]}{page_type}"
         resp = self.interactor.get_page(base_path, headers=headers, label=f"Sites.{site_name}.{page_name}.Ui")
-        return resp.json()
+        return resp
 
-    def fetch_site_tab_record_json(self, site_name: str, page_name: str) -> Dict[str, Any]:
+    def navigate_to_tab_and_record_if_applicable(self, site_name: str, page_name: str) -> Response:
         """
-        Navigate to a recordList page on a site, then grab a random page from that site
+        Navigates to a site page, either a record, interface, action or report.
+        If a record, then clicks on a random record on the first page.
 
         Note: Any record available in the record list as a recordLink will be hit using this function.  There is no
         guarantee that this record will be of any specific type and may not point to a record view.
 
         Args:
             site_name: Site Url stub
             page_name: Page Url stub
 
         Returns: Response of report/action, or in the case of a record, response of record object
         """
-        resp_json = self.fetch_site_tab_json(site_name, page_name)
+        resp = self.navigate_to_tab(site_name, page_name)
         if not self._sites[site_name].pages[page_name].page_type == PageType.RECORD:
-            raise Exception(f"Page {page_name} on site {site_name} is not of type record")
+            return resp
         headers = self._setup_headers_with_sail_json()
         if page_name not in self._sites_records:
-            records_for_page, errors = get_all_records_from_json(resp_json)
+            records_for_page, errors = get_all_records_from_json(resp.json())
             self._sites_records[page_name] = records_for_page
         records = list(self._sites_records[page_name])
         if not records:
-            raise Exception(f"No records found for site={site_name}, page={page_name}")
+            log.error(f"No records found for site={site_name}, page={page_name}")
+            return resp
         record_key = random.choice(list(self._sites_records[page_name]))
         label = f"Sites.{site_name}.{page_name}." + format_label(record_key, "::", 0)[:30]
         record_id = record_key.split("::")[1]
         record_resp = self.interactor.get_page(
             f"/suite/sites/{site_name}/page/{page_name}/nav",
             headers=headers,
             label=label + ".Nav")
         # TODO: Add ability to go to arbitrary stubs
         headers = self.interactor.setup_feed_headers()
         record_resp = self.interactor.get_page(
             f"/suite/rest/a/sites/latest/{site_name}/page/{page_name}/record/{record_id}/view/summary",
             headers=headers,
             label=label + ".View")
-        return record_resp.json()
+        return record_resp
 
-    def get_all(self, search_string: Optional[str] = None, locust_request_label: Optional[str] = None) -> Dict[str, Any]:
+    def navigate_to_tab_and_record_get_form(self, site_name: str, page_name: str) -> SailUiForm:
+        """
+        Navigates to a site page, either a record, action or report.
+        If it is a record, then clicks on a random record instance on the first page
+
+        Args:
+            site_name: Site Url stub
+            page_name: Page Url stub
+
+        Returns: SailUiForm of a report/action, or in the case of a record, SailUiForm of a record instance
+        """
+
+        site_page_response: Response = self.navigate_to_tab_and_record_if_applicable(site_name, page_name)
+        form_uri = site_page_response.request.path_url
+        site_page_json_response = site_page_response.json()
+        if site_page_json_response.get("feed"):
+            record_view_response = get_record_summary_view_response(site_page_json_response)
+            breadcrumb = f"Sites.{site_name}.{page_name}.SailUi"
+            return SailUiForm(self.interactor, json.loads(record_view_response), form_uri, breadcrumb=breadcrumb)
+        else:
+            breadcrumb = f"Sites.{site_name}.{page_name}.SailUi"
+            return SailUiForm(self.interactor, site_page_json_response, form_uri, breadcrumb=breadcrumb)
+
+    def get_all(self, search_string: str = None, locust_request_label: str = None) -> Dict[str, Any]:
         """
         Gets and stores data for all sites, including all of their url stubs
         """
         headers = self._setup_headers_with_sail_json()
         uri = NEWS_NAV_PATH[0]
         if self.interactor.url_pattern_version == 1:
             uri += "p."
@@ -178,25 +212,34 @@
         if 'redirect' not in page_resp_json:
             log.error(f"Could not find page data with a redirect for site {site_name} page {page_name}")
             return None
         link_type_raw = page_resp_json['redirect']['#t']
         page_type = self._get_type_from_link_type(link_type_raw)
         return Page(page_name, page_type)
 
-    def get_site_page_type(self, site_name: str, page_name: str) -> 'PageType':
-        if site_name not in self._sites:
-            self.get_site_data_by_site_name(site_name)
+    def visit_and_get_form(self, site_name: str, page_name: str) -> 'SailUiForm':
+        """
+        Get a SailUiForm for a Task, Report or Action
 
-        if site_name not in self._sites:
-            raise SiteNotFoundException(f"The site with name '{site_name}' could not be found")
-        site: Site = self._sites[site_name]
-        if page_name not in [page.page_name for page in site.pages.values()]:
-            raise PageNotFoundException(f"The site with name '{site_name}' does not contain the page {page_name}")
-        page = site.pages[page_name]
-        return page.page_type
+        Args:
+            site_name(str): Site where the page exists
+            page_name(str): Page to navigate to
+
+        Returns: SailUiForm
+
+        Example:
+            >>> self.appian.sites.visit_and_get_form("site_name","page_name")
+
+        """
+        resp: Response = self.navigate_to_tab(site_name, page_name)
+        form_uri = resp.request.path_url
+        form_json = resp.json()
+
+        breadcrumb = f"Sites.{site_name}.{page_name}.SailUi"
+        return SailUiForm(self.interactor, form_json, form_uri, breadcrumb=breadcrumb)
 
     def _get_and_memoize_site_data(self, site_name: str, display_name: str, pages_names: List[str]) -> 'Site':
         pages = {}
         for page_name in pages_names:
             page = self.get_site_page(site_name, page_name)
             if page:
                 pages[page_name] = page
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_task_opener.py` & `appian-locust-2.0.0a1/appian_locust/_task_opener.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 
 from . import logger
 from ._interactor import _Interactor
 from .helper import find_component_by_attribute_in_dict
 
 log = logger.getLogger(__name__)
 
@@ -17,15 +17,15 @@
             host (str): Host URL
 
         """
         self.interactor = interactor
 
         self._tasks: Dict[str, Any] = dict()
 
-    def accept_a_task(self, payload: str, task_id: str, headers: Optional[Dict[str, Any]] = None, task_title: str = "", locust_request_label: str = "") -> Dict[str, Any]:
+    def accept_a_task(self, payload: str, task_id: str, headers: Dict[str, Any] = None, task_title: str = "", locust_request_label: str = "") -> Dict[str, Any]:
         """Accept a task if necessary
 
         Args:
             payload (str): string to send as part of accepting a task
             task_id (str): task identifier
             headers (Dict[str, Any], optional): Headers to send. Defaults to {}.
             task_title (str, optional): Task title used to describe the interaction. Defaults to "".
@@ -48,15 +48,15 @@
         headers["X-HTTP-Method-Override"] = "PUT"
 
         label = locust_request_label or f'Tasks.{task_title}.Status'
         resp = self.interactor.post_page(uri=uri, payload=payload, headers=headers,
                                          label=label)
         return resp.json()
 
-    def visit_by_task_id(self, task_title: str, task_id: str, extra_headers: Optional[Dict[str, Any]] = None, locust_request_label: str = "") -> Dict[str, Any]:
+    def visit_by_task_id(self, task_title: str, task_id: str, extra_headers: Dict[str, Any] = None, locust_request_label: str = "") -> Dict[str, Any]:
         """Vist a task page and the corresponding json using the task_id
 
         Args:
             task_title (str): Title to identify the task
             task_id (str): Id used to navigate to the task
             extra_headers (Dict[str, Any], optional): Extra headers, used for sites requests. Defaults to None.
             locust_request_label (str, optional): label to be used within locust
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_tasks.py` & `appian-locust-2.0.0a1/appian_locust/_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Union, Optional
+from typing import Any, Dict, Union
 
 from . import logger
 from ._base import _Base
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error
 from ._task_opener import _TaskOpener
 from .uiform import SailUiForm
@@ -27,15 +27,15 @@
 
         """
         self.interactor = interactor
         self.task_opener = _TaskOpener(self.interactor)
         self._tasks: Dict[str, Any] = dict()
         self._next_uri: Union[str, None] = _Tasks.INITIAL_FEED_URI
 
-    def get_all(self, search_string: Optional[str] = None, locust_request_label: str = "Tasks") -> Dict[str, Any]:
+    def get_all(self, search_string: str = None, locust_request_label: str = "Tasks") -> Dict[str, Any]:
         """
         Retrieves all the available "tasks" and associated metadata from "Appian-Tempo-Tasks"
 
         Note: All the retrieved data about tasks is stored in the private variable self._tasks
 
         Returns (dict): List of tasks and associated metadata
 
@@ -145,35 +145,61 @@
         """
         _, current_task = super().get(self._tasks, task_name, exact_match)
         if not current_task:
             e = Exception(f'There is no task with name "{task_name}" in the system under test (Exact match = {exact_match})')
             log_locust_error(e, raise_error=True)
         return current_task
 
-    def get_task_form_json(self, task_name: str, locust_request_label: str = "", exact_match: bool = True) -> Dict[str, Any]:
+    def visit(self, task_name: str, exact_match: bool = True) -> Dict[str, Any]:
         """
         This function calls the API for the specific task to get its "form" data
 
         Args:
             task_name (str): Name of the task to be called.
             exact_match (bool, optional): Should task name match exactly or to be partial match. Default : True
 
         Returns (dict): Response of task's Get UI call in dictionary
 
         Examples:
 
             If full name of task is known,
 
-            >>> self.appian.task.get_task_form_json("task_name")
+            >>> self.appian.task.visit("task_name")
 
             If only partial name is known,
 
-            >>> self.appian.task.get_task_form_json("task_name", exact_match=False)
+            >>> self.appian.task.visit("task_name", exact_match=False)
 
         """
-        breadcrumb = locust_request_label
+
         task = self.get_task(task_name, exact_match)
+
         clean_id = task["id"].replace("t-", "")
         children = task.get("content", {}).get("children", [])
         task_title = children[0]
 
-        return self.task_opener.visit_by_task_id(task_title=task_title, task_id=clean_id, locust_request_label=breadcrumb)
+        return self.task_opener.visit_by_task_id(task_title, clean_id)
+
+    def visit_and_get_form(self, task_name: str, exact_match: bool = True, locust_request_label: str = "") -> SailUiForm:
+        """
+        Gets the SailUiForm given a task name
+
+        Args:
+            task_name (str): Name of the task to search for
+            exact_match (bool, optional): Whether or not a full match is returned. Defaults to True.
+            locust_request_label (str, optional): label to be used within locust
+
+        Returns:
+            SailUiForm: SAIL form for the task
+        """
+        initial_task_resp: dict = self.get_task(task_name, exact_match)
+        clean_id = initial_task_resp["id"].replace("t-", "")
+        children = initial_task_resp.get("content", {}).get("children", [])
+        task_title = children[0]
+
+        if not locust_request_label:
+            breadcrumb = f"Tasks.{task_title}"
+        else:
+            breadcrumb = locust_request_label
+        form_json = self.task_opener.visit_by_task_id(breadcrumb, clean_id)
+        form_uri = "/suite/rest/a/task/latest/{}/form".format(clean_id)
+        return SailUiForm(self.interactor, form_json, form_uri, breadcrumb=breadcrumb)
```

### Comparing `appian-locust-2.0.0a0/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.0a1/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a0/appian_locust/appianclient.py` & `appian-locust-2.0.0a1/appian_locust/appianclient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import greenlet
 import os
 import re
 import urllib.parse
 import uuid
-from typing import List, Tuple, Optional, Callable, Generator
 
 from locust import SequentialTaskSet, TaskSet
 from locust.clients import HttpSession
 from requests import Response
+from typing import List, Tuple
 
 from . import logger
-from .feature_flag import FeatureFlag
-from ._feature_toggle_helper import (get_client_feature_toggles,
-                                     override_default_feature_flags,
-                                     set_mobile_feature_flags)
+from .exceptions import MissingConfigurationException
+from .loadDriverUtils import utils, DEFAULT_CONFIG_PATH
+from ._actions import _Actions
+from ._admin import Admin
+from ._app_importer import AppImporter
+from ._design import Design
+from ._feature_flag import FeatureFlag
+from ._feature_toggle_helper import get_client_feature_toggles, override_default_flags, set_mobile_feature_flags
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error
-from .exceptions import MissingConfigurationException
-from .tempo_navigator import TempoNavigator
-from .visitor import Visitor
-from .site_helper import SiteHelper
+from ._news import _News
+from ._records import _Records
+from ._reports import _Reports
+from ._sites import _Sites
+from ._tasks import _Tasks
 
 log = logger.getLogger(__name__)
 
 
 # Can be called during an initalization event of a locust test to
 # procedurally generate Appian credentials
 def procedurally_generate_credentials(CONFIG: dict) -> None:
@@ -105,15 +110,15 @@
     def fire(self, *args: str, **kwargs: int) -> None:
         pass
 
     def context(self, *args: str, **kwargs: int) -> dict:
         return {}
 
 
-def appian_client_without_locust(host: str, record_mode: bool = False, base_path_override: Optional[str] = None) -> 'AppianClient':
+def appian_client_without_locust(host: str, record_mode: bool = False, base_path_override: str = None) -> 'AppianClient':
     """
     Returns an AppianClient that can be used without locust to make requests against a host, e.g.
 
     >>> appian_client_without_locust()
     >>> client.login(auth=('username', 'password'))
     >>> client.get_client_feature_toggles()
 
@@ -124,89 +129,175 @@
     inner_client = HttpSession(_trim_trailing_slash(host), NoOpEvents(), NoOpEvents())
     if record_mode:
         setattr(inner_client, 'record_mode', True)
     return AppianClient(inner_client, host=host, base_path_override=base_path_override)
 
 
 class AppianClient:
-    def __init__(self, session: HttpSession, host: str, base_path_override: Optional[str] = None, portals_mode: bool = False) -> None:
+    def __init__(self, session: HttpSession, host: str, base_path_override: str = None, portals_mode: bool = False,
+                 config_path: str = DEFAULT_CONFIG_PATH) -> None:
         """
         Appian client class contains all the required functions to interact with Tempo.
 
         Note: This class will be called inside ``AppianTaskSet`` so it is not necessary to call this explicitly in a test.
         ``self.appian`` can be used directly in a test.
 
         Args:
             session: Locust session/client object
             host (str): Host URL
+            base_path_override (str): override for sites where /suite is not the base path
+            config_path (str): path to configuration file
 
         """
         self.client = session
         self.portals_mode = portals_mode
         self.host = _trim_trailing_slash(host)
-        self._interactor = _Interactor(self.client, self.host, portals_mode=portals_mode)
 
-        self._visitor = Visitor(self._interactor)
-        self._site_helper = SiteHelper(self._interactor)
-        self._tempo_navigator = TempoNavigator(self._interactor)
+        timeout = 300
+        if os.path.exists(config_path):
+            config_timeout = utils.load_config(config_path).get('request_timeout', None)
+            if config_timeout:
+                log.info(f"Overriding default timeout to {config_timeout}s")
+                timeout = config_timeout
+
+        self._interactor = _Interactor(self.client, self.host, portals_mode=portals_mode, request_timeout=timeout)
+
+        self._actions = _Actions(self.interactor)
+        self._admin = Admin(self.interactor)
+        self._design = Design(self.interactor)
+        self._news = _News(self.interactor)
+        self._records = _Records(self.interactor)
+        self._reports = _Reports(self.interactor)
+        self._tasks = _Tasks(self.interactor)
+        self._sites = _Sites(self.interactor)
+        self._app_importer = AppImporter(self.interactor)
 
         # Adding a few session specific attributes to self.client to that it can be carried and handled by session
         # in case of having multiple sessions in the future.
         setattr(self.client, "feature_flag", "")
         setattr(self.client, "feature_flag_extended", "")
 
         # Used for sites where /suite is not in the URL, i.e. local builds
         setattr(self.client, "base_path_override", base_path_override)
 
     @property
-    def visitor(self) -> Visitor:
+    def interactor(self) -> _Interactor:
+        """
+        Interactor that can be used to make lower level requests against Appian
+
+        See :doc:`_interactor <appian_locust._interactor>`
+        """
+        return self._interactor
+
+    @property
+    def actions(self) -> _Actions:
+        """
+        API for querying, starting and completing actions
+
+        See :doc:`_actions <appian_locust._actions>`
+        """
+        return self._actions
+
+    @property
+    def admin(self) -> Admin:
+        """
+        API for interacting with the Admin Console
+
+        See :doc:`_actions <appian_locust._admin>`
+        """
+        return self._admin
+
+    @property
+    def app_importer(self) -> AppImporter:
+        """
+        API for importing applications
+
+        See :doc:`_app_importer <appian_locust._app_importer>`
+        """
+        return self._app_importer
+
+    @property
+    def design(self) -> Design:
+        """
+        API for interacting with /design
+
+        See :doc:`_actions <appian_locust._design>`
+        """
+        return self._design
+
+    @property
+    def news(self) -> _News:
         """
-        Visitor that can be used to navigate to different types of pages in an Appian instance
+        API for interacting with the news feed
+
+        See :doc:`_news <appian_locust._news>`
         """
-        return self._visitor
+        return self._news
 
     @property
-    def tempo_navigator(self) -> TempoNavigator:
+    def records(self) -> _Records:
         """
-        Tempo Navigator that can be used to fetch objects which can provide metadata about Tempo Tabs
+        API for interacting with record lists and record dashboards
+
+        See :doc:`_records <appian_locust._records>`
         """
-        return self._tempo_navigator
+        return self._records
 
     @property
-    def site_helper(self) -> SiteHelper:
+    def reports(self) -> _Reports:
         """
-        SiteHelper used for interactions that do not require a UI
+        API for importing applications
+
+        See :doc:`_reports <appian_locust._reports>`
+        """
+        return self._reports
+
+    @property
+    def tasks(self) -> _Tasks:
         """
-        return self._site_helper
+        API for interacting with tasks and task forms in Appian
 
-    def login(self, auth: Optional[list] = None, check_login: bool = True) -> Tuple[HttpSession, Response]:
-        return self._interactor.login(auth, check_login=check_login)
+        See :doc:`_tasks <appian_locust._tasks>`
+        """
+        return self._tasks
+
+    @property
+    def sites(self) -> _Sites:
+        """
+        API for interacting with sites in Appian
+
+        See :doc:`_sites <appian_locust._sites>`
+        """
+        return self._sites
+
+    def login(self, auth: list = None, check_login: bool = True) -> Tuple[HttpSession, Response]:
+        return self.interactor.login(auth, check_login=check_login)
 
     def logout(self) -> None:
         """
         Logout from Appian
         """
         logout_uri = (
             self.host
             + "/suite/logout?targetUrl="
             + urllib.parse.quote(self.host + "/suite/tempo/")
         )
 
-        headers = self._interactor.setup_request_headers(logout_uri)
+        headers = self.interactor.setup_request_headers(logout_uri)
         if hasattr(greenlet.getcurrent(), "minimal_ident"):
-            log.info(f"Logging out user {self._interactor.auth[0]} from greenlet id {greenlet.getcurrent().minimal_ident}")
+            log.info(f"Logging out user {self.interactor.auth[0]} from greenlet id {greenlet.getcurrent().minimal_ident}")
         else:
-            log.info(f"Logging out user {self._interactor.auth[0]} from {greenlet.getcurrent()}")
-        self._interactor.post_page(logout_uri, headers=headers, label="Logout.LoadUi", check_login=False)
+            log.info(f"Logging out user {self.interactor.auth[0]} from {greenlet.getcurrent()}")
+        self.interactor.post_page(logout_uri, headers=headers, label="Logout.LoadUi", check_login=False)
         self.client.cookies.clear()
 
     def get_client_feature_toggles(self) -> None:
         try:
             self.client.feature_flag, self.client.feature_flag_extended = ("7ffceebc", "1bff7f49dc1fffceebc") if self.portals_mode else (
-                get_client_feature_toggles(self._interactor, self.client)
+                get_client_feature_toggles(self.interactor, self.client)
             )
         except Exception as e:
             log_locust_error(e, error_desc="Client Feature Toggles Error")
             raise e
 
 
 class AppianTaskSet(TaskSet):
@@ -219,45 +310,47 @@
         super().__init__(parent)
 
         self.host = self.parent.host
 
         # A set of datatypes cached. Used to populate "X-Appian-Cached-Datatypes" header field
         self.cached_datatype: set = set()
 
-    def on_start(self, portals_mode: bool = False) -> None:
+    def on_start(self, portals_mode: bool = False, config_path: str = DEFAULT_CONFIG_PATH) -> None:
         """
         Overloaded function of Locust's default on_start.
 
         It will create object self.appian and logs in to Appian
 
         Args:
             portals_mode (bool): set to True if connecting to portals site
+            config_path (str): path to configuration file
         """
         self.portals_mode = portals_mode
         self.workerId = str(uuid.uuid4())
         base_path_override = self.parent.base_path_override \
             if hasattr(self.parent, "base_path_override") else ""
-        self._appian = AppianClient(self.client, self.host, base_path_override=base_path_override, portals_mode=portals_mode)
+        self._appian = AppianClient(self.client, self.host, base_path_override=base_path_override,
+                                    portals_mode=portals_mode, config_path=config_path)
         if not portals_mode:
-            self.auth = self._determine_auth()
+            self.auth = self.determine_auth()
             resp = self.appian.login(self.auth)
             test = r'\\\\\\/suite\\\\\\/rest\\\\\\/a\\\\\\/sites\\\\\\/latest\\\\\\/D6JMim\\\\\\/page\\\\\\/(.+)\\\\\\'
             m = re.search(test, resp[1].text)
             if m is None or m.group(1) == 'news':
                 # old way
-                self.appian._interactor.url_pattern_version = 0
+                self.appian.interactor.url_pattern_version = 0
             elif m.group(1) == 'p.news':
                 # new way
-                self.appian._interactor.url_pattern_version = 1
+                self.appian.interactor.url_pattern_version = 1
             else:
                 log.error("appian-locust could not determine appian interaction url pattern.  Please upgrade to the latest version.")
 
         self.appian.get_client_feature_toggles()
 
-    def _determine_auth(self) -> List[str]:
+    def determine_auth(self) -> List[str]:
         """
         Determines what Appian username/password will be used on simulated logins. Auth will be determined
         using the following rules:
 
         If only "auth" key exists in config file, use the corresponding username and password for every login
 
         If only "credentials" key exists, pop one pair of credentials per Locust user until there's only one pair left.
@@ -305,51 +398,48 @@
         """
         A wrapper around the generated AppianClient
         """
         return self._appian
 
     def override_default_flags(self, flags_to_override: List[FeatureFlag]) -> None:
         """
-        `override_default_flags` gets the flag mask to set all of the flags to true given
-        a list of flag enums and overrides the current feature flag extended value to set
-        these flags to true.
+        API for overriding default feature flags.
+
+        See :doc:`override_default_flags <appian_locust._feature_toggle_helper>`
         """
-        def flags_to_override_generator() -> Generator[FeatureFlag, None, None]:
-            yield from flags_to_override
         try:
-            override_default_feature_flags(self.appian._interactor, flags_to_override_generator)
+            override_default_flags(self.appian.interactor, flags_to_override)
         except Exception as e:
             log_locust_error(e, error_desc="Override Default Flags Error")
             raise e
 
     def declare_device_as_mobile(self) -> None:
         """
         API for designating a device as mobile to spoof running on a mobile device.
+
+        See :doc:`declare_device_as_mobile <appian_locust._feature_toggle_helper>`
         """
         try:
-            set_mobile_feature_flags(self.appian._interactor)
-            self.appian._interactor.set_user_agent_to_mobile()
+            set_mobile_feature_flags(self.appian.interactor)
+            self.appian.interactor.set_user_agent_to_mobile()
         except Exception as e:
             log_locust_error(e, error_desc="Override Default Flags Error")
             raise e
 
     def declare_device_as_desktop(self) -> None:
         """
         API for designating a device as desktop to emulate running on a computer device.
         This is done by default, so only use this method when running a mix of mobile and
         desktop tests.
+
+        See :doc:`declare_device_as_mobile <appian_locust._feature_toggle_helper>`
         """
         try:
-            self.appian._interactor.set_user_agent_to_desktop()
+            self.appian.interactor.set_user_agent_to_desktop()
         except Exception as e:
             log_locust_error(e, error_desc="Error setting device as desktop")
             raise e
 
 
 class AppianTaskSequence(SequentialTaskSet, AppianTaskSet):
-    """
-    Appian Locust SequentialTaskSet. Provides functionality of Locust's SequentialTaskSet and Handles creation of basic
-    objects like``self.appian`` and actions like ``login`` and ``logout``
-    """
-
     def __init__(self, parent: SequentialTaskSet) -> None:
         super(AppianTaskSequence, self).__init__(parent)
```

### Comparing `appian-locust-2.0.0a0/appian_locust/exceptions.py` & `appian-locust-2.0.0a1/appian_locust/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a0/appian_locust/feature_flag.py` & `appian-locust-2.0.0a1/appian_locust/_feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a0/appian_locust/helper.py` & `appian-locust-2.0.0a1/appian_locust/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from . import logger
 
 ENV = Environment()
 log = logger.getLogger(__name__)
 
 
-def format_label(label: str, delimiter: Optional[str] = None, index: int = 0) -> str:
+def format_label(label: str, delimiter: str = None, index: int = 0) -> str:
     """
     Simply formats the string by replacing a space with underscores
 
     Args:
         label: string to be formatted
         delimiter: If provided, string will be split by it
         index: used with delimiter parameter, which item will be used in the "split"ed list.
@@ -30,26 +30,26 @@
         if not str(index).isnumeric():
             index = 0
         label = label.split(delimiter)[int(index)]
 
     return label.replace(" ", "_")
 
 
-def _extract(obj: Any, key: str, vals: List[Any]) -> Generator:
+def extract(obj: Any, key: str, vals: List[Any]) -> Generator:
     """Recursively search for values of key in JSON tree."""
     if isinstance(obj, dict):
         for k, v in obj.items():
             if isinstance(v, (dict, list)):
-                yield from _extract(v, key, vals)
+                yield from extract(v, key, vals)
             elif k == key and v in vals:
                 yield obj
 
     elif isinstance(obj, list):
         for item in obj:
-            yield from _extract(item, key, vals)
+            yield from extract(item, key, vals)
 
 
 def extract_values(obj: Dict[str, Any], key: str, val: Any) -> List[Dict[str, Any]]:
     """
     Pull all values of specified key from nested JSON.
 
     Args:
@@ -57,15 +57,15 @@
         key (str): tuple of key and value.
         val (any): value, which can be any type
 
     Returns:
         list of matched key-value pairs
 
     """
-    return list(_extract(obj, key, [val]))
+    return list(extract(obj, key, [val]))
 
 
 def extract_values_multiple_key_values(obj: Dict[str, Any], key: str, vals: List[Any]) -> List[Dict[str, Any]]:
     """
     Pull all values where the key value matches an entry in vals from nested JSON.
 
     Args:
@@ -73,43 +73,35 @@
         key (str): a key in the dictionary
         vals (List[any]): A list of values corresponding to the key, which can be any type
 
     Returns:
         list of matched key-value pairs
 
     """
-    return list(_extract(obj, key, vals))
+    return list(extract(obj, key, vals))
 
 
-def _extract_item_by_label(obj: Union[dict, list], label: str) -> Generator:
+def extract_item_by_label(obj: Union[dict, list], label: str) -> Generator:
     """
     Recursively search for all fields with a matching label in JSON tree.
     And return as a generator
     """
     if isinstance(obj, dict):
         for k, v in obj.items():
             if k == label:
                 yield v
-            yield from _extract_item_by_label(v, label)
+            yield from extract_item_by_label(v, label)
     elif isinstance(obj, list):
         for v in obj:
-            yield from _extract_item_by_label(v, label)
+            yield from extract_item_by_label(v, label)
 
 
 def extract_all_by_label(obj: Union[dict, list], label: str) -> list:
-    """
-    Recursively search for all fields with a matching label in JSON tree.
-    Args:
-        obj: The json tree to search for fields in
-        label: The label used to identify elements we want to return
-
-    Returns (list): A list of all elements in obj that match label
-
-    """
-    return [elem for elem in _extract_item_by_label(obj, label)]
+    """Recursively search for all fields with a matching label in JSON tree."""
+    return [elem for elem in extract_item_by_label(obj, label)]
 
 
 def get_random_item(list_of_items: List[Any], exclude: List[Any] = []) -> Any:
     """
     Gets a random item from the given list excluding the items if any provided
 
     Args:
@@ -143,16 +135,18 @@
 
     Returns:
         List with filtered values
 
     """
     # Exact Matches gets priority even when exact match is set to false
     return_list = list(filter(lambda current_item: (
-        current_item.split("::")[0] == filter_string), list_var))
+        current_item == filter_string), list_var))
     if not exact_match:
+        return_list = list(filter(lambda current_item: (
+            current_item == filter_string), list_var))
         return_list.extend(list(filter(lambda current_item: (
             bool(re.search(".*" + re.escape(filter_string) + ".*", current_item)) and current_item not in return_list),
             list_var)))
     return return_list
 
 
 def _validate_component_found(component: Optional[Dict[str, Any]], label: str, type: Optional[str] = None) -> None:
@@ -337,17 +331,17 @@
                 return tree
             index -= 1
 
         trees_to_search = list(tree.values()) + trees_to_search
 
     if not raise_error:
         return None
-    if type and not type_check_passed_once:
+    if not type_check_passed_once:
         raise ComponentNotFoundException(f"No components with type '{type}' found on page")
-    if attribute and not attribute_check_passed_once:
+    if not attribute_check_passed_once:
         raise ComponentNotFoundException(f"No components with {attribute} '{value}' found on page")
     raise Exception(f"Index: '{originial_index}' out of range")
 
 
 def find_component_by_attribute_and_index_in_dict(attribute: str, value: str, index: int, component_tree: Dict[str, Any]) -> Any:
     """
     Find a UI component by the given attribute (label for example) in a dictionary
@@ -408,19 +402,11 @@
                 gevent.sleep(wait_time)
             return value
         return wrapper_decorator
     return decorator
 
 
 def get_username(auth: list) -> str:
-    """
-    Returns the username from an auth list
-    Args:
-        auth: Appian Locust authorization list
-
-    Returns (str): Username from auth list
-
-    """
     if auth and len(auth) >= 1 and auth[0]:
         return auth[0]
     else:
         return ""
```

### Comparing `appian-locust-2.0.0a0/appian_locust/loadDriverUtils.py` & `appian-locust-2.0.0a1/appian_locust/loadDriverUtils.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,30 +17,22 @@
         "exec_start_end_task": 1,
     },
     "skip_machine_setup": False,
     "auth": ["username", "password"]
 }
 
 log = logger.getLogger(__name__)
+DEFAULT_CONFIG_PATH = "./config.json"
 
 
 class loadDriverUtils:
     def __init__(self) -> None:
         self.c = default_config
 
-    def load_config(self, config_file: str = "./config.json") -> dict:
-        """
-        Load a json configuration file into a dictionary
-        Args:
-            config_file: Location where config file can be found
-
-        Returns (dict): Dictionary containing configuration. Will also be stored in
-                        loadDriverUtils.c
-
-        """
+    def load_config(self, config_file: str = DEFAULT_CONFIG_PATH) -> dict:
         if os.path.exists(config_file):
             self.c = json.load(open(config_file))
             return self.c
         else:
             log.error("Failed to load config ({}), exiting.".format(config_file))
             log.error("Example config:{}".format(json.dumps(default_config,
                                                             indent=2)))
```

### Comparing `appian-locust-2.0.0a0/appian_locust/logger.py` & `appian-locust-2.0.0a1/appian_locust/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Optional
 
 """
 Custom logger module borrowing all the functionality of original python's logger module.
 Additionally it sets the format of the log to '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 
 Make sure to name the logger "log" or anything other than "logger" on the receiving script to ensure Mypy conformity
 
@@ -14,15 +13,15 @@
     >>> log.info("Info message")
 
 """
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
 
-def getLogger(name: Optional[str] = None) -> logging.Logger:
+def getLogger(name: str = None) -> logging.Logger:
     """
 
     Args:
         name(str, optional): Name of the logger. it is common practice to use file name here but it can be anything.
 
     Returns: logger object
```

### Comparing `appian-locust-2.0.0a0/appian_locust/uiform.py` & `appian-locust-2.0.0a1/appian_locust/uiform.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import datetime
 import enum
 import errno
 import json
 import os
 import random
 import warnings
-from typing import Any, Dict, List, Union, Optional, TYPE_CHECKING
+from typing import Any, Dict, List, Union, Optional
 from urllib.parse import quote, urlparse
-from copy import deepcopy
 
-from appian_locust._records_helper import _is_grid
+from appian_locust.records_helper import _is_grid
 
 from . import logger
 from ._grid_interactor import GridInteractor
 from ._interactor import _Interactor
 from ._locust_error_handler import raises_locust_error
 from ._task_opener import _TaskOpener
 from ._ui_reconciler import UiReconciler
-from .exceptions import InvalidComponentException, ChoiceNotFoundException
+from .exceptions import ComponentNotFoundException, InvalidComponentException, ChoiceNotFoundException
 from .helper import (extract_all_by_label, find_component_by_attribute_and_index_in_dict,
                      find_component_by_attribute_in_dict, find_component_by_index_in_dict,
                      find_component_by_label_and_type_dict, find_component_by_type_and_attribute_and_index_in_dict)
-from ._records_helper import (get_url_stub_from_record_list_url_path)
-
-if TYPE_CHECKING:
-    from .record_uiform import RecordInstanceUiForm
+from .records_helper import (get_record_header_response,
+                             get_record_summary_view_response,
+                             get_url_stub_from_record_list_url_path)
 
 KEY_UUID = "uuid"
 KEY_CONTEXT = "context"
 START_PROCESS_LINK_TYPE = 'StartProcessLink'
 PROCESS_TASK_LINK_TYPE = 'ProcessTaskLink'
 COMPONENTS_THAT_CAN_BE_FILLED = ["ParagraphField", "TextField", "SearchBoxWidget"]
 
@@ -37,54 +35,75 @@
 
 class ClientMode(enum.Enum):
     TEMPO = 'TEMPO'
     DESIGN = 'DESIGN'
 
 
 class SailUiForm:
-    def __init__(self, interactor: _Interactor, state: Dict[str, Any], breadcrumb: str = "SailUi"):
+    def __init__(self, interactor: _Interactor, state: Dict[str, Any], url: str, breadcrumb: str = "SailUi"):
         """
-        Appian rendered UI that provides page interactivity. ``SailUiForm`` is a base class that is abstracted
-        by specific Appian form types to handle requirements or provide metadata unique to that page.
+        UIForm Class used to interact with a SAIL form used in an action, record, etc..
 
         Args:
             base: Action, Record, etc.. interactor object
             state: JSON representation of the initial form
             latest_state: JSON representation of the last to the the form
             url: Url to make updates to the form
             breadcrumbs: Path used to create locust labels
 
         """
-        self._interactor: _Interactor = interactor
-        self.task_opener: _TaskOpener = _TaskOpener(self._interactor)
-        self._state: Dict[str, Any] = state
-        self.form_url = ""
-        self.form_url = self._get_update_url_for_reeval(state)
-        if any(key not in self._state for key in (KEY_CONTEXT, KEY_UUID)):
+        self.interactor: _Interactor = interactor
+        self.task_opener: _TaskOpener = _TaskOpener(self.interactor)
+        self.state: Dict[str, Any] = state
+        self.form_url = url
+        if any(key not in self.state for key in (KEY_CONTEXT, KEY_UUID)):
             return None
-        self.context: dict = self._state[KEY_CONTEXT]
-        self.uuid: str = self._state[KEY_UUID]
+        self.context: dict = self.state[KEY_CONTEXT]
+        self.uuid: str = self.state[KEY_UUID]
         self.grid_interactor: GridInteractor = GridInteractor()
         self.reconciler: UiReconciler = UiReconciler()
         self.breadcrumb = breadcrumb
 
         # Cache data types on opening new form
-        self._interactor.datatype_cache.cache(self._state)
+        self.interactor.datatype_cache.cache(self.state)
+
+    def get_response(self) -> Optional[Dict[str, Any]]:
+        """
+        Latest state response
+
+        Returns (dict): The last recorded response
+
+        """
+        warnings.warn("The method 'get_response' is deprecated, just do 'self.state' to get the latest returned value")
+        return self.state
 
-    def get_latest_state(self) -> Dict[str, Any]:
+    @property
+    def latest_state(self) -> Optional[Dict[str, Any]]:
         """
-        Provides a deep copy of latest state of UI form.
+        Latest state response
+
+        Returns (dict): The last recorded response
 
-        Returns (dict): deep copy of last recorded response.
+        """
+        warnings.warn("The method 'latest_state' is deprecated, just do 'self.state' on the last returned value")
+        return self.state
 
+    def get_latest_form(self) -> 'SailUiForm':
         """
-        return deepcopy(self._state)
+        Latest ui form
+
+        Returns (dict): The ui form with its current ui
+
+        """
+        warnings.warn("The method 'get_latest_form' is deprecated, "
+                      "ui is now updated on each call, you can just chain methods without calling `get_latest_form`")
+        return self
 
     def __str__(self) -> str:
-        return f"self_state={json.dumps(self._state,indent=4)}"
+        return f"self_state={json.dumps(self.state,indent=4)}"
 
     @raises_locust_error
     def fill_field_by_attribute_and_index(self, attribute: str, attribute_value: str, fill_value: str, index: int = 1, locust_request_label: str = "") -> 'SailUiForm':
         """
         Selects a Field by "attribute" and its value provided "attribute_value" and an index if more than one Field is found
         and fills it with text "fill_value"
 
@@ -106,27 +125,27 @@
             # and fills it with "Hello, Testing"
 
             >>> form.fill_field_by_attribute_and_index("label", "Write a comment", "Hello, Testing", 2)
             # selects the second Component with the "label" attribute having "Write a comment" value
             # and fills it with "Hello, Testing"
 
         """
-        component = find_component_by_attribute_and_index_in_dict(attribute, attribute_value, index, self._state)
+        component = find_component_by_attribute_and_index_in_dict(attribute, attribute_value, index, self.state)
 
         if component.get("#t", "") not in COMPONENTS_THAT_CAN_BE_FILLED:
             raise Exception(f"The Component with '{attribute}' = '{attribute_value}' is not a component that can be filled")
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         locust_label = locust_request_label or f"{self.breadcrumb}.FillTextFieldByAttribute.{attribute}"
-        new_state = self._interactor.fill_textfield(
+        new_state = self.interactor.fill_textfield(
             reeval_url, component, fill_value, self.context, self.uuid, label=locust_label)
         if not new_state:
             raise Exception(f"No response returned when trying to update the field with '{attribute}' = '{attribute_value}' at index '{index}'")
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def fill_text_field(self, label: str, value: str, is_test_label: bool = False, locust_request_label: str = "", index: int = 1) -> 'SailUiForm':
         """
         Fills a field on the form, if there is one present with the following label (case sensitive)
         Otherwise throws a NotFoundException
 
@@ -166,27 +185,27 @@
 
         Examples:
 
             >>> form.fill_field_by_index("ParagraphField", 1, "Hello, Testing")
             # selects the first ParagraphField with the value "Hello, Testing"
 
         """
-        component = find_component_by_index_in_dict(type_of_component, index, self._state)
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        component = find_component_by_index_in_dict(type_of_component, index, self.state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         locust_label = locust_request_label or f"{self.breadcrumb}.FillTextFieldByIndex.{index}"
-        new_state = self._interactor.fill_textfield(
+        new_state = self.interactor.fill_textfield(
             reeval_url, component, text_to_fill, self.context, self.uuid, label=locust_label)
         if not new_state:
             raise Exception(
                 f'''
                     No response returned when trying to fill: '{text_to_fill}' in the component: '{type_of_component}'
                     with index: '{index}' on the current page")
                 ''')
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def fill_field_by_any_attribute(self, attribute: str, value_for_attribute: str, text_to_fill: str, locust_request_label: str = "", index: int = 1) -> 'SailUiForm':
         """
         Selects a Field by "attribute" and its value provided "value_for_attribute"
         and fills it with text "text_to_fill"
 
@@ -242,18 +261,18 @@
             >>> form.fill_picker_field('Title','My New Novel')
             >>> form.fill_picker_field('People','Jeff George')
             >>> form.fill_picker_field('Customer', 'GAC Guyana', identifier='code')
 
         """
         # pickerFieldCustom will add a test-Label at the level where the suggestions/saveInto exist
         test_label = f'test-{label}'
-        component = find_component_by_label_and_type_dict('testLabel', test_label, 'PickerWidget', self._state)
+        component = find_component_by_label_and_type_dict('testLabel', test_label, 'PickerWidget', self.state)
 
         locust_label = fill_request_label or f"{self.breadcrumb}.FillPickerField.{label}"
-        new_state = self._interactor.fill_pickerfield_text(
+        new_state = self.interactor.fill_pickerfield_text(
             self.form_url, component, value, self.context, self.uuid, label=locust_label)
 
         if not new_state:
             raise Exception(f"No response returned when trying to update field with label '{label}'")
 
         component = find_component_by_label_and_type_dict('testLabel', test_label, 'PickerWidget', new_state)
 
@@ -277,15 +296,15 @@
             raise Exception(f"Could not extract picker values '{id_index}' from suggestions_list {suggestions_list}")
 
         v_choice = random.choice(range(len(v_or_id)))
 
         dict_value = identifiers[v_choice]
 
         locust_label = pick_request_label or f"{self.breadcrumb}.SelectPickerSuggestion.{label}"
-        newer_state = self._interactor.select_pickerfield_suggestion(
+        newer_state = self.interactor.select_pickerfield_suggestion(
             self.form_url, component, dict_value, self.context, self.uuid, label=locust_label)
 
         if not newer_state:
             raise Exception(f"No response returned when trying to update field with label '{label}'")
 
         return self._reconcile_state(newer_state)
 
@@ -373,25 +392,25 @@
 
     def _click(self, label: str, is_test_label: bool = False, locust_request_label: str = "", index: int = 1) -> 'SailUiForm':
         """
         Internal function wrapped by various click methods
         """
         attribute_to_find = 'testLabel' if is_test_label else 'label'
 
-        component = find_component_by_attribute_and_index_in_dict(attribute_to_find, label, index, self._state)
+        component = find_component_by_attribute_and_index_in_dict(attribute_to_find, label, index, self.state)
 
         locust_label = locust_request_label or f"{self.breadcrumb}.Click.{label}"
         new_state = self._dispatch_click(component=component, locust_label=locust_label)
 
         # get the re-eval URI from links object of the response (new_state)
         reeval_url = self._get_update_url_for_reeval(new_state)
 
         if not new_state:
             raise Exception(f"No response returned when trying to click button with label '{label}'")
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def click_card_layout_by_index(self, index: int, locust_request_label: str = "") -> 'SailUiForm':
         """
         Clicks a card layout link by index.
         This method will find the CardLayout component on the UI by index and then perform
         the click behavior on its Link component.
@@ -408,36 +427,36 @@
         Examples:
             This finds link field on the 2nd card layout on the page and clicks it. It handles StartProcessLink as well, so
             no need to call click_start_process_link() when it is on a CardLayout.
 
             >>> form.click_card_layout_by_index(2)
 
         """
-        component = find_component_by_index_in_dict("CardLayout", index, self._state)
+        component = find_component_by_index_in_dict("CardLayout", index, self.state)
 
         if not component.get("link"):
             raise Exception(f"CardLayout found at index: {index} does not have a link on it")
 
         link_component = component.get('link')
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickCardLayout.Index.{index}"
         if link_component["#t"] == "StartProcessLink":
             site_name = link_component["siteUrlStub"] or "D6JMim"
             page_name = link_component["sitePageUrlStub"]
             new_state = self._click_start_process_link(site_name, page_name, False, link_component, locust_request_label=locust_label)
         else:
-            new_state = self._interactor.click_component(self.form_url, link_component, self.context, self.uuid, label=locust_label)
+            new_state = self.interactor.click_component(self.form_url, link_component, self.context, self.uuid, label=locust_label)
 
         if not new_state:
             raise Exception(f"No response returned when trying to click card layout at index '{index}'")
 
         reeval_url = self._get_update_url_for_reeval(new_state)
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
-    def click_record_link_by_attribute_and_index(self, attribute: str = "", attribute_value: str = "", index: int = 1, locust_request_label: str = "") -> 'RecordInstanceUiForm':
+    def click_record_link_by_attribute_and_index(self, attribute: str = "", attribute_value: str = "", index: int = 1, locust_request_label: str = "") -> 'SailUiForm':
         """
         Click the index'th record link on the form if there is one present with an attribute matching attribute_value
         If no attribute is provided, the index'th record link is selected from all record links in the form
         Otherwise throws a ComponentNotFoundException
 
         Keyword Args:
             attribute(str): Attribute to check for 'attribute_value' (default: "")
@@ -445,43 +464,42 @@
             index(int): Index of record link to click (default: 1)
             locust_request_label(str): Label used to identify the request for locust statistics
 
         Returns (SailUiForm): The record form (feed) for the linked record.
 
         """
         component_type = 'RecordLink'
-        component = find_component_by_type_and_attribute_and_index_in_dict(self._state, component_type, attribute, attribute_value, index)
+        component = find_component_by_type_and_attribute_and_index_in_dict(self.state, component_type, attribute, attribute_value, index)
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickRecordLink"
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.click_record_link(reeval_url, component, self.context, self.uuid,
-                                                       locust_label=locust_label)
-        from .record_uiform import RecordInstanceUiForm
-        return RecordInstanceUiForm(self._interactor, new_state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.click_record_link(reeval_url, component, self.context, self.uuid,
+                                                      locust_label=locust_label)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
-    def click_record_link(self, label: str, is_test_label: bool = False, locust_request_label: str = "") -> 'RecordInstanceUiForm':
+    def click_record_link(self, label: str, is_test_label: bool = False, locust_request_label: str = "") -> 'SailUiForm':
         """
         Click a record link on the form if there is one present with the following label (case sensitive)
         Otherwise throws a ComponentNotFoundException
 
         Args:
             label(str): Label of the record link to click
             is_test_label(bool): If you are clicking a record link via a test label instead of a label, set this boolean to true
 
         Keyword Args:
             locust_request_label(str): Label used to identify the request for locust statistics
 
-        Returns (RecordUiForm): The record form (feed) for the linked record.
+        Returns (SailUiForm): The record form (feed) for the linked record.
 
         """
         attribute_to_find = 'testLabel' if is_test_label else 'label'
         return self.click_record_link_by_attribute_and_index(attribute=attribute_to_find, attribute_value=label, locust_request_label=locust_request_label)
 
     @raises_locust_error
-    def click_record_link_by_index(self, index: int, locust_request_label: str = "") -> 'RecordInstanceUiForm':
+    def click_record_link_by_index(self, index: int, locust_request_label: str = "") -> 'SailUiForm':
         """
         Click the index'th record link on the form
         Otherwise throws a ComponentNotFoundException
 
         Args:
             index(int): Index of the record link to click (1-based)
 
@@ -490,37 +508,36 @@
 
         Returns (SailUiForm): The record form (feed) for the linked record.
 
         """
         return self.click_record_link_by_attribute_and_index(index=index, locust_request_label=locust_request_label)
 
     @raises_locust_error
-    def click_record_view_link(self, label: str, locust_request_label: str = "") -> 'RecordInstanceUiForm':
+    def click_record_view_link(self, label: str, locust_request_label: str = "") -> 'SailUiForm':
         """
         Click a record view link on the form if there is one present with the following label (case sensitive)
         Otherwise throws a ComponentNotFoundException
 
         Args:
             label(str): Label of the record link to click
 
         Keyword Args:
             locust_request_label(str): Label used to identify the request for locust statistics
 
         Returns (SailUiForm): The record form (feed) for the linked record.
 
         """
         view_tab_label = f"{label}_tab"
-        outer_component = find_component_by_attribute_in_dict(attribute="testLabel", value=view_tab_label, component_tree=self._state)
+        outer_component = find_component_by_attribute_in_dict(attribute="testLabel", value=view_tab_label, component_tree=self.state)
         component = outer_component["link"]
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickRecordLink"
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.click_record_link(reeval_url, component, self.context, self.uuid,
-                                                       locust_label=locust_label)
-        from .record_uiform import RecordInstanceUiForm
-        return RecordInstanceUiForm(self._interactor, new_state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.click_record_link(reeval_url, component, self.context, self.uuid,
+                                                      locust_label=locust_label)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def click_start_process_link(self, label: str, site_name: str, page_name: str, is_mobile: bool = False, locust_request_label: str = "") -> 'SailUiForm':
         """
         Clicks a start process link on the form by label
         If no link is found, throws a ComponentNotFoundException
 
@@ -536,20 +553,22 @@
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
             >>> form.click_start_process_link('Request upgrade')
 
         """
 
-        component = find_component_by_label_and_type_dict('label', label, START_PROCESS_LINK_TYPE, self._state)
+        component = find_component_by_label_and_type_dict('label', label, START_PROCESS_LINK_TYPE, self.state)
 
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickStartProcessLink.{label}"
         new_state = self._click_start_process_link(site_name, page_name, is_mobile, component, locust_request_label=locust_label)
 
-        return self._reconcile_state(new_state)
+        # get the re-eval URI from links object of the response (new_state)
+        reeval_url = self._get_update_url_for_reeval(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def click_start_process_link_on_mobile(self, label: str, site_name: str, page_name: str, locust_request_label: str = "") -> 'SailUiForm':
         """
         Clicks a start process link on the form by label (for Mobile)
         If no link is found, throws a ComponentNotFoundException
 
@@ -580,17 +599,17 @@
         process_model_opaque_id = component.get("processModelOpaqueId", "")
         cache_key = component.get("cacheKey", "")
         if not process_model_opaque_id:
             raise Exception(f"StartProcessLink component does not have process model opaque id set.")
         elif not cache_key:
             raise Exception(f"StartProcessLink component does not have cache key set.")
 
-        return self._interactor.click_start_process_link(component=component, process_model_opaque_id=process_model_opaque_id,
-                                                         cache_key=cache_key, site_name=site_name, page_name=page_name, is_mobile=is_mobile,
-                                                         locust_request_label=locust_request_label)
+        return self.interactor.click_start_process_link(component=component, process_model_opaque_id=process_model_opaque_id,
+                                                        cache_key=cache_key, site_name=site_name, page_name=page_name, is_mobile=is_mobile,
+                                                        locust_request_label=locust_request_label)
 
     def _dispatch_click(self, component: Dict[str, Any], locust_label: str) -> Dict[str, Any]:
         """
         Dispatches the appropriate link interaction based on the link type if appropriate
 
         Args:
             link_component (Dict[str, Any]): Link component to interact with
@@ -622,17 +641,17 @@
             headers = {
                 'X-Site-UrlStub': site_name,
                 'X-Page-UrlStub': page_name,
                 'X-Client-Mode': 'SITES'
             }
             new_state = self.task_opener.visit_by_task_id(task_name, task_id, extra_headers=headers)
         elif link_component:
-            new_state = self._interactor.click_component(self.form_url, link_component, self.context, self.uuid, label=locust_label)
+            new_state = self.interactor.click_component(self.form_url, link_component, self.context, self.uuid, label=locust_label)
         else:
-            new_state = self._interactor.click_component(self.form_url, component, self.context, self.uuid, label=locust_label)
+            new_state = self.interactor.click_component(self.form_url, component, self.context, self.uuid, label=locust_label)
         return new_state
 
     @raises_locust_error
     def click_related_action(self, label: str, locust_request_label: str = "") -> 'SailUiForm':
         """
         Clicks a related action (either a related action button or link) on the form by label
         If no link is found, throws a ComponentNotFoundException
@@ -657,15 +676,15 @@
             or if it is a related action link on the summary view UI (which opens in a dialog).
 
             >>> header_form = feed_form.get_record_header_form() or feed_form.get_record_view_form()
 
             >>> header_form.click_related_action('Request upgrade')
 
         """
-        component = find_component_by_attribute_in_dict('label', label, self._state)
+        component = find_component_by_attribute_in_dict('label', label, self.state)
 
         # Support scenario where related action label is found within outer "ButtonWidget" rather than directly in "RelatedActionLink" component
         if "source" not in component:
             component = component.get("link", "")
         component_source = component.get("source", "")
         record_type_stub = component_source.get("recordTypeStub", "")
         opaque_related_action_id = component_source.get("opaqueRelatedActionId", "")
@@ -677,18 +696,20 @@
 
         if not record_type_stub or not opaque_record_id or not opaque_related_action_id:
             raise Exception(f'''
                             Related Action link component does not have recordTypeStub or opaqueRecordId or opaqueRelatedActionId set.
                             ''')
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickRelatedActionLink.{label}"
 
-        new_state = self._interactor.click_related_action(component, record_type_stub=record_type_stub, opaque_record_id=opaque_record_id,
-                                                          opaque_related_action_id=opaque_related_action_id,
-                                                          locust_request_label=locust_label, open_in_a_dialog=open_action_in_a_dialog)
-        return self._reconcile_state(new_state)
+        new_state = self.interactor.click_related_action(component, record_type_stub=record_type_stub, opaque_record_id=opaque_record_id,
+                                                         opaque_related_action_id=opaque_related_action_id,
+                                                         locust_request_label=locust_label, open_in_a_dialog=open_action_in_a_dialog)
+        # get the re-eval URI from links object of the response (new_state)
+        reeval_url = self._get_update_url_for_reeval(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def get_dropdown_items(self, label: str, is_test_label: bool = False) -> List[str]:
         """
         Gets all dropdown items for the dropdown label provided on the form
         If no dropdown found, throws a NotFoundException
 
@@ -702,15 +723,15 @@
         Examples:
 
             >>> form.get_dropdown_items('MyDropdown')
 
         """
         attribute_to_find = 'testLabel' if is_test_label else 'label'
         component = find_component_by_attribute_in_dict(
-            attribute_to_find, label, self._state)
+            attribute_to_find, label, self.state)
 
         choices: list = component.get('choices')
         if choices is None or not isinstance(choices, list):
             raise InvalidComponentException(f"No choices found for component {label}, is the component a Dropdown?")
         return choices
 
     @raises_locust_error
@@ -734,38 +755,38 @@
         Examples:
 
             >>> form.select_dropdown_item('MyDropdown', 'My First Choice')
 
         """
         attribute_to_find = 'testLabel' if is_test_label else 'label'
         component = find_component_by_attribute_in_dict(
-            attribute_to_find, label, self._state)
+            attribute_to_find, label, self.state)
 
         choices: list = component.get('choices')
         if not choices:
             raise InvalidComponentException(f"No choices found for component {label}, is the component a Dropdown?")
         if not isinstance(choice_label, list) and choice_label not in choices:
             raise ChoiceNotFoundException(f"Choice {choice_label} not found for component {label}, valid choices were {choices}")
 
         index = choices.index(choice_label) + 1  # Appian is _sigh_ one indexed
         locust_label = locust_request_label or f'{self.breadcrumb}.SelectDropdownWithLabel.{label}'
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
 
         # Opting to use this field, rather than self.form_url, because 'sail-application-url' is the same between web and mobile
-        url = self._state.get('sail-application-url')
+        url = self.state.get('sail-application-url')
         # url_stub should only be populated if the page is a record list
         url_stub = get_url_stub_from_record_list_url_path(url)
 
-        new_state = self._interactor.send_dropdown_update(
+        new_state = self.interactor.send_dropdown_update(
             reeval_url, component, self.context, self.uuid, index=index, label=locust_label, url_stub=url_stub)
         if not new_state:
             raise Exception(
                 f"No response returned when trying to click button with label '{label}'")
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def select_multi_dropdown_item(self, label: str, choice_label: List[str], locust_request_label: str = "", is_test_label: bool = False) -> 'SailUiForm':
         """
         Selects a multiple dropdown item on the form
         If no multiple dropdown found, throws a NotFoundException
         If no element found, throws a ChoiceNotFoundException
@@ -784,37 +805,37 @@
         Examples:
 
             >>> form.select_multi_dropdown_item('MyMultiDropdown', ['My First Choice','My Second Choice'])
 
         """
         attribute_to_find = 'testLabel' if is_test_label else 'label'
         component = find_component_by_attribute_in_dict(
-            attribute_to_find, label, self._state)
+            attribute_to_find, label, self.state)
 
         choices: list = component.get('choices')
         if not choices:
             raise InvalidComponentException(f"No choices found for component {label}, is the component a Dropdown?")
         if not isinstance(choice_label, list) and choice_label not in choices:
             raise ChoiceNotFoundException(f"Choice {choice_label} not found for component {label}, valid choices were {choices}")
         index_multi = [choices.index(current_label) + 1 for current_label in choice_label]  # Appian is _sigh_ one indexed
         locust_label = locust_request_label or f'{self.breadcrumb}.SelectMultupleDropdownWithLabel.{choice_label}'
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
 
         # Opting to use this field, rather than self.form_url, because 'sail-application-url' is the same between web and mobile
-        url = self._state.get('sail-application-url')
+        url = self.state.get('sail-application-url')
         # url_stub should only be populated if the page is a record list
         url_stub = get_url_stub_from_record_list_url_path(url)
 
-        new_state = self._interactor.send_multiple_dropdown_update(
+        new_state = self.interactor.send_multiple_dropdown_update(
             reeval_url, component, self.context, self.uuid, index=index_multi, label=locust_label, url_stub=url_stub)
         if not new_state:
             raise Exception(
                 f"No response returned when trying to click button with label '{label}'")
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     def _check_checkbox_by_attribute(self, attribute: str, value_for_attribute: str, indices: List[int], locust_request_label: str = "") -> 'SailUiForm':
         """
         Function that checks checkboxes.
         It finds checkboxes by the attribute and its value provided.
 
         Args:
@@ -823,27 +844,27 @@
             indices(str): Indices of the checkbox to check. Pass None or empty to uncheck all
 
         Keyword Args:
             locust_request_label(str): Label used to identify the request for locust statistics
 
         Returns (SailUiForm): The latest state of the UiForm
         """
-        component = find_component_by_attribute_in_dict(attribute, value_for_attribute, self._state,
+        component = find_component_by_attribute_in_dict(attribute, value_for_attribute, self.state,
                                                         throw_attribute_exception=True)
 
         locust_label = locust_request_label or f'{self.breadcrumb}.CheckCheckboxByAttribute.{attribute}'
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.select_checkbox_item(
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.select_checkbox_item(
             reeval_url, component, self.context, self.uuid, indices=indices, context_label=locust_label)
         if not new_state:
             raise Exception(f'''No response returned when trying to check checkbox which was found with attribute: '{attribute}'
                             and its value: '{value_for_attribute}' on the current page
                             ''')
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def check_checkbox_by_test_label(self, test_label: str, indices: List[int], locust_request_label: str = "") -> 'SailUiForm':
         """
         Checks a checkbox by its testLabel attribute
         Indices are positions to be checked
 
@@ -909,26 +930,26 @@
 
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
 
         """
         # find the TabButtonGroup, which is the  model we need for the SaveRequest
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
 
-        tab_group_component = find_component_by_attribute_in_dict('testLabel', tab_group_test_label, self._state)
-        new_state = self._interactor.click_selected_tab(
+        tab_group_component = find_component_by_attribute_in_dict('testLabel', tab_group_test_label, self.state)
+        new_state = self.interactor.click_selected_tab(
             reeval_url, tab_group_component, tab_label, self.context, self.uuid)
         if not new_state:
             raise Exception(
                 f'''No response returned when trying to click a tab with label: '{tab_label}'
                 inside the TabButtonGroup component with testLabel: '{tab_group_test_label}'''
             )
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def upload_document_to_upload_field(self, label: str, file_path: Union[str, List], locust_request_label: str = "") -> 'SailUiForm':
         """
         Uploads a document to a named upload field
         There are two steps to this which can fail, one is the document upload, the other
         is finding the component and applying the update.
@@ -945,15 +966,15 @@
         Examples:
 
             >>> form.upload_document_to_upload_field('Upload File', "/usr/local/appian/File.zip")
             >>> form.upload_document_to_upload_field('Upload Properties', "/usr/local/appian/File.properties")
 
         """
         component = find_component_by_attribute_in_dict(
-            'label', label, self._state)
+            'label', label, self.state)
 
         # Inner component can be the upload field
         if component.get('#t') != 'FileUploadWidget' and 'contents' in component:
             component = component['contents']
 
         # Check again to see if the wrong component
         if component.get('#t') != 'FileUploadWidget':
@@ -966,17 +987,17 @@
         if type(file_path) != str:
             raise Exception(f"Provided file_path {file_path} was not a string, was instead of type '{type(file_path)}'")
 
         is_encrypted = component.get("isEncrypted", False)
 
         if not os.path.exists(str(file_path)):
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), file_path)
-        doc_id = self._interactor.upload_document_to_server(str(file_path), is_encrypted=is_encrypted)
+        doc_id = self.interactor.upload_document_to_server(str(file_path), is_encrypted=is_encrypted)
         locust_label = locust_request_label or f"{self.breadcrumb}.FileUpload.{label}"
-        new_state = self._interactor.upload_document_to_field(
+        new_state = self.interactor.upload_document_to_field(
             self.form_url, component, self.context, self.uuid, doc_id=doc_id, locust_label=locust_label)
         if not new_state:
             raise Exception(
                 f"No response returned when trying to upload file to field '{label}'")
         return self._reconcile_state(new_state)
 
     @raises_locust_error
@@ -997,15 +1018,15 @@
 
         Example:
 
             >>> form.multi_upload_document_to_upload_field('Upload Files', ["/usr/local/appian/File1.zip", "/usr/local/appian/File2.zip"])
 
         """
         component = find_component_by_attribute_in_dict(
-            'label', label, self._state)
+            'label', label, self.state)
 
         # Inner component can be the upload field
         if component.get('#t') != 'MultipleFileUploadWidget' and 'contents' in component:
             component = component['contents']
 
         # Check again to see if the wrong component
         if component.get('#t') != 'MultipleFileUploadWidget':
@@ -1016,17 +1037,17 @@
 
         is_encrypted = component.get("isEncrypted", False)
 
         doc_ids: List[int] = []
         for file_path in file_paths:
             if not os.path.exists(file_path):
                 raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), file_path)
-            doc_ids.append(self._interactor.upload_document_to_server(file_path, is_encrypted=is_encrypted))
+            doc_ids.append(self.interactor.upload_document_to_server(file_path, is_encrypted=is_encrypted))
         locust_label = locust_request_label or f"{self.breadcrumb}.MultiFileUpload.{label}"
-        new_state = self._interactor.upload_document_to_field(
+        new_state = self.interactor.upload_document_to_field(
             self.form_url, component, self.context, self.uuid, doc_id=doc_ids, locust_label=locust_label)
         if not new_state:
             raise Exception(
                 f"No response returned when trying to upload file(s) to field '{label}'")
         return self._reconcile_state(new_state)
 
     @raises_locust_error
@@ -1048,27 +1069,27 @@
             >>> form.fill_date_field('Today', datetime.date.today())
             >>> form.fill_date_field('Date of Birth', datetime.date(1992, 12, 30))
 
         """
         if not isinstance(date_input, datetime.date):
             raise Exception("Input must be of type datetime.date")
         field_type = 'DatePickerField'
-        date_field = find_component_by_label_and_type_dict('label', label, field_type, self._state)
+        date_field = find_component_by_label_and_type_dict('label', label, field_type, self.state)
 
         locust_label = locust_request_label or f'{self.breadcrumb}.FillDateField'
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
 
-        new_state = self._interactor.update_date_field(
+        new_state = self.interactor.update_date_field(
             reeval_url, date_field, date_input, self.context, self.uuid, locust_label=locust_label)
         if not new_state:
             raise Exception(f'''No response returned when trying to update: '{label}'
                             with its value: '{date_input}' on the current page
                             ''')
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def fill_datetime_field(self, label: str, datetime_input: datetime.datetime, locust_request_label: str = "") -> 'SailUiForm':
         """
         Fills a datetime field with the specified datetime
 
         NOTE: this does one api call for both the date and time, whereas filling the elements on screen requires
@@ -1089,30 +1110,30 @@
             >>> form.fill_datetime_field('Now', datetime.datetime.now())
             >>> form.fill_datetime_field('Date and Time of Birth', datetime.datetime(1992, 12, 30, 12, 30, 5))
 
         """
         if not isinstance(datetime_input, datetime.datetime):
             raise Exception("Input must be of type datetime.datetime")
         field_type = 'DateTimePickerField'
-        datetime_field = find_component_by_label_and_type_dict('label', label, field_type, self._state)
+        datetime_field = find_component_by_label_and_type_dict('label', label, field_type, self.state)
 
         locust_label = locust_request_label or f'{self.breadcrumb}.FillDateTimeField'
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
 
-        new_state = self._interactor.update_datetime_field(
+        new_state = self.interactor.update_datetime_field(
             reeval_url, datetime_field, datetime_input, self.context, self.uuid, locust_label=locust_label)
         if not new_state:
             raise Exception(f'''No response returned when trying to update: '{label}'
                             with its value: '{datetime_input}' on the current page
                             ''')
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
-    def select_rows_in_grid(self, rows: List[int], label: Optional[str] = None, index: Optional[int] = None, locust_request_label: str = "") -> 'SailUiForm':
+    def select_rows_in_grid(self, rows: List[int], label: str = None, index: int = None, locust_request_label: str = "") -> 'SailUiForm':
         """
         Selects rows in a grid
         Either a label or an index is required, indices are useful if there is no title for the grid
 
         Args:
             rows(List[int]): The rows to select
             label(str): Label of the grid
@@ -1123,27 +1144,27 @@
 
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
 
             >>> form.select_rows_in_grid(rows=[1], label='my nice grid')
         """
-        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=label, index=index)
+        grid = self.grid_interactor.find_grid_by_label_or_index(self.state, label=label, index=index)
         grid_label = self.grid_interactor.format_grid_display_label(grid)
 
         new_grid_save = self.grid_interactor.select_rows(grid, rows)
         context_label = locust_request_label or f"{self.breadcrumb}.Grid.SelectRows.{grid_label}"
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
-                                                                self.context, self.uuid, context_label=context_label)
-        return self._reconcile_state(new_state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
+                                                               self.context, self.uuid, context_label=context_label)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
-    def move_to_end_of_paging_grid(self, label: Optional[str] = None, index: Optional[int] = None, locust_request_label: str = "") -> 'SailUiForm':
+    def move_to_end_of_paging_grid(self, label: str = None, index: int = None, locust_request_label: str = "") -> 'SailUiForm':
         """
         Moves to the end of a paging grid, if possible
         Either a label or an index is required, indices are useful if there is no title for the grid
 
         Args:
             label(str): Label of the grid
             index(int): Index of the grid
@@ -1153,54 +1174,54 @@
 
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
 
             >>> form.move_to_end_of_paging_grid(label='my nice grid')
         """
-        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=label, index=index)
+        grid = self.grid_interactor.find_grid_by_label_or_index(self.state, label=label, index=index)
         grid_label = self.grid_interactor.format_grid_display_label(grid)
 
         new_grid_save = self.grid_interactor.move_to_last_page(grid)
         context_label = locust_request_label or f"{self.breadcrumb}.Grid.MoveToEnd.{grid_label}"
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
-                                                                self.context, self.uuid, context_label=context_label)
-        return self._reconcile_state(new_state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
+                                                               self.context, self.uuid, context_label=context_label)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
-    def move_to_beginning_of_paging_grid(self, label: Optional[str] = None, index: Optional[int] = None, locust_request_label: str = "") -> 'SailUiForm':
+    def move_to_beginning_of_paging_grid(self, label: str = None, index: int = None, locust_request_label: str = "") -> 'SailUiForm':
         """
         Moves to the beginning of a paging grid, if possible
         Either a label or an index is required, indices are useful if there is no title for the grid
 
         Args:
             label(str): Label of the grid
             index(int): Index of the grid
 
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
 
             >>> form.move_to_beginning_of_paging_grid(label='my nice grid')
         """
-        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=label, index=index)
+        grid = self.grid_interactor.find_grid_by_label_or_index(self.state, label=label, index=index)
         grid_label = self.grid_interactor.format_grid_display_label(grid)
 
         new_grid_save = self.grid_interactor.move_to_first_page(grid)
         context_label = locust_request_label or f"{self.breadcrumb}.Grid.MoveToBeginning.{grid_label}"
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
-                                                                self.context, self.uuid, context_label=context_label)
-        return self._reconcile_state(new_state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
+                                                               self.context, self.uuid, context_label=context_label)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
-    def move_to_left_in_paging_grid(self, label: Optional[str] = None, index: Optional[int] = None, locust_request_label: str = "") -> 'SailUiForm':
+    def move_to_left_in_paging_grid(self, label: str = None, index: int = None, locust_request_label: str = "") -> 'SailUiForm':
         """
         Moves to the left in a paging grid, if possible
         It might require getting the state of the grid if you've moved to the end/ previous part of the grid
         Either a label or an index is required, indices are useful if there is no title for the grid
 
         Args:
             label(str): Label of the grid
@@ -1211,27 +1232,27 @@
 
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
 
             >>> form.move_to_left_in_paging_grid(label='my nice grid')
         """
-        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=label, index=index)
+        grid = self.grid_interactor.find_grid_by_label_or_index(self.state, label=label, index=index)
         grid_label = self.grid_interactor.format_grid_display_label(grid)
 
         new_grid_save = self.grid_interactor.move_to_the_left(grid)
         context_label = locust_request_label or f"{self.breadcrumb}.Grid.MoveLeft.{grid_label}"
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
-                                                                self.context, self.uuid, context_label=context_label)
-        return self._reconcile_state(new_state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
+                                                               self.context, self.uuid, context_label=context_label)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
-    def move_to_right_in_paging_grid(self, label: Optional[str] = None, index: Optional[int] = None, locust_request_label: str = "") -> 'SailUiForm':
+    def move_to_right_in_paging_grid(self, label: str = None, index: int = None, locust_request_label: str = "") -> 'SailUiForm':
         """
         Moves to the right in a paging grid, if possible
         It might require getting the state of the grid if you've moved within the grid
         Either a label or an index is required, indices are useful if there is no title for the grid
 
         Args:
             label(str): Label of the grid
@@ -1242,27 +1263,27 @@
 
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
 
             >>> form.move_to_right_in_paging_grid(index=0) # move to right in first grid on the page
         """
-        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=label, index=index)
+        grid = self.grid_interactor.find_grid_by_label_or_index(self.state, label=label, index=index)
         grid_label = self.grid_interactor.format_grid_display_label(grid)
 
         new_grid_save = self.grid_interactor.move_to_the_right(grid)
         context_label = locust_request_label or f"{self.breadcrumb}.Grid.MoveRight.{grid_label}"
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
-                                                                self.context, self.uuid, context_label=context_label)
-        return self._reconcile_state(new_state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
+                                                               self.context, self.uuid, context_label=context_label)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
-    def sort_paging_grid(self, label: Optional[str] = None, index: Optional[int] = None, field_name: str = "", ascending: bool = False, locust_request_label: str = "") -> 'SailUiForm':
+    def sort_paging_grid(self, label: str = None, index: int = None, field_name: str = "", ascending: bool = False, locust_request_label: str = "") -> 'SailUiForm':
         """
         Sorts a paging grid by the field name, which is not necessarily the same as the label of the column
         And might require inspecting the JSON to determine what the sort field is
 
         Sorts by ascending = False by default, override to set it to True
 
         Either a label or an index is required, indices are useful if there is no title for the grid
@@ -1280,24 +1301,24 @@
 
         Examples:
 
             >>> form.sort_paging_grid(index=0,field_name='Total',ascending=True)
         """
         if not field_name:
             raise Exception("Field to sort cannot be blank when sorting a grid")
-        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=label, index=index)
+        grid = self.grid_interactor.find_grid_by_label_or_index(self.state, label=label, index=index)
         grid_label = self.grid_interactor.format_grid_display_label(grid)
 
         new_grid_save = self.grid_interactor.sort_grid(field_name=field_name, paging_grid=grid, ascending=ascending)
         context_label = locust_request_label or f"{self.breadcrumb}.Grid.Sort.{grid_label}.{field_name}"
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
-        new_state = self._interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
-                                                                self.context, self.uuid, context_label=context_label)
-        return self._reconcile_state(new_state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
+        new_state = self.interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
+                                                               self.context, self.uuid, context_label=context_label)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def select_card_choice_field_by_label(self, label: str, index: int, locust_request_label: str = "") -> 'SailUiForm':
         """
         Select a card by it's lable
         Index is position to be selected
 
@@ -1311,24 +1332,24 @@
 
             >>> form.select_card_choice_field_by_label('myLabel', 1)  # selects the first item
 
         """
         context_label = locust_request_label or f"{self.breadcrumb}.CardChoice.SelectByLabel.{label}"
         label = "cardChoiceField-" + label
         component = find_component_by_attribute_in_dict(
-            'testLabel', label, self._state)
+            'testLabel', label, self.state)
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         new_value = component["identifiers"][index - 1]
-        new_state = self._interactor.click_generic_element(
+        new_state = self.interactor.click_generic_element(
             reeval_url, component, self.context, self.uuid, new_value=new_value, label=context_label)
         if not new_state:
             raise Exception(
                 f"No response returned when trying to select card choice field with testLabel '{label}'")
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def select_radio_button_by_test_label(self, test_label: str, index: int, locust_request_label: str = "") -> 'SailUiForm':
         """
         Selects a radio button by its test label
         Index is position to be selected
 
@@ -1340,24 +1361,24 @@
 
         Examples:
 
             >>> form.select_radio_button_by_test_label('myTestLabel', 1)  # selects the first item
 
         """
         component = find_component_by_attribute_in_dict(
-            'testLabel', test_label, self._state)
+            'testLabel', test_label, self.state)
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         context_label = locust_request_label or f"{self.breadcrumb}.RadioButton.SelectByTestLabel.{test_label}"
-        new_state = self._interactor.select_radio_button(
+        new_state = self.interactor.select_radio_button(
             reeval_url, component, self.context, self.uuid, index=index, context_label=context_label)
         if not new_state:
             raise Exception(
                 f"No response returned when trying to select radio button with testLabel '{test_label}'")
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def select_radio_button_by_label(self, label: str, index: int, locust_request_label: str = "") -> 'SailUiForm':
         """
         Selects a radio button by its label
         Index is position to be selected
 
@@ -1372,24 +1393,24 @@
 
         Examples:
 
             >>> form.select_radio_button_by_label('myLabel', 1)  # selects the first item
 
         """
         component = find_component_by_attribute_in_dict(
-            'label', label, self._state)
+            'label', label, self.state)
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         context_label = locust_request_label or f"{self.breadcrumb}.RadioButton.SelectByLabel.{label}"
-        new_state = self._interactor.select_radio_button(
+        new_state = self.interactor.select_radio_button(
             reeval_url, component, self.context, self.uuid, index=index, context_label=context_label)
         if not new_state:
             raise Exception(
                 f"No response returned when trying to select radio button with label '{label}'")
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def select_nav_card_by_index(self, nav_group_label: str, index: int, is_test_label: bool = False, locust_request_label: str = "") -> 'SailUiForm':
         """
         Selects an element of a navigation card group by its index
 
         Args:
@@ -1423,49 +1444,112 @@
 
         Examples:
 
             >>> form.select_radio_button_by_index(1, 1)  # selects the first item in the first radio button field
 
         """
         component = find_component_by_index_in_dict(
-            'RadioButtonField', field_index, self._state)
+            'RadioButtonField', field_index, self.state)
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         context_label = locust_request_label or f"{self.breadcrumb}.RadioButton.SelectByIndex.{index}"
-        new_state = self._interactor.select_radio_button(
+        new_state = self.interactor.select_radio_button(
             reeval_url, component, self.context, self.uuid, index=index, context_label=context_label)
         if not new_state:
             raise Exception(
                 f"No response returned when trying to select radio button with index '{field_index}'")
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     def go_to_next_record_grid_page(self, locust_request_label: str = "") -> 'SailUiForm':
         context_label = locust_request_label or f"{self.breadcrumb}.NextPage"
-        headers = self._interactor.setup_request_headers()
+        headers = self.interactor.setup_request_headers()
         headers["Accept"] = "application/vnd.appian.tv.ui+json"
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         label = 'NEXT'
-        if not _is_grid(self._state):
+        if not _is_grid(self.state):
             raise Exception("Not a grid record list")
         component = find_component_by_attribute_in_dict(
-            'label', label, self._state)
-        new_state = self._interactor.interact_with_record_grid(
+            'label', label, self.state)
+        new_state = self.interactor.interact_with_record_grid(
             post_url=reeval_url, grid_component=component, context=self.context, uuid=self.uuid, context_label=context_label)
         if not new_state:
             raise Exception(
                 f"No response returned when navigating to next page on record list '{reeval_url}'")
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
+
+    def get_record_header_form(self) -> 'SailUiForm':
+        """
+        Extracts the embedded record header form from a record "feed" form to enable interaction with components in the record header.
+
+        Returns (SailUiForm): The record header UiForm embedded within a record "feed" form.
+
+        Examples:
+
+            >>> form.get_record_header_form()
+
+        """
+        # self in this case is a record form (feed) containing embedded forms (header and view form)
+        record_header_response = json.loads(get_record_header_response(self.state))
+
+        # record "feed" form has no breadcrumb - set up a breadcrumb
+        self.breadcrumb = "Record.HeaderForm.SailUi"
+
+        reeval_url = self._get_update_url_for_reeval(record_header_response)
+        return SailUiForm(self.interactor, record_header_response, reeval_url,
+                          breadcrumb=self.breadcrumb)
+
+    def get_record_view_form(self) -> 'SailUiForm':
+        """
+        Extracts the embedded record view form from a record "feed" form to enable interaction with components in the record view.
+
+        Returns (SailUiForm): The record view UiForm embedded within a record "feed" form.
+
+        Examples:
+
+            >>> form.get_record_view_form()
+
+        """
+        record_view_response = json.loads(get_record_summary_view_response(self.state))
+
+        # record "feed" form has no breadcrumb - set up a breadcrumb
+        self.breadcrumb = "Record.ViewForm.SailUi"
+
+        reeval_url = self._get_update_url_for_reeval(record_view_response)
+        return SailUiForm(self.interactor, record_view_response, reeval_url, breadcrumb=self.breadcrumb)
+
+    def filter_records_using_searchbox(self, search_term: str = "", locust_request_label: str = "") -> 'SailUiForm':
+        """
+        This method allows you to Filter the Record Type List (displaying record instance for a specific record type)
+        which makes the same request when typing something in the search box and reloading the page.
+        More interactions (with the filtered list) can be performed on the returned SailUiForm Object.
+
+        Note: This is different from how an end user interacts with the SearchBox. In that case you would type something in the box
+        and when you would unfocus from the box a reevaluation happens and then you click the 'Search' button which returns the filtered
+        results.
+
+        Examples:
+
+            >>> form.filter_records_using_searchbox('Donuts')
+
+        Returns (SailUiForm): The record type list UiForm with the filtered results.
+        """
+        context_label = locust_request_label or f"{self.breadcrumb}.RecordType.SearchByText"
+        search_uri = f"{self.form_url}?searchTerm={quote(search_term)}"
+
+        headers = self.interactor.setup_sail_headers()
+        response = self.interactor.get_page(uri=search_uri, headers=headers, label=context_label)
+        return SailUiForm(self.interactor, response.json(), self.form_url, breadcrumb=context_label)
 
     def assert_no_validations_present(self) -> 'SailUiForm':
         """
         Raises an exception if there are validations present on the form, otherwise, returns the form as is
 
         Returns (SailUiForm): Form as it was when validations were asserted
         """
-        validations: list = extract_all_by_label(self._state, "validations")
+        validations: list = extract_all_by_label(self.state, "validations")
         validation_present = False
         for validation in validations:
             if validation:
                 log.error(f'Validations were found in the form {self.breadcrumb}, validation: {validation}')
                 validation_present = True
         if validation_present:
             raise Exception(f"At least one validation was found in the form {self.breadcrumb}")
@@ -1491,28 +1575,28 @@
             >>> ...
             >>> form.click('Submit')
             >>> initial_form.refresh_after_record_action('Request upgrade')
 
         """
 
         record_action_component = find_component_by_attribute_in_dict(
-            'label', label, self._state)
+            'label', label, self.state)
 
         record_action_trigger_component = find_component_by_attribute_in_dict(
-            '_actionName', 'sail:record-action-trigger', self._state)
+            '_actionName', 'sail:record-action-trigger', self.state)
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         locust_label = locust_request_label or f"{self.breadcrumb}.RefreshAfterRecordAction.{label}"
-        new_state = self._interactor.refresh_after_record_action(
+        new_state = self.interactor.refresh_after_record_action(
             reeval_url, record_action_component, record_action_trigger_component, self.context, self.uuid, label=locust_label)
 
         if not new_state:
             raise Exception(f"No response returned when trying to refresh after record action '{label}'")
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
     @raises_locust_error
     def click_record_search_button_by_index(self, index: int = 1, locust_request_label: str = "") -> 'SailUiForm':
         """
         Clicks the Search button of a record grid.
 
         Args:
@@ -1524,47 +1608,45 @@
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
 
             >>> form.click_record_search_button_by_index(1)
 
         """
-        component = find_component_by_index_in_dict("SearchBoxWidget", index, self._state)
+        component = find_component_by_index_in_dict("SearchBoxWidget", index, self.state)
 
-        reeval_url = self._get_update_url_for_reeval(self._state)
+        reeval_url = self._get_update_url_for_reeval(self.state)
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickRecordSearchButtonByIndex.{index}"
-        new_state = self._interactor.click_record_search_button(
+        new_state = self.interactor.click_record_search_button(
             reeval_url, component, self.context, self.uuid, label=locust_label)
 
         if not new_state:
             raise Exception(f"No response returned when trying to click record search button at index '{index}'")
 
-        return self._reconcile_state(new_state)
+        return self._reconcile_state(new_state, form_url=reeval_url)
 
-    def _reconcile_state(self, new_state: dict) -> 'SailUiForm':
-        self._interactor.datatype_cache.cache(new_state)
-        self._state = self.reconciler.reconcile_ui(self._state, new_state)
-        self.form_url = self._get_update_url_for_reeval(self._state)
-        self.uuid = self._state.get(KEY_UUID) or self.uuid
-        self.context = self._state.get(KEY_CONTEXT) or self.context
+    def _reconcile_state(self, new_state: dict, form_url: str = "") -> 'SailUiForm':
+        self.interactor.datatype_cache.cache(new_state)
+        self.state = self.reconciler.reconcile_ui(self.state, new_state)
+        self.form_url = form_url or self.form_url
+        self.uuid = self.state.get(KEY_UUID) or self.uuid
+        self.context = self.state.get(KEY_CONTEXT) or self.context
         return self
 
     def _get_update_url_for_reeval(self, state: Dict[str, Any]) -> str:
         """
         This function looks at the links object in a SAIL response
         and finds the URL for "rel"="update", which is then used to do other
         interactions on the form.
         """
 
         # If state is None (usually for tests) we return empty string for re-eval url
         if not state:
             return ""
-        reeval_url = self.form_url
-        if "links" not in state:
-            return reeval_url
         # get the re-eval URI from links object of the response (new_state)
         list_of_links = state["links"]
+        reeval_url = self.form_url
         for link_object in list_of_links:
             if link_object.get("rel") == "update":
                 reeval_url = urlparse(link_object.get("href", "")).path
                 break
         return reeval_url
```

### Comparing `appian-locust-2.0.0a0/appian_locust.egg-info/SOURCES.txt` & `appian-locust-2.0.0a1/appian_locust.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,35 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 appian_locust/__init__.py
 appian_locust/_actions.py
 appian_locust/_admin.py
+appian_locust/_app_importer.py
 appian_locust/_base.py
 appian_locust/_design.py
+appian_locust/_feature_flag.py
 appian_locust/_feature_toggle_helper.py
 appian_locust/_grid_interactor.py
 appian_locust/_interactor.py
 appian_locust/_locust_error_handler.py
 appian_locust/_news.py
-appian_locust/_portals.py
 appian_locust/_records.py
-appian_locust/_records_helper.py
 appian_locust/_reports.py
 appian_locust/_save_request_builder.py
 appian_locust/_sites.py
 appian_locust/_task_opener.py
 appian_locust/_tasks.py
 appian_locust/_ui_reconciler.py
-appian_locust/actions_info.py
 appian_locust/appianclient.py
-appian_locust/application_uiform.py
-appian_locust/design_object_type.py
-appian_locust/design_object_uiform.py
-appian_locust/design_uiform.py
 appian_locust/exceptions.py
-appian_locust/feature_flag.py
 appian_locust/helper.py
 appian_locust/loadDriverUtils.py
 appian_locust/logger.py
-appian_locust/news_info.py
-appian_locust/record_list_uiform.py
-appian_locust/record_uiform.py
-appian_locust/records_info.py
-appian_locust/reports_info.py
-appian_locust/site_helper.py
-appian_locust/tasks_info.py
-appian_locust/tempo_navigator.py
+appian_locust/records_helper.py
 appian_locust/uiform.py
-appian_locust/visitor.py
 appian_locust.egg-info/PKG-INFO
 appian_locust.egg-info/SOURCES.txt
 appian_locust.egg-info/dependency_links.txt
 appian_locust.egg-info/requires.txt
 appian_locust.egg-info/top_level.txt
```

### Comparing `appian-locust-2.0.0a0/setup.cfg` & `appian-locust-2.0.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a0/setup.py` & `appian-locust-2.0.0a1/setup.py`

 * *Files identical despite different names*

