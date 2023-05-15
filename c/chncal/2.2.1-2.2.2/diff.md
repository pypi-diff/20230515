# Comparing `tmp/chncal-2.2.1.tar.gz` & `tmp/chncal-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chncal-2.2.1.tar", last modified: Sat Feb 25 10:27:18 2023, max compression
+gzip compressed data, was "chncal-2.2.2.tar", last modified: Mon May 15 11:08:30 2023, max compression
```

## Comparing `chncal-2.2.1.tar` & `chncal-2.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 10:27:18.465978 chncal-2.2.1/
--rw-rw-rw-   0        0        0     1068 2022-08-22 06:16:21.000000 chncal-2.2.1/LICENSE
--rw-rw-rw-   0        0        0     2360 2023-02-25 10:27:18.464973 chncal-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1970 2022-08-28 04:05:52.000000 chncal-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 10:27:17.691878 chncal-2.2.1/chncal/
--rw-rw-rw-   0        0        0      730 2023-02-25 10:26:46.000000 chncal-2.2.1/chncal/__init__.py
--rw-rw-rw-   0        0        0    21004 2023-02-10 04:51:14.000000 chncal-2.2.1/chncal/apis.py
--rw-rw-rw-   0        0        0    69806 2023-02-16 13:23:02.000000 chncal-2.2.1/chncal/constants.py
--rw-rw-rw-   0        0        0     8480 2023-02-16 13:23:14.000000 chncal-2.2.1/chncal/constants_fate.py
--rw-rw-rw-   0        0        0  9509384 2023-02-16 13:23:14.000000 chncal-2.2.1/chncal/constants_hko.py
--rw-rw-rw-   0        0        0  3923457 2023-02-16 13:23:04.000000 chncal-2.2.1/chncal/constants_trade_dates.py
--rw-rw-rw-   0        0        0     2501 2022-10-03 12:21:06.000000 chncal-2.2.1/chncal/constants_wuxing.py
--rw-rw-rw-   0        0        0     8342 2022-10-03 12:21:06.000000 chncal-2.2.1/chncal/constants_zodiac_marry.py
-drwxrwxrwx   0        0        0        0 2023-02-25 10:27:18.463945 chncal-2.2.1/chncal/data/
--rw-rw-rw-   0        0        0      105 2022-08-22 06:08:12.000000 chncal-2.2.1/chncal/data/__init__.py
--rw-rw-rw-   0        0        0    49817 2023-01-18 01:47:59.000000 chncal-2.2.1/chncal/data/data.py
--rw-rw-rw-   0        0        0     3056 2022-08-26 06:40:24.000000 chncal-2.2.1/chncal/data/fate_weights.py
--rw-rw-rw-   0        0        0    13132 2023-01-23 14:50:48.000000 chncal-2.2.1/chncal/data/hko_calendar.py
--rw-rw-rw-   0        0        0     4570 2022-10-03 12:21:06.000000 chncal-2.2.1/chncal/solar_terms.py
-drwxrwxrwx   0        0        0        0 2023-02-25 10:27:18.457001 chncal-2.2.1/chncal.egg-info/
--rw-rw-rw-   0        0        0     2360 2023-02-25 10:27:15.000000 chncal-2.2.1/chncal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-02-25 10:27:17.000000 chncal-2.2.1/chncal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 10:27:15.000000 chncal-2.2.1/chncal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-25 10:27:17.000000 chncal-2.2.1/chncal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-25 10:27:18.466939 chncal-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      861 2022-12-15 06:47:26.000000 chncal-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:08:30.878711 chncal-2.2.2/
+-rw-rw-rw-   0        0        0     1073 2023-02-25 10:45:56.000000 chncal-2.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2337 2023-05-15 11:08:30.875710 chncal-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1970 2022-08-28 04:05:52.000000 chncal-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 11:08:30.836676 chncal-2.2.2/chncal/
+-rw-rw-rw-   0        0        0      730 2023-05-15 11:07:53.000000 chncal-2.2.2/chncal/__init__.py
+-rw-rw-rw-   0        0        0    21004 2023-02-10 04:51:14.000000 chncal-2.2.2/chncal/apis.py
+-rw-rw-rw-   0        0        0    69806 2023-05-12 02:03:19.000000 chncal-2.2.2/chncal/constants.py
+-rw-rw-rw-   0        0        0     8480 2023-05-12 02:03:24.000000 chncal-2.2.2/chncal/constants_fate.py
+-rw-rw-rw-   0        0        0  9509384 2023-05-12 02:03:24.000000 chncal-2.2.2/chncal/constants_hko.py
+-rw-rw-rw-   0        0        0  3958798 2023-05-12 02:03:20.000000 chncal-2.2.2/chncal/constants_trade_dates.py
+-rw-rw-rw-   0        0        0     2501 2022-10-03 12:21:06.000000 chncal-2.2.2/chncal/constants_wuxing.py
+-rw-rw-rw-   0        0        0     8342 2022-10-03 12:21:06.000000 chncal-2.2.2/chncal/constants_zodiac_marry.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:08:30.871706 chncal-2.2.2/chncal/data/
+-rw-rw-rw-   0        0        0      105 2022-08-22 06:08:12.000000 chncal-2.2.2/chncal/data/__init__.py
+-rw-rw-rw-   0        0        0    49817 2023-01-18 01:47:59.000000 chncal-2.2.2/chncal/data/data.py
+-rw-rw-rw-   0        0        0     3056 2022-08-26 06:40:24.000000 chncal-2.2.2/chncal/data/fate_weights.py
+-rw-rw-rw-   0        0        0    13132 2023-01-23 14:50:48.000000 chncal-2.2.2/chncal/data/hko_calendar.py
+-rw-rw-rw-   0        0        0     4570 2022-10-03 12:21:06.000000 chncal-2.2.2/chncal/solar_terms.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:08:30.855697 chncal-2.2.2/chncal.egg-info/
+-rw-rw-rw-   0        0        0     2337 2023-05-15 11:08:25.000000 chncal-2.2.2/chncal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-05-15 11:08:29.000000 chncal-2.2.2/chncal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:08:25.000000 chncal-2.2.2/chncal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 11:08:25.000000 chncal-2.2.2/chncal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 11:08:30.878711 chncal-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      861 2022-12-15 06:47:26.000000 chncal-2.2.2/setup.py
```

### Comparing `chncal-2.2.1/LICENSE` & `chncal-2.2.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Genlovy Hoo
+Copyright (c) 2022-2023 Genlovy Hoo
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `chncal-2.2.1/PKG-INFO` & `chncal-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: chncal
-Version: 2.2.1
+Version: 2.2.2
 Summary: Check if some day is holiday in china.
 Home-page: https://github.com/Genlovy-Hoo/chncal
 Author: Genlovy Hoo
 Author-email: genlovhyy@163.com
 License: MIT License
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 中国节假日
 
 判断某年某月某一天是不是工作日/节假日。
 
@@ -79,9 +78,7 @@
 [chncal](https://github.com/Genlovy-Hoo/chncal/)
 
 Pypi
 
 [chncal](https://pypi.org/project/chncal/)
 
 感谢使用和支持！
-
-
```

