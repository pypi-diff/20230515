# Comparing `tmp/ewoksppf-0.1.3.tar.gz` & `tmp/ewoksppf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksppf-0.1.3.tar", last modified: Wed Mar 29 07:49:10 2023, max compression
+gzip compressed data, was "dist/ewoksppf-0.1.4.tar", last modified: Mon May 15 16:49:49 2023, max compression
```

## Comparing `ewoksppf-0.1.3.tar` & `ewoksppf-0.1.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      980 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1226 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22611 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/bindings.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/ppfrunscript.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 07:49:04.000000 ewoksppf-0.1.3/src/ewoksppf/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_examples.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAdd.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAdd2.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAddA.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAddA2B.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAddABC2D.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAddB.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAddB2C.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAddC2D.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorAddWithoutSleep.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorCheck.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorDiamondTest.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorTest.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonErrorHandlerTest.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_end.py
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow1.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow10.py
--rw-rw-rw-   0 root         (0) root         (0)     4178 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow11.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow12.py
--rw-rw-rw-   0 root         (0) root         (0)     3056 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow13.py
--rw-rw-rw-   0 root         (0) root         (0)     3486 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow14.py
--rw-rw-rw-   0 root         (0) root         (0)     3306 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow15.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow16.py
--rw-rw-rw-   0 root         (0) root         (0)     1821 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow17.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow18.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow19.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow2.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-03-29 07:46:52.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow20.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow21.py
--rw-rw-rw-   0 root         (0) root         (0)     3685 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow22.py
--rw-rw-rw-   0 root         (0) root         (0)     3169 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow23.py
--rw-rw-rw-   0 root         (0) root         (0)     5821 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow24.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow3.py
--rw-rw-rw-   0 root         (0) root         (0)     2592 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow6.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow7.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow8.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-03-29 07:42:25.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow9.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-03-29 07:36:31.000000 ewoksppf-0.1.3/src/ewoksppf/tests/test_workflow_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      980 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2189 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      177 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-29 07:49:10.000000 ewoksppf-0.1.3/src/ewoksppf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-15 16:44:42.000000 ewoksppf-0.1.4/src/ewoksppf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22611 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/bindings.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/ppfrunscript.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:49:43.000000 ewoksppf-0.1.4/src/ewoksppf/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_examples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAdd.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAdd2.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAddA.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAddA2B.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAddABC2D.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAddB.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAddB2C.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAddC2D.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorAddWithoutSleep.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorCheck.py
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorDiamondTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonErrorHandlerTest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_end.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow10.py
+-rw-rw-rw-   0 root         (0) root         (0)     4178 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow11.py
+-rw-rw-rw-   0 root         (0) root         (0)     3154 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow12.py
+-rw-rw-rw-   0 root         (0) root         (0)     3056 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow13.py
+-rw-rw-rw-   0 root         (0) root         (0)     3486 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow14.py
+-rw-rw-rw-   0 root         (0) root         (0)     3306 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow15.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow16.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow17.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow18.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow19.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow20.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow21.py
+-rw-rw-rw-   0 root         (0) root         (0)     3685 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow22.py
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow23.py
+-rw-rw-rw-   0 root         (0) root         (0)     5821 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow24.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow3.py
+-rw-rw-rw-   0 root         (0) root         (0)     2592 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow6.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow7.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow8.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow9.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-15 15:51:24.000000 ewoksppf-0.1.4/src/ewoksppf/tests/test_workflow_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-15 16:49:49.000000 ewoksppf-0.1.4/src/ewoksppf.egg-info/top_level.txt
```

### Comparing `ewoksppf-0.1.3/LICENSE.md` & `ewoksppf-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/PKG-INFO` & `ewoksppf-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksppf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pypushflow binding for Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksppf/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksppf/
 Project-URL: Documentation, https://ewoksppf.readthedocs.io/
```

### Comparing `ewoksppf-0.1.3/setup.cfg` & `ewoksppf-0.1.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	ewokscore >=0.3.1
+	ewokscore >=0.4.1
 	pypushflow >=0.4.0
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
@@ -44,19 +44,14 @@
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 
-[build_sphinx]
-project = ewoksppf
-version = attr: ewoksppf.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [egg_info]
 tag_build =
```

### Comparing `ewoksppf-0.1.3/src/ewoksppf/bindings.py` & `ewoksppf-0.1.4/src/ewoksppf/bindings.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/ppfrunscript.py` & `ewoksppf-0.1.4/src/ewoksppf/ppfrunscript.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         inputs=kwargs,
         varinfo=varinfo,
         execinfo=execinfo,
     )
 
     task.execute()
 
-    return task.output_transfer_data
+    return task.get_output_transfer_data()
```

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_examples.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_actors/pythonActorDiamondTest.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_actors/pythonActorDiamondTest.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_end.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_end.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow1.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow1.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow10.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow10.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow11.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow11.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow12.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow12.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow13.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow13.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow14.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow14.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow15.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow15.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow16.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow16.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow17.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow17.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow18.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow18.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow19.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow19.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow2.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow2.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow20.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow20.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow21.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow21.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow22.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow22.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow23.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow23.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow24.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow24.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow3.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow3.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow6.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow6.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow7.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow7.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow8.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow8.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_ppf_workflow9.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_ppf_workflow9.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf/tests/test_workflow_events.py` & `ewoksppf-0.1.4/src/ewoksppf/tests/test_workflow_events.py`

 * *Files identical despite different names*

### Comparing `ewoksppf-0.1.3/src/ewoksppf.egg-info/PKG-INFO` & `ewoksppf-0.1.4/src/ewoksppf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksppf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pypushflow binding for Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksppf/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksppf/
 Project-URL: Documentation, https://ewoksppf.readthedocs.io/
```

### Comparing `ewoksppf-0.1.3/src/ewoksppf.egg-info/SOURCES.txt` & `ewoksppf-0.1.4/src/ewoksppf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

