# Comparing `tmp/cfdp-1.1.3.tar.gz` & `tmp/cfdp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdp-1.1.3.tar", last modified: Wed Dec 15 16:45:47 2021, max compression
+gzip compressed data, was "cfdp-2.0.0.tar", last modified: Mon May 15 20:53:00 2023, max compression
```

## Comparing `cfdp-1.1.3.tar` & `cfdp-2.0.0.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.410566 cfdp-1.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1066 2021-12-15 16:45:39.000000 cfdp-1.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2590 2021-12-15 16:45:47.410566 cfdp-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2272 2021-12-15 16:45:39.000000 cfdp-1.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-15 16:45:47.410566 cfdp-1.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      568 2021-12-15 16:45:39.000000 cfdp-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.395564 cfdp-1.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.399565 cfdp-1.1.3/src/cfdp/
--rw-rw-rw-   0 root         (0) root         (0)      207 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5784 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    17964 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.401565 cfdp-1.1.3/src/cfdp/filestore/
--rw-rw-rw-   0 root         (0) root         (0)       71 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/filestore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/filestore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5543 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/filestore/native.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.404565 cfdp-1.1.3/src/cfdp/machines/
--rw-rw-rw-   0 root         (0) root         (0)      124 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/machines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10752 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/machines/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5684 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/machines/receiver1.py
--rw-rw-rw-   0 root         (0) root         (0)    21843 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/machines/receiver2.py
--rw-rw-rw-   0 root         (0) root         (0)     6720 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/machines/sender1.py
--rw-rw-rw-   0 root         (0) root         (0)    18653 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/machines/sender2.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/machines/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.405565 cfdp-1.1.3/src/cfdp/meta/
--rw-rw-rw-   0 root         (0) root         (0)       73 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/meta/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/meta/datafield.py
--rw-rw-rw-   0 root         (0) root         (0)     5333 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/meta/filestore.py
--rw-rw-rw-   0 root         (0) root         (0)    21346 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/meta/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.408566 cfdp-1.1.3/src/cfdp/pdu/
--rw-rw-rw-   0 root         (0) root         (0)      177 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3361 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/ack.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/eof.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/filedata.py
--rw-rw-rw-   0 root         (0) root         (0)     3575 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/finished.py
--rw-rw-rw-   0 root         (0) root         (0)     4960 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/header.py
--rw-rw-rw-   0 root         (0) root         (0)     3557 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/keep_alive.py
--rw-rw-rw-   0 root         (0) root         (0)     6822 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     7421 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/nak.py
--rw-rw-rw-   0 root         (0) root         (0)     2815 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/pdu/prompt.py
--rw-rw-rw-   0 root         (0) root         (0)     3295 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.410566 cfdp-1.1.3/src/cfdp/transport/
--rw-rw-rw-   0 root         (0) root         (0)      126 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/transport/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1772 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/transport/udp.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2021-12-15 16:45:39.000000 cfdp-1.1.3/src/cfdp/transport/zmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 16:45:47.400565 cfdp-1.1.3/src/cfdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2590 2021-12-15 16:45:47.000000 cfdp-1.1.3/src/cfdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2021-12-15 16:45:47.000000 cfdp-1.1.3/src/cfdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-15 16:45:47.000000 cfdp-1.1.3/src/cfdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-12-15 16:45:47.000000 cfdp-1.1.3/src/cfdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-12-15 16:45:47.000000 cfdp-1.1.3/src/cfdp.egg-info/top_level.txt
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.016820 cfdp-2.0.0/
+-rw-r--r--   0 artur     (1000) artur     (1000)     1066 2023-05-15 19:26:16.000000 cfdp-2.0.0/LICENSE.txt
+-rw-r--r--   0 artur     (1000) artur     (1000)     2487 2023-05-15 20:53:00.016820 cfdp-2.0.0/PKG-INFO
+-rw-r--r--   0 artur     (1000) artur     (1000)     2276 2023-05-15 19:26:16.000000 cfdp-2.0.0/README.md
+-rw-r--r--   0 artur     (1000) artur     (1000)      261 2023-05-15 20:52:42.000000 cfdp-2.0.0/pyproject.toml
+-rw-r--r--   0 artur     (1000) artur     (1000)       38 2023-05-15 20:53:00.016820 cfdp-2.0.0/setup.cfg
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.010153 cfdp-2.0.0/src/
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.010153 cfdp-2.0.0/src/cfdp/
+-rw-r--r--   0 artur     (1000) artur     (1000)      185 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3533 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/constants.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    19844 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/core.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1438 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/event.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/filestore/
+-rw-r--r--   0 artur     (1000) artur     (1000)       71 2023-03-14 21:54:24.000000 cfdp-2.0.0/src/cfdp/filestore/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1184 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/filestore/base.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     5551 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/filestore/native.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/machines/
+-rw-r--r--   0 artur     (1000) artur     (1000)      124 2023-03-14 21:54:24.000000 cfdp-2.0.0/src/cfdp/machines/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    10633 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/base.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     5695 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/receiver1.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    21150 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/receiver2.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     6383 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/sender1.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    17933 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/sender2.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1278 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/timer.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/meta/
+-rw-r--r--   0 artur     (1000) artur     (1000)       73 2023-03-14 21:54:24.000000 cfdp-2.0.0/src/cfdp/meta/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)      279 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/meta/datafield.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     5339 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/meta/filestore.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    21597 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/meta/message.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/pdu/
+-rw-r--r--   0 artur     (1000) artur     (1000)      177 2023-03-14 21:54:24.000000 cfdp-2.0.0/src/cfdp/pdu/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3329 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/ack.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     4258 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/eof.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3278 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/filedata.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3574 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/finished.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     5151 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/header.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3681 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/keep_alive.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     7088 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/metadata.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     8221 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/nak.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     2750 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/prompt.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3380 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transaction.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/transport/
+-rw-r--r--   0 artur     (1000) artur     (1000)        0 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)      532 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/base.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1241 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/spp.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1995 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/udp.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1488 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/zmq.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.010153 cfdp-2.0.0/src/cfdp.egg-info/
+-rw-r--r--   0 artur     (1000) artur     (1000)     2487 2023-05-15 20:53:00.000000 cfdp-2.0.0/src/cfdp.egg-info/PKG-INFO
+-rw-r--r--   0 artur     (1000) artur     (1000)     1162 2023-05-15 20:53:00.000000 cfdp-2.0.0/src/cfdp.egg-info/SOURCES.txt
+-rw-r--r--   0 artur     (1000) artur     (1000)        1 2023-05-15 20:53:00.000000 cfdp-2.0.0/src/cfdp.egg-info/dependency_links.txt
+-rw-r--r--   0 artur     (1000) artur     (1000)        5 2023-05-15 20:53:00.000000 cfdp-2.0.0/src/cfdp.egg-info/top_level.txt
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.016820 cfdp-2.0.0/tests/
+-rw-r--r--   0 artur     (1000) artur     (1000)    23479 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_series_F1.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    26767 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_series_F2.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    20780 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_series_F3.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    12808 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_series_F4.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1328 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_spp.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1984 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_zmq.py
```

### Comparing `cfdp-1.1.3/LICENSE.txt` & `cfdp-2.0.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 LibreCube
+Copyright (c) 2023 LibreCube
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cfdp-1.1.3/PKG-INFO` & `cfdp-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: cfdp
-Version: 1.1.3
-Summary: CCSDS File Delivery Protocol
-Home-page: https://gitlab.com/librecube/lib/python-cfdp
-Author-email: info@librecube.org
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-Provides-Extra: zmq
-License-File: LICENSE.txt
-
 # Python CFDP
 
 The CCSDS File Delivery Protocol (CFDP) was developed by the
 [Consultative Committee for Space Data Systems (CCSDS)](https://public.ccsds.org).
 The CFDP protocol provides reliable transfer of files from one endpoint to
 another and has been designed to work well over space links that suffer
 from outtakes and long delays. The basic operation of CFDP is to transfer a
@@ -40,25 +27,20 @@
 
 Clone the repository and then install via pip:
 
 ```
 $ pip install cfdp
 ```
 
-If you intend to use ZMQ as transport layer then install as:
-
-```
-$ pip install cfdp[zmq]
-```
+> Depending on the transport layer to use with CFDP, one needs to install additional dependencies.
 
 ## Documentation
 
 Find the detailed documentation [here](docs/README.md).
 
-
 ## Tests
 
 The protocol is tested for cross-support as outlined in CCSDS CFDP Yellow Book.
 See [tests/README.md](tests/README.md) for details.
 
 ## Contribute
 
@@ -73,9 +55,7 @@
 If you are having issues, please let us know. Reach us at
 [Matrix](https://app.element.io/#/room/#librecube.org:matrix.org)
 or via [Email](mailto:info@librecube.org).
 
 ## License
 
 The project is licensed under the MIT license. See the [LICENSE](./LICENSE.txt) file for details.
-
-
```

### Comparing `cfdp-1.1.3/README.md` & `cfdp-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: cfdp
+Version: 2.0.0
+Summary: CCSDS File Delivery Protocol
+Author-email: LibreCube <info@librecube.org>
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Python CFDP
 
 The CCSDS File Delivery Protocol (CFDP) was developed by the
 [Consultative Committee for Space Data Systems (CCSDS)](https://public.ccsds.org).
 The CFDP protocol provides reliable transfer of files from one endpoint to
 another and has been designed to work well over space links that suffer
 from outtakes and long delays. The basic operation of CFDP is to transfer a
@@ -27,25 +36,20 @@
 
 Clone the repository and then install via pip:
 
 ```
 $ pip install cfdp
 ```
 
-If you intend to use ZMQ as transport layer then install as:
-
-```
-$ pip install cfdp[zmq]
-```
+> Depending on the transport layer to use with CFDP, one needs to install additional dependencies.
 
 ## Documentation
 
 Find the detailed documentation [here](docs/README.md).
 
-
 ## Tests
 
 The protocol is tested for cross-support as outlined in CCSDS CFDP Yellow Book.
 See [tests/README.md](tests/README.md) for details.
 
 ## Contribute
```

### Comparing `cfdp-1.1.3/src/cfdp/constants.py` & `cfdp-2.0.0/src/cfdp/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 class ProtocolVersion:
     VERSION_1 = 0
     VERSION_2 = 1
 
 
 class TransmissionMode:
     ACKNOWLEDGED = 0
@@ -124,7 +123,28 @@
 
 class ChecksumType:
     MODULAR = 0
     PROXIMITY1 = 1
     CRC32C = 2
     IEEE = 3
     NULL = 15
+
+
+DEFAULT_MAX_FILE_SEGMENT_LEN = 4096
+DEFAULT_INACTIVITY_TIMEOUT = 30
+DEFAULT_ACK_TIMER_LIMIT = 5
+DEFAULT_ACK_TIMER_EXPIRATION_LIMIT = 3
+DEFAULT_NAK_TIMER_INTERVAL = 5
+DEFAULT_NAK_TIMER_EXPIRATION_LIMIT = 5
+DEFAULT_FAULT_HANDLERS = {
+    ConditionCode.POSITIVE_ACK_LIMIT_REACHED: FaultHandlerAction.CANCEL,
+    ConditionCode.KEEP_ALIVE_LIMIT_REACHED: FaultHandlerAction.CANCEL,
+    ConditionCode.INVALID_TRANSMISSION_MODE: FaultHandlerAction.CANCEL,
+    ConditionCode.FILESTORE_REJECTION: FaultHandlerAction.CANCEL,
+    ConditionCode.FILE_CHECKSUM_FAILURE: FaultHandlerAction.CANCEL,
+    ConditionCode.FILE_SIZE_ERROR: FaultHandlerAction.CANCEL,
+    ConditionCode.NAK_LIMIT_REACHED: FaultHandlerAction.CANCEL,
+    ConditionCode.INACTIVITY_DETECTED: FaultHandlerAction.CANCEL,
+    ConditionCode.INVALID_FILE_STRUCTURE: FaultHandlerAction.CANCEL,
+    ConditionCode.CHECK_LIMIT_REACHED: FaultHandlerAction.CANCEL,
+    ConditionCode.UNSUPPORTED_CHECKSUM_TYPE: FaultHandlerAction.CANCEL,
+}
```

### Comparing `cfdp-1.1.3/src/cfdp/core.py` & `cfdp-2.0.0/src/cfdp/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,103 @@
 import queue
-import time
 import threading
 
 from . import logger
-from .constants import TransmissionMode, PduTypeCode, DirectiveCode,\
-    Direction, MachineState, ConditionCode, DirectiveSubTypeCode,\
-    TransactionStatus
+from .constants import (
+    TransmissionMode,
+    PduTypeCode,
+    DirectiveCode,
+    Direction,
+    MachineState,
+    ConditionCode,
+    DirectiveSubTypeCode,
+    TransactionStatus,
+    ChecksumType,
+    DEFAULT_FAULT_HANDLERS,
+    DEFAULT_INACTIVITY_TIMEOUT,
+    DEFAULT_ACK_TIMER_LIMIT,
+    DEFAULT_ACK_TIMER_EXPIRATION_LIMIT,
+    DEFAULT_NAK_TIMER_INTERVAL,
+    DEFAULT_NAK_TIMER_EXPIRATION_LIMIT,
+)
 from .event import Event, EventType
 from .transaction import Transaction
 from .machines import Sender1, Receiver1, Sender2, Receiver2
-from .pdu import PduHeader, MetadataPdu, FiledataPdu, EofPdu, FinishedPdu,\
-    NakPdu, AckPdu, KeepAlivePdu, PromptPdu
+from .pdu import (
+    PduHeader,
+    MetadataPdu,
+    FiledataPdu,
+    EofPdu,
+    FinishedPdu,
+    NakPdu,
+    AckPdu,
+    KeepAlivePdu,
+    PromptPdu,
+)
 from .meta import process_user_message as meta_process_user_message
 
 
 class CfdpEntity:
 
     """
     The CfdpUser keeps a dict of active state machines in the form:
         self.machines = {(a1, b1): c1, (a2,b2): c2}
     where the key is the transaction id, which is a tuple with
     a = source_entity_id, b = seq_number, and value c = transaction instance.
     """
 
-    def __init__(self, config):
-        self.config = config
+    def __init__(
+        self,
+        entity_id,
+        filestore,
+        transport,
+        eof_sent_indication_required=False,
+        eof_received_indication_required=False,
+        filesegment_received_indication_required=False,
+        transaction_finished_indication_required=False,
+        suspended_indication_required=False,
+        resumed_indication_required=False,
+        default_fault_handlers=DEFAULT_FAULT_HANDLERS,
+        transaction_inactivity_limit=DEFAULT_INACTIVITY_TIMEOUT,
+        positive_ack_timer_interval=DEFAULT_ACK_TIMER_LIMIT,
+        positive_ack_timer_expiration_limit=DEFAULT_ACK_TIMER_EXPIRATION_LIMIT,
+        nak_timer_interval=DEFAULT_NAK_TIMER_INTERVAL,
+        nak_timer_expiration_limit=DEFAULT_NAK_TIMER_EXPIRATION_LIMIT,
+    ):
+        self.entity_id = entity_id
+        self.filestore = filestore
+        self.transport = transport
+        self.eof_sent_indication_required = eof_sent_indication_required
+        self.eof_received_indication_required = eof_received_indication_required
+        self.filesegment_received_indication_required = (
+            filesegment_received_indication_required
+        )
+        self.transaction_finished_indication_required = (
+            transaction_finished_indication_required
+        )
+        self.suspended_indication_required = suspended_indication_required
+        self.resumed_indication_required = resumed_indication_required
+        self.default_fault_handlers = default_fault_handlers
+        self.transaction_inactivity_limit = transaction_inactivity_limit
+        self.positive_ack_timer_interval = positive_ack_timer_interval
+        self.positive_ack_timer_expiration_limit = positive_ack_timer_expiration_limit
+        self.nak_timer_interval = nak_timer_interval
+        self.nak_timer_expiration_limit = nak_timer_expiration_limit
 
-        self.entity_id = config.local_entity.entity_id
-        self.filestore = config.filestore
-        self.transport = config.transport
         self.transport.indication = lambda x: self.pdu_received(x)
 
         self._transaction_seq_counter = 0
         self.machines = {}
-        self.messages_to_user = []
 
         self._event_queue = queue.Queue()
         self._event_thread = threading.Thread(target=self._event_handler)
         self._event_thread.kill = False
         self._event_thread.start()
 
+        self._messages_to_user_queue = queue.Queue()
         self._message_thread = threading.Thread(target=self._message_handler)
         self._message_thread.kill = False
         self._message_thread.start()
 
         self._file_data_queue = queue.Queue()
 
     def _increment_transaction_seq_counter(self):
@@ -57,101 +111,112 @@
         machine = self.machines.get(transaction_id)
         if machine is None:
             return True
         else:
             return machine.state == MachineState.COMPLETED
 
     def _event_handler(self):
-        thread = threading.currentThread()
+        thread = threading.current_thread()
         while not thread.kill:
-            time.sleep(0.01)
             try:
-                event, pdu = self._event_queue.get(block=False)
+                event, pdu = self._event_queue.get(timeout=1000)
+                if thread.kill:
+                    break
                 machine = self.machines.get(event.transaction.id)
                 if machine:
                     machine.update_state(event, pdu)
             except queue.Empty:
                 pass
 
     def _message_handler(self):
-        thread = threading.currentThread()
-        while True and not thread.kill:
-            time.sleep(0.01)
-            if self.messages_to_user:
-                message = self.messages_to_user.pop()
+        thread = threading.current_thread()
+        while not thread.kill:
+            try:
+                message = self._messages_to_user_queue.get(timeout=1000)
+                if thread.kill:
+                    break
                 logger.info("Processing user message %s" % str(message))
                 self.process_user_message(message)
+            except queue.Empty:
+                pass
 
     def shutdown(self):
         self._event_thread.kill = True
         self._message_thread.kill = True
+        self._event_queue.put([0, 0])  # needed to break the loop
+        self._messages_to_user_queue.put(0)  # needed to break the loop
 
     """ CFDP service requests """
 
     def put(
-            self,
-            destination_id,
-            source_filename=None,
-            destination_filename=None,
-            segmentation_control=None,  # not implemented
-            fault_handler_overrides=None,
-            flow_label=None,  # not implemented
-            transmission_mode=None,
-            closure_requested=False,  # not implemented
-            messages_to_user=None,
-            filestore_requests=None):
-
+        self,
+        destination_id,
+        source_filename=None,
+        destination_filename=None,
+        segmentation_control=None,  # not implemented
+        fault_handler_overrides=None,
+        flow_label=None,  # not implemented
+        transmission_mode=None,
+        closure_requested=False,  # not implemented
+        messages_to_user=None,
+        filestore_requests=None,
+        checksum_type=ChecksumType.MODULAR,
+    ):
         seq_number = self._increment_transaction_seq_counter()
 
         transaction = Transaction(
             kernel=self,
             source_entity_id=self.entity_id,
             seq_number=seq_number,
             destination_entity_id=destination_id,
             transmission_mode=transmission_mode,
             source_filename=source_filename,
             destination_filename=destination_filename,
             fault_handler_overrides=fault_handler_overrides,
             messages_to_user=messages_to_user,
             filestore_requests=filestore_requests,
-            checksum_type=self.config.get(destination_id).type_of_checksum)
+            checksum_type=checksum_type,
+        )
 
         if transmission_mode == TransmissionMode.UNACKNOWLEDGED:
             machine = Sender1(self, transaction)
         else:
             machine = Sender2(self, transaction)
         self.machines[transaction.id] = machine
         self.trigger_event(Event(transaction, EventType.E0_ENTERED_STATE))
-        self.trigger_event(Event(
-            transaction, EventType.E30_RECEIVED_PUT_REQUEST))
+        self.trigger_event(Event(transaction, EventType.E30_RECEIVED_PUT_REQUEST))
         return transaction.id
 
     def cancel(self, transaction_id):
         machine = self.machines.get(transaction_id)
         if machine:
-            self.trigger_event(Event(
-                machine.transaction, EventType.E33_RECEIVED_CANCEL_REQUEST))
+            self.trigger_event(
+                Event(machine.transaction, EventType.E33_RECEIVED_CANCEL_REQUEST)
+            )
 
     def suspend(self, transaction_id):
         machine = self.machines.get(transaction_id)
         if machine:
-            self.trigger_event(Event(
-                machine.transaction, EventType.E31_RECEIVED_SUSPEND_REQUEST))
+            self.trigger_event(
+                Event(machine.transaction, EventType.E31_RECEIVED_SUSPEND_REQUEST)
+            )
 
     def resume(self, transaction_id):
         machine = self.machines.get(transaction_id)
         if machine:
-            self.trigger_event(Event(
-                machine.transaction, EventType.E32_RECEIVED_RESUME_REQUEST))
+            self.trigger_event(
+                Event(machine.transaction, EventType.E32_RECEIVED_RESUME_REQUEST)
+            )
 
     def report(self, transaction_id):
         machine = self.machines.get(transaction_id)
         if machine:
-            self.trigger_event(Event(
-                machine.transaction, EventType.E34_RECEIVED_REPORT_REQUEST))
+            self.trigger_event(
+                Event(machine.transaction, EventType.E34_RECEIVED_REPORT_REQUEST)
+            )
 
     """ CFDP service indications """
 
     def transaction_indication(self, transaction_id):
         """
         The Transaction.indication primitive shall be used to indicate the
         Transaction identifier to the source CFDP user.
@@ -162,104 +227,91 @@
         """
         The EOF-Sent.indication primitive shall be used to notify the source
         CFDP user of the initial transmission of a transaction’s EOF PDU.
         """
         logger.info("[%s] EOF sent indication" % str(transaction_id))
 
     def transaction_finished_indication(
-            self,
-            transaction_id,
-            condition_code,
-            file_status,
-            delivery_code,
-            filestore_responses=None,
-            status_report=None):
+        self,
+        transaction_id,
+        condition_code,
+        file_status,
+        delivery_code,
+        filestore_responses=None,
+        status_report=None,
+    ):
         """
         The Transaction-Finished.indication primitive shall be used to indicate
         to the source or destination CFDP user that the transaction is complete
         and that the source CFDP user is authorized to modify or delete any
         retransmission buffer (file) that it was sharing with the protocol
         entity to conserve persistent storage space.
         """
-        logger.info(
-            "[%s] Transaction finished indication" % str(transaction_id))
+        logger.info("[%s] Transaction finished indication" % str(transaction_id))
 
     def metadata_received_indication(
-            self,
-            transaction_id,
-            source_entity_id,
-            file_size=None,
-            source_filename=None,
-            destination_filename=None,
-            messages_to_user=None):
+        self,
+        transaction_id,
+        source_entity_id,
+        file_size=None,
+        source_filename=None,
+        destination_filename=None,
+        messages_to_user=None,
+    ):
         """
         The Metadata-Recv.indication primitive shall be used to indicate to the
         destination CFDP user that the metadata associated with a transaction
         has been received.
         """
         logger.info(
-            "[%s] Metadata received indication (%s bytes)" %
-            (str(transaction_id), str(file_size)))
+            "[%s] Metadata received indication (%s bytes)"
+            % (str(transaction_id), str(file_size))
+        )
 
     def filesegment_received_indication(
-            self,
-            transaction_id,
-            offset,
-            length,
-            record_continuation_state=None,
-            length_of_segment_metadata=None,
-            segment_metadata=None):
+        self,
+        transaction_id,
+        offset,
+        length,
+        record_continuation_state=None,
+        length_of_segment_metadata=None,
+        segment_metadata=None,
+    ):
         """
         The File-Segment-Recv.indication primitive shall be used to indicate
         the receipt of individual file data (non-metadata) segments to the
         destination CFDP user.
         """
         logger.info(
-            "[%s] Filesegment received indication (offset %s, lenght %s)" %
-            (transaction_id, offset, length))
+            "[%s] Filesegment received indication (offset %s, lenght %s)"
+            % (transaction_id, offset, length)
+        )
 
-    def suspended_indication(
-            self,
-            transaction_id,
-            condition_code):
+    def suspended_indication(self, transaction_id, condition_code):
         logger.info("[%s] Suspended indication" % str(transaction_id))
 
-    def resumed_indication(
-            self,
-            transaction_id,
-            progress):
+    def resumed_indication(self, transaction_id, progress):
         logger.info("[%s] Resumed indication" % str(transaction_id))
 
-    def report_indication(
-            self,
-            transaction_id,
-            status_report):
+    def report_indication(self, transaction_id, status_report):
         """
         The Report.indication primitive shall be used to report to the CFDP
         user on the status of a transaction.
         """
         logger.info("[%s] Report indication" % str(transaction_id))
 
-    def fault_indication(
-            self,
-            transaction_id,
-            condition_code,
-            progress):
+    def fault_indication(self, transaction_id, condition_code, progress):
         """
         The Fault.indication primitive shall be used to indicate to the
         CFDP user the occurrence of a fault condition for which the designated
         fault handler was ‘Ignore’.
         """
         logger.info("[%s] Fault indication" % str(transaction_id))
 
-    def abandoned_indication(
-            self,
-            transaction_id,
-            condition_code,
-            progress):
+    def abandoned_indication(self, transaction_id, condition_code, progress):
         """
         The Abandoned.indication primitive shall be used to indicate to the
         CFDP user the occurrence of a fault condition for which the designated
         fault handler was ‘Abandon’.
         """
         logger.info("[%s] Abandoned indication" % str(transaction_id))
 
@@ -274,59 +326,55 @@
     """ Link state procedures """
 
     def freeze(self, receiving_entity_id):
         # freeze transmission for all transactions for which it is the
         # sending entity and the specified remote entity is the receiving one
         for transaction_id, machine in self.machines.items():
             if transaction_id[0] == self.entity_id:
-                if machine.transaction.destination_entity_id ==\
-                        receiving_entity_id:
-                    self.trigger_event(Event(
-                        machine.transaction,
-                        EventType.E40_RECEIVED_FREEZE))
+                if machine.transaction.destination_entity_id == receiving_entity_id:
+                    self.trigger_event(
+                        Event(machine.transaction, EventType.E40_RECEIVED_FREEZE)
+                    )
 
     def thaw(self, receiving_entity_id):
         for transaction_id, machine in self.machines.items():
             if transaction_id[0] == self.entity_id:
-                if machine.transaction.destination_entity_id ==\
-                        receiving_entity_id:
-                    self.trigger_event(Event(
-                        machine.transaction,
-                        EventType.E41_RECEIVED_THAW))
+                if machine.transaction.destination_entity_id == receiving_entity_id:
+                    self.trigger_event(
+                        Event(machine.transaction, EventType.E41_RECEIVED_THAW)
+                    )
 
     def pdu_received(self, data):
-        """ See CCSDS 720.2-G-3, chapter 5.4 """
+        """See CCSDS 720.2-G-3, chapter 5.4"""
 
         pdu = self._get_pdu_object(data)
 
         mode = pdu.pdu_header.transmission_mode
         direction = pdu.pdu_header.direction
         transaction_id = (
             pdu.pdu_header.source_entity_id,
-            pdu.pdu_header.transaction_seq_number)
+            pdu.pdu_header.transaction_seq_number,
+        )
 
         if transaction_id in self.machines:
             machine = self.machines[transaction_id]
         else:
             machine = None
 
         if machine and machine.transmission_mode == mode:
-
             if machine.state is not MachineState.COMPLETED:
                 # deliver pdu to that state machine
                 self._send_pdu_to_state_machine(machine, pdu)
 
             else:
                 del self.machines[transaction_id]  # remove old state machine
-                self._run_action_for_incoming_pdu(
-                    mode, direction, transaction_id, pdu)
+                self._run_action_for_incoming_pdu(mode, direction, transaction_id, pdu)
 
         else:
-            self._run_action_for_incoming_pdu(
-                mode, direction, transaction_id, pdu)
+            self._run_action_for_incoming_pdu(mode, direction, transaction_id, pdu)
 
     def _get_pdu_object(self, raw_pdu):
         "Take the raw input and return proper PDU object"
 
         pdu_header = PduHeader.decode(raw_pdu)
 
         # determine type of PDU
@@ -359,121 +407,127 @@
 
             else:
                 raise RuntimeError
 
         return pdu
 
     def _send_pdu_to_state_machine(self, machine, pdu):
-
         if isinstance(pdu, MetadataPdu):
-            self.trigger_event(Event(
-                machine.transaction, EventType.E10_RECEIVED_METADATA), pdu)
+            self.trigger_event(
+                Event(machine.transaction, EventType.E10_RECEIVED_METADATA), pdu
+            )
 
         elif isinstance(pdu, FiledataPdu):
-            self.trigger_event(Event(
-                machine.transaction, EventType.E11_RECEIVED_FILEDATA), pdu)
+            self.trigger_event(
+                Event(machine.transaction, EventType.E11_RECEIVED_FILEDATA), pdu
+            )
 
         elif isinstance(pdu, EofPdu):
             if pdu.condition_code == ConditionCode.NO_ERROR:
-                self.trigger_event(Event(
-                    machine.transaction,
-                    EventType.E12_RECEIVED_EOF_NO_ERROR), pdu)
+                self.trigger_event(
+                    Event(machine.transaction, EventType.E12_RECEIVED_EOF_NO_ERROR), pdu
+                )
             else:
-                self.trigger_event(Event(
-                    machine.transaction,
-                    EventType.E13_RECEIVED_EOF_CANCEL), pdu)
+                self.trigger_event(
+                    Event(machine.transaction, EventType.E13_RECEIVED_EOF_CANCEL), pdu
+                )
 
         elif isinstance(pdu, AckPdu):
-
             if pdu.directive_code_ack == DirectiveCode.EOF:
-                self.trigger_event(Event(
-                    machine.transaction,
-                    EventType.E14_RECEIVED_ACK_EOF), pdu)
+                self.trigger_event(
+                    Event(machine.transaction, EventType.E14_RECEIVED_ACK_EOF), pdu
+                )
             elif pdu.directive_code_ack == DirectiveCode.FINISHED:
-                self.trigger_event(Event(
-                    machine.transaction,
-                    EventType.E18_RECEIVED_ACK_FINISHED), pdu)
+                self.trigger_event(
+                    Event(machine.transaction, EventType.E18_RECEIVED_ACK_FINISHED), pdu
+                )
             else:
                 raise NotImplementedError
 
         elif isinstance(pdu, FinishedPdu):
             if pdu.condition_code == ConditionCode.NO_ERROR:
-                self.trigger_event(Event(
-                    machine.transaction,
-                    EventType.E16_RECEIVED_FINISHED_NO_ERROR), pdu)
+                self.trigger_event(
+                    Event(
+                        machine.transaction, EventType.E16_RECEIVED_FINISHED_NO_ERROR
+                    ),
+                    pdu,
+                )
             else:
-                self.trigger_event(Event(
-                    machine.transaction,
-                    EventType.E17_RECEIVED_FINISHED_CANCEL), pdu)
+                self.trigger_event(
+                    Event(machine.transaction, EventType.E17_RECEIVED_FINISHED_CANCEL),
+                    pdu,
+                )
 
         elif isinstance(pdu, NakPdu):
-            self.trigger_event(Event(
-                machine.transaction,
-                EventType.E15_RECEIVED_NAK), pdu)
+            self.trigger_event(
+                Event(machine.transaction, EventType.E15_RECEIVED_NAK), pdu
+            )
 
         else:
             raise RuntimeError
 
-    def _run_action_for_incoming_pdu(
-            self, mode, direction, transaction_id, pdu):
-        """ See CCSDS 720.2-G-3, Chapter 5.4, Table 5-5 """
+    def _run_action_for_incoming_pdu(self, mode, direction, transaction_id, pdu):
+        """See CCSDS 720.2-G-3, Chapter 5.4, Table 5-5"""
 
-        if direction == Direction.TOWARD_SENDER\
-                and mode == TransmissionMode.UNACKNOWLEDGED:
+        if (
+            direction == Direction.TOWARD_SENDER
+            and mode == TransmissionMode.UNACKNOWLEDGED
+        ):
             # ignore
             pass
 
-        elif direction == Direction.TOWARD_SENDER\
-                and mode == TransmissionMode.ACKNOWLEDGED:
-
+        elif (
+            direction == Direction.TOWARD_SENDER
+            and mode == TransmissionMode.ACKNOWLEDGED
+        ):
             if isinstance(pdu, FinishedPdu):
                 logger.debug("[{}] Send Ack Finished".format(transaction_id))
                 ack_pdu = AckPdu(
                     direction=Direction.TOWARD_RECEIVER,
                     transmission_mode=pdu.pdu_header.transmission_mode,
                     source_entity_id=pdu.pdu_header.source_entity_id,
                     transaction_seq_number=pdu.pdu_header.transaction_seq_number,
                     destination_entity_id=pdu.pdu_header.destination_entity_id,
                     #
                     directive_code_ack=DirectiveCode.FINISHED,
                     directive_subtype_code=DirectiveSubTypeCode.ACK_FINISHED,
                     condition_code=ConditionCode.NO_ERROR,
-                    transaction_status=TransactionStatus.UNDEFINED)
-                address = self.config.get(
-                    pdu.pdu_header.destination_entity_id).ut_address
-                self.transport.request(ack_pdu.encode(), address)
+                    transaction_status=TransactionStatus.UNDEFINED,
+                )
+                self.transport.request(ack_pdu.encode())
 
         elif direction == Direction.TOWARD_RECEIVER:
-
             # start a new state machine
-            if isinstance(pdu, MetadataPdu)\
-                    or isinstance(pdu, FiledataPdu)\
-                    or isinstance(pdu, EofPdu):
-
+            if (
+                isinstance(pdu, MetadataPdu)
+                or isinstance(pdu, FiledataPdu)
+                or isinstance(pdu, EofPdu)
+            ):
                 if isinstance(pdu, MetadataPdu):
                     transaction = Transaction(
                         self,
                         pdu.pdu_header.source_entity_id,
                         pdu.pdu_header.transaction_seq_number,
                         pdu.pdu_header.destination_entity_id,
                         pdu.pdu_header.transmission_mode,
                         pdu.source_filename,
-                        pdu.destination_filename)
+                        pdu.destination_filename,
+                    )
                 else:
                     transaction = Transaction(
                         self,
                         pdu.pdu_header.source_entity_id,
                         pdu.pdu_header.transaction_seq_number,
                         pdu.pdu_header.destination_entity_id,
-                        pdu.pdu_header.transmission_mode)
+                        pdu.pdu_header.transmission_mode,
+                    )
 
                 machine = self._new_state_machine(transaction, pdu)
                 self.machines[transaction_id] = machine
-                self.trigger_event(
-                    Event(transaction, EventType.E0_ENTERED_STATE))
+                self.trigger_event(Event(transaction, EventType.E0_ENTERED_STATE))
                 self._send_pdu_to_state_machine(machine, pdu)
 
     def _new_state_machine(self, transaction, pdu):
         if pdu.pdu_header.transmission_mode == TransmissionMode.UNACKNOWLEDGED:
             machine = Receiver1(self, transaction)
         else:
             machine = Receiver2(self, transaction)
```

### Comparing `cfdp-1.1.3/src/cfdp/event.py` & `cfdp-2.0.0/src/cfdp/event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-
-
 class Event:
-
     def __init__(self, transaction, type):
         self.transaction = transaction
         self.type = type
 
 
 class EventType:
     E0_ENTERED_STATE = "ENTERED_STATE"
```

### Comparing `cfdp-1.1.3/src/cfdp/filestore/base.py` & `cfdp-2.0.0/src/cfdp/filestore/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 class VirtualFileStore:
 
     """
     The Virtual File Store (VFS) is an abstraction of file system. An
     implementation must provide the methods listed below.
 
     An implementation can map the VFS to a platform dependent native file
```

### Comparing `cfdp-1.1.3/src/cfdp/filestore/native.py` & `cfdp-2.0.0/src/cfdp/filestore/native.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,50 +20,48 @@
 
     def __init__(self, rootpath):
         super().__init__()
         self.rootpath = os.path.abspath(rootpath)
 
     def get_native_path(self, path):
         # convert from virtual filestore path to absolute native path
-        path_items = path.split('/')
-        path_items = [x for x in path_items if x != '']
+        path_items = path.split("/")
+        path_items = [x for x in path_items if x != ""]
         if path_items:
             path = os.path.join(*path_items)
         else:
-            path = ''
+            path = ""
         return os.path.join(self.rootpath, path)
 
     def get_virtual_path(self, path):
         # convert from native relative path to virtual path
-        path = '/'.join(os.path.normpath(path).split(os.path.sep))
-        if not path.startswith('/'):
-            path = '/' + path
+        path = "/".join(os.path.normpath(path).split(os.path.sep))
+        if not path.startswith("/"):
+            path = "/" + path
         return path
 
     def create_file(self, filepath):
-        NativeFileHandle(self.get_native_path(filepath), 'wb').close()
+        NativeFileHandle(self.get_native_path(filepath), "wb").close()
 
     def delete_file(self, filepath):
         os.remove(self.get_native_path(filepath))
 
     def rename_file(self, filepath1, filepath2):
-        os.rename(
-            self.get_native_path(filepath1),
-            self.get_native_path(filepath2))
+        os.rename(self.get_native_path(filepath1), self.get_native_path(filepath2))
 
     def append_file(self, filepath1, filepath2):
-        fh1 = open(self.get_native_path(filepath1), 'ab')
-        fh2 = open(self.get_native_path(filepath2), 'rb')
+        fh1 = open(self.get_native_path(filepath1), "ab")
+        fh2 = open(self.get_native_path(filepath2), "rb")
         fh1.write(fh2.read())
         fh1.close()
         fh2.close()
 
     def replace_file(self, filepath1, filepath2):
-        fh1 = open(self.get_native_path(filepath1), 'wb')
-        fh2 = open(self.get_native_path(filepath2), 'rb')
+        fh1 = open(self.get_native_path(filepath1), "wb")
+        fh2 = open(self.get_native_path(filepath2), "rb")
         fh1.write(fh2.read())
         fh1.close()
         fh2.close()
 
     def create_directory(self, dirpath):
         os.mkdir(self.get_native_path(dirpath))
 
@@ -80,52 +78,54 @@
         for dirname in dirnames:
             fullpath = os.path.join(dirpath, dirname)
             relpath = os.path.relpath(fullpath, self.rootpath)
             line = "{},{},{},{}\n".format(
                 "d",
                 self.get_virtual_path(relpath),
                 os.path.getsize(fullpath),
-                os.path.getmtime(fullpath))
+                os.path.getmtime(fullpath),
+            )
             listing += line
         for filename in filenames:
             fullpath = os.path.join(dirpath, filename)
             relpath = os.path.relpath(fullpath, self.rootpath)
             line = "{},{},{},{}\n".format(
                 "f",
                 self.get_virtual_path(relpath),
                 os.path.getsize(fullpath),
-                os.path.getmtime(fullpath))
+                os.path.getmtime(fullpath),
+            )
             listing += line
         return listing
 
