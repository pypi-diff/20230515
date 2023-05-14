# Comparing `tmp/python-llm-0.1.3.tar.gz` & `tmp/python-llm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-llm-0.1.3.tar", last modified: Sun May 14 23:03:34 2023, max compression
+gzip compressed data, was "python-llm-0.1.4.tar", last modified: Sun May 14 23:04:38 2023, max compression
```

## Comparing `python-llm-0.1.3.tar` & `python-llm-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:03:34.366044 python-llm-0.1.3/
--rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.3/LICENSE
--rw-r--r--   0 danielgross   (501) staff       (20)     1682 2023-05-14 23:03:34.365932 python-llm-0.1.3/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)     1458 2023-05-14 22:59:17.000000 python-llm-0.1.3/README.md
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:03:34.364674 python-llm-0.1.3/llm/
--rw-r--r--   0 danielgross   (501) staff       (20)       69 2023-05-13 13:51:59.000000 python-llm-0.1.3/llm/__init__.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:03:34.364984 python-llm-0.1.3/llm/api/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.3/llm/api/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2376 2023-05-14 14:49:00.000000 python-llm-0.1.3/llm/api/claude.py
--rw-r--r--   0 danielgross   (501) staff       (20)      980 2023-03-30 14:01:26.000000 python-llm-0.1.3/llm/api/openaiapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2384 2023-05-14 14:49:01.000000 python-llm-0.1.3/llm/main.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1781 2023-05-13 13:24:32.000000 python-llm-0.1.3/llm/util.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:03:34.365521 python-llm-0.1.3/python_llm.egg-info/
--rw-r--r--   0 danielgross   (501) staff       (20)     1682 2023-05-14 23:03:34.000000 python-llm-0.1.3/python_llm.egg-info/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)      336 2023-05-14 23:03:34.000000 python-llm-0.1.3/python_llm.egg-info/SOURCES.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-14 23:03:34.000000 python-llm-0.1.3/python_llm.egg-info/dependency_links.txt
--rw-r--r--   0 danielgross   (501) staff       (20)      146 2023-05-14 23:03:34.000000 python-llm-0.1.3/python_llm.egg-info/requires.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-14 23:03:34.000000 python-llm-0.1.3/python_llm.egg-info/top_level.txt
--rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-14 23:03:34.366077 python-llm-0.1.3/setup.cfg
--rw-r--r--   0 danielgross   (501) staff       (20)      597 2023-05-14 23:03:14.000000 python-llm-0.1.3/setup.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:03:34.365787 python-llm-0.1.3/tests/
--rw-r--r--   0 danielgross   (501) staff       (20)     2749 2023-05-14 22:54:04.000000 python-llm-0.1.3/tests/test_claude.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2097 2023-05-14 22:53:48.000000 python-llm-0.1.3/tests/test_openai.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.403267 python-llm-0.1.4/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.4/LICENSE
+-rw-r--r--   0 danielgross   (501) staff       (20)     1735 2023-05-14 23:04:38.403165 python-llm-0.1.4/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)     1458 2023-05-14 22:59:17.000000 python-llm-0.1.4/README.md
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.401872 python-llm-0.1.4/llm/
+-rw-r--r--   0 danielgross   (501) staff       (20)       69 2023-05-13 13:51:59.000000 python-llm-0.1.4/llm/__init__.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.402170 python-llm-0.1.4/llm/api/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.4/llm/api/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2376 2023-05-14 14:49:00.000000 python-llm-0.1.4/llm/api/claude.py
+-rw-r--r--   0 danielgross   (501) staff       (20)      980 2023-03-30 14:01:26.000000 python-llm-0.1.4/llm/api/openaiapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2384 2023-05-14 14:49:01.000000 python-llm-0.1.4/llm/main.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     1781 2023-05-13 13:24:32.000000 python-llm-0.1.4/llm/util.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.402762 python-llm-0.1.4/python_llm.egg-info/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1735 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)      336 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      146 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/requires.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/top_level.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-14 23:04:38.403297 python-llm-0.1.4/setup.cfg
+-rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-14 23:04:32.000000 python-llm-0.1.4/setup.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.403006 python-llm-0.1.4/tests/
+-rw-r--r--   0 danielgross   (501) staff       (20)     2749 2023-05-14 22:54:04.000000 python-llm-0.1.4/tests/test_claude.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2097 2023-05-14 22:53:48.000000 python-llm-0.1.4/tests/test_openai.py
```

### Comparing `python-llm-0.1.3/LICENSE` & `python-llm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.3/PKG-INFO` & `python-llm-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: python-llm
-Version: 0.1.3
+Version: 0.1.4
 Summary: An LLM wrapper for Humans
+Home-page: https://github.com/danielgross/python-llm
 Author: Daniel Gross
 Author-email: d@dcgross.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-llm: A LLM API for Humans
```

### Comparing `python-llm-0.1.3/README.md` & `python-llm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.3/llm/api/claude.py` & `python-llm-0.1.4/llm/api/claude.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.3/llm/api/openaiapi.py` & `python-llm-0.1.4/llm/api/openaiapi.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.3/llm/main.py` & `python-llm-0.1.4/llm/main.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.3/llm/util.py` & `python-llm-0.1.4/llm/util.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.3/python_llm.egg-info/PKG-INFO` & `python-llm-0.1.4/python_llm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: python-llm
-Version: 0.1.3
+Version: 0.1.4
 Summary: An LLM wrapper for Humans
+Home-page: https://github.com/danielgross/python-llm
 Author: Daniel Gross
 Author-email: d@dcgross.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-llm: A LLM API for Humans
```

### Comparing `python-llm-0.1.3/setup.py` & `python-llm-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     requirements = f.read().splitlines()
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='python-llm',
-    version='0.1.3',
+    version='0.1.4',
     author='Daniel Gross',
     author_email='d@dcgross.com',
     description='An LLM wrapper for Humans',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(include=['llm', 'llm.*']),
+    url="https://github.com/danielgross/python-llm",
     classifiers=[
     ],
     python_requires='>=3.6',
     install_requires=requirements,
 )
```

### Comparing `python-llm-0.1.3/tests/test_claude.py` & `python-llm-0.1.4/tests/test_claude.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.3/tests/test_openai.py` & `python-llm-0.1.4/tests/test_openai.py`

 * *Files identical despite different names*

