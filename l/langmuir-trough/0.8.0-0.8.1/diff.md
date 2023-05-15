# Comparing `tmp/langmuir_trough-0.8.0.tar.gz` & `tmp/langmuir_trough-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langmuir_trough-0.8.0.tar", last modified: Fri May 12 20:43:09 2023, max compression
+gzip compressed data, was "langmuir_trough-0.8.1.tar", last modified: Mon May 15 20:02:57 2023, max compression
```

## Comparing `langmuir_trough-0.8.0.tar` & `langmuir_trough-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.703785 langmuir_trough-0.8.0/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.699881 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/
--rw-r--r--   0 gutow    (60685682) staff       (20)    10405 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)      819 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/SOURCES.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/dependency_links.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)      348 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/requires.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        7 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/top_level.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)    10405 2023-05-12 20:43:09.703604 langmuir_trough-0.8.0/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)     9751 2023-05-12 20:07:19.000000 langmuir_trough-0.8.0/README.md
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.700005 langmuir_trough-0.8.0/Trough/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.700886 langmuir_trough-0.8.0/Trough/Trough_Control/
--rw-r--r--   0 gutow    (60685682) staff       (20)      153 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_Control/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      313 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_Control/message_utils.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9991 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_Control/simulation.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    37129 2023-05-12 20:07:19.000000 langmuir_trough-0.8.0/Trough/Trough_Control/trough_util.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.703163 langmuir_trough-0.8.0/Trough/Trough_GUI/
--rw-r--r--   0 gutow    (60685682) staff       (20)    30280 2023-05-12 19:37:48.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/Collect_data.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    28605 2023-05-12 14:45:53.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/Monitor_Calibrate.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     3017 2023-04-28 14:28:17.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    24079 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/calibration_utils.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    15590 2023-05-12 18:11:19.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/command_widgets.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     2614 2023-05-10 20:38:39.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/conversions.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    10038 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/status_widgets.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      103 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-05-12 20:43:09.703823 langmuir_trough-0.8.0/setup.cfg
--rw-r--r--   0 gutow    (60685682) staff       (20)     1597 2023-05-12 20:14:13.000000 langmuir_trough-0.8.0/setup.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-15 20:02:57.512973 langmuir_trough-0.8.1/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-15 20:02:57.510632 langmuir_trough-0.8.1/Langmuir_Trough.egg-info/
+-rw-r--r--   0 gutow    (60685682) staff       (20)    10502 2023-05-15 20:02:57.000000 langmuir_trough-0.8.1/Langmuir_Trough.egg-info/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)      819 2023-05-15 20:02:57.000000 langmuir_trough-0.8.1/Langmuir_Trough.egg-info/SOURCES.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-05-15 20:02:57.000000 langmuir_trough-0.8.1/Langmuir_Trough.egg-info/dependency_links.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)      348 2023-05-15 20:02:57.000000 langmuir_trough-0.8.1/Langmuir_Trough.egg-info/requires.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        7 2023-05-15 20:02:57.000000 langmuir_trough-0.8.1/Langmuir_Trough.egg-info/top_level.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)    10502 2023-05-15 20:02:57.512801 langmuir_trough-0.8.1/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9848 2023-05-15 19:59:46.000000 langmuir_trough-0.8.1/README.md
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-15 20:02:57.510768 langmuir_trough-0.8.1/Trough/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-15 20:02:57.511306 langmuir_trough-0.8.1/Trough/Trough_Control/
+-rw-r--r--   0 gutow    (60685682) staff       (20)      153 2023-03-29 22:32:39.000000 langmuir_trough-0.8.1/Trough/Trough_Control/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      313 2023-03-29 22:32:39.000000 langmuir_trough-0.8.1/Trough/Trough_Control/message_utils.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9991 2023-03-29 22:32:39.000000 langmuir_trough-0.8.1/Trough/Trough_Control/simulation.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    37190 2023-05-15 19:57:00.000000 langmuir_trough-0.8.1/Trough/Trough_Control/trough_util.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-15 20:02:57.512397 langmuir_trough-0.8.1/Trough/Trough_GUI/
+-rw-r--r--   0 gutow    (60685682) staff       (20)    30280 2023-05-12 20:48:35.000000 langmuir_trough-0.8.1/Trough/Trough_GUI/Collect_data.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    28605 2023-05-12 14:45:53.000000 langmuir_trough-0.8.1/Trough/Trough_GUI/Monitor_Calibrate.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     3017 2023-04-28 14:28:17.000000 langmuir_trough-0.8.1/Trough/Trough_GUI/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    24079 2023-03-29 22:32:39.000000 langmuir_trough-0.8.1/Trough/Trough_GUI/calibration_utils.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    15590 2023-05-12 20:48:35.000000 langmuir_trough-0.8.1/Trough/Trough_GUI/command_widgets.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     2614 2023-05-10 20:38:39.000000 langmuir_trough-0.8.1/Trough/Trough_GUI/conversions.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    10038 2023-03-29 22:32:39.000000 langmuir_trough-0.8.1/Trough/Trough_GUI/status_widgets.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      103 2023-03-29 22:32:39.000000 langmuir_trough-0.8.1/Trough/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-05-15 20:02:57.513005 langmuir_trough-0.8.1/setup.cfg
+-rw-r--r--   0 gutow    (60685682) staff       (20)     1597 2023-05-15 19:59:46.000000 langmuir_trough-0.8.1/setup.py
```

### Comparing `langmuir_trough-0.8.0/Langmuir_Trough.egg-info/PKG-INFO` & `langmuir_trough-0.8.1/Langmuir_Trough.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langmuir-trough
-Version: 0.8.0
+Version: 0.8.1
 Summary: Controls and collects data from Gutow Lab Langmuir Trough.
 Home-page: https://github.com/gutow/Langmuir_Trough.git
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -125,14 +125,16 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.8.1 (May 15, 2023)
+  * BUG_FIX: Needed to reset cycles_on and cycles_off when speed updated.
 * 0.8.0 (May 12, 2023)
   * Added capability to do very slow compressions (< 1 cm/min) by moving the 
     barriers intermittently at near their lowest continuous speed.
   * Now record datapoint time_stamps as actual_time_stamp - run_time_stamp. 
     This avoids round off errors in the html based data storage file.
   * BUG_FIXES:
     * Errors in conversion of speeds between units.