-    def open(self, filepath, mode='rb'):
+    def open(self, filepath, mode="rb"):
         return NativeFileHandle(self.get_native_path(filepath), mode)
 
     def open_tempfile(self):
         return NativeTemporaryFileHandle()
 
     def is_file(self, filepath):
         return os.path.isfile(self.get_native_path(filepath))
 
     def get_size(self, filepath):
         return os.path.getsize(self.get_native_path(filepath))
 
     def join_path(self, *args):
-        return '/'.join(args)
+        return "/".join(args)
 
 
 class NativeFileHandle:
 
     """
     The NativeFileHandle provides a generic interface to Python's 'open'
     function. It also implements method for calculating the file checksum.
 
     """
 
-    def __init__(self, filepath, mode='rb'):
+    def __init__(self, filepath, mode="rb"):
         self.handle = open(filepath, mode)
 
     def get_file_size(self):
         pass
 
     def seek(self, *args, **kwargs):
         return self.handle.seek(*args, **kwargs)
@@ -142,32 +142,31 @@
     def close(self, *args, **kwargs):
         return self.handle.close(*args, **kwargs)
 
     def calculate_checksum(self, type):
         if type == 0:  # Modular, see Annex F of CCSC 727.0-B-5
             file_size = self.handle.seek(0, 2)
             checksum = 0
-            a = b''
+            a = b""
             x = 0
             while x < file_size:
                 self.handle.seek(x)
                 if x > file_size - 4:
                     a = self.handle.read(file_size % 4)
-                    int_a = int(a.hex(), 16) * 2**((4 - file_size % 4)*8)
+                    int_a = int(a.hex(), 16) * 2 ** ((4 - file_size % 4) * 8)
                 else:
                     a = self.handle.read(4)
                     int_a = int(a.hex(), 16)
                 checksum = checksum + int_a
                 x = x + 4
-            checksum = checksum % 2**32
+            checksum = checksum % 2 ** 32
             return checksum
         elif type == 15:  # Null checksum
             return 0
         else:
             # TODO: implemented other checksum algorithms
             raise NotImplementedError
 
 
 class NativeTemporaryFileHandle(NativeFileHandle):
-
     def __init__(self):
         self.handle = tempfile.TemporaryFile()
```

### Comparing `cfdp-1.1.3/src/cfdp/machines/base.py` & `cfdp-2.0.0/src/cfdp/machines/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from cfdp import logger
-from cfdp.constants import MachineState, DeliveryCode, ConditionCode,\
-    Direction, FileStatus, FaultHandlerAction
+from cfdp.constants import (
+    MachineState,
+    DeliveryCode,
+    ConditionCode,
+    Direction,
+    FileStatus,
+    FaultHandlerAction,
+)
 from cfdp.event import Event, EventType
 
 
 class Machine:
-
     def __init__(self, kernel, transaction):
         self.kernel = kernel
         self.transaction = transaction
 
     def trigger_event(self, event_type):
         self.kernel.trigger_event(Event(self.transaction, event_type))
 
-    def _initialize(self):
+    def initialize(self):
         # as per CCSDS 720.2-G-3, Page 5-13, g)
         self.condition_code = ConditionCode.NO_ERROR
         self.delivery_code = DeliveryCode.DATA_INCOMPLETE
         self.frozen = False
         self.metadata_received = False
         self.pdu_received = False
         self.suspended = False
@@ -26,270 +31,273 @@
         self.status_report = None
 
         self.received_file_size = 0
         self.file_open = False
         self.received_file_segments = {}
         self.nak_list = []
 
-    def _shutdown(self):
+    def shutdown(self):
         if self.transaction.file_handle:
             self.transaction.file_handle.close()
             self.transaction.file_handle = None
         self.state = MachineState.COMPLETED
 
-    def _issue_transaction_indication(self):
+    def issue_transaction_indication(self):
         self.kernel.transaction_indication(self.transaction.id)
 
-    def _issue_eof_sent_indication(self):
-        if self.kernel.config.get(self.kernel.entity_id).eof_sent_indication:
+    def issue_eof_sent_indication(self):
+        if self.kernel.eof_sent_indication_required:
             self.kernel.eof_sent_indication(self.transaction.id)
 
-    def _issue_transaction_finished_indication(self):
-        if self.kernel.config.get(
-                self.kernel.entity_id).transaction_finished_indication:
+    def issue_transaction_finished_indication(self):
+        if self.kernel.transaction_finished_indication_required:
             self.kernel.transaction_finished_indication(
                 self.transaction.id,
                 self.condition_code,
                 self.file_status,
                 self.delivery_code,
                 self.filestore_responses,
-                self.status_report)
+                self.status_report,
+            )
 
-    def _issue_metadata_received_indication(self, file_size):
+    def issue_metadata_received_indication(self, file_size):
         self.kernel.metadata_received_indication(
             self.transaction.id,
             self.transaction.source_entity_id,
             file_size,
             self.transaction.source_filename,
             self.transaction.destination_filename,
-            self.transaction.messages_to_user)
+            self.transaction.messages_to_user,
+        )
 
-    def _issue_filesegment_received_indication(self, offset, length):
-        if self.kernel.config.get(
-                self.kernel.entity_id).file_segment_recv_indication:
+    def issue_filesegment_received_indication(self, offset, length):
+        if self.kernel.filesegment_received_indication_required:
             self.kernel.filesegment_received_indication(
-                self.transaction.id,
-                offset,
-                length)
+                self.transaction.id, offset, length
+            )
 
-    def _issue_suspended_indication(self):
-        if self.kernel.config.get(self.kernel.entity_id).suspended_indication:
-            self.kernel.suspended_indication(
-                self.transaction.id,
-                self.condition_code)
+    def issue_suspended_indication(self):
+        if self.kernel.suspended_indication_required:
+            self.kernel.suspended_indication(self.transaction.id, self.condition_code)
 
-    def _issue_resumed_indication(self):
-        if self.kernel.config.get(self.kernel.entity_id).resumed_indication:
+    def issue_resumed_indication(self):
+        if self.kernel.resumed_indication_required:
             self.kernel.resumed_indication(
-                self.transaction.id,
-                self.transaction.get_progress())
+                self.transaction.id, self.transaction.get_progress()
+            )
 
-    def _issue_report_indication(self):
-        self.kernel.report_indication(
-            self.transaction.id,
-            self.status_report)
+    def issue_report_indication(self):
+        self.kernel.report_indication(self.transaction.id, self.status_report)
 
-    def _issue_abandoned_indication(self):
+    def issue_abandoned_indication(self):
         self.kernel.abandoned_indication(
-            self.transaction.id,
-            self.condition_code,
-            self.transaction.get_progress())
+            self.transaction.id, self.condition_code, self.transaction.get_progress()
+        )
 
-    def _issue_eof_received_indication(self):
-        if self.kernel.config.get(self.kernel.entity_id).eof_recv_indication:
+    def issue_eof_received_indication(self):
+        if self.kernel.eof_received_indication_required:
             self.kernel.eof_received_indication(self.transaction.id)
 
-    def _fault_inactivity(self):
-        logger.error(
-            "[{}] Fault: Inactivity timeout".format(self.transaction.id))
+    def fault_inactivity(self):
+        logger.error("[{}] Fault: Inactivity timeout".format(self.transaction.id))
         fault_handler = self.transaction.get_fault_handler(
-            ConditionCode.INACTIVITY_DETECTED)
-        self._run_fault_handler(fault_handler)
+            ConditionCode.INACTIVITY_DETECTED
+        )
+        self.run_fault_handler(fault_handler)
 
-    def _fault_filestore(self):
-        logger.error(
-            "[{}] Fault: Filestore".format(self.transaction.id))
+    def fault_filestore(self):
+        logger.error("[{}] Fault: Filestore".format(self.transaction.id))
         fault_handler = self.transaction.get_fault_handler(
-            ConditionCode.FILESTORE_REJECTION)
-        self._run_fault_handler(fault_handler)
+            ConditionCode.FILESTORE_REJECTION
+        )
+        self.run_fault_handler(fault_handler)
 
-    def _fault_ack_limit(self):
-        logger.error(
-            "[{}] Fault: Ack limit".format(self.transaction.id))
+    def fault_ack_limit(self):
+        logger.error("[{}] Fault: Ack limit".format(self.transaction.id))
         fault_handler = self.transaction.get_fault_handler(
-            ConditionCode.POSITIVE_ACK_LIMIT_REACHED)
-        self._run_fault_handler(fault_handler)
+            ConditionCode.POSITIVE_ACK_LIMIT_REACHED
+        )
+        self.run_fault_handler(fault_handler)
 
-    def _fault_file_size(self):
-        logger.error(
-            "[{}] Fault: File size".format(self.transaction.id))
+    def fault_file_size(self):
+        logger.error("[{}] Fault: File size".format(self.transaction.id))
         fault_handler = self.transaction.get_fault_handler(
-            ConditionCode.FILE_SIZE_ERROR)
-        self._run_fault_handler(fault_handler)
+            ConditionCode.FILE_SIZE_ERROR
+        )
+        self.run_fault_handler(fault_handler)
 
-    def _fault_file_checksum(self):
-        logger.error(
-            "[{}] Fault: File checksum".format(self.transaction.id))
+    def fault_file_checksum(self):
+        logger.error("[{}] Fault: File checksum".format(self.transaction.id))
         fault_handler = self.transaction.get_fault_handler(
-            ConditionCode.FILE_CHECKSUM_FAILURE)
-        self._run_fault_handler(fault_handler)
+            ConditionCode.FILE_CHECKSUM_FAILURE
+        )
+        self.run_fault_handler(fault_handler)
 
-    def _fault_nak_limit(self):
-        logger.error(
-            "[{}] Fault: Nak limit".format(self.transaction.id))
+    def fault_nak_limit(self):
+        logger.error("[{}] Fault: Nak limit".format(self.transaction.id))
         fault_handler = self.transaction.get_fault_handler(
-            ConditionCode.NAK_LIMIT_REACHED)
-        self._run_fault_handler(fault_handler)
+            ConditionCode.NAK_LIMIT_REACHED
+        )
+        self.run_fault_handler(fault_handler)
 
