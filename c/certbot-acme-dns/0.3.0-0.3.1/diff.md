# Comparing `tmp/certbot-acme-dns-0.3.0.tar.gz` & `tmp/certbot-acme-dns-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-acme-dns-0.3.0.tar", last modified: Fri Mar  3 13:09:17 2023, max compression
+gzip compressed data, was "certbot-acme-dns-0.3.1.tar", last modified: Mon May 15 10:41:24 2023, max compression
```

## Comparing `certbot-acme-dns-0.3.0.tar` & `certbot-acme-dns-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-03 13:09:17.563829 certbot-acme-dns-0.3.0/
--rw-r--r--   0 user       (501) staff       (20)       90 2023-03-03 12:34:47.000000 certbot-acme-dns-0.3.0/.gitignore
--rw-r--r--   0 user       (501) staff       (20)     1293 2023-03-03 10:28:44.000000 certbot-acme-dns-0.3.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     2996 2023-03-03 13:09:17.563649 certbot-acme-dns-0.3.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     2172 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.0/README.md
--rw-r--r--   0 user       (501) staff       (20)     4821 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.0/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-03-03 13:09:17.563868 certbot-acme-dns-0.3.0/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-03 13:09:17.558279 certbot-acme-dns-0.3.0/src/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-03 13:09:17.559489 certbot-acme-dns-0.3.0/src/certbot_acme_dns/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-03 13:09:17.560970 certbot-acme-dns-0.3.0/src/certbot_acme_dns/_internal/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns/_internal/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2969 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns/_internal/acme_dns.py
--rw-r--r--   0 user       (501) staff       (20)     3410 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns/_internal/caa.py
--rw-r--r--   0 user       (501) staff       (20)     1234 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns/_internal/util.py
--rw-r--r--   0 user       (501) staff       (20)     7975 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns/plugin.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns/py.typed
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-03 13:09:17.560211 certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     2996 2023-03-03 13:09:17.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      684 2023-03-03 13:09:17.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-03-03 13:09:17.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       67 2023-03-03 13:09:17.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       73 2023-03-03 13:09:17.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       17 2023-03-03 13:09:17.000000 certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-03 13:09:17.563343 certbot-acme-dns-0.3.0/tests/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/tests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1048 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/tests/conftest.py
--rw-r--r--   0 user       (501) staff       (20)     3679 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/tests/test_acme_dns.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/tests/test_caa.py
--rw-r--r--   0 user       (501) staff       (20)      103 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/tests/test_plugin.py
--rw-r--r--   0 user       (501) staff       (20)      210 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.0/tests/test_utils.py
+drwxrwxrwx   0 user       (501) staff       (20)        0 2023-05-15 10:41:24.560049 certbot-acme-dns-0.3.1/
+-rw-r--r--   0 user       (501) staff       (20)       90 2023-03-03 12:34:47.000000 certbot-acme-dns-0.3.1/.gitignore
+-rw-r--r--   0 user       (501) staff       (20)     1293 2023-03-03 10:28:44.000000 certbot-acme-dns-0.3.1/LICENSE
+-rw-rw-rw-   0 user       (501) staff       (20)     2996 2023-05-15 10:41:24.559848 certbot-acme-dns-0.3.1/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     2172 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.1/README.md
+-rw-r--r--   0 user       (501) staff       (20)     4821 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.1/pyproject.toml
+-rw-rw-rw-   0 user       (501) staff       (20)       38 2023-05-15 10:41:24.560089 certbot-acme-dns-0.3.1/setup.cfg
+drwxrwxrwx   0 user       (501) staff       (20)        0 2023-05-15 10:41:24.555317 certbot-acme-dns-0.3.1/src/
+drwxrwxrwx   0 user       (501) staff       (20)        0 2023-05-15 10:41:24.556684 certbot-acme-dns-0.3.1/src/certbot_acme_dns/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns/__init__.py
+drwxrwxrwx   0 user       (501) staff       (20)        0 2023-05-15 10:41:24.558303 certbot-acme-dns-0.3.1/src/certbot_acme_dns/_internal/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns/_internal/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2969 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns/_internal/acme_dns.py
+-rw-r--r--   0 user       (501) staff       (20)     3410 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns/_internal/caa.py
+-rw-r--r--   0 user       (501) staff       (20)     1234 2023-03-03 12:54:39.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns/_internal/util.py
+-rw-r--r--   0 user       (501) staff       (20)     7974 2023-05-15 10:29:59.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns/plugin.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns/py.typed
+drwxrwxrwx   0 user       (501) staff       (20)        0 2023-05-15 10:41:24.557409 certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     2996 2023-05-15 10:41:24.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      684 2023-05-15 10:41:24.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 10:41:24.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       67 2023-05-15 10:41:24.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       73 2023-05-15 10:41:24.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       17 2023-05-15 10:41:24.000000 certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/top_level.txt
+drwxrwxrwx   0 user       (501) staff       (20)        0 2023-05-15 10:41:24.559559 certbot-acme-dns-0.3.1/tests/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/tests/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1048 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/tests/conftest.py
+-rw-r--r--   0 user       (501) staff       (20)     3679 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/tests/test_acme_dns.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/tests/test_caa.py
+-rw-r--r--   0 user       (501) staff       (20)      103 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/tests/test_plugin.py
+-rw-r--r--   0 user       (501) staff       (20)      210 2023-03-03 09:57:40.000000 certbot-acme-dns-0.3.1/tests/test_utils.py
```

### Comparing `certbot-acme-dns-0.3.0/LICENSE` & `certbot-acme-dns-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot-acme-dns-0.3.0/PKG-INFO` & `certbot-acme-dns-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-acme-dns
-Version: 0.3.0
+Version: 0.3.1
 Summary: ACME DNS Authenticator plugin for Certbot
 Author-email: Patrik Hagara <patrihagar+certbot-acme-dns@gmail.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/phagara/certbot-acme-dns
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `certbot-acme-dns-0.3.0/README.md` & `certbot-acme-dns-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `certbot-acme-dns-0.3.0/pyproject.toml` & `certbot-acme-dns-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `certbot-acme-dns-0.3.0/src/certbot_acme_dns/_internal/acme_dns.py` & `certbot-acme-dns-0.3.1/src/certbot_acme_dns/_internal/acme_dns.py`

 * *Files identical despite different names*