### Comparing `chncal-2.2.1/README.md` & `chncal-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/__init__.py` & `chncal-2.2.2/chncal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # from __future__ import absolute_import, unicode_literals
 
-__version__ = '2.2.1'
+__version__ = '2.2.2'
 
 from .apis import (
     find_workday,
     get_dates,
     get_holiday_detail,
     get_holidays,
     get_solar_terms,
```

### Comparing `chncal-2.2.1/chncal/apis.py` & `chncal-2.2.2/chncal/apis.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/constants.py` & `chncal-2.2.2/chncal/constants.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/constants_fate.py` & `chncal-2.2.2/chncal/constants_fate.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/constants_hko.py` & `chncal-2.2.2/chncal/constants_hko.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/constants_trade_dates.py` & `chncal-2.2.2/chncal/constants_trade_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6009,14 +6009,99 @@
     ("CFFEX", datetime.date(year=2023, month=2, day=10)): 1,
     ("CFFEX", datetime.date(year=2023, month=2, day=11)): 0,
     ("CFFEX", datetime.date(year=2023, month=2, day=12)): 0,
     ("CFFEX", datetime.date(year=2023, month=2, day=13)): 1,
     ("CFFEX", datetime.date(year=2023, month=2, day=14)): 1,
     ("CFFEX", datetime.date(year=2023, month=2, day=15)): 1,
     ("CFFEX", datetime.date(year=2023, month=2, day=16)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=17)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=18)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=19)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=20)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=21)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=22)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=23)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=24)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=25)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=26)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=27)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=28)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=1)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=2)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=3)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=4)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=5)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=6)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=7)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=8)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=9)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=10)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=11)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=12)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=13)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=14)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=15)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=16)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=17)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=18)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=19)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=20)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=21)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=22)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=23)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=24)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=25)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=26)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=27)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=28)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=29)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=30)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=31)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=1)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=2)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=3)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=4)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=5)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=6)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=7)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=8)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=9)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=10)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=11)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=12)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=13)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=14)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=15)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=16)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=17)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=18)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=19)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=20)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=21)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=22)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=23)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=24)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=25)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=26)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=27)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=28)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=29)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=30)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=1)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=2)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=3)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=4)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=5)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=6)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=7)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=8)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=9)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=10)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=11)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=13)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=14)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=15)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=16)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=17)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=18)): 1,
