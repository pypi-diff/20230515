# Comparing `tmp/pyecl-0.0.1.tar.gz` & `tmp/pyecl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecl-0.0.1.tar", last modified: Tue Feb 14 01:31:01 2023, max compression
+gzip compressed data, was "pyecl-0.1.0.tar", last modified: Mon May 15 14:25:31 2023, max compression
```

## Comparing `pyecl-0.0.1.tar` & `pyecl-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-02-14 01:31:01.608244 pyecl-0.0.1/
--rw-r--r--   0 bruno      (501) staff       (20)      130 2023-02-14 01:31:01.608305 pyecl-0.0.1/PKG-INFO
--rw-r--r--   0 bruno      (501) staff       (20)     6901 2023-02-03 20:54:18.000000 pyecl-0.0.1/README.md
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-02-14 01:31:01.607504 pyecl-0.0.1/pyecl/
--rw-r--r--   0 bruno      (501) staff       (20)        0 2023-02-14 01:17:07.000000 pyecl-0.0.1/pyecl/__init__.py
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-02-14 01:31:01.608121 pyecl-0.0.1/pyecl.egg-info/
--rw-r--r--   0 bruno      (501) staff       (20)      130 2023-02-14 01:31:01.000000 pyecl-0.0.1/pyecl.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (501) staff       (20)      190 2023-02-14 01:31:01.000000 pyecl-0.0.1/pyecl.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (501) staff       (20)        1 2023-02-14 01:31:01.000000 pyecl-0.0.1/pyecl.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (501) staff       (20)        1 2023-02-14 01:31:01.000000 pyecl-0.0.1/pyecl.egg-info/not-zip-safe
--rw-r--r--   0 bruno      (501) staff       (20)        6 2023-02-14 01:31:01.000000 pyecl-0.0.1/pyecl.egg-info/top_level.txt
--rw-r--r--   0 bruno      (501) staff       (20)      144 2023-02-14 01:31:01.608546 pyecl-0.0.1/setup.cfg
--rw-r--r--   0 bruno      (501) staff       (20)       37 2023-02-03 23:23:53.000000 pyecl-0.0.1/setup.py
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-05-15 14:25:31.880397 pyecl-0.1.0/
+-rw-r--r--   0 bruno      (501) staff       (20)     1508 2023-05-15 14:19:23.000000 pyecl-0.1.0/LICENSE
+-rw-r--r--   0 bruno      (501) staff       (20)      152 2023-05-15 14:25:31.880460 pyecl-0.1.0/PKG-INFO
+-rw-r--r--   0 bruno      (501) staff       (20)     6901 2023-02-03 20:54:18.000000 pyecl-0.1.0/README.md
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-05-15 14:25:31.878630 pyecl-0.1.0/pyecl/
+-rw-r--r--   0 bruno      (501) staff       (20)       70 2023-05-15 05:07:25.000000 pyecl-0.1.0/pyecl/__init__.py
+-rw-r--r--   0 bruno      (501) staff       (20)    18162 2023-05-15 05:07:25.000000 pyecl-0.1.0/pyecl/constellation.py
+-rw-r--r--   0 bruno      (501) staff       (20)     3383 2023-05-15 05:07:25.000000 pyecl-0.1.0/pyecl/exceptions.py
+-rw-r--r--   0 bruno      (501) staff       (20)    33976 2023-05-15 05:07:25.000000 pyecl-0.1.0/pyecl/models.py
+-rw-r--r--   0 bruno      (501) staff       (20)      743 2023-05-15 05:07:25.000000 pyecl-0.1.0/pyecl/utils.py
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-05-15 14:25:31.879609 pyecl-0.1.0/pyecl.egg-info/
+-rw-r--r--   0 bruno      (501) staff       (20)      152 2023-05-15 14:25:31.000000 pyecl-0.1.0/pyecl.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (501) staff       (20)      417 2023-05-15 14:25:31.000000 pyecl-0.1.0/pyecl.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (501) staff       (20)        1 2023-05-15 14:25:31.000000 pyecl-0.1.0/pyecl.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (501) staff       (20)        1 2023-02-14 01:31:01.000000 pyecl-0.1.0/pyecl.egg-info/not-zip-safe
+-rw-r--r--   0 bruno      (501) staff       (20)       48 2023-05-15 14:25:31.000000 pyecl-0.1.0/pyecl.egg-info/requires.txt
+-rw-r--r--   0 bruno      (501) staff       (20)       12 2023-05-15 14:25:31.000000 pyecl-0.1.0/pyecl.egg-info/top_level.txt
+-rw-r--r--   0 bruno      (501) staff       (20)      195 2023-05-15 14:25:31.880715 pyecl-0.1.0/setup.cfg
+-rw-r--r--   0 bruno      (501) staff       (20)       37 2023-02-03 23:23:53.000000 pyecl-0.1.0/setup.py
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-05-15 14:25:31.880245 pyecl-0.1.0/tests/
+-rw-r--r--   0 bruno      (501) staff       (20)        0 2023-05-15 05:07:25.000000 pyecl-0.1.0/tests/__init__.py
+-rw-r--r--   0 bruno      (501) staff       (20)     8488 2023-05-15 05:07:25.000000 pyecl-0.1.0/tests/test_binary_object_representation.py
+-rw-r--r--   0 bruno      (501) staff       (20)     7050 2023-05-15 05:07:25.000000 pyecl-0.1.0/tests/test_constellation.py
+-rw-r--r--   0 bruno      (501) staff       (20)     2196 2023-05-15 05:07:25.000000 pyecl-0.1.0/tests/test_variable_unit.py
```

### Comparing `pyecl-0.0.1/README.md` & `pyecl-0.1.0/README.md`

 * *Files identical despite different names*

