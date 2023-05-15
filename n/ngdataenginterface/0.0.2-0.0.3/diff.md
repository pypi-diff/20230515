# Comparing `tmp/ngdataenginterface-0.0.2.tar.gz` & `tmp/ngdataenginterface-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.0.2.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.0.3.tar", max compression
```

## Comparing `ngdataenginterface-0.0.2.tar` & `ngdataenginterface-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-15 12:31:49.902879 ngdataenginterface-0.0.2/README.md
--rw-r--r--   0        0        0      142 2023-05-15 12:29:25.669304 ngdataenginterface-0.0.2/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0       81 2023-05-13 23:05:56.692992 ngdataenginterface-0.0.2/ngdataenginterface/analytical/__init__.py
--rw-r--r--   0        0        0     2429 2023-05-14 13:19:30.069437 ngdataenginterface-0.0.2/ngdataenginterface/analytical/core.py
--rw-r--r--   0        0        0      320 2023-05-13 23:05:46.744602 ngdataenginterface-0.0.2/ngdataenginterface/core/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-12 21:04:05.629165 ngdataenginterface-0.0.2/ngdataenginterface/core/aws_interface.py
--rw-r--r--   0        0        0     1555 2023-05-12 21:02:23.087434 ngdataenginterface-0.0.2/ngdataenginterface/core/partition.py
--rw-r--r--   0        0        0     5623 2023-05-14 13:26:34.351445 ngdataenginterface-0.0.2/ngdataenginterface/core/read.py
--rw-r--r--   0        0        0     2779 2023-05-12 21:06:35.367623 ngdataenginterface-0.0.2/ngdataenginterface/core/schema.py
--rw-r--r--   0        0        0     2187 2023-05-13 23:06:35.839602 ngdataenginterface-0.0.2/ngdataenginterface/core/utils_emr.py
--rw-r--r--   0        0        0     1424 2023-05-12 21:02:23.094795 ngdataenginterface-0.0.2/ngdataenginterface/core/validations.py
--rw-r--r--   0        0        0     4362 2023-05-12 21:06:41.435742 ngdataenginterface-0.0.2/ngdataenginterface/core/write.py
--rw-r--r--   0        0        0      174 2023-05-13 23:05:37.644998 ngdataenginterface-0.0.2/ngdataenginterface/process/__init__.py
--rw-r--r--   0        0        0     4027 2023-05-13 22:58:04.137492 ngdataenginterface-0.0.2/ngdataenginterface/process/cleansing.py
--rw-r--r--   0        0        0      408 2023-05-13 22:54:38.433696 ngdataenginterface-0.0.2/ngdataenginterface/process/export_redshift.py
--rw-r--r--   0        0        0     6859 2023-05-13 23:07:08.550764 ngdataenginterface-0.0.2/ngdataenginterface/process/pismo.py
--rw-r--r--   0        0        0      400 2023-05-15 12:37:50.999635 ngdataenginterface-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/README.md
+-rw-r--r--   0        0        0      142 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/ngdataenginterface/analytical/__init__.py
+-rw-r--r--   0        0        0     2429 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/ngdataenginterface/analytical/core.py
+-rw-r--r--   0        0        0      320 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/ngdataenginterface/core/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/aws_interface.py
+-rw-r--r--   0        0        0     1555 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/partition.py
+-rw-r--r--   0        0        0     5623 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/read.py
+-rw-r--r--   0        0        0     2779 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/schema.py
+-rw-r--r--   0        0        0     2187 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/utils_emr.py
+-rw-r--r--   0        0        0     1424 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/validations.py
+-rw-r--r--   0        0        0     4362 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/write.py
+-rw-r--r--   0        0        0      174 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/process/__init__.py
+-rw-r--r--   0        0        0     4027 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/process/cleansing.py
+-rw-r--r--   0        0        0      408 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/process/export_redshift.py
+-rw-r--r--   0        0        0     6859 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/process/pismo.py
+-rw-r--r--   0        0        0      422 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.3/PKG-INFO
```

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/analytical/core.py` & `ngdataenginterface-0.0.3/ngdataenginterface/analytical/core.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/core/aws_interface.py` & `ngdataenginterface-0.0.3/ngdataenginterface/core/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/core/partition.py` & `ngdataenginterface-0.0.3/ngdataenginterface/core/partition.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/core/read.py` & `ngdataenginterface-0.0.3/ngdataenginterface/core/read.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/core/schema.py` & `ngdataenginterface-0.0.3/ngdataenginterface/core/schema.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/core/utils_emr.py` & `ngdataenginterface-0.0.3/ngdataenginterface/core/utils_emr.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/core/validations.py` & `ngdataenginterface-0.0.3/ngdataenginterface/core/validations.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/core/write.py` & `ngdataenginterface-0.0.3/ngdataenginterface/core/write.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/process/cleansing.py` & `ngdataenginterface-0.0.3/ngdataenginterface/process/cleansing.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.2/ngdataenginterface/process/pismo.py` & `ngdataenginterface-0.0.3/ngdataenginterface/process/pismo.py`

 * *Files identical despite different names*