-    def _run_fault_handler(self, fault_handler):
+    def run_fault_handler(self, fault_handler):
         if fault_handler == FaultHandlerAction.CANCEL:
             self.trigger_event(EventType.E33_RECEIVED_CANCEL_REQUEST)
         elif fault_handler == FaultHandlerAction.SUSPEND:
             self.trigger_event(EventType.E31_RECEIVED_SUSPEND_REQUEST)
         elif fault_handler == FaultHandlerAction.IGNORE:
             logger.info("Fault is being ignored. Continuing.")
         elif fault_handler == FaultHandlerAction.ABANDON:
             self.trigger_event(EventType.E2_ABANDON_TRANSACTION)
         else:
             raise ValueError
 
-    def _open_source_file(self):
+    def open_sourcefile(self):
         if not self.kernel.filestore.is_file(self.transaction.source_filename):
-            self._fault_filestore()
-        self.transaction.file_handle =\
-            self.kernel.filestore.open(self.transaction.source_filename)
+            self.fault_filestore()
+        self.transaction.file_handle = self.kernel.filestore.open(
+            self.transaction.source_filename
+        )
 
-    def _is_comm_layer_ready(self):
+    def is_comm_layer_ready(self):
         return self.kernel.transport.is_ready()
 
-    def _is_entire_file_sent(self):
+    def is_entire_file_sent(self):
         return self.transaction.is_file_send_complete()
 
-    def _is_ack_limit_reached(self):
+    def is_ack_limit_reached(self):
         return self.ack_timer.is_limit_reached()
 
-    def _is_file_data_queued(self):
+    def is_file_data_queued(self):
         if self.nak_list:
             return True
         else:
             return False
 
-    def _queue_nakked_data(self, pdu):
+    def queue_nakked_data(self, pdu):
         if pdu.segment_requests:
             self.nak_list.extend(pdu.segment_requests)
             self.nak_list = list(sorted(set(self.nak_list)))
 
-    def _restart_inactivity_timer(self):
+    def restart_inactivity_timer(self):
         if not self.suspended:
             self.inactivity_timer.restart()
 
-    def _resume_inactivity_timer(self):
+    def resume_inactivity_timer(self):
         if not self.suspended:
             self.inactivity_timer.restart()
 
-    def _suspend_inactivity_timer(self):
+    def suspend_inactivity_timer(self):
         self.inactivity_timer.cancel()
 
-    def _restart_ack_timer(self):
+    def restart_ack_timer(self):
         self.ack_timer.restart()
 
-    def _cancel_ack_timer(self):
+    def cancel_ack_timer(self):
         self.ack_timer.cancel()
 
-    def _suspend_ack_timer(self):
+    def is_ack_timer_running(self):
+        return not self.ack_timer.suspended
+
+    def is_ack_timer_suspended(self):
+        return self.ack_timer.suspended
+
+    def suspend_ack_timer(self):
         self.ack_timer.suspended = True
-        self.ack_timer.stop()
+        self.ack_timer.cancel()
 
-    def _resume_ack_timer(self):
+    def resume_ack_timer(self):
         self.ack_timer.suspended = False
-        self._restart_ack_timer()
+        self.ack_timer.restart()
 
-    def _open_temp_file(self):
+    def open_tempfile(self):
         self.transaction.file_handle = self.kernel.filestore.open_tempfile()
 
-    def _close_temp_file(self):
+    def close_tempfile(self):
         self.transaction.file_handle.close()
 
-    def _copy_temp_file_to_dest_file(self):
-        fh = self.kernel.filestore.open(
-            self.transaction.destination_filename, 'wb')
+    def copy_tempfile_to_destfile(self):
+        fh = self.kernel.filestore.open(self.transaction.destination_filename, "wb")
         self.transaction.file_handle.seek(0)
         fh.write(self.transaction.file_handle.read())
         fh.close()
 
-    def _is_file_transfer(self):
-        if self.transaction.source_filename is None\
-                or len(self.transaction.source_filename) == 0:
+    def is_file_transfer(self):
+        if (
+            self.transaction.source_filename is None
+            or len(self.transaction.source_filename) == 0
+        ):
             return False
         return True
 
-    def _is_file_size_error(self, file_size):
+    def is_file_size_error(self, file_size):
         if self.received_file_size > file_size:
             return True
         else:
             return False
 
-    def _is_file_checksum_failure(self, checksum):
+    def is_file_checksum_failure(self, checksum):
         # calculate checksum from file handle directly,
         # as it may be a temporary file
         calculated_checksum = self.transaction.file_handle.calculate_checksum(
-            self.transaction.checksum_type)
+            self.transaction.checksum_type
+        )
         if calculated_checksum != checksum:
             return True
         else:
             return False
 
-    def _store_file_data(self, pdu):
+    def store_file_data(self, pdu):
         self.transaction.file_handle.seek(pdu.segment_offset)
         self.transaction.file_handle.write(pdu.file_data)
         self.received_file_segments[pdu.segment_offset] = len(pdu.file_data)
 
-    def _update_received_file_size(self, pdu):
+    def update_received_file_size(self, pdu):
         if self.received_file_size < pdu.segment_offset + len(pdu.file_data):
             self.received_file_size = pdu.segment_offset + len(pdu.file_data)
 
-    def _process_metadata_options(self, pdu):
+    def process_metadata_options(self, pdu):
         self.transaction.filestore_requests = pdu.filestore_requests
         self.transaction.messages_to_user = pdu.messages_to_user
         # process user messages
         for message in self.transaction.messages_to_user:
             message.originating_transaction = self.transaction
-            self.kernel.messages_to_user.append(message)
+            self.kernel._messages_to_user_queue.put(message)
 
-    def _restart_nak_timer(self):
+    def restart_nak_timer(self):
         self.nak_timer.restart()
 
-    def _cancel_nak_timer(self):
+    def cancel_nak_timer(self):
         self.nak_timer.cancel()
 
-    def _reuse_senders_first_pdu_header(self, pdu):
+    def reuse_senders_first_pdu_header(self, pdu):
         # as per CCSDS 702.2-G-3, 5.6.1 l)
         if not self.pdu_received:
             self.pdu_received = True
             self.first_pdu_header = pdu.pdu_header
             # reverse the direction field
             if pdu.pdu_header.direction == Direction.TOWARD_RECEIVER:
                 self.first_pdu_header.direction = Direction.TOWARD_SENDER
             else:
                 self.first_pdu_header.direction = Direction.RECEIVER
 
-    def _is_nak_list_empty(self):
+    def is_nak_list_empty(self):
         if self.nak_list:
             return False
         else:
             return True
 
-    def _update_nak_list(self, event, file_size=None):
+    def update_nak_list(self, event, file_size=None):
         self.nak_list = []
         pointer = 0
         if not self.metadata_received:
             self.nak_list.append((0, 0))
         for offset, length in sorted(self.received_file_segments.items()):
             if offset > pointer:
                 self.nak_list.append((pointer, offset))
             pointer = offset + length
         if file_size is not None:
             if pointer < file_size:
                 self.nak_list.append((pointer, file_size))
 
-    def _get_segment_requests(self):
+    def get_segment_requests(self):
         return self.nak_list
```

### Comparing `cfdp-1.1.3/src/cfdp/machines/receiver1.py` & `cfdp-2.0.0/src/cfdp/machines/receiver1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,146 @@
 from cfdp import logger
-from cfdp.constants import MachineState, TransmissionMode, DeliveryCode,\
-    ConditionCode
+from cfdp.constants import MachineState, TransmissionMode, DeliveryCode, ConditionCode
 from cfdp.event import EventType
 from cfdp.meta import execute_filestore_requests
-from .timer import Timer
+from .timer import InactivityTimer
 from .base import Machine
 
 
 class Receiver1(Machine):
 
     """Implementation of Class 1 (unacknowledged transfer) receiver."""
 
     def __init__(self, kernel, transaction):
         super().__init__(kernel, transaction)
         self.transmission_mode = TransmissionMode.UNACKNOWLEDGED
         self.state = MachineState.WAIT_FOR_MD
 
         # inactivity timer
-        timeout = kernel.config.get(
-            transaction.source_entity_id).transaction_inactivity_limit
-        self.inactivity_timer = Timer(
-            self, timeout, EventType.E27_INACTIVITY_TIMEOUT)
+        timeout = kernel.transaction_inactivity_limit
+        self.inactivity_timer = InactivityTimer(
+            self, timeout, EventType.E27_INACTIVITY_TIMEOUT
+        )
 
     def update_state(self, event, pdu=None):
-        """ See state table given in CCSDS 720.2-G-3, Table 5-2 """
-        logger.debug("[{}] Event: {}".format(self.transaction.id, event.type))
+        """See state table given in CCSDS 720.2-G-3, Table 5-2"""
+        logger.debug(
+            "[{}] Event: {}, State: {}".format(
+                self.transaction.id, event.type, self.state
+            )
+        )
 
         if pdu:
-            self._restart_inactivity_timer()  # as per CCSDS 720.2-G-3, 5.3.7
+            self.restart_inactivity_timer()  # as per CCSDS 720.2-G-3, 5.3.7
 
         if self.state == MachineState.WAIT_FOR_MD:
-
             if event.type == EventType.E0_ENTERED_STATE:
-                self._initialize()
-                self._restart_inactivity_timer()
+                self.initialize()
+                self.restart_inactivity_timer()
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E3_NOTICE_OF_CANCELLATION:
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E10_RECEIVED_METADATA:
-                self._issue_metadata_received_indication(pdu.file_size)
-                if self._is_file_transfer():
-                    self._open_temp_file()
-                self._process_metadata_options(pdu)
+                self.issue_metadata_received_indication(pdu.file_size)
+                if self.is_file_transfer():
+                    self.open_tempfile()
+                self.process_metadata_options(pdu)
                 self.state = MachineState.WAIT_FOR_EOF
 
             elif event.type == EventType.E12_RECEIVED_EOF_NO_ERROR:
                 logger.info(
-                    "[{}] Finished without Metadata received"
-                    .format(self.transaction.id))
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                    "[{}] Finished without Metadata received".format(
+                        self.transaction.id
+                    )
+                )
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E13_RECEIVED_EOF_CANCEL:
                 self.condition_code = pdu.condition_code
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E27_INACTIVITY_TIMEOUT:
-                self._restart_inactivity_timer()
-                self._fault_inactivity()
+                self.restart_inactivity_timer()
+                self.fault_inactivity()
 
             elif event.type == EventType.E33_RECEIVED_CANCEL_REQUEST:
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
                 self.trigger_event(EventType.E3_NOTICE_OF_CANCELLATION)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             else:
                 logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                    "[{}] Event: {} not applicable for this state: {}".format(
+                        self.transaction.id, event.type, self.state
+                    )
+                )
 
         elif self.state == MachineState.WAIT_FOR_EOF:
-
             if event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E3_NOTICE_OF_CANCELLATION:
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E11_RECEIVED_FILEDATA:
-                self._issue_filesegment_received_indication(
-                    pdu.segment_offset, len(pdu.file_data))
-                if self._is_file_transfer():
-                    self._store_file_data(pdu)
-                    self._update_received_file_size(pdu)
+                self.issue_filesegment_received_indication(
+                    pdu.segment_offset, len(pdu.file_data)
+                )
+                if self.is_file_transfer():
+                    self.store_file_data(pdu)
+                    self.update_received_file_size(pdu)
 
             elif event.type == EventType.E12_RECEIVED_EOF_NO_ERROR:
-                self._issue_eof_received_indication()
+                self.issue_eof_received_indication()
 
-                if self._is_file_transfer():
-                    if self._is_file_size_error(pdu.file_size):
-                        self._fault_file_size()
-                    if self._is_file_checksum_failure(pdu.file_checksum):
-                        self._fault_file_checksum()
+                if self.is_file_transfer():
+                    if self.is_file_size_error(pdu.file_size):
+                        self.fault_file_size()
+                    if self.is_file_checksum_failure(pdu.file_checksum):
+                        self.fault_file_checksum()
 
                     self.delivery_code = DeliveryCode.DATA_COMPLETE
-                    self._copy_temp_file_to_dest_file()
-                    self._close_temp_file()
+                    self.copy_tempfile_to_destfile()
+                    self.close_tempfile()
 
                 if self.transaction.filestore_requests:
                     execute_filestore_requests(
-                        self.kernel, self.transaction.filestore_requests)
+                        self.kernel, self.transaction.filestore_requests
+                    )
 
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E13_RECEIVED_EOF_CANCEL:
                 self.condition_code = pdu.condition_code
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E27_INACTIVITY_TIMEOUT:
-                self._restart_inactivity_timer()
-                self._fault_inactivity()
+                self.restart_inactivity_timer()
+                self.fault_inactivity()
 
             elif event.type == EventType.E33_RECEIVED_CANCEL_REQUEST:
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
                 self.trigger_event(EventType.E3_NOTICE_OF_CANCELLATION)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             else:
-                logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                pass  # ignore an event not applicable for this state
 
-    def _shutdown(self):
-        super()._shutdown()
+    def shutdown(self):
+        super().shutdown()
         self.inactivity_timer.shutdown()
```

### Comparing `cfdp-1.1.3/src/cfdp/machines/receiver2.py` & `cfdp-2.0.0/src/cfdp/machines/receiver2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from cfdp import logger
-from cfdp.constants import MachineState, TransmissionMode, DeliveryCode,\
-    ConditionCode, DirectiveCode, DirectiveSubTypeCode, TransactionStatus
+from cfdp.constants import (
+    MachineState,
+    TransmissionMode,
+    DeliveryCode,
+    ConditionCode,
+    DirectiveCode,
+    DirectiveSubTypeCode,
+    TransactionStatus,
+)
 from cfdp.event import EventType
 from cfdp.pdu import NakPdu, AckPdu, FinishedPdu
 from cfdp.meta import execute_filestore_requests
 from .timer import InactivityTimer, AckTimer, NakTimer
 from .base import Machine
 
 
@@ -15,137 +22,133 @@
     def __init__(self, kernel, transaction):
         super().__init__(kernel, transaction)
         self.transmission_mode = TransmissionMode.ACKNOWLEDGED
         self.state = MachineState.WAIT_FOR_EOF
         self.file_size = None
 
         # inactivity timer
-        timeout = kernel.config.get(
-            transaction.source_entity_id).transaction_inactivity_limit
+        timeout = kernel.transaction_inactivity_limit
         self.inactivity_timer = InactivityTimer(
-            self, timeout, EventType.E27_INACTIVITY_TIMEOUT)
+            self, timeout, EventType.E27_INACTIVITY_TIMEOUT
+        )
 
         # ack timer
-        timeout = kernel.config.get(
-            transaction.source_entity_id).positive_ack_timer_interval
-        limit = kernel.config.get(
-            transaction.source_entity_id).positive_ack_timer_expiration_limit
-        self.ack_timer = AckTimer(
-            self, timeout, EventType.E25_ACK_TIMEOUT, limit)
+        timeout = kernel.positive_ack_timer_interval
+        limit = kernel.positive_ack_timer_expiration_limit
+        self.ack_timer = AckTimer(self, timeout, EventType.E25_ACK_TIMEOUT, limit)
 
         # nak timer
-        timeout = kernel.config.get(
-            transaction.source_entity_id).nak_timer_interval
-        limit = kernel.config.get(
-            transaction.source_entity_id).nak_timer_expiration_limit
-        self.nak_timer = NakTimer(
-            self, timeout, EventType.E26_NAK_TIMEOUT, limit)
+        timeout = kernel.nak_timer_interval
+        limit = kernel.nak_timer_expiration_limit
+        self.nak_timer = NakTimer(self, timeout, EventType.E26_NAK_TIMEOUT, limit)
 
     def update_state(self, event, pdu=None):
-        """ See state table given in CCSDS 720.2-G-3, Table 5-4 """
+        """See state table given in CCSDS 720.2-G-3, Table 5-4"""
         logger.debug(
             "[{}] Event: {}, State: {}".format(
-                event.transaction.id, event.type, self.state))
+                event.transaction.id, event.type, self.state
+            )
+        )
 
         if pdu:
-            self._restart_inactivity_timer()  # as per CCSDS 720.2-G-3, 5.3.7
+            self.restart_inactivity_timer()  # as per CCSDS 720.2-G-3, 5.3.7
 
         if self.state == MachineState.WAIT_FOR_EOF:
-
             if event.type == EventType.E0_ENTERED_STATE:
-                self._initialize()
-                self._restart_inactivity_timer()
+                self.initialize()
+                self.restart_inactivity_timer()
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E3_NOTICE_OF_CANCELLATION:
                 self.state = MachineState.TRANSACTION_CANCELLED
                 self.trigger_event(EventType.E0_ENTERED_STATE)
 
             elif event.type == EventType.E4_NOTICE_OF_SUSPENSION:
                 if not self.suspended:
-                    self._issue_suspended_indication()
+                    self.issue_suspended_indication()
                     self.suspended = True
                     if not self.frozen:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E5_SUSPEND_TIMERS:
-                self._suspend_inactivity_timer()
+                self.suspend_inactivity_timer()
 
             elif event.type == EventType.E6_RESUME_TIMERS:
-                self._resume_inactivity_timer()
+                self.resume_inactivity_timer()
 
             elif event.type == EventType.E10_RECEIVED_METADATA:
-                self._reuse_senders_first_pdu_header(pdu)
+                self.reuse_senders_first_pdu_header(pdu)
                 if not self.metadata_received:
                     self.metadata_received = True
                     self.file_size = pdu.file_size
-                    self._issue_metadata_received_indication(pdu.file_size)
-                    if self._is_file_transfer():
+                    self.issue_metadata_received_indication(pdu.file_size)
+                    if self.is_file_transfer():
                         if not self.file_open:
-                            self._open_temp_file()
+                            self.open_tempfile()
                             self.file_open = True
-                    self._update_nak_list(event, self.file_size)
-                    self._process_metadata_options(pdu)
+                    self.update_nak_list(event, self.file_size)
+                    self.process_metadata_options(pdu)
 
             elif event.type == EventType.E11_RECEIVED_FILEDATA:
-                self._issue_filesegment_received_indication(
-                    pdu.segment_offset, len(pdu.file_data))
-                self._reuse_senders_first_pdu_header(pdu)
+                self.issue_filesegment_received_indication(
+                    pdu.segment_offset, len(pdu.file_data)
+                )
+                self.reuse_senders_first_pdu_header(pdu)
                 if not self.file_open:
-                    self._open_temp_file()
+                    self.open_tempfile()
                     self.file_open = True
-                self._store_file_data(pdu)
-                self._update_received_file_size(pdu)
-                self._update_nak_list(event, self.file_size)
+                self.store_file_data(pdu)
+                self.update_received_file_size(pdu)
+                self.update_nak_list(event, self.file_size)
 
             elif event.type == EventType.E12_RECEIVED_EOF_NO_ERROR:
-                self._reuse_senders_first_pdu_header(pdu)
-                self._update_nak_list(event, pdu.file_size)
-                self._send_ack_eof()
+                self.reuse_senders_first_pdu_header(pdu)
+                self.update_nak_list(event, pdu.file_size)
+                self.send_ack_eof()
 
-                if self._is_file_size_error(pdu.file_size):
-                    self._fault_file_size()
+                if self.is_file_size_error(pdu.file_size):
+                    self.fault_file_size()
 
                 self.received_file_checksum = pdu.file_checksum
 
-                if self._is_nak_list_empty():
+                if self.is_nak_list_empty():
                     self.state = MachineState.SEND_FINISHED
                 else:
                     self.state = MachineState.GET_MISSING_DATA
                 self.trigger_event(EventType.E0_ENTERED_STATE)
 
             elif event.type == EventType.E13_RECEIVED_EOF_CANCEL:
-                self._reuse_senders_first_pdu_header(pdu)
+                self.reuse_senders_first_pdu_header(pdu)
                 self.condition_code = pdu.condition_code
-                self._send_ack_eof()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_ack_eof()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E27_INACTIVITY_TIMEOUT:
-                self._fault_inactivity()
+                self.fault_inactivity()
 
             elif event.type == EventType.E31_RECEIVED_SUSPEND_REQUEST:
                 self.trigger_event(EventType.E4_NOTICE_OF_SUSPENSION)
 
             elif event.type == EventType.E32_RECEIVED_RESUME_REQUEST:
                 if self.suspended:
-                    self._issue_resumed_indication()
+                    self.issue_resumed_indication()
                     self.suspended = False
                     if not self.frozen:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             elif event.type == EventType.E33_RECEIVED_CANCEL_REQUEST:
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
                 self.trigger_event(EventType.E3_NOTICE_OF_CANCELLATION)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             elif event.type == EventType.E40_RECEIVED_FREEZE:
                 if not self.frozen:
                     self.frozen = True
                     if not self.suspended:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
@@ -153,111 +156,110 @@
                 if self.frozen:
                     self.frozen = False
                     if not self.suspended:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             else:
                 logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                    "[{}] Event: {} not applicable for this state: {}".format(
+                        self.transaction.id, event.type, self.state
+                    )
+                )
 
         elif self.state == MachineState.GET_MISSING_DATA:
-
             if event.type == EventType.E0_ENTERED_STATE:
                 if not self.suspended and not self.frozen:
-                    self._send_nak()
-                self._restart_nak_timer()
+                    self.send_nak()
+                self.restart_nak_timer()
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E3_NOTICE_OF_CANCELLATION:
                 self.state = MachineState.TRANSACTION_CANCELLED
                 self.trigger_event(EventType.E0_ENTERED_STATE)
 
             elif event.type == EventType.E4_NOTICE_OF_SUSPENSION:
                 if not self.suspended:
-                    self._issue_suspended_indication()
+                    self.issue_suspended_indication()
                     self.suspended = True
                     if not self.frozen:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E5_SUSPEND_TIMERS:
-                self._suspend_inactivity_timer()
+                self.suspend_inactivity_timer()
 
             elif event.type == EventType.E6_RESUME_TIMERS:
-                self._restart_inactivity_timer()
+                self.restart_inactivity_timer()
 
             elif event.type == EventType.E10_RECEIVED_METADATA:
                 if not self.metadata_received:
                     self.transaction.source_filename = pdu.source_filename
-                    self.transaction.destination_filename =\
-                        pdu.destination_filename
-                    self.transaction.filestore_requests =\
-                        pdu.filestore_requests
+                    self.transaction.destination_filename = pdu.destination_filename
+                    self.transaction.filestore_requests = pdu.filestore_requests
                     self.transaction.messages_to_user = pdu.messages_to_user
 
                     self.metadata_received = True
                     self.file_size = pdu.file_size
-                    self._issue_metadata_received_indication(pdu.file_size)
+                    self.issue_metadata_received_indication(pdu.file_size)
 
-                    if self._is_file_transfer():
+                    if self.is_file_transfer():
                         if not self.file_open:
-                            self._open_temp_file()
+                            self.open_temp_file()
                             self.file_open = True
-                    self._update_nak_list(event, self.file_size)
-                    self._process_metadata_options(pdu)
+                    self.update_nak_list(event, self.file_size)
+                    self.process_metadata_options(pdu)
 
             elif event.type == EventType.E11_RECEIVED_FILEDATA:
                 if not self.file_open:
-                    self._open_temp_file()
+                    self.open_temp_file()
                     self.file_open = True
-                self._store_file_data(pdu)
-                self._update_received_file_size(pdu)
-                self._update_nak_list(event, self.file_size)
+                self.store_file_data(pdu)
+                self.update_received_file_size(pdu)
+                self.update_nak_list(event, self.file_size)
 
             elif event.type == EventType.E12_RECEIVED_EOF_NO_ERROR:
-                self._send_ack_eof()
+                self.send_ack_eof()
 
             elif event.type == EventType.E13_RECEIVED_EOF_CANCEL:
                 self.condition_code = pdu.condition_code
-                self._send_ack_eof()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_ack_eof()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E26_NAK_TIMEOUT:
-                self._restart_nak_timer()
-                if self._is_nak_list_empty():
+                self.restart_nak_timer()
+                if self.is_nak_list_empty():
                     self.state = MachineState.SEND_FINISHED
                     self.trigger_event(EventType.E0_ENTERED_STATE)
                 elif not self.suspended and not self.frozen:
                     if self.nak_timer.is_limit_reached():
-                        self._fault_nak_limit()
-                    self._send_nak()
+                        self.fault_nak_limit()
+                    self.send_nak()
 
             elif event.type == EventType.E27_INACTIVITY_TIMEOUT:
-                self._fault_inactivity()
+                self.fault_inactivity()
 
             elif event.type == EventType.E31_RECEIVED_SUSPEND_REQUEST:
                 self.trigger_event(EventType.E4_NOTICE_OF_SUSPENSION)
 
             elif event.type == EventType.E32_RECEIVED_RESUME_REQUEST:
                 if self.suspended:
