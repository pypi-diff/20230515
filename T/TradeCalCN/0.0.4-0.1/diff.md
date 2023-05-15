# Comparing `tmp/TradeCalCN-0.0.4.tar.gz` & `tmp/TradeCalCN-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TradeCalCN-0.0.4.tar", last modified: Mon May 15 12:44:02 2023, max compression
+gzip compressed data, was "TradeCalCN-0.1.tar", last modified: Mon May 15 11:53:19 2023, max compression
```

## Comparing `TradeCalCN-0.0.4.tar` & `TradeCalCN-0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zhouweilun   (501) staff       (20)        0 2023-05-15 12:44:02.755306 TradeCalCN-0.0.4/
--rw-r--r--   0 zhouweilun   (501) staff       (20)       54 2023-05-15 12:44:02.755096 TradeCalCN-0.0.4/PKG-INFO
--rw-rw-r--   0 zhouweilun   (501) staff       (20)       51 2023-05-15 12:40:18.000000 TradeCalCN-0.0.4/README.md
-drwxr-xr-x   0 zhouweilun   (501) staff       (20)        0 2023-05-15 12:44:02.754176 TradeCalCN-0.0.4/TradeCalCN/
--rw-rw-r--   0 zhouweilun   (501) staff       (20)       29 2023-05-15 12:40:18.000000 TradeCalCN-0.0.4/TradeCalCN/__init__.py
--rw-rw-r--   0 zhouweilun   (501) staff       (20)     7937 2023-05-15 12:40:18.000000 TradeCalCN-0.0.4/TradeCalCN/calendar_test.py
-drwxr-xr-x   0 zhouweilun   (501) staff       (20)        0 2023-05-15 12:44:02.754937 TradeCalCN-0.0.4/TradeCalCN.egg-info/
--rw-r--r--   0 zhouweilun   (501) staff       (20)       54 2023-05-15 12:44:02.000000 TradeCalCN-0.0.4/TradeCalCN.egg-info/PKG-INFO
--rw-r--r--   0 zhouweilun   (501) staff       (20)      244 2023-05-15 12:44:02.000000 TradeCalCN-0.0.4/TradeCalCN.egg-info/SOURCES.txt
--rw-r--r--   0 zhouweilun   (501) staff       (20)        1 2023-05-15 12:44:02.000000 TradeCalCN-0.0.4/TradeCalCN.egg-info/dependency_links.txt
--rw-r--r--   0 zhouweilun   (501) staff       (20)       16 2023-05-15 12:44:02.000000 TradeCalCN-0.0.4/TradeCalCN.egg-info/requires.txt
--rw-r--r--   0 zhouweilun   (501) staff       (20)       11 2023-05-15 12:44:02.000000 TradeCalCN-0.0.4/TradeCalCN.egg-info/top_level.txt
--rw-rw-r--   0 zhouweilun   (501) staff       (20)       89 2023-05-15 12:40:18.000000 TradeCalCN-0.0.4/pyproject.toml
--rw-r--r--   0 zhouweilun   (501) staff       (20)       38 2023-05-15 12:44:02.755425 TradeCalCN-0.0.4/setup.cfg
+drwxr-xr-x   0 zhouweilun   (501) staff       (20)        0 2023-05-15 11:53:19.963751 TradeCalCN-0.1/
+-rw-r--r--   0 zhouweilun   (501) staff       (20)      394 2023-05-15 11:53:19.963827 TradeCalCN-0.1/PKG-INFO
+-rw-r--r--   0 zhouweilun   (501) staff       (20)       51 2023-05-15 10:22:12.000000 TradeCalCN-0.1/README.md
+drwxr-xr-x   0 zhouweilun   (501) staff       (20)        0 2023-05-15 11:53:19.962604 TradeCalCN-0.1/TradeCalCN/
+-rw-r--r--   0 zhouweilun   (501) staff       (20)       26 2023-05-15 10:22:12.000000 TradeCalCN-0.1/TradeCalCN/__init__.py
+-rw-r--r--   0 zhouweilun   (501) staff       (20)     7937 2023-05-15 10:22:12.000000 TradeCalCN-0.1/TradeCalCN/calendar_test.py
+drwxr-xr-x   0 zhouweilun   (501) staff       (20)        0 2023-05-15 11:53:19.963626 TradeCalCN-0.1/TradeCalCN.egg-info/
+-rw-r--r--   0 zhouweilun   (501) staff       (20)      394 2023-05-15 11:53:19.000000 TradeCalCN-0.1/TradeCalCN.egg-info/PKG-INFO
+-rw-r--r--   0 zhouweilun   (501) staff       (20)      248 2023-05-15 11:53:19.000000 TradeCalCN-0.1/TradeCalCN.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouweilun   (501) staff       (20)        1 2023-05-15 11:53:19.000000 TradeCalCN-0.1/TradeCalCN.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouweilun   (501) staff       (20)       16 2023-05-15 11:53:19.000000 TradeCalCN-0.1/TradeCalCN.egg-info/requires.txt
+-rw-r--r--   0 zhouweilun   (501) staff       (20)       11 2023-05-15 11:53:19.000000 TradeCalCN-0.1/TradeCalCN.egg-info/top_level.txt
+-rw-r--r--   0 zhouweilun   (501) staff       (20)       79 2023-05-15 11:53:19.964114 TradeCalCN-0.1/setup.cfg
+-rw-r--r--   0 zhouweilun   (501) staff       (20)      585 2023-05-15 10:22:12.000000 TradeCalCN-0.1/setup.py
```

### Comparing `TradeCalCN-0.0.4/TradeCalCN/calendar_test.py` & `TradeCalCN-0.1/TradeCalCN/calendar_test.py`

 * *Files identical despite different names*