```

### Comparing `langmuir_trough-0.8.0/Langmuir_Trough.egg-info/SOURCES.txt` & `langmuir_trough-0.8.1/Langmuir_Trough.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/PKG-INFO` & `langmuir_trough-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langmuir_trough
-Version: 0.8.0
+Version: 0.8.1
 Summary: Controls and collects data from Gutow Lab Langmuir Trough.
 Home-page: https://github.com/gutow/Langmuir_Trough.git
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -125,14 +125,16 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.8.1 (May 15, 2023)
+  * BUG_FIX: Needed to reset cycles_on and cycles_off when speed updated.
 * 0.8.0 (May 12, 2023)
   * Added capability to do very slow compressions (< 1 cm/min) by moving the 
     barriers intermittently at near their lowest continuous speed.
   * Now record datapoint time_stamps as actual_time_stamp - run_time_stamp. 
     This avoids round off errors in the html based data storage file.
   * BUG_FIXES:
     * Errors in conversion of speeds between units.
```

### Comparing `langmuir_trough-0.8.0/README.md` & `langmuir_trough-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.8.1 (May 15, 2023)
+  * BUG_FIX: Needed to reset cycles_on and cycles_off when speed updated.
 * 0.8.0 (May 12, 2023)
   * Added capability to do very slow compressions (< 1 cm/min) by moving the 
     barriers intermittently at near their lowest continuous speed.
   * Now record datapoint time_stamps as actual_time_stamp - run_time_stamp. 
     This avoids round off errors in the html based data storage file.
   * BUG_FIXES:
     * Errors in conversion of speeds between units.
```

### Comparing `langmuir_trough-0.8.0/Trough/Trough_Control/simulation.py` & `langmuir_trough-0.8.1/Trough/Trough_Control/simulation.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/Trough/Trough_Control/trough_util.py` & `langmuir_trough-0.8.1/Trough/Trough_Control/trough_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -822,14 +822,16 @@
             elif cmd[0] == 'Direction':
                 # set the direction
                 direction = cmd[1]
                 if (direction != -1) and (direction != 0) and (direction != 1):
                     direction = 0
             elif cmd[0] == 'Speed':
                 # set the speed
+                cycles_on = 1
+                cycles_off = 0
                 requested_speed = cmd[1]
                 if requested_speed > 1:
                     requested_speed = 1
                 if requested_speed < 0:
                     requested_speed = 0
                 if requested_speed < 0.1:
                     # set up cycles to go at lower speeds
```

### Comparing `langmuir_trough-0.8.0/Trough/Trough_GUI/Collect_data.py` & `langmuir_trough-0.8.1/Trough/Trough_GUI/Collect_data.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/Trough/Trough_GUI/Monitor_Calibrate.py` & `langmuir_trough-0.8.1/Trough/Trough_GUI/Monitor_Calibrate.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/Trough/Trough_GUI/__init__.py` & `langmuir_trough-0.8.1/Trough/Trough_GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/Trough/Trough_GUI/calibration_utils.py` & `langmuir_trough-0.8.1/Trough/Trough_GUI/calibration_utils.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/Trough/Trough_GUI/command_widgets.py` & `langmuir_trough-0.8.1/Trough/Trough_GUI/command_widgets.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/Trough/Trough_GUI/conversions.py` & `langmuir_trough-0.8.1/Trough/Trough_GUI/conversions.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/Trough/Trough_GUI/status_widgets.py` & `langmuir_trough-0.8.1/Trough/Trough_GUI/status_widgets.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.8.0/setup.py` & `langmuir_trough-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="langmuir_trough",
-    version="0.8.0",
+    version="0.8.1",
     description="Controls and collects data from Gutow Lab Langmuir Trough.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gutow/Langmuir_Trough.git",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="",
```