-                    self._issue_resumed_indication()
+                    self.issue_resumed_indication()
                     self.suspended = False
                     if not self.frozen:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             elif event.type == EventType.E33_RECEIVED_CANCEL_REQUEST:
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
                 self.trigger_event(EventType.E3_NOTICE_OF_CANCELLATION)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             elif event.type == EventType.E40_RECEIVED_FREEZE:
                 if not self.frozen:
                     self.frozen = True
                     if not self.suspended:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
@@ -265,98 +267,99 @@
                 if self.frozen:
                     self.frozen = False
                     if not self.suspended:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             else:
                 logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                    "[{}] Event: {} not applicable for this state: {}".format(
+                        self.transaction.id, event.type, self.state
+                    )
+                )
 
         elif self.state == MachineState.SEND_FINISHED:
-
             if event.type == EventType.E0_ENTERED_STATE:
                 self.delivery_code = DeliveryCode.DATA_COMPLETE
-                self._cancel_nak_timer()
+                self.cancel_nak_timer()
 
-                if self._is_file_transfer():
-                    if self._is_file_checksum_failure(
-                            self.received_file_checksum):
-                        self._fault_file_checksum()
-                    self._copy_temp_file_to_dest_file()
-                    self._close_temp_file()
+                if self.is_file_transfer():
+                    if self.is_file_checksum_failure(self.received_file_checksum):
+                        self.fault_file_checksum()
+                    self.copy_tempfile_to_destfile()
+                    self.close_tempfile()
 
                 if self.transaction.filestore_requests:
                     execute_filestore_requests(
-                        self.kernel, self.transaction.filestore_requests)
+                        self.kernel, self.transaction.filestore_requests
+                    )
 
-                self._send_finished()
-                self._restart_ack_timer()
+                self.send_finished()
+                self.restart_ack_timer()
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E3_NOTICE_OF_CANCELLATION:
                 self.state = MachineState.TRANSACTION_CANCELLED
                 self.trigger_event(EventType.E0_ENTERED_STATE)
 
             elif event.type == EventType.E4_NOTICE_OF_SUSPENSION:
                 if not self.suspended:
-                    self._issue_suspended_indication()
+                    self.issue_suspended_indication()
                     self.suspended = True
                     if not self.frozen:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E5_SUSPEND_TIMERS:
-                self._suspend_inactivity_timer()
-                self._suspend_ack_timer()
+                self.suspend_inactivity_timer()
+                self.suspend_ack_timer()
 
             elif event.type == EventType.E6_RESUME_TIMERS:
-                self._restart_inactivity_timer()
-                self._resume_ack_timer()
+                self.restart_inactivity_timer()
+                self.resume_ack_timer()
 
             elif event.type == EventType.E12_RECEIVED_EOF_NO_ERROR:
-                self._send_ack_eof()
+                self.send_ack_eof()
 
             elif event.type == EventType.E13_RECEIVED_EOF_CANCEL:
                 self.condition_code = pdu.condition_code
-                self._send_ack_eof()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_ack_eof()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E18_RECEIVED_ACK_FINISHED:
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E25_ACK_TIMEOUT:
-                self._restart_ack_timer()
+                self.restart_ack_timer()
                 if self.ack_timer.is_limit_reached():
-                    self._fault_ack_limit()
-                self._send_finished()
+                    self.fault_ack_limit()
+                self.send_finished()
 
             elif event.type == EventType.E27_INACTIVITY_TIMEOUT:
-                self._fault_inactivity()
+                self.fault_inactivity()
 
             elif event.type == EventType.E31_RECEIVED_SUSPEND_REQUEST:
                 self.trigger_event(EventType.E4_NOTICE_OF_SUSPENSION)
 
             elif event.type == EventType.E32_RECEIVED_RESUME_REQUEST:
                 if self.suspended:
-                    self._issue_resumed_indication()
+                    self.issue_resumed_indication()
                     self.suspended = False
                     if not self.frozen:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             elif event.type == EventType.E33_RECEIVED_CANCEL_REQUEST:
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
                 self.trigger_event(EventType.E3_NOTICE_OF_CANCELLATION)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             elif event.type == EventType.E40_RECEIVED_FREEZE:
                 if not self.frozen:
                     self.frozen = True
                     if not self.suspended:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
@@ -364,146 +367,142 @@
                 if self.frozen:
                     self.frozen = False
                     if not self.suspended:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             else:
                 logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                    "[{}] Event: {} not applicable for this state: {}".format(
+                        self.transaction.id, event.type, self.state
+                    )
+                )
 
         elif self.state == MachineState.TRANSACTION_CANCELLED:
-
             if event.type == EventType.E0_ENTERED_STATE:
                 self.suspended = False
-                self._send_finished()
-                self._restart_ack_timer()
+                self.send_finished()
+                self.restart_ack_timer()
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E4_NOTICE_OF_SUSPENSION:
                 if not self.suspended:
-                    self._issue_suspended_indication()
+                    self.issue_suspended_indication()
                     self.suspended = True
                     if not self.frozen:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E5_SUSPEND_TIMERS:
-                self._suspend_inactivity_timer()
-                self._suspend_ack_timer()
+                self.suspend_inactivity_timer()
+                self.suspend_ack_timer()
 
             elif event.type == EventType.E6_RESUME_TIMERS:
-                self._restart_inactivity_timer()
-                self._resume_ack_timer()
+                self.restart_inactivity_timer()
+                self.resume_ack_timer()
 
             elif event.type == EventType.E13_RECEIVED_EOF_CANCEL:
                 self.condition_code = pdu.condition_code
-                self._send_ack_eof()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_ack_eof()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E18_RECEIVED_ACK_FINISHED:
                 if self.condition_code != ConditionCode.NO_ERROR:
-                    self._issue_transaction_finished_indication()
-                    self._shutdown()
+                    self.issue_transaction_finished_indication()
+                    self.shutdown()
 
             elif event.type == EventType.E25_ACK_TIMEOUT:
-                self._restart_ack_timer()
+                self.restart_ack_timer()
                 if self.ack_timer.is_limit_reached():
                     self.trigger_event(EventType.E2_ABANDON_TRANSACTION)
                 else:
                     self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
-                    self._send_finished()
+                    self.send_finished()
 
             elif event.type == EventType.E27_INACTIVITY_TIMEOUT:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E31_RECEIVED_SUSPEND_REQUEST:
                 self.trigger_event(EventType.E4_NOTICE_OF_SUSPENSION)
 
             elif event.type == EventType.E32_RECEIVED_RESUME_REQUEST:
                 if self.suspended:
-                    self._issue_resumed_indication()
+                    self.issue_resumed_indication()
                     self.suspended = False
                     if not self.frozen:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             elif event.type == EventType.E40_RECEIVED_FREEZE:
                 if not self.frozen:
                     self.frozen = True
                     if not self.suspended:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E41_RECEIVED_THAW:
                 if self.frozen:
                     self.frozen = False
                     if not self.suspended:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             else:
-                logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                pass  # ignore an event not applicable for this state
 
-    def _shutdown(self):
-        super()._shutdown()
+    def shutdown(self):
+        super().shutdown()
         self.inactivity_timer.shutdown()
         self.ack_timer.shutdown()
         self.nak_timer.shutdown()
 
-    def _send_nak(self):
+    def send_nak(self):
         logger.debug("[{}] Send Nak".format(self.transaction.id))
-        segment_requests = self._get_segment_requests()
+        segment_requests = self.get_segment_requests()
         pdu = NakPdu(
             direction=self.first_pdu_header.direction,
             transmission_mode=self.first_pdu_header.transmission_mode,
             source_entity_id=self.first_pdu_header.source_entity_id,
             transaction_seq_number=self.first_pdu_header.transaction_seq_number,
             destination_entity_id=self.first_pdu_header.destination_entity_id,
             #
             start_of_scope=0,
             end_of_scope=self.received_file_size,
-            segment_requests=segment_requests)
-        address = self.kernel.config.get(
-            self.first_pdu_header.source_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            segment_requests=segment_requests,
+        )
+        self.kernel.transport.request(pdu.encode())
 
-    def _send_ack_eof(self):
+    def send_ack_eof(self):
         logger.debug("[{}] Send Ack EOF".format(self.transaction.id))
         pdu = AckPdu(
             direction=self.first_pdu_header.direction,
             transmission_mode=self.first_pdu_header.transmission_mode,
             source_entity_id=self.first_pdu_header.source_entity_id,
             transaction_seq_number=self.first_pdu_header.transaction_seq_number,
             destination_entity_id=self.first_pdu_header.destination_entity_id,
             #
             directive_code_ack=DirectiveCode.EOF,
             directive_subtype_code=DirectiveSubTypeCode.ACK_OTHERS,
             condition_code=self.condition_code,
-            transaction_status=TransactionStatus.UNDEFINED)
-        address = self.kernel.config.get(
-            self.first_pdu_header.source_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            transaction_status=TransactionStatus.UNDEFINED,
+        )
+        self.kernel.transport.request(pdu.encode())
 
-    def _send_finished(self):
+    def send_finished(self):
         logger.debug("[{}] Send Finished".format(self.transaction.id))
         pdu = FinishedPdu(
             direction=self.first_pdu_header.direction,
             transmission_mode=self.first_pdu_header.transmission_mode,
             source_entity_id=self.first_pdu_header.source_entity_id,
             transaction_seq_number=self.first_pdu_header.transaction_seq_number,
             destination_entity_id=self.first_pdu_header.destination_entity_id,
             #
             condition_code=self.condition_code,
             delivery_code=self.delivery_code,
             file_status=self.file_status,
             filestore_responses=self.filestore_responses,
-            fault_location=None)
-        address = self.kernel.config.get(
-            self.first_pdu_header.source_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            fault_location=None,
+        )
+        self.kernel.transport.request(pdu.encode())
```

### Comparing `cfdp-1.1.3/src/cfdp/machines/sender1.py` & `cfdp-2.0.0/src/cfdp/machines/sender1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from cfdp import logger
-from cfdp.constants import MachineState, ConditionCode, TransmissionMode,\
-    Direction
+from cfdp.constants import MachineState, ConditionCode, TransmissionMode, Direction
 from cfdp.event import EventType
 from cfdp.pdu import MetadataPdu, FiledataPdu, EofPdu
 from .base import Machine
 
 
 class Sender1(Machine):
 
@@ -12,141 +11,140 @@
 
     def __init__(self, kernel, transaction):
         super().__init__(kernel, transaction)
         self.transmission_mode = TransmissionMode.UNACKNOWLEDGED
         self.state = MachineState.SEND_METADATA
 
     def update_state(self, event, pdu=None):
-        """ See state table given in CCSDS 720.2-G-3, Table 5-1 """
-        logger.debug("[{}] Event: {}".format(event.transaction.id, event.type))
+        """See state table given in CCSDS 720.2-G-3, Table 5-1"""
+        logger.debug(
+            "[{}] Event: {}, State: {}".format(
+                event.transaction.id, event.type, self.state
+            )
+        )
 
         if self.state == MachineState.SEND_METADATA:
-
             if event.type == EventType.E0_ENTERED_STATE:
-                self._initialize()
+                self.initialize()
 
             elif event.type == EventType.E30_RECEIVED_PUT_REQUEST:
-                self._issue_transaction_indication()
-                self._send_metadata()
-                if self._is_file_transfer():
+                self.issue_transaction_indication()
+                self.send_metadata()
+                if self.is_file_transfer():
                     self.state = MachineState.SEND_FILE
                     self.trigger_event(EventType.E0_ENTERED_STATE)
                 else:
-                    self._send_eof()
-                    self._issue_eof_sent_indication()
-                    self._issue_transaction_finished_indication()
-                    self._shutdown()
+                    self.send_eof()
+                    self.issue_eof_sent_indication()
+                    self.issue_transaction_finished_indication()
+                    self.shutdown()
 
             else:
                 logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                    "[{}] Event: {} not applicable for this state: {}".format(
+                        self.transaction.id, event.type, self.state
+                    )
+                )
 
         elif self.state == MachineState.SEND_FILE:
-
             if event.type == EventType.E0_ENTERED_STATE:
-                self._open_source_file()
+                self.open_sourcefile()
                 self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E1_SEND_FILE_DATA:
                 if not self.suspended and not self.frozen:
-                    if self._is_comm_layer_ready():
-                        self._send_file_data()
-                        if self._is_entire_file_sent():
-                            self._send_eof()
-                            self._issue_eof_sent_indication()
-                            self._issue_transaction_finished_indication()
-                            self._shutdown()
+                    if self.is_comm_layer_ready():
+                        self.send_file_data()
+                        if self.is_entire_file_sent():
+                            self.send_eof()
+                            self.issue_eof_sent_indication()
+                            self.issue_transaction_finished_indication()
+                            self.shutdown()
                             return  # stop here
                     self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E3_NOTICE_OF_CANCELLATION:
-                self._send_eof()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_eof()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E4_NOTICE_OF_SUSPENSION:
                 if not self.suspended:
-                    self._issue_suspended_indication()
+                    self.issue_suspended_indication()
                     self.suspended = True
 
             elif event.type == EventType.E31_RECEIVED_SUSPEND_REQUEST:
                 self.trigger_event(EventType.E4_NOTICE_OF_SUSPENSION)
 
             elif event.type == EventType.E32_RECEIVED_RESUME_REQUEST:
                 if self.suspended:
-                    self._issue_resumed_indication()
+                    self.issue_resumed_indication()
                     self.suspended = False
                     if not self.frozen:
                         self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E33_RECEIVED_CANCEL_REQUEST:
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
                 self.trigger_event(EventType.E3_NOTICE_OF_CANCELLATION)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             elif event.type == EventType.E40_RECEIVED_FREEZE:
                 self.frozen = True
 
             elif event.type == EventType.E41_RECEIVED_THAW:
                 if self.frozen:
                     self.frozen = False
                     if not self.suspended:
                         self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             else:
-                logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                pass  # ignore an event not applicable for this state
 
-    def _send_metadata(self):
+    def send_metadata(self):
         logger.debug("[{}] Send Metadata".format(self.transaction.id))
         pdu = MetadataPdu(
             direction=Direction.TOWARD_RECEIVER,
             transmission_mode=self.transmission_mode,
             source_entity_id=self.transaction.source_entity_id,
             transaction_seq_number=self.transaction.seq_number,
             destination_entity_id=self.transaction.destination_entity_id,
             file_size=self.transaction.get_file_size(),
             source_filename=self.transaction.source_filename,
             destination_filename=self.transaction.destination_filename,
             filestore_requests=self.transaction.filestore_requests,
-            messages_to_user=self.transaction.messages_to_user)
-        address = self.kernel.config.get(
-            self.transaction.destination_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            messages_to_user=self.transaction.messages_to_user,
+        )
+        self.kernel.transport.request(pdu.encode())
 
-    def _send_file_data(self):
+    def send_file_data(self):
         logger.debug("[{}] Send Filedata".format(self.transaction.id))
         offset, data = self.transaction.get_file_segment()
         pdu = FiledataPdu(
             direction=Direction.TOWARD_RECEIVER,
             transmission_mode=self.transmission_mode,
             source_entity_id=self.transaction.source_entity_id,
             transaction_seq_number=self.transaction.seq_number,
             destination_entity_id=self.transaction.destination_entity_id,
             segment_offset=offset,
-            file_data=data)
-        address = self.kernel.config.get(
-            self.transaction.destination_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            file_data=data,
+        )
+        self.kernel.transport.request(pdu.encode())
 
-    def _send_eof(self):
+    def send_eof(self):
         logger.debug("[{}] Send EOF".format(self.transaction.id))
         pdu = EofPdu(
             direction=Direction.TOWARD_RECEIVER,
             transmission_mode=self.transmission_mode,
             source_entity_id=self.transaction.source_entity_id,
             transaction_seq_number=self.transaction.seq_number,
             destination_entity_id=self.transaction.destination_entity_id,
             condition_code=self.condition_code,
             file_checksum=self.transaction.get_file_checksum(),
-            file_size=self.transaction.get_file_size())
-        address = self.kernel.config.get(
-            self.transaction.destination_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            file_size=self.transaction.get_file_size(),
+        )
+        self.kernel.transport.request(pdu.encode())
```

### Comparing `cfdp-1.1.3/src/cfdp/machines/sender2.py` & `cfdp-2.0.0/src/cfdp/machines/sender2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from cfdp import logger
-from cfdp.constants import MachineState, ConditionCode, Direction,\
-    DirectiveCode, TransactionStatus, TransmissionMode, DirectiveSubTypeCode
+from cfdp.constants import (
+    MachineState,
+    ConditionCode,
+    Direction,
+    DirectiveCode,
+    TransactionStatus,
+    TransmissionMode,
+    DirectiveSubTypeCode,
+)
 from cfdp.event import EventType
 from cfdp.pdu import MetadataPdu, FiledataPdu, EofPdu, AckPdu
 from .timer import InactivityTimer, AckTimer
 from .base import Machine
 
 
 class Sender2(Machine):
@@ -13,221 +20,220 @@
 
     def __init__(self, kernel, transaction):
         super().__init__(kernel, transaction)
         self.transmission_mode = TransmissionMode.ACKNOWLEDGED
         self.state = MachineState.SEND_METADATA
 
         # inactivity timer
-        timeout = kernel.config.get(
-            transaction.destination_entity_id).transaction_inactivity_limit
+        timeout = kernel.transaction_inactivity_limit
         self.inactivity_timer = InactivityTimer(
-            self, timeout, EventType.E27_INACTIVITY_TIMEOUT)
+            self, timeout, EventType.E27_INACTIVITY_TIMEOUT
+        )
 
         # ack timer
-        timeout = kernel.config.get(
-            transaction.destination_entity_id).positive_ack_timer_interval
-        limit = kernel.config.get(transaction.destination_entity_id)\
-            .positive_ack_timer_expiration_limit
-        self.ack_timer = AckTimer(
-            self, timeout, EventType.E25_ACK_TIMEOUT, limit)
+        timeout = kernel.positive_ack_timer_interval
+        limit = kernel.positive_ack_timer_expiration_limit
+        self.ack_timer = AckTimer(self, timeout, EventType.E25_ACK_TIMEOUT, limit)
 
     def update_state(self, event, pdu=None):
-        """ See state table given in CCSDS 720.2-G-3, Table 5-3 """
+        """See state table given in CCSDS 720.2-G-3, Table 5-3"""
         logger.debug(
             "[{}] Event: {}, State: {}".format(
-                event.transaction.id, event.type, self.state))
+                event.transaction.id, event.type, self.state
+            )
+        )
 
         if pdu:
-            self._restart_inactivity_timer()  # as per CCSDS 720.2-G-3, 5.3.7
+            self.restart_inactivity_timer()  # as per CCSDS 720.2-G-3, 5.3.7
 
         if self.state == MachineState.SEND_METADATA:
-
             if event.type == EventType.E0_ENTERED_STATE:
-                self._initialize()
+                self.initialize()
 
             elif event.type == EventType.E30_RECEIVED_PUT_REQUEST:
-                self._issue_transaction_indication()
-                self._send_metadata()
-                if self._is_file_transfer():
+                self.issue_transaction_indication()
+                self.send_metadata()
+                if self.is_file_transfer():
                     self.state = MachineState.SEND_FILE
                 else:
                     self.state = MachineState.SEND_EOF
                 self.trigger_event(EventType.E0_ENTERED_STATE)
 
             else:
                 logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                    "[{}] Event: {} not applicable for this state: {}".format(
+                        self.transaction.id, event.type, self.state
+                    )
+                )
 
         elif self.state == MachineState.SEND_FILE:
-
             if event.type == EventType.E0_ENTERED_STATE:
-                self._open_source_file()
+                self.open_sourcefile()
                 self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E1_SEND_FILE_DATA:
-                if not self.frozen\
-                        and not self.suspended:
-                    if self._is_comm_layer_ready():
-                        self._send_file_data()
-                        if self._is_entire_file_sent():
+                if not self.frozen and not self.suspended:
+                    if self.is_comm_layer_ready():
+                        self.send_file_data()
+                        if self.is_entire_file_sent():
                             self.state = MachineState.SEND_EOF
                             self.trigger_event(EventType.E0_ENTERED_STATE)
                     self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E3_NOTICE_OF_CANCELLATION:
                 self.state = MachineState.TRANSACTION_CANCELLED
                 self.trigger_event(EventType.E0_ENTERED_STATE)
 
             elif event.type == EventType.E4_NOTICE_OF_SUSPENSION:
                 if not self.suspended:
-                    self._issue_suspended_indication()
+                    self.issue_suspended_indication()
                     self.suspended = True
                     if not self.frozen:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E5_SUSPEND_TIMERS:
-                self._suspend_inactivity_timer()
+                self.suspend_inactivity_timer()
 
             elif event.type == EventType.E6_RESUME_TIMERS:
                 self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E15_RECEIVED_NAK:
                 if not self.suspended and not self.frozen:
-                    self._queue_nakked_data(pdu)
+                    self.queue_nakked_data(pdu)
 
             elif event.type == EventType.E17_RECEIVED_FINISHED_CANCEL:
                 self.condition_code = pdu.condition_code
-                self._send_ack_finished()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_ack_finished()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E31_RECEIVED_SUSPEND_REQUEST:
                 self.trigger_event(EventType.E4_NOTICE_OF_SUSPENSION)
 
             elif event.type == EventType.E32_RECEIVED_RESUME_REQUEST:
                 if self.suspended:
-                    self._issue_resumed_indication()
+                    self.issue_resumed_indication()
                     self.suspended = False
                     if not self.frozen:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             elif event.type == EventType.E33_RECEIVED_CANCEL_REQUEST:
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
                 self.trigger_event(EventType.E3_NOTICE_OF_CANCELLATION)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             elif event.type == EventType.E40_RECEIVED_FREEZE:
                 if not self.frozen:
                     self.frozen = True
                     if not self.suspended:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E41_RECEIVED_THAW:
                 if self.frozen:
                     self.frozen = False
                     if not self.suspended:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             else:
-                logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                raise ValueError(
+                    "[{}] Event: {} not applicable for this state: {}".format(
+                        self.transaction.id, event.type, self.state
+                    )
+                )
 
         elif self.state == MachineState.SEND_EOF:
-
             if event.type == EventType.E0_ENTERED_STATE:
-                self._send_eof()
-                self._issue_eof_sent_indication()
-                self._restart_ack_timer()
-                self._restart_inactivity_timer()
+                self.send_eof()
+                self.issue_eof_sent_indication()
+                self.restart_ack_timer()
+                self.restart_inactivity_timer()
 
             elif event.type == EventType.E1_SEND_FILE_DATA:
                 if not self.suspended and not self.frozen:
-                    if self._is_file_data_queued():
-                        if self._is_comm_layer_ready():
-                            self._send_missing_file_data()
+                    if self.is_file_data_queued():
+                        if self.is_comm_layer_ready():
+                            self.send_missing_file_data()
                         self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E3_NOTICE_OF_CANCELLATION:
                 self.state = MachineState.TRANSACTION_CANCELLED
                 self.trigger_event(EventType.E0_ENTERED_STATE)
 
             elif event.type == EventType.E4_NOTICE_OF_SUSPENSION:
                 if not self.suspended:
-                    self._issue_suspended_indication()
+                    self.issue_suspended_indication()
                     self.suspended = True
                     if not self.frozen:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E5_SUSPEND_TIMERS:
-                self._suspend_inactivity_timer()
-                if self._is_ack_timer_running():
-                    self._suspend_ack_timer()
+                self.suspend_inactivity_timer()
+                if self.is_ack_timer_running():
+                    self.suspend_ack_timer()
 
             elif event.type == EventType.E6_RESUME_TIMERS:
                 self._resume_inactivity_timer()
-                if self._is_ack_timer_suspended():
-                    self._resume_ack_timer()
+                if self.is_ack_timer_suspended():
+                    self.resume_ack_timer()
                 self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E14_RECEIVED_ACK_EOF:
-                self._cancel_ack_timer()
+                self.cancel_ack_timer()
 
             elif event.type == EventType.E15_RECEIVED_NAK:
                 if not self.suspended and not self.frozen:
-                    self._queue_nakked_data(pdu)
+                    self.queue_nakked_data(pdu)
                     self.trigger_event(EventType.E1_SEND_FILE_DATA)
 
             elif event.type == EventType.E16_RECEIVED_FINISHED_NO_ERROR:
-                self._send_ack_finished()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_ack_finished()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E17_RECEIVED_FINISHED_CANCEL:
                 self.condition_code = pdu.condition_code
