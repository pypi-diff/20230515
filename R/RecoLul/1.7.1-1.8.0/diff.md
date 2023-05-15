# Comparing `tmp/RecoLul-1.7.1.tar.gz` & `tmp/RecoLul-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecoLul-1.7.1.tar", last modified: Tue Apr  4 02:32:12 2023, max compression
+gzip compressed data, was "RecoLul-1.8.0.tar", last modified: Mon May 15 02:02:39 2023, max compression
```

## Comparing `RecoLul-1.7.1.tar` & `RecoLul-1.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-04-04 02:32:12.932175 RecoLul-1.7.1/
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1069 2022-10-28 02:03:59.000000 RecoLul-1.7.1/LICENSE
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1051 2023-04-04 02:32:12.932175 RecoLul-1.7.1/PKG-INFO
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      643 2023-02-06 08:29:19.000000 RecoLul-1.7.1/README.md
-drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-04-04 02:32:12.928176 RecoLul-1.7.1/RecoLul.egg-info/
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1051 2023-04-04 02:32:12.000000 RecoLul-1.7.1/RecoLul.egg-info/PKG-INFO
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      434 2023-04-04 02:32:12.000000 RecoLul-1.7.1/RecoLul.egg-info/SOURCES.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        1 2023-04-04 02:32:12.000000 RecoLul-1.7.1/RecoLul.egg-info/dependency_links.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       45 2023-04-04 02:32:12.000000 RecoLul-1.7.1/RecoLul.egg-info/entry_points.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       81 2023-04-04 02:32:12.000000 RecoLul-1.7.1/RecoLul.egg-info/requires.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        8 2023-04-04 02:32:12.000000 RecoLul-1.7.1/RecoLul.egg-info/top_level.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      100 2022-10-19 06:32:10.000000 RecoLul-1.7.1/pyproject.toml
-drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-04-04 02:32:12.932175 RecoLul-1.7.1/recolul/
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       22 2023-04-04 02:31:47.000000 RecoLul-1.7.1/recolul/__init__.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     4020 2023-04-04 02:22:28.000000 RecoLul-1.7.1/recolul/cli.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1325 2023-02-06 04:58:11.000000 RecoLul-1.7.1/recolul/config.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1237 2023-02-06 07:38:04.000000 RecoLul-1.7.1/recolul/duration.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      924 2023-02-09 07:26:16.000000 RecoLul-1.7.1/recolul/plotting.py
-drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-04-04 02:32:12.932175 RecoLul-1.7.1/recolul/recoru/
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        0 2023-02-22 01:29:18.000000 RecoLul-1.7.1/recolul/recoru/__init__.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     2411 2023-04-04 02:18:53.000000 RecoLul-1.7.1/recolul/recoru/attendance_chart.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1723 2023-02-22 02:34:58.000000 RecoLul-1.7.1/recolul/recoru/recoru_session.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     2351 2023-04-04 02:22:09.000000 RecoLul-1.7.1/recolul/time.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      739 2023-04-04 02:32:12.932175 RecoLul-1.7.1/setup.cfg
+drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-05-15 02:02:39.462144 RecoLul-1.8.0/
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1069 2022-10-28 02:03:59.000000 RecoLul-1.8.0/LICENSE
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1051 2023-05-15 02:02:39.462144 RecoLul-1.8.0/PKG-INFO
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      643 2023-02-06 08:29:19.000000 RecoLul-1.8.0/README.md
+drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-05-15 02:02:39.458144 RecoLul-1.8.0/RecoLul.egg-info/
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1051 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/PKG-INFO
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      434 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/SOURCES.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        1 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/dependency_links.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       45 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/entry_points.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       81 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/requires.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        8 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/top_level.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      100 2022-10-19 06:32:10.000000 RecoLul-1.8.0/pyproject.toml
+drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-05-15 02:02:39.462144 RecoLul-1.8.0/recolul/
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       22 2023-05-15 02:01:29.000000 RecoLul-1.8.0/recolul/__init__.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     4020 2023-04-07 06:25:37.000000 RecoLul-1.8.0/recolul/cli.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1325 2023-02-06 04:58:11.000000 RecoLul-1.8.0/recolul/config.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1237 2023-02-06 07:38:04.000000 RecoLul-1.8.0/recolul/duration.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      924 2023-02-09 07:26:16.000000 RecoLul-1.8.0/recolul/plotting.py
+drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-05-15 02:02:39.462144 RecoLul-1.8.0/recolul/recoru/
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        0 2023-02-22 01:29:18.000000 RecoLul-1.8.0/recolul/recoru/__init__.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     2516 2023-05-15 01:53:12.000000 RecoLul-1.8.0/recolul/recoru/attendance_chart.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1723 2023-02-22 02:34:58.000000 RecoLul-1.8.0/recolul/recoru/recoru_session.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     2416 2023-05-15 01:57:40.000000 RecoLul-1.8.0/recolul/time.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      739 2023-05-15 02:02:39.462144 RecoLul-1.8.0/setup.cfg
```

### Comparing `RecoLul-1.7.1/LICENSE` & `RecoLul-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RecoLul-1.7.1/PKG-INFO` & `RecoLul-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecoLul
-Version: 1.7.1
+Version: 1.8.0
 Summary: Overtime management for RecoRu
 Home-page: https://github.com/Maerig/recolul
 Author: Jean-Loup Roussel-Clouet
 Author-email: jean-loup@cryptact.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `RecoLul-1.7.1/README.md` & `RecoLul-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `RecoLul-1.7.1/RecoLul.egg-info/PKG-INFO` & `RecoLul-1.8.0/RecoLul.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecoLul
-Version: 1.7.1
+Version: 1.8.0
 Summary: Overtime management for RecoRu
 Home-page: https://github.com/Maerig/recolul
 Author: Jean-Loup Roussel-Clouet
 Author-email: jean-loup@cryptact.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `RecoLul-1.7.1/recolul/cli.py` & `RecoLul-1.8.0/recolul/cli.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.7.1/recolul/config.py` & `RecoLul-1.8.0/recolul/config.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.7.1/recolul/duration.py` & `RecoLul-1.8.0/recolul/duration.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.7.1/recolul/plotting.py` & `RecoLul-1.8.0/recolul/plotting.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.7.1/recolul/recoru/attendance_chart.py` & `RecoLul-1.8.0/recolul/recoru/attendance_chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class ChartColumn(str, Enum):
     DATE = "日付"
     WORKPLACE = "作業場所"
     CATEGORY = "勤務区分"
     START = "開始"
     END = "終了"
     WORK_TIME = "労働時間"
+    MEMO = "メモ"
 
 
 class ChartEntry:
     """Single cell of the attendance chart"""
     def __init__(self, tag: Tag):
         self._tag = tag
 
@@ -85,9 +86,13 @@
     def clock_out_time(self) -> str:
         return self[ChartColumn.END].text
 
     @property
     def work_time(self) -> str:
         return self[ChartColumn.WORK_TIME].text
 
+    @property
+    def memo(self) -> str:
+        return self[ChartColumn.MEMO].text
+
 
 AttendanceChart: TypeAlias = list[ChartRow]
```

### Comparing `RecoLul-1.7.1/recolul/recoru/recoru_session.py` & `RecoLul-1.8.0/recolul/recoru/recoru_session.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.7.1/recolul/time.py` & `RecoLul-1.8.0/recolul/time.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,18 @@
             continue
 
         day = row.day
         if not day.text:
             continue
 
         days.append(day.text)
-        required_time = Duration(0 if day.color in ["blue", "red"] else 8 * 60)  # No required hours for holidays
+        if day.color in ["blue", "red"] and "swap day" not in row.memo.lower():
+            required_time = Duration(0)
+        else:
+            required_time = Duration(8 * 60)
         work_time = get_work_time(row)
         overtime_history.append(work_time - required_time)
         total_workplace_times[row.workplace.text] += work_time
 
     return days, overtime_history, total_workplace_times
```

### Comparing `RecoLul-1.7.1/setup.cfg` & `RecoLul-1.8.0/setup.cfg`

 * *Files identical despite different names*

