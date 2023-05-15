# Comparing `tmp/confik-1.0.5.tar.gz` & `tmp/confik-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confik-1.0.5.tar", last modified: Sat May 13 04:50:40 2023, max compression
+gzip compressed data, was "confik-1.0.6.tar", last modified: Mon May 15 05:59:04 2023, max compression
```

## Comparing `confik-1.0.5.tar` & `confik-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-13 04:50:40.086280 confik-1.0.5/
--rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-13 04:50:40.086156 confik-1.0.5/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      690 2023-05-12 07:45:30.000000 confik-1.0.5/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-13 04:50:40.085117 confik-1.0.5/confik/
--rw-r--r--   0 leondaz    (501) staff       (20)      836 2023-05-13 04:49:24.000000 confik-1.0.5/confik/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.5/confik/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2491 2023-05-13 04:26:49.000000 confik-1.0.5/confik/parsers.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1268 2023-05-13 04:46:31.000000 confik-1.0.5/confik/proxies.py
--rw-r--r--   0 leondaz    (501) staff       (20)      619 2023-05-13 04:49:37.000000 confik-1.0.5/confik/utils.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-13 04:50:40.085573 confik-1.0.5/confik.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-13 04:50:40.000000 confik-1.0.5/confik.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      319 2023-05-13 04:50:40.000000 confik-1.0.5/confik.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-13 04:50:40.000000 confik-1.0.5/confik.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-13 04:50:40.000000 confik-1.0.5/confik.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-13 04:50:40.086325 confik-1.0.5/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-13 04:50:31.000000 confik-1.0.5/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-13 04:50:40.085910 confik-1.0.5/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-12 06:07:05.000000 confik-1.0.5/tests/test_confik_parser.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2285 2023-05-13 04:48:49.000000 confik-1.0.5/tests/test_read_environment_variables.py
--rw-r--r--   0 leondaz    (501) staff       (20)      149 2023-05-13 04:27:37.000000 confik-1.0.5/tests/test_utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 05:59:04.784889 confik-1.0.6/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1069 2023-05-13 06:57:00.000000 confik-1.0.6/LICENSE
+-rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-15 05:59:04.784756 confik-1.0.6/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     1089 2023-05-13 07:02:08.000000 confik-1.0.6/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 05:59:04.783519 confik-1.0.6/confik/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1037 2023-05-13 06:59:23.000000 confik-1.0.6/confik/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.6/confik/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2434 2023-05-15 05:57:52.000000 confik-1.0.6/confik/parsers.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1268 2023-05-13 04:46:31.000000 confik-1.0.6/confik/proxies.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      619 2023-05-13 04:49:37.000000 confik-1.0.6/confik/utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 05:59:04.784056 confik-1.0.6/confik.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-15 05:59:04.000000 confik-1.0.6/confik.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      327 2023-05-15 05:59:04.000000 confik-1.0.6/confik.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-15 05:59:04.000000 confik-1.0.6/confik.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-15 05:59:04.000000 confik-1.0.6/confik.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-15 05:59:04.784927 confik-1.0.6/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-15 05:58:25.000000 confik-1.0.6/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 05:59:04.784500 confik-1.0.6/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-13 05:42:01.000000 confik-1.0.6/tests/test_confik_parser.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2924 2023-05-15 05:57:52.000000 confik-1.0.6/tests/test_read_environment_variables.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      149 2023-05-13 04:27:37.000000 confik-1.0.6/tests/test_utils.py
```

### Comparing `confik-1.0.5/confik/__init__.py` & `confik-1.0.6/confik/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from pathlib import Path
+from typing import Union
+
 from .exceptions import ConfikError
 from .parsers import ConfikParser
 from .utils import boolean, csv
 
 confik = ConfikParser()
 
 
@@ -20,7 +23,12 @@
     :param cast: A function to call on the value after it's found
     :param default_factory: A function to call with the key to return a value if the value was not found
     :param choices: A choices list to ensure that the value is in it
     :param raise_exception: Raise exceptions if the value was not found
     :return: str
     """
     return confik.get(key, default, cast, default_factory, choices, raise_exception)
+
+
+def read_env(path: Union[str, Path]) -> ConfikParser:
+    """Creates a ConfikParser, it's provided for convenience"""
+    return ConfikParser(path)
```

### Comparing `confik-1.0.5/confik/parsers.py` & `confik-1.0.6/confik/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,14 @@
         key,
         cast,
         default,
         default_factory,
         choices,
         raise_exception,
     ):
-        if choices is None:
-            choices = set()
-
         assert isinstance(key, str), "key must be a string"
         assert isinstance(cast, Callable) or cast is None, "cast must be a callable"
         assert (
             isinstance(default_factory, Callable) or default_factory is None
         ), "Must provide a callable for default_factory"
         assert not all(
             [default, default_factory]
```

### Comparing `confik-1.0.5/confik/proxies.py` & `confik-1.0.6/confik/proxies.py`

 * *Files identical despite different names*

### Comparing `confik-1.0.5/confik/utils.py` & `confik-1.0.6/confik/utils.py`

 * *Files identical despite different names*

### Comparing `confik-1.0.5/tests/test_read_environment_variables.py` & `confik-1.0.6/tests/test_read_environment_variables.py`

 * *Files 22% similar despite different names*

```diff
@@ -77,13 +77,36 @@
 def test_read_integer():
     env = confik.get("VARIABLE_WITH_INTEGER", cast=int)
     assert isinstance(env, int)
 
 
 def test_read_not_bool_as_bool():
     with pytest.raises(AssertionError):
-        env = confik.get("PATH", cast=bool)
+        confik.get("PATH", cast=bool)
 
 
 def test_confik_boolean_same_as_python_bool():
     with pytest.raises(AssertionError):
-        env = confik.get("PATH", cast=confik.boolean)
+        confik.get("PATH", cast=confik.boolean)
+
+
+def test_read_value_with_equal_signs():
+    env = confik.get("URL_WITH_QUERY_PARAMS")
+    assert env == "http://localhost:8000/api/orders?branch_id=qwe241="
+
+
+def test_env_in_choices():
+    choices = ["C1", "C2", "C3"]
+    env = confik.get("VARIABLE_WITH_CHOICES", choices=choices)
+
+    assert (
+        env in choices
+    ), "VARIABLE_WITH_CHOICES has a value {v} which is not in provided choices {c}".format(
+        v=env, c=", ".join(choices)
+    )
+
+
+def test_default_in_choices():
+    choices = ["C1", "C2", "C3"]
+
+    with pytest.raises(AssertionError):
+        confik.get("VARIABLE_WITH_CHOICES", choices=choices, default="C_NOT_IN_CHOICES")
```