-                self._send_ack_finished()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_ack_finished()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E25_ACK_TIMEOUT:
-                self._restart_ack_timer()
-                if self._is_ack_limit_reached():
-                    self._fault_ack_limit()
-                self._send_eof()
+                self.restart_ack_timer()
+                if self.is_ack_limit_reached():
+                    self.fault_ack_limit()
+                self.send_eof()
 
             elif event.type == EventType.E27_INACTIVITY_TIMEOUT:
-                self._fault_inactivity()
+                self.fault_inactivity()
 
             elif event.type == EventType.E31_RECEIVED_SUSPEND_REQUEST:
                 self.trigger_event(EventType.E4_NOTICE_OF_SUSPENSION)
 
             elif event.type == EventType.E32_RECEIVED_RESUME_REQUEST:
                 if self.suspended:
-                    self._issue_resumed_indication()
+                    self.issue_resumed_indication()
                     self.suspended = False
                     if not self.frozen:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             elif event.type == EventType.E33_RECEIVED_CANCEL_REQUEST:
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
                 self.trigger_event(EventType.E3_NOTICE_OF_CANCELLATION)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             elif event.type == EventType.E40_RECEIVED_FREEZE:
                 if not self.frozen:
                     self.frozen = True
                     if not self.suspended:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
@@ -235,151 +241,147 @@
                 if self.frozen:
                     self.frozen = False
                     if not self.suspended:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             else:
                 logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                    "[{}] Event: {} not applicable for this state: {}".format(
+                        self.transaction.id, event.type, self.state
+                    )
+                )
 
         elif self.state == MachineState.TRANSACTION_CANCELLED:
-
             if event.type == EventType.E0_ENTERED_STATE:
                 self.suspended = False
                 self.condition_code = ConditionCode.CANCEL_REQUEST_RECEIVED
-                self._send_eof()
-                self._issue_eof_sent_indication()
-                self._restart_ack_timer()
-                self._restart_inactivity_timer()
+                self.send_eof()
+                self.issue_eof_sent_indication()
+                self.restart_ack_timer()
+                self.restart_inactivity_timer()
 
             elif event.type == EventType.E2_ABANDON_TRANSACTION:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E4_NOTICE_OF_SUSPENSION:
                 if not self.suspended:
-                    self._issue_suspended_indication()
+                    self.issue_suspended_indication()
                     self.suspended = True
                     if not self.frozen:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E5_SUSPEND_TIMERS:
-                self._suspend_inactivity_timer()
-                self._suspend_ack_timer()
+                self.suspend_inactivity_timer()
+                self.suspend_ack_timer()
 
             elif event.type == EventType.E6_RESUME_TIMERS:
-                self._resume_inactivity_timer()
-                self._resume_ack_timer()
+                self.resume_inactivity_timer()
+                self.resume_ack_timer()
 
             elif event.type == EventType.E14_RECEIVED_ACK_EOF:
                 if self.condition_code != ConditionCode.NO_ERROR:
-                    self._issue_transaction_finished_indication()
-                    self._shutdown()
+                    self.issue_transaction_finished_indication()
+                    self.shutdown()
 
             elif event.type == EventType.E17_RECEIVED_FINISHED_CANCEL:
                 self.condition_code = pdu.condition_code
-                self._send_ack_finished()
-                self._issue_transaction_finished_indication()
-                self._shutdown()
+                self.send_ack_finished()
+                self.issue_transaction_finished_indication()
+                self.shutdown()
 
             elif event.type == EventType.E25_ACK_TIMEOUT:
-                self._restart_ack_timer()
-                if self._is_ack_limit_reached():
+                self.restart_ack_timer()
+                if self.is_ack_limit_reached():
                     self.trigger_event(EventType.E2_ABANDON_TRANSACTION)
                 else:
-                    self._send_eof()
+                    self.send_eof()
 
             elif event.type == EventType.E27_INACTIVITY_TIMEOUT:
-                self._issue_abandoned_indication()
-                self._shutdown()
+                self.issue_abandoned_indication()
+                self.shutdown()
 
             elif event.type == EventType.E31_RECEIVED_SUSPEND_REQUEST:
                 self.trigger_event(EventType.E4_NOTICE_OF_SUSPENSION)
 
             elif event.type == EventType.E32_RECEIVED_RESUME_REQUEST:
                 if self.suspended:
-                    self._issue_resumed_indication()
+                    self.issue_resumed_indication()
                     self.suspended = False
                     if not self.frozen:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             elif event.type == EventType.E34_RECEIVED_REPORT_REQUEST:
-                self._issue_report_indication()
+                self.issue_report_indication()
 
             elif event.type == EventType.E40_RECEIVED_FREEZE:
                 if not self.frozen:
                     self.frozen = True
                     if not self.suspended:
                         self.trigger_event(EventType.E5_SUSPEND_TIMERS)
 
             elif event.type == EventType.E41_RECEIVED_THAW:
                 if self.frozen:
                     self.frozen = False
                     if not self.suspended:
                         self.trigger_event(EventType.E6_RESUME_TIMERS)
 
             else:
-                logger.debug(
-                    "[{}] Event: {} not applicable for this state: {}"
-                    .format(self.transaction.id, event.type, self.state))
+                pass  # ignore an event not applicable for this state
 
-    def _shutdown(self):
-        super()._shutdown()
+    def shutdown(self):
+        super().shutdown()
         self.inactivity_timer.shutdown()
         self.ack_timer.shutdown()
 
-    def _send_metadata(self):
+    def send_metadata(self):
         logger.debug("[{}] Send Metadata".format(self.transaction.id))
         pdu = MetadataPdu(
             direction=Direction.TOWARD_RECEIVER,
             transmission_mode=self.transmission_mode,
             source_entity_id=self.transaction.source_entity_id,
             transaction_seq_number=self.transaction.seq_number,
             destination_entity_id=self.transaction.destination_entity_id,
             file_size=self.transaction.get_file_size(),
             source_filename=self.transaction.source_filename,
             destination_filename=self.transaction.destination_filename,
             filestore_requests=self.transaction.filestore_requests,
-            messages_to_user=self.transaction.messages_to_user)
-        address = self.kernel.config.get(
-            self.transaction.destination_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            messages_to_user=self.transaction.messages_to_user,
+        )
+        self.kernel.transport.request(pdu.encode())
 
-    def _send_file_data(self):
+    def send_file_data(self):
         logger.debug("[{}] Send Filedata".format(self.transaction.id))
         offset, data = self.transaction.get_file_segment()
         pdu = FiledataPdu(
             direction=Direction.TOWARD_RECEIVER,
             transmission_mode=self.transmission_mode,
             source_entity_id=self.transaction.source_entity_id,
             transaction_seq_number=self.transaction.seq_number,
             destination_entity_id=self.transaction.destination_entity_id,
             segment_offset=offset,
-            file_data=data)
-        address = self.kernel.config.get(
-            self.transaction.destination_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            file_data=data,
+        )
+        self.kernel.transport.request(pdu.encode())
 
-    def _send_eof(self):
+    def send_eof(self):
         logger.debug("[{}] Send EOF".format(self.transaction.id))
         pdu = EofPdu(
             direction=Direction.TOWARD_RECEIVER,
             transmission_mode=self.transmission_mode,
             source_entity_id=self.transaction.source_entity_id,
             transaction_seq_number=self.transaction.seq_number,
             destination_entity_id=self.transaction.destination_entity_id,
             condition_code=self.condition_code,
             file_checksum=self.transaction.get_file_checksum(),
-            file_size=self.transaction.get_file_size())
-        address = self.kernel.config.get(
-            self.transaction.destination_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            file_size=self.transaction.get_file_size(),
+        )
+        self.kernel.transport.request(pdu.encode())
 
-    def _send_missing_file_data(self):
+    def send_missing_file_data(self):
         logger.debug("[{}] Send Missing Filedata".format(self.transaction.id))
         start, end = self.nak_list.pop(0)
         length = end - start
 
         if start == 0 and length == 0:
             pdu = MetadataPdu(
                 direction=Direction.TOWARD_RECEIVER,
@@ -387,39 +389,38 @@
                 source_entity_id=self.transaction.source_entity_id,
                 transaction_seq_number=self.transaction.seq_number,
                 destination_entity_id=self.transaction.destination_entity_id,
                 file_size=self.transaction.get_file_size(),
                 source_filename=self.transaction.source_filename,
                 destination_filename=self.transaction.destination_filename,
                 filestore_requests=self.transaction.filestore_requests,
-                messages_to_user=self.transaction.messages_to_user)
+                messages_to_user=self.transaction.messages_to_user,
+            )
         else:
             _, file_data = self.transaction.get_file_segment(start, length)
             pdu = FiledataPdu(
                 direction=Direction.TOWARD_RECEIVER,
                 transmission_mode=self.transmission_mode,
                 source_entity_id=self.transaction.source_entity_id,
                 transaction_seq_number=self.transaction.seq_number,
                 destination_entity_id=self.transaction.destination_entity_id,
                 #
                 segment_offset=start,
-                file_data=file_data)
-        address = self.kernel.config.get(
-            self.transaction.destination_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+                file_data=file_data,
+            )
+        self.kernel.transport.request(pdu.encode())
 
-    def _send_ack_finished(self):
+    def send_ack_finished(self):
         logger.debug("[{}] Send Ack Finished".format(self.transaction.id))
         pdu = AckPdu(
             direction=Direction.TOWARD_RECEIVER,
             transmission_mode=self.transmission_mode,
             source_entity_id=self.transaction.source_entity_id,
             transaction_seq_number=self.transaction.seq_number,
             destination_entity_id=self.transaction.destination_entity_id,
             #
             directive_code_ack=DirectiveCode.FINISHED,
             directive_subtype_code=DirectiveSubTypeCode.ACK_FINISHED,
             condition_code=self.condition_code,
-            transaction_status=TransactionStatus.UNDEFINED)
-        address = self.kernel.config.get(
-            self.transaction.destination_entity_id).ut_address
-        self.kernel.transport.request(pdu.encode(), address)
+            transaction_status=TransactionStatus.UNDEFINED,
+        )
+        self.kernel.transport.request(pdu.encode())
```

### Comparing `cfdp-1.1.3/src/cfdp/machines/timer.py` & `cfdp-2.0.0/src/cfdp/machines/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import threading
 
 from cfdp import logger
 from cfdp.event import Event
 
 
 class Timer:
-
     def __init__(self, machine, timeout, raise_event, expiration_limit=None):
         self.machine = machine
         self.timeout = timeout
         self.raise_event = raise_event
         self._timer = None
         self._expiration_limit = expiration_limit
         self._expiration_counter = 0
@@ -26,15 +25,16 @@
         if self._timer:
             self._timer.cancel()
 
     def _expired(self):
         logger.debug("Timer expired {}".format(type(self)))
         self._expiration_counter += 1
         self.machine.kernel.trigger_event(
-            Event(self.machine.transaction, self.raise_event))
+            Event(self.machine.transaction, self.raise_event)
+        )
 
     def is_limit_reached(self):
         if self._expiration_limit is None:
             return False
         else:
             return self._expiration_counter >= self._expiration_limit
```

### Comparing `cfdp-1.1.3/src/cfdp/meta/filestore.py` & `cfdp-2.0.0/src/cfdp/meta/filestore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 from cfdp import logger
 from cfdp.constants import TypeFieldCode, ActionCode
 from .datafield import TypeLengthValue
 
 
 class FilestoreRequest(TypeLengthValue):
-
     def __init__(self, action_code, first_filename, second_filename=None):
         self.type = TypeFieldCode.FILESTORE_REQUEST
 
         self.action_code = action_code
         self.first_filename = first_filename
         self.second_filename = second_filename
 
     def encode(self):
-
         data = bytes([(self.action_code << 4)])
 
-        value = self.first_filename.encode('utf-8')
+        value = self.first_filename.encode("utf-8")
         length = len(value)
         data += bytes([length])
         data += value
 
         if self.second_filename:
-            value = self.second_filename.encode('utf-8')
+            value = self.second_filename.encode("utf-8")
             length = len(value)
             data += bytes([length])
             data += value
 
         self.value = data
         return super().encode()
 
 
 def execute_filestore_requests(kernel, filestore_requests):
-
     for filestore_request in filestore_requests:
-
         if filestore_request.action_code == ActionCode.CREATE_FILE:
             filename = filestore_request.first_filename.decode()
             logger.info("Create file: <{}>".format(filename))
             try:
                 kernel.filestore.create_file(filename)
             except Exception:
                 logger.error("Failed to create file <{}>".format(filename))
@@ -50,62 +46,63 @@
                 kernel.filestore.delete_file(filename)
             except Exception:
                 logger.error("Failed to delete file: <{}>".format(filename))
 
         elif filestore_request.action_code == ActionCode.RENAME_FILE:
             filename1 = filestore_request.first_filename.decode()
             filename2 = filestore_request.second_filename.decode()
-            logger.info("Rename file: <{}> to <{}>".format(
-                filename1, filename2))
+            logger.info("Rename file: <{}> to <{}>".format(filename1, filename2))
             try:
                 kernel.filestore.rename_file(filename1, filename2)
             except Exception:
-                logger.error("Failed to rename file <{}> to <{}>".format(
-                    filename1, filename2))
+                logger.error(
+                    "Failed to rename file <{}> to <{}>".format(filename1, filename2)
+                )
 
         elif filestore_request.action_code == ActionCode.APPEND_FILE:
             filename1 = filestore_request.first_filename.decode()
             filename2 = filestore_request.second_filename.decode()
-            logger.info("Append file <{}> with <{}>".format(
-                filename1, filename2))
+            logger.info("Append file <{}> with <{}>".format(filename1, filename2))
             try:
                 kernel.filestore.append_file(filename1, filename2)
             except Exception:
-                logger.error("Failed to append file <{}> with <{}>".format(
-                    filename1, filename2))
+                logger.error(
+                    "Failed to append file <{}> with <{}>".format(filename1, filename2)
+                )
 
         elif filestore_request.action_code == ActionCode.REPLACE_FILE:
             filename1 = filestore_request.first_filename.decode()
             filename2 = filestore_request.second_filename.decode()
-            logger.info("Replace content of file <{}> by <{}>".format(
-                filename1, filename2))
+            logger.info(
+                "Replace content of file <{}> by <{}>".format(filename1, filename2)
+            )
             try:
                 kernel.filestore.replace_file(filename1, filename2)
             except Exception:
                 logger.error(
                     "Failed to replace content of <{}> by <{}>".format(
-                        filename1, filename2))
+                        filename1, filename2
+                    )
+                )
 
         elif filestore_request.action_code == ActionCode.CREATE_DIRECTORY:
             dirname = filestore_request.first_filename.decode()
             logger.info("Create directory: <{}>".format(dirname))
             try:
                 kernel.filestore.create_directory(dirname)
             except Exception:
-                logger.error(
-                    "Failed to create directory: <{}>".format(dirname))
+                logger.error("Failed to create directory: <{}>".format(dirname))
 
         elif filestore_request.action_code == ActionCode.REMOVE_DIRECTORY:
             dirname = filestore_request.first_filename.decode()
             logger.info("Remove directory: <{}>".format(dirname))
             try:
                 kernel.filestore.remove_directory(dirname)
             except Exception:
-                logger.error(
-                    "Failed to delete directory: <{}>".format(dirname))
+                logger.error("Failed to delete directory: <{}>".format(dirname))
 
         elif filestore_request.action_code == ActionCode.DENY_FILE:
             filename = filestore_request.first_filename.decode()
             logger.info("Deny file: <{}>".format(filename))
             try:
                 kernel.filestore.delete_file(filename)
             except Exception:
@@ -119,18 +116,19 @@
             except Exception:
                 pass
 
 
 def extract_filestore_request(data):
     action_code = data[0] >> 4
     length_of_first_filename = data[1]
-    first_filename = data[2:2+length_of_first_filename]
+    first_filename = data[2 : 2 + length_of_first_filename]
 
     if action_code in [
-            ActionCode.RENAME_FILE,
-            ActionCode.APPEND_FILE,
-            ActionCode.REPLACE_FILE]:
-        second_filename = data[3+length_of_first_filename:]
+        ActionCode.RENAME_FILE,
+        ActionCode.APPEND_FILE,
+        ActionCode.REPLACE_FILE,
+    ]:
+        second_filename = data[3 + length_of_first_filename :]
     else:
         second_filename = None
 
     return FilestoreRequest(action_code, first_filename, second_filename)
```

### Comparing `cfdp-1.1.3/src/cfdp/meta/message.py` & `cfdp-2.0.0/src/cfdp/meta/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,377 +6,355 @@
 
 
 def get_required_octets(number):
     return max(math.ceil(math.log(number + 1, 2) / 8), 1)
 
 
 class MessageToUser(TypeLengthValue):
-
     def __init__(self):
         self.type = TypeFieldCode.MESSAGE_TO_USER
 
 
 class ReservedMessageToUser(MessageToUser):
-
     def __init__(self):
         super().__init__()
-        self.message_identifier = 'cfdp'
+        self.message_identifier = "cfdp"
 
 
 class OriginatingTransactionId(ReservedMessageToUser):
-
     def __init__(self, source_entity_id, transaction_seq_number):
         super().__init__()
         self.message_type = MessageType.ORIGINATING_TRANSACTION_ID
 
         self.source_entity_id = source_entity_id
         self.transaction_seq_number = transaction_seq_number
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
 
         length_of_entity_id = get_required_octets(self.source_entity_id) - 1
-        length_of_seq_number = get_required_octets(
-            self.transaction_seq_number) - 1
-        data += bytes([
-            (0 << 7) +
-            (length_of_entity_id << 4) +
-            (0 << 3) +
-            length_of_seq_number])
+        length_of_seq_number = get_required_octets(self.transaction_seq_number) - 1
+        data += bytes(
+            [(0 << 7) + (length_of_entity_id << 4) + (0 << 3) + length_of_seq_number]
+        )
 
         x = []
 
         for i in range(length_of_entity_id + 1):