### Comparing `certbot-acme-dns-0.3.0/src/certbot_acme_dns/_internal/caa.py` & `certbot-acme-dns-0.3.1/src/certbot_acme_dns/_internal/caa.py`

 * *Files identical despite different names*

### Comparing `certbot-acme-dns-0.3.0/src/certbot_acme_dns/_internal/util.py` & `certbot-acme-dns-0.3.1/src/certbot_acme_dns/_internal/util.py`

 * *Files identical despite different names*

### Comparing `certbot-acme-dns-0.3.0/src/certbot_acme_dns/plugin.py` & `certbot-acme-dns-0.3.1/src/certbot_acme_dns/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         force_interactive: bool = False,
         decorate: bool = True,
     ) -> None:
         """Backwards compatibility wrapper for the notification display utility."""
         return zope.component.getUtility(IDisplay).notification(  # type: ignore[no-any-return]
             message=message,
             pause=pause,
-            wrape=wrap,
+            wrap=wrap,
             force_interactive=force_interactive,
             decorate=decorate,
         )
 
 
 from ._internal.acme_dns import AcmeDns, AcmeDnsAccount
 from ._internal.caa import CaaSecurityChecker, CaaUnconfigured
```

### Comparing `certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/PKG-INFO` & `certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-acme-dns
-Version: 0.3.0
+Version: 0.3.1
 Summary: ACME DNS Authenticator plugin for Certbot
 Author-email: Patrik Hagara <patrihagar+certbot-acme-dns@gmail.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/phagara/certbot-acme-dns
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `certbot-acme-dns-0.3.0/src/certbot_acme_dns.egg-info/SOURCES.txt` & `certbot-acme-dns-0.3.1/src/certbot_acme_dns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-acme-dns-0.3.0/tests/conftest.py` & `certbot-acme-dns-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `certbot-acme-dns-0.3.0/tests/test_acme_dns.py` & `certbot-acme-dns-0.3.1/tests/test_acme_dns.py`

 * *Files identical despite different names*

