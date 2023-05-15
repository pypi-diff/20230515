# Comparing `tmp/qrftp-1.1.tar.gz` & `tmp/qrftp-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrftp-1.1.tar", last modified: Mon May 15 01:51:37 2023, max compression
+gzip compressed data, was "qrftp-1.2.tar", last modified: Mon May 15 02:24:54 2023, max compression
```

## Comparing `qrftp-1.1.tar` & `qrftp-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 01:51:37.049177 qrftp-1.1/
--rw-rw-rw-   0        0        0      201 2023-05-15 01:51:37.049177 qrftp-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-15 01:51:37.033156 qrftp-1.1/qrftp/
--rw-rw-rw-   0        0        0     2420 2023-05-15 01:13:06.000000 qrftp-1.1/qrftp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:51:37.048150 qrftp-1.1/qrftp.egg-info/
--rw-rw-rw-   0        0        0      201 2023-05-15 01:51:36.000000 qrftp-1.1/qrftp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-05-15 01:51:36.000000 qrftp-1.1/qrftp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 01:51:36.000000 qrftp-1.1/qrftp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-15 01:51:36.000000 qrftp-1.1/qrftp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 01:51:36.000000 qrftp-1.1/qrftp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 01:51:36.000000 qrftp-1.1/qrftp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 01:51:37.050157 qrftp-1.1/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-05-15 01:51:27.000000 qrftp-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:24:54.575331 qrftp-1.2/
+-rw-rw-rw-   0        0        0      201 2023-05-15 02:24:54.574331 qrftp-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-15 02:24:54.560330 qrftp-1.2/qrftp/
+-rw-rw-rw-   0        0        0     2437 2023-05-15 02:17:22.000000 qrftp-1.2/qrftp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:24:54.573330 qrftp-1.2/qrftp.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-05-15 02:24:54.000000 qrftp-1.2/qrftp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-15 02:24:54.000000 qrftp-1.2/qrftp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 02:24:54.000000 qrftp-1.2/qrftp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-15 02:24:54.000000 qrftp-1.2/qrftp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 02:24:54.000000 qrftp-1.2/qrftp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 02:24:54.000000 qrftp-1.2/qrftp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 02:24:54.575331 qrftp-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-05-15 02:24:26.000000 qrftp-1.2/setup.py
```

### Comparing `qrftp-1.1/qrftp/__init__.py` & `qrftp-1.2/qrftp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/bash
 import functools
 import http.server
 import qrcode
 import socket
 import socketserver
 import sys
 from pathlib import Path
```