-            x.append((self.source_entity_id >> (8*i)) & 0xff)
+            x.append((self.source_entity_id >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         x = []
 
         for i in range(length_of_seq_number + 1):
-            x.append((self.transaction_seq_number >> (8*i)) & 0xff)
+            x.append((self.transaction_seq_number >> (8 * i)) & 0xFF)
 
         x.reverse()
         data += bytes(x)
 
         self.value = data
         return super().encode()
 
 
 class ProxyPutRequest(ReservedMessageToUser):
-
     def __init__(
-            self, destination_entity_id,
-            source_filename=None, destination_filename=None):
+        self, destination_entity_id, source_filename=None, destination_filename=None
+    ):
         super().__init__()
         self.message_type = MessageType.PROXY_PUT_REQUEST
 
         self.destination_entity_id = destination_entity_id
         self.source_filename = source_filename
         self.destination_filename = destination_filename
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
 
-        length_of_entity_id = get_required_octets(
-            self.destination_entity_id)
+        length_of_entity_id = get_required_octets(self.destination_entity_id)
         data += bytes([length_of_entity_id])
         x = []
         for i in range(length_of_entity_id):
-            x.append((self.destination_entity_id >> (8*i)) & 0xff)
+            x.append((self.destination_entity_id >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
-        value = self.source_filename.encode('utf-8')
+        value = self.source_filename.encode("utf-8")
         length = len(value)
         data += bytes([length])
         data += value
 
-        value = self.destination_filename.encode('utf-8')
+        value = self.destination_filename.encode("utf-8")
         length = len(value)
         data += bytes([length])
         data += value
 
         self.value = data
         return super().encode()
 
 
 class ProxyPutCancel(ReservedMessageToUser):
-
     def __init__(self, entity_id, seq_number):
         super().__init__()
         self.message_type = MessageType.PROXY_PUT_CANCEL
 
         self.entity_id = entity_id
         self.seq_number = seq_number
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
         self.value = data
 
         length_of_entity_id = get_required_octets(self.entity_id)
 
         data += bytes([length_of_entity_id])
 
         x = []
 
         for i in range(length_of_entity_id):
-            x.append((self.entity_id >> (8*i)) & 0xff)
+            x.append((self.entity_id >> (8 * i)) & 0xFF)
 
         x.reverse()
         data += bytes(x)
 
         length_of_seq_number = get_required_octets(self.seq_number)
         data += bytes([length_of_seq_number])
 
         x = []
 
         for i in range(length_of_seq_number):
-            x.append((self.seq_number >> (8*i)) & 0xff)
+            x.append((self.seq_number >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         self.value = data
         return super().encode()
 
 
 class DirectoryListingRequest(ReservedMessageToUser):
-
     def __init__(self, remote_directory, local_file):
         super().__init__()
         self.message_type = MessageType.DIRECTORY_LISTING_REQUEST
 
         self.directory_name = remote_directory
         self.directory_file_name = local_file
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
 
-        value = self.directory_name.encode('utf-8')
+        value = self.directory_name.encode("utf-8")
         length = len(value)
         data += bytes([length])
         data += value
 
-        value = self.directory_file_name.encode('utf-8')
+        value = self.directory_file_name.encode("utf-8")
         length = len(value)
         data += bytes([length])
         data += value
 
         self.value = data
         return super().encode()
 
 
 class DirectoryListingResponse(ReservedMessageToUser):
-
-    def __init__(
-            self, remote_directory, local_file, listing_response_code=0x00):
+    def __init__(self, remote_directory, local_file, listing_response_code=0x00):
         super().__init__()
         self.message_type = MessageType.DIRECTORY_LISTING_RESPONSE
 
         self.listing_response_code = listing_response_code
         self.directory_name = remote_directory
         self.directory_file_name = local_file
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
 
         data += bytes([self.listing_response_code])
 
-        value = self.directory_name.encode('utf-8')
+        value = self.directory_name.encode("utf-8")
         length = len(value)
         data += bytes([length])
         data += value
 
-        value = self.directory_file_name.encode('utf-8')
+        value = self.directory_file_name.encode("utf-8")
         length = len(value)
         data += bytes([length])
         data += value
 
         self.value = data
         return super().encode()
 
 
 class RemoteSuspendRequest(ReservedMessageToUser):
-
-    def __init__(
-            self, source_entity_id, transaction_seq_number):
+    def __init__(self, source_entity_id, transaction_seq_number):
         super().__init__()
         self.message_type = MessageType.REMOTE_SUSPEND_REQUEST
 
         self.source_entity_id = source_entity_id
         self.transaction_seq_number = transaction_seq_number
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
 
         length_of_entity_id = get_required_octets(self.source_entity_id) - 1
-        length_of_seq_number = get_required_octets(
-            self.transaction_seq_number) - 1
+        length_of_seq_number = get_required_octets(self.transaction_seq_number) - 1
 
-        data += bytes([
-            (0 << 7) +
-            (length_of_entity_id << 4) +
-            (0 << 3) +
-            length_of_seq_number])
+        data += bytes(
+            [(0 << 7) + (length_of_entity_id << 4) + (0 << 3) + length_of_seq_number]
+        )
 
         x = []
 
         for i in range(length_of_entity_id + 1):
-            x.append((self.source_entity_id >> (8*i)) & 0xff)
+            x.append((self.source_entity_id >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         x = []
 
         for i in range(length_of_seq_number + 1):
-            x.append((self.transaction_seq_number >> (8*i)) & 0xff)
+            x.append((self.transaction_seq_number >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         self.value = data
         return super().encode()
 
 
 class RemoteSuspendResponse(ReservedMessageToUser):
-
     def __init__(
-            self, source_entity_id, transaction_seq_number,
-            suspension_indicator=1, transaction_status=0):
+        self,
+        source_entity_id,
+        transaction_seq_number,
+        suspension_indicator=1,
+        transaction_status=0,
+    ):
         super().__init__()
         self.message_type = MessageType.REMOTE_SUSPEND_RESPONSE
 
         self.suspension_indicator = suspension_indicator
         self.transaction_status = transaction_status
         self.source_entity_id = source_entity_id
         self.transaction_seq_number = transaction_seq_number
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
 
-        data += bytes([
-            (self.suspension_indicator << 7) +
-            (self.transaction_status << 5)])
+        data += bytes(
+            [(self.suspension_indicator << 7) + (self.transaction_status << 5)]
+        )
 
         length_of_entity_id = get_required_octets(self.source_entity_id) - 1
-        length_of_seq_number = get_required_octets(
-            self.transaction_seq_number) - 1
+        length_of_seq_number = get_required_octets(self.transaction_seq_number) - 1
 
-        data += bytes([
-            (0 << 7) +
-            (length_of_entity_id << 4) +
-            (0 << 3) +
-            length_of_seq_number])
+        data += bytes(
+            [(0 << 7) + (length_of_entity_id << 4) + (0 << 3) + length_of_seq_number]
+        )
 
         x = []
 
         for i in range(length_of_entity_id + 1):
-            x.append((self.source_entity_id >> (8*i)) & 0xff)
+            x.append((self.source_entity_id >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         x = []
 
         for i in range(length_of_seq_number + 1):
-            x.append((self.transaction_seq_number >> (8*i)) & 0xff)
+            x.append((self.transaction_seq_number >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         self.value = data
         return super().encode()
 
 
 class RemoteResumeRequest(ReservedMessageToUser):
-
-    def __init__(
-            self, source_entity_id, transaction_seq_number):
+    def __init__(self, source_entity_id, transaction_seq_number):
         super().__init__()
         self.message_type = MessageType.REMOTE_RESUME_REQUEST
 
         self.source_entity_id = source_entity_id
         self.transaction_seq_number = transaction_seq_number
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
 
         length_of_entity_id = get_required_octets(self.source_entity_id) - 1
 
-        length_of_seq_number = get_required_octets(
-            self.transaction_seq_number) - 1
-        data += bytes([
-            (0 << 7) +
-            (length_of_entity_id << 4) +
-            (0 << 3) +
-            length_of_seq_number])
+        length_of_seq_number = get_required_octets(self.transaction_seq_number) - 1
+        data += bytes(
+            [(0 << 7) + (length_of_entity_id << 4) + (0 << 3) + length_of_seq_number]
+        )
 
         x = []
 
         for i in range(length_of_entity_id + 1):
-            x.append((self.source_entity_id >> (8*i)) & 0xff)
+            x.append((self.source_entity_id >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
         x = []
         for i in range(length_of_seq_number + 1):
-            x.append((self.transaction_seq_number >> (8*i)) & 0xff)
+            x.append((self.transaction_seq_number >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         self.value = data
         return super().encode()
 
 
 class RemoteResumeResponse(ReservedMessageToUser):
-
     def __init__(
-            self, source_entity_id, transaction_seq_number,
-            suspension_indicator=1, transaction_status=0):
+        self,
+        source_entity_id,
+        transaction_seq_number,
+        suspension_indicator=1,
+        transaction_status=0,
+    ):
         super().__init__()
         self.message_type = MessageType.REMOTE_RESUME_RESPONSE
 
         self.suspension_indicator = suspension_indicator
         self.transaction_status = transaction_status
         self.source_entity_id = source_entity_id
         self.transaction_seq_number = transaction_seq_number
 
     def encode(self):
-        data = self.message_identifier.encode('utf-8')
+        data = self.message_identifier.encode("utf-8")
         data += bytes([self.message_type])
 
-        data += bytes([
-            (self.suspension_indicator << 7) +
-            (self.transaction_status << 5)])
+        data += bytes(
+            [(self.suspension_indicator << 7) + (self.transaction_status << 5)]
+        )
 
         length_of_entity_id = get_required_octets(self.source_entity_id) - 1
-        length_of_seq_number = get_required_octets(
-            self.transaction_seq_number) - 1
+        length_of_seq_number = get_required_octets(self.transaction_seq_number) - 1
 
-        data += bytes([
-            (0 << 7) +
-            (length_of_entity_id << 4) +
-            (0 << 3) +
-            length_of_seq_number])
+        data += bytes(
+            [(0 << 7) + (length_of_entity_id << 4) + (0 << 3) + length_of_seq_number]
+        )
 
         x = []
 
         for i in range(length_of_entity_id + 1):
-            x.append((self.source_entity_id >> (8*i)) & 0xff)
+            x.append((self.source_entity_id >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         x = []
 
         for i in range(length_of_seq_number + 1):
-            x.append((self.transaction_seq_number >> (8*i)) & 0xff)
+            x.append((self.transaction_seq_number >> (8 * i)) & 0xFF)
         x.reverse()
         data += bytes(x)
 
         self.value = data
         return super().encode()
 
 
@@ -385,141 +363,159 @@
     messages_to_user = []
     fault_handler_overrides = []
     flow_label = []
 
     while databytes:
         type = databytes[0]
         length = databytes[1]
-        data = databytes[2:2+length]
-        databytes = databytes[2+length:]
+        data = databytes[2 : 2 + length]
+        databytes = databytes[2 + length :]
 
         if type == TypeFieldCode.FILESTORE_REQUEST:
             filestore_request = extract_filestore_request(data)
             filestore_requests.append(filestore_request)
 
         if type == TypeFieldCode.MESSAGE_TO_USER:
             message_to_user = extract_message_to_user(data)
             messages_to_user.append(message_to_user)
 
-    return filestore_requests, messages_to_user,\
-        fault_handler_overrides, flow_label
+    return filestore_requests, messages_to_user, fault_handler_overrides, flow_label
 
 
 def extract_message_to_user(data):
-
-    if not data.startswith(b'cfdp'):
+    if not data.startswith(b"cfdp"):
         # non-standard user messages
         raise NotImplementedError
 
     message_type = data[4]
     data = data[5:]
 
     if message_type == MessageType.ORIGINATING_TRANSACTION_ID:
         length_of_entity_id = (data[0] >> 4) + 1
         length_of_seq_number = (data[0] & 0x0F) + 1
         source_entity_id = int.from_bytes(
-            data[2:2+length_of_entity_id], byteorder='big', signed=False)
+            data[2 : 2 + length_of_entity_id], byteorder="big", signed=False
+        )
         transaction_seq_number = int.from_bytes(
-            data[2+length_of_entity_id:], byteorder='big', signed=False)
-        return OriginatingTransactionId(
-            source_entity_id, transaction_seq_number)
+            data[2 + length_of_entity_id :], byteorder="big", signed=False
+        )
+        return OriginatingTransactionId(source_entity_id, transaction_seq_number)
 
     elif message_type == MessageType.PROXY_PUT_REQUEST:
         len_destination_entity_id = data[0]
         offset = 1
         destination_entity_id = int.from_bytes(
-            data[offset:offset+len_destination_entity_id],
-            byteorder='big', signed=False)
+            data[offset : offset + len_destination_entity_id],
+            byteorder="big",
+            signed=False,
+        )
         offset += len_destination_entity_id
         len_source_filename = data[offset]
         offset += 1
-        source_filename = data[offset:offset+len_source_filename]
+        source_filename = data[offset : offset + len_source_filename]
         offset += len_source_filename
         len_destination_filename = data[offset]
         offset += 1
-        destination_filename = data[offset:offset+len_destination_filename]
+        destination_filename = data[offset : offset + len_destination_filename]
         return ProxyPutRequest(
-            destination_entity_id, source_filename, destination_filename)
+            destination_entity_id, source_filename, destination_filename
+        )
 
     elif message_type == MessageType.PROXY_PUT_CANCEL:
         len_entity_id = data[0]
         offset = 1
         entity_id = int.from_bytes(
-            data[offset:offset+len_entity_id], byteorder='big', signed=False)
+            data[offset : offset + len_entity_id], byteorder="big", signed=False
+        )
         offset += len_entity_id
         len_seq_number = data[offset]
         offset += 1
         seq_number = int.from_bytes(
-            data[offset:offset+len_seq_number], byteorder='big', signed=False)
+            data[offset : offset + len_seq_number], byteorder="big", signed=False
+        )
         return ProxyPutCancel(entity_id, seq_number)
 
     elif message_type == MessageType.DIRECTORY_LISTING_REQUEST:
         length_of_first_filename = data[0]
-        directory_name = data[1:1+length_of_first_filename]
-        directory_file_name = data[2+length_of_first_filename:]
+        directory_name = data[1 : 1 + length_of_first_filename]
+        directory_file_name = data[2 + length_of_first_filename :]
         return DirectoryListingRequest(directory_name, directory_file_name)
 
     elif message_type == MessageType.DIRECTORY_LISTING_RESPONSE:
         listing_response_code = data[0]
         length_of_directory_name = data[1]
-        directory_name = data[2:2+length_of_directory_name]
-        directory_file_name = data[3+length_of_directory_name:]
+        directory_name = data[2 : 2 + length_of_directory_name]
+        directory_file_name = data[3 + length_of_directory_name :]
         return DirectoryListingResponse(
-            directory_name, directory_file_name, listing_response_code)
+            directory_name, directory_file_name, listing_response_code
+        )
 
     elif message_type == MessageType.REMOTE_SUSPEND_REQUEST:
         length_of_entity_id = (data[0] >> 4) + 1
         length_of_seq_number = (data[0] & 0x0F) + 1
         source_entity_id = int.from_bytes(
-            data[1:1+length_of_entity_id], byteorder='big', signed=False)
+            data[1 : 1 + length_of_entity_id], byteorder="big", signed=False
+        )
         transaction_seq_number = int.from_bytes(
-            data[1+length_of_entity_id:], byteorder='big', signed=False)
+            data[1 + length_of_entity_id :], byteorder="big", signed=False
+        )
         return RemoteSuspendRequest(source_entity_id, transaction_seq_number)
 
     elif message_type == MessageType.REMOTE_SUSPEND_RESPONSE:
-        suspension_indicator = (data[0] >> 7)
+        suspension_indicator = data[0] >> 7
         transaction_status = (data[0] >> 7) & 0x03
         length_of_entity_id = (data[1] >> 4) + 1
         length_of_seq_number = (data[1] & 0x0F) + 1
         source_entity_id = int.from_bytes(
-            data[2:2+length_of_entity_id], byteorder='big', signed=False)
+            data[2 : 2 + length_of_entity_id], byteorder="big", signed=False
+        )
         transaction_seq_number = int.from_bytes(
-            data[2+length_of_seq_number:], byteorder='big', signed=False)
+            data[2 + length_of_seq_number :], byteorder="big", signed=False
+        )
         return RemoteSuspendResponse(
-            source_entity_id, transaction_seq_number,
-            suspension_indicator, transaction_status)
+            source_entity_id,
+            transaction_seq_number,
+            suspension_indicator,
+            transaction_status,
+        )
 
     elif message_type == MessageType.REMOTE_RESUME_REQUEST:
         length_of_entity_id = (data[0] >> 4) + 1
         length_of_seq_number = (data[0] & 0x0F) + 1
         source_entity_id = int.from_bytes(
-            data[1:1+length_of_entity_id], byteorder='big', signed=False)
+            data[1 : 1 + length_of_entity_id], byteorder="big", signed=False
+        )
         transaction_seq_number = int.from_bytes(
-            data[1+length_of_entity_id:], byteorder='big', signed=False)
+            data[1 + length_of_entity_id :], byteorder="big", signed=False
+        )
         return RemoteResumeRequest(source_entity_id, transaction_seq_number)
 
     elif message_type == MessageType.REMOTE_RESUME_RESPONSE:
-        suspension_indicator = (data[0] >> 7)
+        suspension_indicator = data[0] >> 7
         transaction_status = (data[0] >> 7) & 0x03
         length_of_entity_id = (data[1] >> 4) + 1
         length_of_seq_number = (data[1] & 0x0F) + 1
         source_entity_id = int.from_bytes(
-            data[2:2+length_of_entity_id], byteorder='big', signed=False)
+            data[2 : 2 + length_of_entity_id], byteorder="big", signed=False
+        )
         transaction_seq_number = int.from_bytes(
-            data[2+length_of_seq_number:], byteorder='big', signed=False)
+            data[2 + length_of_seq_number :], byteorder="big", signed=False
+        )
         return RemoteResumeResponse(
-            source_entity_id, transaction_seq_number,
-            suspension_indicator, transaction_status)
+            source_entity_id,
+            transaction_seq_number,
+            suspension_indicator,
+            transaction_status,
+        )
 
     else:
         raise NotImplementedError
 
 
 def process_user_message(kernel, message):
-
     if isinstance(message, OriginatingTransactionId):
         pass
 
     elif isinstance(message, ProxyPutRequest):
         destination_entity_id = message.destination_entity_id
         source_filename = message.source_filename.decode()
         destination_filename = message.destination_filename.decode()
@@ -531,26 +527,29 @@
             destination_id=destination_entity_id,
             source_filename=source_filename,
             destination_filename=destination_filename,
             transmission_mode=transmission_mode,
             messages_to_user=[
                 OriginatingTransactionId(
                     source_entity_id=source_entity_id,
-                    transaction_seq_number=transaction_seq_number)])
+                    transaction_seq_number=transaction_seq_number,
+                )
+            ],
+        )
 
     elif isinstance(message, ProxyPutCancel):
         transaction_id = (message.entity_id, message.seq_number)
         kernel.cancel(transaction_id)
 
     elif isinstance(message, DirectoryListingRequest):
         dirname = message.directory_name.decode()
         listing = kernel.filestore.list_directory(dirname)
 
         filename = kernel.filestore.join_path(dirname, ".listing")
-        fh = kernel.filestore.open(filename, 'wt')
+        fh = kernel.filestore.open(filename, "wt")
         fh.write(listing)
         fh.close()
 
         # send file and directory response
         destination_id = message.originating_transaction.source_entity_id
         transmission_mode = message.originating_transaction.transmission_mode
 
@@ -563,61 +562,72 @@
             source_filename=filename,
             destination_filename=destination_filename,
             transmission_mode=transmission_mode,
             messages_to_user=[
                 DirectoryListingResponse(directory_name, destination_filename),
                 OriginatingTransactionId(
                     source_entity_id=source_entity_id,
-                    transaction_seq_number=transaction_seq_number)])
+                    transaction_seq_number=transaction_seq_number,
+                ),
+            ],
+        )
 
     elif isinstance(message, DirectoryListingResponse):
         # TODO: let user add a callback to be triggered with directory listing
         pass
 
     elif isinstance(message, RemoteSuspendRequest):
-        transaction_id = (
-            message.source_entity_id, message.transaction_seq_number)
+        transaction_id = (message.source_entity_id, message.transaction_seq_number)
         kernel.suspend(transaction_id)
         transmission_mode = message.originating_transaction.transmission_mode
         source_entity_id = message.originating_transaction.source_entity_id
         transaction_seq_number = message.originating_transaction.seq_number
         kernel.put(
             destination_id=source_entity_id,
             transmission_mode=transmission_mode,
             messages_to_user=[
                 RemoteSuspendResponse(
                     source_entity_id=message.source_entity_id,
-                    transaction_seq_number=message.transaction_seq_number),
+                    transaction_seq_number=message.transaction_seq_number,
+                ),
                 OriginatingTransactionId(
                     source_entity_id=source_entity_id,
-                    transaction_seq_number=transaction_seq_number)])
+                    transaction_seq_number=transaction_seq_number,
+                ),
+            ],
+        )
 
     elif isinstance(message, RemoteSuspendResponse):
         kernel.suspended_indication(
             (message.source_entity_id, message.transaction_seq_number),
-            message.transaction_status)
+            message.transaction_status,
+        )
 
     elif isinstance(message, RemoteResumeRequest):
-        transaction_id = (
-            message.source_entity_id, message.transaction_seq_number)
+        transaction_id = (message.source_entity_id, message.transaction_seq_number)
         kernel.resume(transaction_id)
         transmission_mode = message.originating_transaction.transmission_mode
         source_entity_id = message.originating_transaction.source_entity_id
         transaction_seq_number = message.originating_transaction.seq_number
         kernel.put(
             destination_id=source_entity_id,
             transmission_mode=transmission_mode,
             messages_to_user=[
                 RemoteResumeResponse(
                     source_entity_id=message.source_entity_id,
-                    transaction_seq_number=message.transaction_seq_number),
+                    transaction_seq_number=message.transaction_seq_number,
+                ),
                 OriginatingTransactionId(
                     source_entity_id=source_entity_id,
-                    transaction_seq_number=transaction_seq_number)])
+                    transaction_seq_number=transaction_seq_number,
+                ),
+            ],
+        )
 
     elif isinstance(message, RemoteResumeResponse):
         kernel.resumed_indication(
             (message.source_entity_id, message.transaction_seq_number),
-            message.transaction_status)
+            message.transaction_status,
+        )
 
     else:
         raise NotImplementedError
```

### Comparing `cfdp-1.1.3/src/cfdp/pdu/ack.py` & `cfdp-2.0.0/src/cfdp/pdu/ack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from cfdp.constants import DirectiveCode, PduTypeCode
 from .header import PduHeader
 
 
 class AckPdu:
-
     def __init__(
-            self,
-            # pdu header parameters
-            direction=None,
-            transmission_mode=None,
-            crc_flag=0,
-            large_file_flag=0,
-            pdu_data_field_length=None,
-            segmentation_control=0,
-            length_of_entity_ids=0,
-            segmentation_metadata_flag=0,
-            length_of_seq_number=0,
-            source_entity_id=None,
-            transaction_seq_number=None,
-            destination_entity_id=None,
-            # ack pdu parameters
-            directive_code_ack=None,
-            directive_subtype_code=None,
-            condition_code=None,
-            transaction_status=None):
+        self,
+        # pdu header parameters
+        direction=None,
+        transmission_mode=None,
+        crc_flag=0,
+        large_file_flag=0,
+        pdu_data_field_length=None,
+        segmentation_control=0,
+        length_of_entity_ids=0,
+        segmentation_metadata_flag=0,
+        length_of_seq_number=0,
+        source_entity_id=None,
+        transaction_seq_number=None,
+        destination_entity_id=None,
+        # ack pdu parameters
+        directive_code_ack=None,
+        directive_subtype_code=None,
+        condition_code=None,
+        transaction_status=None,
+    ):
         self.directive_code = DirectiveCode.ACK
         self.directive_code_ack = directive_code_ack
         self.directive_subtype_code = directive_subtype_code
         self.condition_code = condition_code
         self.transaction_status = transaction_status
 
         self.pdu_header = PduHeader(
@@ -39,33 +39,35 @@
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=segmentation_control,
             length_of_entity_ids=length_of_entity_ids,
             segmentation_metadata_flag=segmentation_metadata_flag,
             length_of_seq_number=length_of_seq_number,
             source_entity_id=source_entity_id,
             transaction_seq_number=transaction_seq_number,
-            destination_entity_id=destination_entity_id)
+            destination_entity_id=destination_entity_id,
+        )
 
     def encode(self):
-        databytes = bytes([
-            self.directive_code,
-            (self.directive_code_ack << 4) +
-            (self.directive_subtype_code),
-            (self.condition_code << 4),
-            (self.transaction_status << 6)])
+        databytes = bytes(
+            [
+                self.directive_code,
+                (self.directive_code_ack << 4) + (self.directive_subtype_code),
+                (self.condition_code << 4) + (self.transaction_status),
+            ]
+        )
 
         self.pdu_header.pdu_data_field_length = len(databytes)
         return self.pdu_header.encode() + databytes
 
     @classmethod
     def decode(cls, pdu):
-        """ ref: CCSDS 720.2-G-3 Page 2-10 """
+        """ref: CCSDS 720.2-G-3 Page 2-10"""
 
         pdu_header = PduHeader.decode(pdu)
-        pdu_data = pdu[len(pdu_header):]
+        pdu_data = pdu[len(pdu_header) :]
         pdu_data_field_length = len(pdu_data)
 
         return cls(
             # pdu header parameters
             direction=pdu_header.direction,
             transmission_mode=pdu_header.transmission_mode,
             crc_flag=pdu_header.crc_flag,
@@ -76,10 +78,11 @@
             segmentation_metadata_flag=pdu_header.segmentation_metadata_flag,
             length_of_seq_number=pdu_header.length_of_seq_number,
             source_entity_id=pdu_header.source_entity_id,
             transaction_seq_number=pdu_header.transaction_seq_number,
             destination_entity_id=pdu_header.destination_entity_id,
             # ack pdu parameters
             directive_code_ack=(pdu_data[1] >> 4),
-            directive_subtype_code=(pdu_data[1] & 0x0f),
+            directive_subtype_code=(pdu_data[1] & 0x0F),
             condition_code=(pdu_data[2] >> 4),
-            transaction_status=(pdu_data[2] & 0x03))
+            transaction_status=(pdu_data[2] & 0x03),
+        )
```

### Comparing `cfdp-1.1.3/src/cfdp/pdu/eof.py` & `cfdp-2.0.0/src/cfdp/pdu/eof.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from cfdp.constants import DirectiveCode, PduTypeCode
 from .header import PduHeader
 
 
 class EofPdu:
-
     def __init__(
-            self,
-            # pdu header parameters
-            direction=None,
-            transmission_mode=None,
-            crc_flag=0,
-            large_file_flag=0,
-            pdu_data_field_length=None,
-            segmentation_control=0,
-            length_of_entity_ids=0,
-            segmentation_metadata_flag=0,
-            length_of_seq_number=0,
-            source_entity_id=None,
-            transaction_seq_number=None,
-            destination_entity_id=None,
-            # eof pdu parameters
-            condition_code=None,
-            file_checksum=None,
-            file_size=None,
-            fault_location=None):
+        self,
+        # pdu header parameters
+        direction=None,
+        transmission_mode=None,
+        crc_flag=0,
+        large_file_flag=0,
+        pdu_data_field_length=None,
+        segmentation_control=0,
+        length_of_entity_ids=0,
+        segmentation_metadata_flag=0,
+        length_of_seq_number=0,
+        source_entity_id=None,
+        transaction_seq_number=None,
+        destination_entity_id=None,
+        # eof pdu parameters
+        condition_code=None,
+        file_checksum=None,
+        file_size=None,
+        fault_location=None,
+    ):
         self.directive_code = DirectiveCode.EOF
         self.condition_code = condition_code
         self.file_checksum = file_checksum
         self.file_size = file_size
 
         self.pdu_header = PduHeader(
             pdu_type=PduTypeCode.FILE_DIRECTIVE,
@@ -38,54 +38,66 @@
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=segmentation_control,
             length_of_entity_ids=length_of_entity_ids,
             segmentation_metadata_flag=segmentation_metadata_flag,
             length_of_seq_number=length_of_seq_number,
             source_entity_id=source_entity_id,
             transaction_seq_number=transaction_seq_number,
-            destination_entity_id=destination_entity_id)
+            destination_entity_id=destination_entity_id,
+        )
 
     def encode(self):
-        databytes = bytes([
-            self.directive_code,
-            self.condition_code << 4,
-            (self.file_checksum >> 24) & 0xff,
-            (self.file_checksum >> 16) & 0xff,
-            (self.file_checksum >> 8) & 0xff,
-            (self.file_checksum) & 0xff])
+        databytes = bytes(
+            [
+                self.directive_code,
+                self.condition_code << 4,
+                (self.file_checksum >> 24) & 0xFF,
+                (self.file_checksum >> 16) & 0xFF,
+                (self.file_checksum >> 8) & 0xFF,
+                (self.file_checksum) & 0xFF,
+            ]
+        )
 
         if not self.pdu_header.large_file_flag:
-            databytes += bytes([
-                (self.file_size >> 24) & 0xff,
-                (self.file_size >> 16) & 0xff,
-                (self.file_size >> 8) & 0xff,
-                (self.file_size) & 0xff])
+            databytes += bytes(
+                [
+                    (self.file_size >> 24) & 0xFF,
+                    (self.file_size >> 16) & 0xFF,
+                    (self.file_size >> 8) & 0xFF,
+                    (self.file_size) & 0xFF,
+                ]
+            )
         else:
-            databytes += bytes([
-                (self.file_size >> 56) & 0xff,
-                (self.file_size >> 48) & 0xff,
-                (self.file_size >> 40) & 0xff,
-                (self.file_size >> 32) & 0xff,
-                (self.file_size >> 24) & 0xff,
-                (self.file_size >> 16) & 0xff,
-                (self.file_size >> 8) & 0xff,
-                (self.file_size) & 0xff])
+            databytes += bytes(
+                [
+                    (self.file_size >> 56) & 0xFF,
+                    (self.file_size >> 48) & 0xFF,
+                    (self.file_size >> 40) & 0xFF,
+                    (self.file_size >> 32) & 0xFF,
+                    (self.file_size >> 24) & 0xFF,
+                    (self.file_size >> 16) & 0xFF,
+                    (self.file_size >> 8) & 0xFF,
+                    (self.file_size) & 0xFF,
+                ]
+            )
 
         self.pdu_header.pdu_data_field_length = len(databytes)
         return self.pdu_header.encode() + databytes
 
     @classmethod
     def decode(cls, pdu):
         pdu_header = PduHeader.decode(pdu)
-        pdu_data = pdu[len(pdu_header):]
+        pdu_data = pdu[len(pdu_header) :]
         pdu_data_field_length = len(pdu_data)
 
