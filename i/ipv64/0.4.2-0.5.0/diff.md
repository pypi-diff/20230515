# Comparing `tmp/ipv64-0.4.2.tar.gz` & `tmp/ipv64-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipv64-0.4.2.tar", last modified: Sat Jan  7 14:04:55 2023, max compression
+gzip compressed data, was "ipv64-0.5.0.tar", last modified: Mon May 15 17:44:24 2023, max compression
```

## Comparing `ipv64-0.4.2.tar` & `ipv64-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-07 14:04:55.539309 ipv64-0.4.2/
--rw-rw-rw-   0        0        0     1084 2022-11-16 15:45:47.000000 ipv64-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     2689 2023-01-07 14:04:55.540308 ipv64-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2371 2023-01-07 13:02:08.000000 ipv64-0.4.2/README.md
--rw-rw-rw-   0        0        0      111 2023-01-07 14:04:55.541311 ipv64-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-01-07 14:04:19.000000 ipv64-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-07 14:04:55.525348 ipv64-0.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-01-07 14:04:55.538310 ipv64-0.4.2/src/ipv64.egg-info/
--rw-rw-rw-   0        0        0     2689 2023-01-07 14:04:55.000000 ipv64-0.4.2/src/ipv64.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-01-07 14:04:55.000000 ipv64-0.4.2/src/ipv64.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-07 14:04:55.000000 ipv64-0.4.2/src/ipv64.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-01-07 14:04:55.000000 ipv64-0.4.2/src/ipv64.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-07 14:04:55.000000 ipv64-0.4.2/src/ipv64.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10967 2023-01-07 14:04:02.000000 ipv64-0.4.2/src/ipv64.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:44:24.966660 ipv64-0.5.0/
+-rw-rw-rw-   0        0        0     1084 2023-05-14 15:54:56.000000 ipv64-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1861 2023-05-15 17:44:24.966660 ipv64-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1525 2023-05-15 17:38:02.000000 ipv64-0.5.0/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-15 17:44:24.967691 ipv64-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-05-15 17:44:21.000000 ipv64-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:44:24.960067 ipv64-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 17:44:24.965660 ipv64-0.5.0/src/ipv64.egg-info/
+-rw-rw-rw-   0        0        0     1861 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6185 2023-05-15 17:40:44.000000 ipv64-0.5.0/src/ipv64.py
```

### Comparing `ipv64-0.4.2/LICENSE` & `ipv64-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipv64-0.4.2/setup.py` & `ipv64-0.5.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'ipv64',
-  version = '0.4.2',
-  description = 'Updater for ipv64.net',
+  version = '0.5.0',
+  description = 'Updater for ipv64.net - ATTENTION THIS VERSION IS NOT COMPATIBLE WITH THE 0.4.2!',
   author = 'R60',
   author_email = 'pypi.nmvk0@getrekt.win',
   url = 'https://github.com/syncip/ipv64',
   py_modules=["ipv64"],
   package_dir={'': 'src'},
   keywords = ['ipv64', 'dyndns', 'updater'],
   long_description=long_description,
   long_description_content_type='text/markdown',
-  install_requires=['dnspython==2.2.1',
-                    'requests==2.28.1',
+  install_requires=['requests==2.28.1',
                     'argparse==1.4.0',
                     ],
 )
```