@@ -17824,14 +17909,99 @@
     ("CZCE", datetime.date(year=2023, month=2, day=10)): 1,
     ("CZCE", datetime.date(year=2023, month=2, day=11)): 0,
     ("CZCE", datetime.date(year=2023, month=2, day=12)): 0,
     ("CZCE", datetime.date(year=2023, month=2, day=13)): 1,
     ("CZCE", datetime.date(year=2023, month=2, day=14)): 1,
     ("CZCE", datetime.date(year=2023, month=2, day=15)): 1,
     ("CZCE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=27)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=28)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=29)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=30)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=1)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=2)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=3)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=12)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=1)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=2)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=3)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=4)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=5)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=6)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=7)): 0,
@@ -28768,14 +28938,99 @@
     ("DCE", datetime.date(year=2023, month=2, day=10)): 1,
     ("DCE", datetime.date(year=2023, month=2, day=11)): 0,
     ("DCE", datetime.date(year=2023, month=2, day=12)): 0,
     ("DCE", datetime.date(year=2023, month=2, day=13)): 1,
     ("DCE", datetime.date(year=2023, month=2, day=14)): 1,
     ("DCE", datetime.date(year=2023, month=2, day=15)): 1,
     ("DCE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=27)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=28)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=29)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=30)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=1)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=2)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=3)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=12)): 1,
     ("INE", datetime.date(year=2017, month=5, day=23)): 1,
     ("INE", datetime.date(year=2017, month=5, day=24)): 1,
     ("INE", datetime.date(year=2017, month=5, day=25)): 1,
     ("INE", datetime.date(year=2017, month=5, day=26)): 1,
     ("INE", datetime.date(year=2017, month=5, day=27)): 0,
     ("INE", datetime.date(year=2017, month=5, day=28)): 0,
     ("INE", datetime.date(year=2017, month=5, day=29)): 0,
@@ -30863,14 +31118,99 @@
     ("INE", datetime.date(year=2023, month=2, day=10)): 1,
     ("INE", datetime.date(year=2023, month=2, day=11)): 0,
     ("INE", datetime.date(year=2023, month=2, day=12)): 0,
     ("INE", datetime.date(year=2023, month=2, day=13)): 1,
     ("INE", datetime.date(year=2023, month=2, day=14)): 1,
     ("INE", datetime.date(year=2023, month=2, day=15)): 1,
     ("INE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=27)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=28)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=29)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=30)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=1)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=2)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=3)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=12)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=28)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=31)): 1,
     ("SHFE", datetime.date(year=1991, month=6, day=1)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=2)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=3)): 1,
@@ -42450,14 +42790,99 @@
     ("SHFE", datetime.date(year=2023, month=2, day=10)): 1,
     ("SHFE", datetime.date(year=2023, month=2, day=11)): 0,
     ("SHFE", datetime.date(year=2023, month=2, day=12)): 0,
     ("SHFE", datetime.date(year=2023, month=2, day=13)): 1,
     ("SHFE", datetime.date(year=2023, month=2, day=14)): 1,
     ("SHFE", datetime.date(year=2023, month=2, day=15)): 1,
     ("SHFE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=27)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=28)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=29)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=30)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=1)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=2)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=3)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=12)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=20)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=21)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=22)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=23)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=24)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=25)): 1,
@@ -54198,14 +54623,99 @@
     ("SSE", datetime.date(year=2023, month=2, day=10)): 1,
     ("SSE", datetime.date(year=2023, month=2, day=11)): 0,
     ("SSE", datetime.date(year=2023, month=2, day=12)): 0,
     ("SSE", datetime.date(year=2023, month=2, day=13)): 1,
     ("SSE", datetime.date(year=2023, month=2, day=14)): 1,
     ("SSE", datetime.date(year=2023, month=2, day=15)): 1,
     ("SSE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=27)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=28)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=29)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=30)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=1)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=2)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=3)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=12)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=3)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=4)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=5)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=6)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=7)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=8)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=9)): 1,
@@ -65750,8 +66260,93 @@
     ("SZSE", datetime.date(year=2023, month=2, day=10)): 1,
     ("SZSE", datetime.date(year=2023, month=2, day=11)): 0,
     ("SZSE", datetime.date(year=2023, month=2, day=12)): 0,
     ("SZSE", datetime.date(year=2023, month=2, day=13)): 1,
     ("SZSE", datetime.date(year=2023, month=2, day=14)): 1,
     ("SZSE", datetime.date(year=2023, month=2, day=15)): 1,
     ("SZSE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=27)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=28)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=29)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=30)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=1)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=2)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=3)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=12)): 1,
 }
```

### Comparing `chncal-2.2.1/chncal/constants_wuxing.py` & `chncal-2.2.2/chncal/constants_wuxing.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/constants_zodiac_marry.py` & `chncal-2.2.2/chncal/constants_zodiac_marry.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/data/data.py` & `chncal-2.2.2/chncal/data/data.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/data/fate_weights.py` & `chncal-2.2.2/chncal/data/fate_weights.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/data/hko_calendar.py` & `chncal-2.2.2/chncal/data/hko_calendar.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal/solar_terms.py` & `chncal-2.2.2/chncal/solar_terms.py`

 * *Files identical despite different names*

### Comparing `chncal-2.2.1/chncal.egg-info/PKG-INFO` & `chncal-2.2.2/chncal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: chncal
-Version: 2.2.1
+Version: 2.2.2
 Summary: Check if some day is holiday in china.
 Home-page: https://github.com/Genlovy-Hoo/chncal
 Author: Genlovy Hoo
 Author-email: genlovhyy@163.com
 License: MIT License
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 中国节假日
 
 判断某年某月某一天是不是工作日/节假日。
 
@@ -79,9 +78,7 @@
 [chncal](https://github.com/Genlovy-Hoo/chncal/)
 
 Pypi
 
 [chncal](https://pypi.org/project/chncal/)
 
 感谢使用和支持！
-
-
```

### Comparing `chncal-2.2.1/setup.py` & `chncal-2.2.2/setup.py`

 * *Files identical despite different names*