-        file_size = int.from_bytes(
-                pdu_data[6:10], "big") if not pdu_header.large_file_flag\
+        file_size = (
+            int.from_bytes(pdu_data[6:10], "big")
+            if not pdu_header.large_file_flag
             else int.from_bytes(pdu_data[6:14], "big")
+        )
 
         return cls(
             # pdu header parameters
             direction=pdu_header.direction,
             transmission_mode=pdu_header.transmission_mode,
             crc_flag=pdu_header.crc_flag,
             large_file_flag=pdu_header.large_file_flag,
@@ -97,8 +109,9 @@
             source_entity_id=pdu_header.source_entity_id,
             transaction_seq_number=pdu_header.transaction_seq_number,
             destination_entity_id=pdu_header.destination_entity_id,
             # eof pdu parameters
             condition_code=pdu_data[1] >> 4,
             file_checksum=int.from_bytes(pdu_data[2:6], "big"),
             file_size=file_size,
-            fault_location=None)  # not yet implemented
+            fault_location=None,
+        )  # not yet implemented
```

### Comparing `cfdp-1.1.3/src/cfdp/pdu/filedata.py` & `cfdp-2.0.0/src/cfdp/pdu/filedata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from cfdp.constants import PduTypeCode
 from .header import PduHeader
 
 
 class FiledataPdu:
-
     def __init__(
-            self,
-            # pdu header parameters
-            direction=None,
-            transmission_mode=None,
-            crc_flag=0,
-            large_file_flag=0,
-            pdu_data_field_length=None,
-            segmentation_control=0,
-            length_of_entity_ids=0,
-            segmentation_metadata_flag=0,
-            length_of_seq_number=0,
-            source_entity_id=None,
-            transaction_seq_number=None,
-            destination_entity_id=None,
-            # filedata pdu parameters
-            record_continuation_state=None,
-            segment_metadata_length=None,
-            segment_metadata=None,
-            segment_offset=None,
-            file_data=None):
+        self,
+        # pdu header parameters
+        direction=None,
+        transmission_mode=None,
+        crc_flag=0,
+        large_file_flag=0,
+        pdu_data_field_length=None,
+        segmentation_control=0,
+        length_of_entity_ids=0,
+        segmentation_metadata_flag=0,
+        length_of_seq_number=0,
+        source_entity_id=None,
+        transaction_seq_number=None,
+        destination_entity_id=None,
+        # filedata pdu parameters
+        record_continuation_state=None,
+        segment_metadata_length=None,
+        segment_metadata=None,
+        segment_offset=None,
+        file_data=None,
+    ):
         if None in [segment_offset, file_data]:
             raise Exception("Must provide all required parameters")
 
         self.segment_offset = segment_offset
         self.file_data = file_data
 
         self.pdu_header = PduHeader(
@@ -40,32 +40,36 @@
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=segmentation_control,
             length_of_entity_ids=length_of_entity_ids,
             segmentation_metadata_flag=segmentation_metadata_flag,
             length_of_seq_number=length_of_seq_number,
             source_entity_id=source_entity_id,
             transaction_seq_number=transaction_seq_number,
-            destination_entity_id=destination_entity_id)
+            destination_entity_id=destination_entity_id,
+        )
 
     def encode(self):
         if self.pdu_header.segmentation_metadata_flag:
             raise NotImplementedError
-        databytes = bytes([
-            (self.segment_offset >> 24) & 0xff,
-            (self.segment_offset >> 16) & 0xff,
-            (self.segment_offset >> 8) & 0xff,
-            (self.segment_offset) & 0xff])
+        databytes = bytes(
+            [
+                (self.segment_offset >> 24) & 0xFF,
+                (self.segment_offset >> 16) & 0xFF,
+                (self.segment_offset >> 8) & 0xFF,
+                (self.segment_offset) & 0xFF,
+            ]
+        )
         databytes += self.file_data
         self.pdu_header.pdu_data_field_length = len(databytes)
         return self.pdu_header.encode() + databytes
 
     @classmethod
     def decode(cls, pdu):
         pdu_header = PduHeader.decode(pdu)
-        pdu_data = pdu[len(pdu_header):]
+        pdu_data = pdu[len(pdu_header) :]
         pdu_data_field_length = len(pdu_data)
 
         return cls(
             # pdu header parameters
             direction=pdu_header.direction,
             transmission_mode=pdu_header.transmission_mode,
             crc_flag=pdu_header.crc_flag,
@@ -76,8 +80,9 @@
             segmentation_metadata_flag=pdu_header.segmentation_metadata_flag,
             length_of_seq_number=pdu_header.length_of_seq_number,
             source_entity_id=pdu_header.source_entity_id,
             transaction_seq_number=pdu_header.transaction_seq_number,
             destination_entity_id=pdu_header.destination_entity_id,
             # filedata pdu parameters
             segment_offset=int.from_bytes(pdu_data[0:4], "big"),
-            file_data=pdu_data[4:])
+            file_data=pdu_data[4:],
+        )
```

### Comparing `cfdp-1.1.3/src/cfdp/pdu/finished.py` & `cfdp-2.0.0/src/cfdp/pdu/finished.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from cfdp.constants import DirectiveCode, PduTypeCode
 from .header import PduHeader
 
 
 class FinishedPdu:
-
     def __init__(
-            self,
-            # pdu header parameters
-            direction=None,
-            transmission_mode=None,
-            crc_flag=0,
-            large_file_flag=0,
-            pdu_data_field_length=None,
-            segmentation_control=0,
-            length_of_entity_ids=0,
-            segmentation_metadata_flag=0,
-            length_of_seq_number=0,
-            source_entity_id=None,
-            transaction_seq_number=None,
-            destination_entity_id=None,
-            # finished pdu parameters
-            condition_code=None,
-            delivery_code=None,
-            file_status=None,
-            filestore_responses=None,
-            fault_location=None):
+        self,
+        # pdu header parameters
+        direction=None,
+        transmission_mode=None,
+        crc_flag=0,
+        large_file_flag=0,
+        pdu_data_field_length=None,
+        segmentation_control=0,
+        length_of_entity_ids=0,
+        segmentation_metadata_flag=0,
+        length_of_seq_number=0,
+        source_entity_id=None,
+        transaction_seq_number=None,
+        destination_entity_id=None,
+        # finished pdu parameters
+        condition_code=None,
+        delivery_code=None,
+        file_status=None,
+        filestore_responses=None,
+        fault_location=None,
+    ):
         self.directive_code = DirectiveCode.FINISHED
         self.condition_code = condition_code
         self.delivery_code = delivery_code
         self.file_status = file_status
         self.filestore_responses = filestore_responses
 
         self.pdu_header = PduHeader(
@@ -40,39 +40,42 @@
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=segmentation_control,
             length_of_entity_ids=length_of_entity_ids,
             segmentation_metadata_flag=segmentation_metadata_flag,
             length_of_seq_number=length_of_seq_number,
             source_entity_id=source_entity_id,
             transaction_seq_number=transaction_seq_number,
-            destination_entity_id=destination_entity_id)
+            destination_entity_id=destination_entity_id,
+        )
 
     def encode(self):
-
-        databytes = bytes([
-            (self.directive_code),
-            (self.condition_code << 4) +
-            (1 << 3) +  # end system status must be 1
-            (self.delivery_code << 2) +
-            (self.file_status)])
+        databytes = bytes(
+            [
+                (self.directive_code),
+                (self.condition_code << 4)
+                + (1 << 3)
+                + (self.delivery_code << 2)  # end system status must be 1
+                + (self.file_status),
+            ]
+        )
 
         if self.filestore_responses:
             for filestore_responses in self.filestore_responses:
                 databytes += filestore_responses.encode()
             raise NotImplementedError
 
         self.pdu_header.pdu_data_field_length = len(databytes)
         return self.pdu_header.encode() + databytes
 
     @classmethod
     def decode(cls, pdu):
-        """ ref: CCSDS 720.2-G-3 Page 2-9 """
+        """ref: CCSDS 720.2-G-3 Page 2-9"""
 
         pdu_header = PduHeader.decode(pdu)
-        pdu_data = pdu[len(pdu_header):]
+        pdu_data = pdu[len(pdu_header) :]
         pdu_data_field_length = len(pdu_data)
 
         return cls(
             # pdu header parameters
             direction=pdu_header.direction,
             transmission_mode=pdu_header.transmission_mode,
             crc_flag=pdu_header.crc_flag,
@@ -86,8 +89,9 @@
             transaction_seq_number=pdu_header.transaction_seq_number,
             destination_entity_id=pdu_header.destination_entity_id,
             # finished pdu parameters
             condition_code=pdu_data[1] >> 4,
             delivery_code=(pdu_data[1] >> 2) & 0x01,
             file_status=pdu_data[1] & 0x03,
             filestore_responses=0,  # TODO
-            fault_location=None)
+            fault_location=None,
+        )
```

### Comparing `cfdp-1.1.3/src/cfdp/pdu/header.py` & `cfdp-2.0.0/src/cfdp/pdu/header.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from cfdp.meta import get_required_octets
 
 
 CFDP_PROTOCOL_VERSION = 1
 
 
 class PduHeader:
-
     def __init__(
-            self,
-            pdu_type=None,
-            direction=None,
-            transmission_mode=None,
-            crc_flag=0,
-            large_file_flag=0,
-            pdu_data_field_length=None,
-            segmentation_control=0,
-            length_of_entity_ids=0,
-            segmentation_metadata_flag=0,
-            length_of_seq_number=0,
-            source_entity_id=None,
-            transaction_seq_number=None,
-            destination_entity_id=None):
-
+        self,
+        pdu_type=None,
+        direction=None,
+        transmission_mode=None,
+        crc_flag=0,
+        large_file_flag=0,
+        pdu_data_field_length=None,
+        segmentation_control=0,
+        length_of_entity_ids=0,
+        segmentation_metadata_flag=0,
+        length_of_seq_number=0,
+        source_entity_id=None,
+        transaction_seq_number=None,
+        destination_entity_id=None,
+    ):
         if None in [
-                pdu_type, direction, transmission_mode, source_entity_id,
-                transaction_seq_number, destination_entity_id]:
+            pdu_type,
+            direction,
+            transmission_mode,
+            source_entity_id,
+            transaction_seq_number,
+            destination_entity_id,
+        ]:
             raise Exception("Must provide all required parameters")
 
         self.version = CFDP_PROTOCOL_VERSION
         self.pdu_type = pdu_type
         self.direction = direction
         self.transmission_mode = transmission_mode
         self.crc_flag = crc_flag
@@ -44,47 +48,49 @@
 
     def encode(self):
         if self.pdu_data_field_length is None:
             raise ValueError("PDU data field length not defined")
 
         self.length_of_entity_ids = max(
             get_required_octets(self.source_entity_id) - 1,
-            get_required_octets(self.destination_entity_id) - 1)
+            get_required_octets(self.destination_entity_id) - 1,
+        )
 
-        databytes = bytes([
-            (self.version << 5) +
-            (self.pdu_type << 4) +
-            (self.direction << 3) +
-            (self.transmission_mode << 2) +
-            (self.crc_flag << 1) +
-            (self.large_file_flag),
-
-            (self.pdu_data_field_length >> 8),
-            (self.pdu_data_field_length & 0xff),
-
-            (self.segmentation_control << 7) +
-            (self.length_of_entity_ids << 4) +
-            (self.segmentation_metadata_flag << 3) +
-            self.length_of_seq_number])
+        databytes = bytes(
+            [
+                (self.version << 5)
+                + (self.pdu_type << 4)
+                + (self.direction << 3)
+                + (self.transmission_mode << 2)
+                + (self.crc_flag << 1)
+                + (self.large_file_flag),
+                (self.pdu_data_field_length >> 8),
+                (self.pdu_data_field_length & 0xFF),
+                (self.segmentation_control << 7)
+                + (self.length_of_entity_ids << 4)
+                + (self.segmentation_metadata_flag << 3)
+                + self.length_of_seq_number,
+            ]
+        )
 
         x = []
         for i in range(self.length_of_entity_ids + 1):
-            x.append((self.source_entity_id >> (8*i)) & 0xff)
+            x.append((self.source_entity_id >> (8 * i)) & 0xFF)
         x.reverse()
         databytes += bytes(x)
 
         x = []
         for i in range(self.length_of_seq_number + 1):
-            x.append((self.transaction_seq_number >> (8*i)) & 0xff)
+            x.append((self.transaction_seq_number >> (8 * i)) & 0xFF)
         x.reverse()
         databytes += bytes(x)
 
         x = []
         for i in range(self.length_of_entity_ids + 1):
-            x.append((self.destination_entity_id >> (8*i)) & 0xff)
+            x.append((self.destination_entity_id >> (8 * i)) & 0xFF)
         x.reverse()
         databytes += bytes(x)
 
         return databytes
 
     def __len__(self):
         entity_id_field_length = 2 * (self.length_of_entity_ids + 1)
@@ -93,27 +99,38 @@
 
     @classmethod
     def decode(cls, pdu):
         pdu_data_field_length = int.from_bytes(pdu[1:3], "big")
         length_of_entity_ids = (pdu[3] >> 4) & 0x07
         length_of_seq_number = pdu[3] & 0x07
 
-        fixed_pdu_end = 32 + (2 * (8 + 8 * length_of_entity_ids))\
-            + (8 + 8 * length_of_seq_number)
-        fixed_pdu_end = 32 + (2 * (8 + 8 * length_of_entity_ids))\
-            + (8 + 8 * length_of_seq_number)
-        source_entity_id = int.from_bytes(pdu[
-            4:(32 + (8 + 8 * length_of_entity_ids))//8], "big")
-        transaction_seq_number = int.from_bytes(pdu[
-            (32 + (8 + 8 * length_of_entity_ids))//8:
-            (32 + (8 + 8 * length_of_entity_ids)
-                + (8 + 8 * length_of_seq_number))//8], "big")
-        destination_entity_id = int.from_bytes(pdu[
-            (32 + (8 + 8 * length_of_entity_ids)
-                + (8 + 8 * length_of_seq_number))//8:fixed_pdu_end//8], "big")
+        fixed_pdu_end = (
+            32 + (2 * (8 + 8 * length_of_entity_ids)) + (8 + 8 * length_of_seq_number)
+        )
+        source_entity_id = int.from_bytes(
+            pdu[4 : (32 + (8 + 8 * length_of_entity_ids)) // 8], "big"
+        )
+        transaction_seq_number = int.from_bytes(
+            pdu[
+                (32 + (8 + 8 * length_of_entity_ids))
+                // 8 : (
+                    32 + (8 + 8 * length_of_entity_ids) + (8 + 8 * length_of_seq_number)
+                )
+                // 8
+            ],
+            "big",
+        )
+        destination_entity_id = int.from_bytes(
+            pdu[
+                (32 + (8 + 8 * length_of_entity_ids) + (8 + 8 * length_of_seq_number))
+                // 8 : fixed_pdu_end
+                // 8
+            ],
+            "big",
+        )
 
         crc_flag = (pdu[0] >> 1) & 0x01
         if crc_flag:
             # TODO
             raise ValueError("PDUs with CRC are not yet supported")
 
         return cls(
@@ -125,8 +142,9 @@
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=(pdu[3] >> 7) & 0x01,
             length_of_entity_ids=length_of_entity_ids,
             segmentation_metadata_flag=(pdu[3] >> 3) & 0x01,
             length_of_seq_number=length_of_seq_number,
             source_entity_id=source_entity_id,
             transaction_seq_number=transaction_seq_number,
-            destination_entity_id=destination_entity_id)
+            destination_entity_id=destination_entity_id,
+        )
```

### Comparing `cfdp-1.1.3/src/cfdp/pdu/keep_alive.py` & `cfdp-2.0.0/src/cfdp/pdu/prompt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,73 @@
 from cfdp.constants import DirectiveCode, PduTypeCode
 from .header import PduHeader
 
 
-class KeepAlivePdu:
-
+class PromptPdu:
     def __init__(
-            self,
-            # pdu header parameters
-            direction=None,
-            transmission_mode=None,
-            crc_flag=0,
-            large_file_flag=0,
-            pdu_data_field_length=None,
-            segmentation_control=0,
-            length_of_entity_ids=0,
-            segmentation_metadata_flag=0,
-            length_of_seq_number=0,
-            source_entity_id=None,
-            transaction_seq_number=None,
-            destination_entity_id=None,
-            # keep alive pdu parameters
-            progress=None):
-        self.directive_code = DirectiveCode.KEEP_ALIVE
-        self.progress = progress
+        self,
+        # pdu header parameters
+        direction=None,
+        transmission_mode=None,
+        crc_flag=0,
+        large_file_flag=0,
+        pdu_data_field_length=None,
+        segmentation_control=0,
+        length_of_entity_ids=0,
+        segmentation_metadata_flag=0,
+        length_of_seq_number=0,
+        source_entity_id=None,
+        transaction_seq_number=None,
+        destination_entity_id=None,
+        # ack pdu parameters
+        response_required=None,
+    ):
+        self.directive_code = DirectiveCode.PROMPT
+        self.response_required = response_required
 
         self.pdu_header = PduHeader(
             pdu_type=PduTypeCode.FILE_DIRECTIVE,
             direction=direction,
             transmission_mode=transmission_mode,
             crc_flag=crc_flag,
             large_file_flag=large_file_flag,
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=segmentation_control,
             length_of_entity_ids=length_of_entity_ids,
             segmentation_metadata_flag=segmentation_metadata_flag,
             length_of_seq_number=length_of_seq_number,
             source_entity_id=source_entity_id,
             transaction_seq_number=transaction_seq_number,
-            destination_entity_id=destination_entity_id)
+            destination_entity_id=destination_entity_id,
+        )
 
     def encode(self):
-
-        databytes = bytes([self.directive_code])
-
-        if not self.pdu_header.large_file_flag:
-            databytes += bytes([
-                (self.progress >> 24) & 0xff,
-                (self.progress >> 16) & 0xff,
-                (self.progress >> 8) & 0xff,
-                (self.progress) & 0xff])
-
-        else:
-
-            databytes += bytes([
-                (self.progress >> 56) & 0xff,
-                (self.progress >> 48) & 0xff,
-                (self.progress >> 40) & 0xff,
-                (self.progress >> 32) & 0xff,
-                (self.progress >> 24) & 0xff,
-                (self.progress >> 16) & 0xff,
-                (self.progress >> 8) & 0xff,
-                (self.progress) & 0xff])
+        databytes = bytes([self.directive_code, (self.response_required << 7) & 0xFF])
 
         self.pdu_header.pdu_data_field_length = len(databytes)
         return self.pdu_header.encode() + databytes
 
     @classmethod
     def decode(cls, pdu):
-        """ ref: CCSDS 720.2-G-3 Page 2-12 """
+        """ref: CCSDS 720.2-G-3 Page 2-11"""
 
         pdu_header = PduHeader.decode(pdu)
-        pdu_data = pdu[len(pdu_header):]
+        pdu_data = pdu[len(pdu_header) :]
         pdu_data_field_length = len(pdu_data)
 
-        progress = int.from_bytes(
-            pdu_data[1:5], "big") if not pdu_header.large_file_flag\
-            else int.from_bytes(pdu_data[1:9], "big")
-
         return cls(
             # pdu header parameters
             direction=pdu_header.direction,
             transmission_mode=pdu_header.transmission_mode,
             crc_flag=pdu_header.crc_flag,
             large_file_flag=pdu_header.large_file_flag,
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=pdu_header.segmentation_control,
             length_of_entity_ids=pdu_header.length_of_entity_ids,
             segmentation_metadata_flag=pdu_header.segmentation_metadata_flag,
             length_of_seq_number=pdu_header.length_of_seq_number,
             source_entity_id=pdu_header.source_entity_id,
             transaction_seq_number=pdu_header.transaction_seq_number,
             destination_entity_id=pdu_header.destination_entity_id,
-            # keep alive pdu parameters
-            progress=progress)
+            # prompt pdu parameters
+            response_required=pdu_data[1] >> 7,
+        )
```

### Comparing `cfdp-1.1.3/src/cfdp/pdu/metadata.py` & `cfdp-2.0.0/src/cfdp/pdu/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from cfdp.constants import DirectiveCode, PduTypeCode
 from cfdp.meta import extract_metadata_options
 from .header import PduHeader
 
 
 class MetadataPdu:
-
     def __init__(
-            self,
-            # pdu header parameters
-            direction=None,
-            transmission_mode=None,
-            crc_flag=0,
-            large_file_flag=0,
-            pdu_data_field_length=None,
-            segmentation_control=0,
-            length_of_entity_ids=0,
-            segmentation_metadata_flag=0,
-            length_of_seq_number=0,
-            source_entity_id=None,
-            transaction_seq_number=None,
-            destination_entity_id=None,
-            # metadata pdu parameters
-            closure_requested=0,
-            checksum_type=0,
-            file_size=None,
-            source_filename=None,
-            destination_filename=None,
-            filestore_requests=None,
-            messages_to_user=None,
-            fault_handler_overrides=None,
-            flow_label=None):
-
+        self,
+        # pdu header parameters
+        direction=None,
+        transmission_mode=None,
+        crc_flag=0,
+        large_file_flag=0,
+        pdu_data_field_length=None,
+        segmentation_control=0,
+        length_of_entity_ids=0,
+        segmentation_metadata_flag=0,
+        length_of_seq_number=0,
+        source_entity_id=None,
+        transaction_seq_number=None,
+        destination_entity_id=None,
+        # metadata pdu parameters
+        closure_requested=0,
+        checksum_type=0,
+        file_size=None,
+        source_filename=None,
+        destination_filename=None,
+        filestore_requests=None,
+        messages_to_user=None,
+        fault_handler_overrides=None,
+        flow_label=None,
+    ):
         self.directive_code = DirectiveCode.METADATA
         self.closure_requested = closure_requested
         self.checksum_type = checksum_type
         self.file_size = file_size
         self.source_filename = source_filename
         self.destination_filename = destination_filename
         self.filestore_requests = filestore_requests
@@ -51,52 +50,61 @@
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=segmentation_control,
             length_of_entity_ids=length_of_entity_ids,
             segmentation_metadata_flag=segmentation_metadata_flag,
             length_of_seq_number=length_of_seq_number,
             source_entity_id=source_entity_id,
             transaction_seq_number=transaction_seq_number,
-            destination_entity_id=destination_entity_id)
+            destination_entity_id=destination_entity_id,
+        )
 
     def encode(self):
-
-        databytes = bytes([
-            self.directive_code,
-            (0 << 7) +
-            (self.closure_requested << 6) +
-            (0 << 4) +
-            self.checksum_type])
+        databytes = bytes(
+            [
+                self.directive_code,
+                (0 << 7)
+                + (self.closure_requested << 6)
+                + (0 << 4)
+                + self.checksum_type,
+            ]
+        )
 
         if not self.pdu_header.large_file_flag:
-            databytes += bytes([
-                (self.file_size >> 24) & 0xff,
-                (self.file_size >> 16) & 0xff,
-                (self.file_size >> 8) & 0xff,
-                (self.file_size) & 0xff])
+            databytes += bytes(
+                [
+                    (self.file_size >> 24) & 0xFF,
+                    (self.file_size >> 16) & 0xFF,
+                    (self.file_size >> 8) & 0xFF,
+                    (self.file_size) & 0xFF,
+                ]
+            )
 
         else:
-            databytes += bytes([
-                (self.file_size >> 56) & 0xff,
-                (self.file_size >> 48) & 0xff,
-                (self.file_size >> 40) & 0xff,
-                (self.file_size >> 32) & 0xff,
-                (self.file_size >> 24) & 0xff,
-                (self.file_size >> 16) & 0xff,
-                (self.file_size >> 8) & 0xff,
-                (self.file_size) & 0xff])
+            databytes += bytes(
+                [
+                    (self.file_size >> 56) & 0xFF,
+                    (self.file_size >> 48) & 0xFF,
+                    (self.file_size >> 40) & 0xFF,
+                    (self.file_size >> 32) & 0xFF,
+                    (self.file_size >> 24) & 0xFF,
+                    (self.file_size >> 16) & 0xFF,
+                    (self.file_size >> 8) & 0xFF,
+                    (self.file_size) & 0xFF,
+                ]
+            )
 
         if self.source_filename:
-            value = self.source_filename.encode('utf-8')
+            value = self.source_filename.encode("utf-8")
             length = len(value)
             databytes += bytes([length])
             databytes += value
         else:
             databytes += bytes([0])
         if self.destination_filename:
-            value = self.destination_filename.encode('utf-8')
+            value = self.destination_filename.encode("utf-8")
             length = len(value)
             databytes += bytes([length])
             databytes += value
         else:
             databytes += bytes([0])
 
         if self.filestore_requests:
@@ -114,57 +122,66 @@
             raise NotImplementedError
 
         self.pdu_header.pdu_data_field_length = len(databytes)
         return self.pdu_header.encode() + databytes
 
     @classmethod
     def decode(cls, pdu):
-        """ ref: CCSDS 720.2-G-3 Page 2-6 """
+        """ref: CCSDS 720.2-G-3 Page 2-6"""
 
         pdu_header = PduHeader.decode(pdu)
-        pdu_data = pdu[len(pdu_header):]
+        pdu_data = pdu[len(pdu_header) :]
         pdu_data_field_length = len(pdu_data)
 
         offset = 9
 
         closure_requested = pdu_data[1] >> 6
 
         offset += 3
-        checksum_type = (pdu_data[offset//8] & 0x0f)
+        checksum_type = pdu_data[offset // 8] & 0x0F
 
         offset += 4
         if pdu_header.large_file_flag:
             file_size = int.from_bytes(
-                pdu_data[offset//8:(offset+64)//8], "big")
+                pdu_data[offset // 8 : (offset + 64) // 8], "big"
+            )
             offset += 64
         else:
             file_size = int.from_bytes(
-                pdu_data[offset//8:(offset+32)//8], "big")
+                pdu_data[offset // 8 : (offset + 32) // 8], "big"
+            )
             offset += 32
 
         length_of_source_filename = int.from_bytes(
-            pdu_data[offset//8:(offset+8)//8], "big")
+            pdu_data[offset // 8 : (offset + 8) // 8], "big"
+        )
 
         offset += 8
         source_filenname = pdu_data[
-            offset//8:(offset + 8 * length_of_source_filename)//8]
+            offset // 8 : (offset + 8 * length_of_source_filename) // 8
+        ]
 
         offset += 8 * length_of_source_filename
         length_of_destination_filename = int.from_bytes(
-            pdu_data[offset//8:(offset+8)//8], "big")
+            pdu_data[offset // 8 : (offset + 8) // 8], "big"
+        )
 
         offset += 8
         destination_filename = pdu_data[
-            offset//8:(offset + 8 * length_of_destination_filename)//8]
+            offset // 8 : (offset + 8 * length_of_destination_filename) // 8
+        ]
 
         offset += 8 * length_of_destination_filename
 
-        filestore_requests, messages_to_user, fault_handler_overrides,\
-            flow_label = extract_metadata_options(
-                pdu_data[offset//8:])
+        (
+            filestore_requests,
+            messages_to_user,
+            fault_handler_overrides,
+            flow_label,
+        ) = extract_metadata_options(pdu_data[offset // 8 :])
 
         return cls(
             # pdu header parameters
             direction=pdu_header.direction,
             transmission_mode=pdu_header.transmission_mode,
             crc_flag=pdu_header.crc_flag,
             large_file_flag=pdu_header.large_file_flag,
@@ -181,8 +198,9 @@
             checksum_type=checksum_type,
             file_size=file_size,
             source_filename=source_filenname.decode(),
             destination_filename=destination_filename.decode(),
             filestore_requests=filestore_requests,
             messages_to_user=messages_to_user,
             fault_handler_overrides=fault_handler_overrides,
-            flow_label=flow_label)
+            flow_label=flow_label,
+        )
```

### Comparing `cfdp-1.1.3/src/cfdp/pdu/nak.py` & `cfdp-2.0.0/src/cfdp/pdu/nak.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from cfdp.constants import DirectiveCode, PduTypeCode
 from .header import PduHeader
 
 
 class NakPdu:
-
     def __init__(
-            self,
-            # pdu header parameters
-            direction=None,
-            transmission_mode=None,
-            crc_flag=0,
-            large_file_flag=0,
-            pdu_data_field_length=None,
-            segmentation_control=0,
-            length_of_entity_ids=0,
-            segmentation_metadata_flag=0,
-            length_of_seq_number=0,
-            source_entity_id=None,
-            transaction_seq_number=None,
-            destination_entity_id=None,
-            # nak pdu parameters
-            start_of_scope=None,
-            end_of_scope=None,
-            segment_requests=None):
+        self,
+        # pdu header parameters
+        direction=None,
+        transmission_mode=None,
+        crc_flag=0,
+        large_file_flag=0,
+        pdu_data_field_length=None,
+        segmentation_control=0,
+        length_of_entity_ids=0,
+        segmentation_metadata_flag=0,
+        length_of_seq_number=0,
+        source_entity_id=None,
+        transaction_seq_number=None,
+        destination_entity_id=None,
+        # nak pdu parameters
+        start_of_scope=None,
+        end_of_scope=None,
+        segment_requests=None,
+    ):
         self.directive_code = DirectiveCode.NAK
         self.start_of_scope = start_of_scope
         self.end_of_scope = end_of_scope
         self.segment_requests = segment_requests
 
         self.pdu_header = PduHeader(
             pdu_type=PduTypeCode.FILE_DIRECTIVE,
@@ -37,144 +37,167 @@
             pdu_data_field_length=pdu_data_field_length,
             segmentation_control=segmentation_control,
             length_of_entity_ids=length_of_entity_ids,
             segmentation_metadata_flag=segmentation_metadata_flag,
             length_of_seq_number=length_of_seq_number,
             source_entity_id=source_entity_id,
             transaction_seq_number=transaction_seq_number,
-            destination_entity_id=destination_entity_id)
+            destination_entity_id=destination_entity_id,
+        )
 
     def encode(self):
-
         databytes = bytes([self.directive_code])
         if not self.pdu_header.large_file_flag:
-
-            databytes += bytes([
-                (self.start_of_scope >> 24) & 0xff,
-                (self.start_of_scope >> 16) & 0xff,
-                (self.start_of_scope >> 8) & 0xff,
-                (self.start_of_scope) & 0xff])
+            databytes += bytes(
+                [
+                    (self.start_of_scope >> 24) & 0xFF,
+                    (self.start_of_scope >> 16) & 0xFF,
+                    (self.start_of_scope >> 8) & 0xFF,
+                    (self.start_of_scope) & 0xFF,
+                ]
+            )
 
         else:
-
-            databytes += bytes([
-                (self.start_of_scope >> 56) & 0xff,
-                (self.start_of_scope >> 48) & 0xff,
-                (self.start_of_scope >> 40) & 0xff,
-                (self.start_of_scope >> 32) & 0xff,
-                (self.start_of_scope >> 24) & 0xff,
-                (self.start_of_scope >> 16) & 0xff,
-                (self.start_of_scope >> 8) & 0xff,
-                (self.start_of_scope) & 0xff])
+            databytes += bytes(
+                [
+                    (self.start_of_scope >> 56) & 0xFF,
+                    (self.start_of_scope >> 48) & 0xFF,
+                    (self.start_of_scope >> 40) & 0xFF,
+                    (self.start_of_scope >> 32) & 0xFF,
+                    (self.start_of_scope >> 24) & 0xFF,
+                    (self.start_of_scope >> 16) & 0xFF,
+                    (self.start_of_scope >> 8) & 0xFF,
+                    (self.start_of_scope) & 0xFF,
+                ]
+            )
 
         if not self.pdu_header.large_file_flag:
-
-            databytes += bytes([
-                (self.end_of_scope >> 24) & 0xff,
-                (self.end_of_scope >> 16) & 0xff,
-                (self.end_of_scope >> 8) & 0xff,
-                (self.end_of_scope) & 0xff])
+            databytes += bytes(
+                [
+                    (self.end_of_scope >> 24) & 0xFF,
+                    (self.end_of_scope >> 16) & 0xFF,
+                    (self.end_of_scope >> 8) & 0xFF,
+                    (self.end_of_scope) & 0xFF,
+                ]
+            )
 
         else:
-
-            databytes += bytes([
-                (self.end_of_scope >> 56) & 0xff,
-                (self.end_of_scope >> 48) & 0xff,
-                (self.end_of_scope >> 40) & 0xff,
-                (self.end_of_scope >> 32) & 0xff,
-                (self.end_of_scope >> 24) & 0xff,
-                (self.end_of_scope >> 16) & 0xff,
-                (self.end_of_scope >> 8) & 0xff,
-                (self.end_of_scope) & 0xff])
+            databytes += bytes(
+                [
+                    (self.end_of_scope >> 56) & 0xFF,
+                    (self.end_of_scope >> 48) & 0xFF,
+                    (self.end_of_scope >> 40) & 0xFF,
+                    (self.end_of_scope >> 32) & 0xFF,
+                    (self.end_of_scope >> 24) & 0xFF,
+                    (self.end_of_scope >> 16) & 0xFF,
+                    (self.end_of_scope >> 8) & 0xFF,
+                    (self.end_of_scope) & 0xFF,
+                ]
+            )
 
         if self.segment_requests:
             for start_offset, end_offset in self.segment_requests:
-
                 if not self.pdu_header.large_file_flag:
-
-                    databytes += bytes([
-                        (start_offset >> 24) & 0xff,
-                        (start_offset >> 16) & 0xff,
-                        (start_offset >> 8) & 0xff,
-                        (start_offset) & 0xff])
+                    databytes += bytes(
+                        [
+                            (start_offset >> 24) & 0xFF,
+                            (start_offset >> 16) & 0xFF,
+                            (start_offset >> 8) & 0xFF,
+                            (start_offset) & 0xFF,
+                        ]
+                    )
 
                 else:
-
-                    databytes += bytes([
-                        (start_offset >> 56) & 0xff,
-                        (start_offset >> 48) & 0xff,
-                        (start_offset >> 40) & 0xff,
-                        (start_offset >> 32) & 0xff,
-                        (start_offset >> 24) & 0xff,
-                        (start_offset >> 16) & 0xff,
-                        (start_offset >> 8) & 0xff,
-                        (start_offset) & 0xff])
+                    databytes += bytes(
+                        [
+                            (start_offset >> 56) & 0xFF,
+                            (start_offset >> 48) & 0xFF,
+                            (start_offset >> 40) & 0xFF,
+                            (start_offset >> 32) & 0xFF,
+                            (start_offset >> 24) & 0xFF,
+                            (start_offset >> 16) & 0xFF,
+                            (start_offset >> 8) & 0xFF,
+                            (start_offset) & 0xFF,
+                        ]
+                    )
 
                 if not self.pdu_header.large_file_flag:
-
-                    databytes += bytes([
-                        (end_offset >> 24) & 0xff,
-                        (end_offset >> 16) & 0xff,
-                        (end_offset >> 8) & 0xff,
-                        (end_offset) & 0xff])
+                    databytes += bytes(
+                        [
+                            (end_offset >> 24) & 0xFF,
+                            (end_offset >> 16) & 0xFF,
+                            (end_offset >> 8) & 0xFF,
+                            (end_offset) & 0xFF,
+                        ]
+                    )
 
                 else:
-
-                    databytes += bytes([
-                        (end_offset >> 56) & 0xff,
-                        (end_offset >> 48) & 0xff,
-                        (end_offset >> 40) & 0xff,
-                        (end_offset >> 32) & 0xff,
-                        (end_offset >> 24) & 0xff,
-                        (end_offset >> 16) & 0xff,
-                        (end_offset >> 8) & 0xff,
-                        (end_offset) & 0xff])
+                    databytes += bytes(
+                        [
+                            (end_offset >> 56) & 0xFF,
+                            (end_offset >> 48) & 0xFF,
+                            (end_offset >> 40) & 0xFF,
+                            (end_offset >> 32) & 0xFF,
+                            (end_offset >> 24) & 0xFF,
+                            (end_offset >> 16) & 0xFF,
+                            (end_offset >> 8) & 0xFF,
+                            (end_offset) & 0xFF,
+                        ]
+                    )
 
         self.pdu_header.pdu_data_field_length = len(databytes)
         return self.pdu_header.encode() + databytes
 
     @classmethod
     def decode(cls, pdu):
-        """ ref: CCSDS 720.2-G-3 Page 2-7 """
+        """ref: CCSDS 720.2-G-3 Page 2-7"""
 
         pdu_header = PduHeader.decode(pdu)
-        pdu_data = pdu[len(pdu_header):]
+        pdu_data = pdu[len(pdu_header) :]
         pdu_data_field_length = len(pdu_data)
 
         offset = 8
         if pdu_header.large_file_flag:
             start_of_scope = int.from_bytes(
-                pdu_data[offset//8:(offset+64)//8], "big")
+                pdu_data[offset // 8 : (offset + 64) // 8], "big"
+            )
             offset += 64
             end_of_scope = int.from_bytes(
-                pdu_data[offset//8:(offset+64)//8], "big")
+                pdu_data[offset // 8 : (offset + 64) // 8], "big"
+            )
             offset += 64
         else:
             start_of_scope = int.from_bytes(
-                pdu_data[offset//8:(offset+32)//8], "big")
+                pdu_data[offset // 8 : (offset + 32) // 8], "big"
+            )
             offset += 32
             end_of_scope = int.from_bytes(
-                pdu_data[offset//8:(offset+32)//8], "big")
+                pdu_data[offset // 8 : (offset + 32) // 8], "big"
+            )
             offset += 32
 
         segment_requests = []
-        while offset < len(pdu_data)*8:
+        while offset < len(pdu_data) * 8:
             if pdu_header.large_file_flag:
                 start_offset = int.from_bytes(
-                    pdu_data[offset//8:(offset+64)//8], "big")
+                    pdu_data[offset // 8 : (offset + 64) // 8], "big"
+                )
                 offset += 64
                 end_offset = int.from_bytes(
-                    pdu_data[offset//8:(offset+64)//8], "big")
+                    pdu_data[offset // 8 : (offset + 64) // 8], "big"
+                )
                 offset += 64
             else:
                 start_offset = int.from_bytes(
-                    pdu_data[offset//8:(offset+32)//8], "big")
+                    pdu_data[offset // 8 : (offset + 32) // 8], "big"
+                )
                 offset += 32
                 end_offset = int.from_bytes(
-                    pdu_data[offset//8:(offset+32)//8], "big")
+                    pdu_data[offset // 8 : (offset + 32) // 8], "big"
+                )
                 offset += 32
             segment_requests.append((start_offset, end_offset))
 
         return cls(
             # pdu header parameters
             direction=pdu_header.direction,
             transmission_mode=pdu_header.transmission_mode,
@@ -187,8 +210,9 @@
             length_of_seq_number=pdu_header.length_of_seq_number,
             source_entity_id=pdu_header.source_entity_id,
             transaction_seq_number=pdu_header.transaction_seq_number,
             destination_entity_id=pdu_header.destination_entity_id,
             # nak pdu parameters
             start_of_scope=start_of_scope,
             end_of_scope=end_of_scope,
-            segment_requests=segment_requests)
+            segment_requests=segment_requests,
+        )
```

### Comparing `cfdp-1.1.3/src/cfdp/transaction.py` & `cfdp-2.0.0/src/cfdp/transaction.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,40 @@
-from .config import DefaultConfig
+from .constants import (
+    ChecksumType,
+    DEFAULT_MAX_FILE_SEGMENT_LEN,
+    DEFAULT_FAULT_HANDLERS,
+)
 
 
 class Transaction:
     """
     A transaction is the end-to-end transmission of a single File Data Unit
     from a single source CFDP entity to a single destination CFDP entity.
 
     A transaction may transfer a file from the local filestore, and/or one or
     more user messages, and/or one or more filestore requests to the
     destination entity.
 
     """
 
     def __init__(
-            self,
-            kernel,
-            source_entity_id,
-            seq_number,
-            destination_entity_id,
-            transmission_mode,
-            source_filename=None,
-            destination_filename=None,
-            fault_handler_overrides=None,
-            messages_to_user=None,
-            filestore_requests=None,
-            checksum_type=0):
+        self,
+        kernel,
+        source_entity_id,
+        seq_number,
+        destination_entity_id,
+        transmission_mode,
+        source_filename=None,
+        destination_filename=None,
+        fault_handler_overrides=None,
+        messages_to_user=None,
+        filestore_requests=None,
+        checksum_type=ChecksumType.MODULAR,
+        maximum_file_segment_length=DEFAULT_MAX_FILE_SEGMENT_LEN,
+    ):
         self.kernel = kernel
         self.source_entity_id = source_entity_id
         self.seq_number = seq_number
         self.destination_entity_id = destination_entity_id
         self.transmission_mode = transmission_mode
         self.source_filename = source_filename
         self.destination_filename = destination_filename
@@ -40,23 +46,24 @@
         self.id = (source_entity_id, seq_number)
         self.file_handle = None
 
         self._file_checksum = None
         self._file_size = None
         self._file_pos = 0
 
-        self.file_segment_size = self.kernel.config.get(
-            self.destination_entity_id).maximum_file_segment_length
+        self.file_segment_size = maximum_file_segment_length
 
     def get_file_size(self):
         if self._file_size is None:
             try:
-                self._file_size = \
-                    self.kernel.filestore.get_size(self.source_filename) if\
-                    self.source_filename else 0
+                self._file_size = (
+                    self.kernel.filestore.get_size(self.source_filename)
+                    if self.source_filename
+                    else 0
+                )
             except FileNotFoundError:
                 self._file_size = 0
         return self._file_size
 
     def get_file_checksum(self):
         if self._file_checksum is None:
             if self.source_filename:
@@ -65,20 +72,20 @@
                 fh.close()
             else:
                 self._file_checksum = 0
         return self._file_checksum
 
     def get_file_segment(self, offset=None, length=None):
         if self.file_handle is None:
-            raise Exception("File handle not defined")
+            raise ValueError("File handle not defined")
 
         if offset is None:
             offset = self._file_pos
         if offset > self._file_size:
-            raise Exception("Exceeded file end")
+            raise ValueError("Exceeded file end")
 
         if length is None:
             length = self.file_segment_size
             self._file_pos += self.file_segment_size
 
         self.file_handle.seek(offset)
         data = self.file_handle.read(length)
@@ -91,8 +98,8 @@
         # TODO...
         return None
 
     def get_fault_handler(self, fault):
         if self.fault_handler_overrides:
             if fault in self.fault_handler_overrides:
                 return self.fault_handler_overrides[fault]
-        return DefaultConfig.fault_handlers[fault]
+        return DEFAULT_FAULT_HANDLERS[fault]
```

### Comparing `cfdp-1.1.3/src/cfdp/transport/base.py` & `cfdp-2.0.0/src/cfdp/transport/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-
-
 class Transport:
-
     def __init__(self):
         self.config = None
 
     def is_ready(self):
         return True
 
     def connect(self, *args, **kwargs):
@@ -17,16 +14,16 @@
     def bind(self, *args, **kwargs):
         pass
 
     def unbind(self, *args, **kwargs):
         pass
 
     # send data
-    def request(self, data, address):
+    def request(self, data):
         raise NotImplementedError
 
     # indication that data was received
-    def indication(self, data, address=None):
+    def indication(self, data):
         pass
 
     def shutdown(self):
         pass
```

### Comparing `cfdp-1.1.3/src/cfdp/transport/zmq.py` & `cfdp-2.0.0/src/cfdp/transport/zmq.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 import threading
-import time
 import zmq
 
-from . import Transport
-from .. import logger
+from .base import Transport
 
 
 class ZmqTransport(Transport):
+    """ZMQ Transport for CFDP PDUs.
+
+    This transport is mostly used for testing and for prototypes.
+    A connection is established by making one entity the host, which does `bind` to a port,
+    and the other entity the client, which does `connect` to the host.
+    """
 
     def __init__(self):
         super().__init__()
         self.context = zmq.Context()
         self.socket = self.context.socket(zmq.PAIR)
 
-        self._incoming_pdu_thread = threading.Thread(
-            target=self._incoming_pdu_handler)
-        self._incoming_pdu_thread.kill = False
-
-    def request(self, data, address):
-        self.socket.send(data)
-
-    def connect(self, remote_entity_id):
-        url = self.config.get(remote_entity_id).ut_address
-        if url is None:
-            logger.warning(
-                "Remote entity %s id not configured" % remote_entity_id)
-        else:
-            self.socket.connect("tcp://{}".format(url))
+        self._thread = threading.Thread(target=self._incoming_pdu_handler)
+        self._thread.kill = False
+
+    def request(self, pdu):
+        self.socket.send(pdu)
+
+    def connect(self, host, port):
+        self.socket.connect(f"tcp://{host}:{port}")
+        self._thread.kill = False
+        self._thread.start()
 
     def disconnect(self):
+        self._thread.kill = True
+        self._thread.join()
         self.socket.close()
 
-    def bind(self):
-        url = self.config.local_entity.ut_address
-        self.socket.bind("tcp://{}".format(url))
-        self._incoming_pdu_thread.start()
+    def bind(self, host, port):
+        self.socket.bind(f"tcp://{host}:{port}")
+        self._thread.kill = False
+        self._thread.start()
 
     def unbind(self):
-        self._incoming_pdu_thread.kill = True
-        self._incoming_pdu_thread.join()
+        self._thread.kill = True
+        self._thread.join()
+        self.context.destroy()
 
     def _incoming_pdu_handler(self):
-        thread = threading.currentThread()
+        thread = threading.current_thread()
         while not thread.kill:
-            time.sleep(0.01)
-            try:
-                # check if pdu was received, then send it to upper layer
-                pdu = self.socket.recv(flags=zmq.NOBLOCK)
+            if self.socket.poll(100):
+                if thread.kill:
+                    break
+                pdu = self.socket.recv()
                 self.indication(pdu)
-            except zmq.Again:
-                pass
-            except zmq.ZMQError:
-                break
-
-    def shutdown(self):
-        self.context.destroy()
```

### Comparing `cfdp-1.1.3/src/cfdp.egg-info/PKG-INFO` & `cfdp-2.0.0/src/cfdp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 Metadata-Version: 2.1
 Name: cfdp
-Version: 1.1.3
+Version: 2.0.0
 Summary: CCSDS File Delivery Protocol
-Home-page: https://gitlab.com/librecube/lib/python-cfdp
-Author-email: info@librecube.org
+Author-email: LibreCube <info@librecube.org>
 License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.4
 Description-Content-Type: text/markdown
-Provides-Extra: zmq
 License-File: LICENSE.txt
 
 # Python CFDP
 
 The CCSDS File Delivery Protocol (CFDP) was developed by the
 [Consultative Committee for Space Data Systems (CCSDS)](https://public.ccsds.org).
 The CFDP protocol provides reliable transfer of files from one endpoint to
@@ -40,25 +36,20 @@
 
 Clone the repository and then install via pip:
 
 ```
 $ pip install cfdp
 ```
 
-If you intend to use ZMQ as transport layer then install as:
-
-```
-$ pip install cfdp[zmq]
-```
+> Depending on the transport layer to use with CFDP, one needs to install additional dependencies.
 
 ## Documentation
 
 Find the detailed documentation [here](docs/README.md).
 
-
 ## Tests
 
 The protocol is tested for cross-support as outlined in CCSDS CFDP Yellow Book.
 See [tests/README.md](tests/README.md) for details.
 
 ## Contribute
 
@@ -73,9 +64,7 @@
 If you are having issues, please let us know. Reach us at
 [Matrix](https://app.element.io/#/room/#librecube.org:matrix.org)
 or via [Email](mailto:info@librecube.org).
 
 ## License
 
 The project is licensed under the MIT license. See the [LICENSE](./LICENSE.txt) file for details.
-
-
```

### Comparing `cfdp-1.1.3/src/cfdp.egg-info/SOURCES.txt` & `cfdp-2.0.0/src/cfdp.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 LICENSE.txt
 README.md
-setup.py
+pyproject.toml
 src/cfdp/__init__.py
-src/cfdp/config.py
 src/cfdp/constants.py
 src/cfdp/core.py
 src/cfdp/event.py
 src/cfdp/transaction.py
 src/cfdp.egg-info/PKG-INFO
 src/cfdp.egg-info/SOURCES.txt
 src/cfdp.egg-info/dependency_links.txt
-src/cfdp.egg-info/requires.txt
 src/cfdp.egg-info/top_level.txt
 src/cfdp/filestore/__init__.py
 src/cfdp/filestore/base.py
 src/cfdp/filestore/native.py
 src/cfdp/machines/__init__.py
 src/cfdp/machines/base.py
 src/cfdp/machines/receiver1.py
@@ -34,9 +32,16 @@
 src/cfdp/pdu/header.py
 src/cfdp/pdu/keep_alive.py
 src/cfdp/pdu/metadata.py
 src/cfdp/pdu/nak.py
 src/cfdp/pdu/prompt.py
 src/cfdp/transport/__init__.py
 src/cfdp/transport/base.py
+src/cfdp/transport/spp.py
 src/cfdp/transport/udp.py
-src/cfdp/transport/zmq.py
+src/cfdp/transport/zmq.py
+tests/test_series_F1.py
+tests/test_series_F2.py
+tests/test_series_F3.py
+tests/test_series_F4.py
+tests/test_spp.py
+tests/test_zmq.py
```

