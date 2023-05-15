# Comparing `tmp/pyplanpro-0.0.6.tar.gz` & `tmp/pyplanpro-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplanpro-0.0.6.tar", last modified: Mon May  8 09:41:01 2023, max compression
+gzip compressed data, was "pyplanpro-0.0.9.tar", last modified: Mon May 15 07:10:31 2023, max compression
```

## Comparing `pyplanpro-0.0.6.tar` & `pyplanpro-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/PyPlanPro/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/PyPlanPro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/models/resource_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/PyPlanPro/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/heuristic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/scheduler_result.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/pyplanpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/tests/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/tests/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/tests/scheduler/test_heuristic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/tests/scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:31.361820 pyplanpro-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-15 07:10:31.361820 pyplanpro-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:31.357819 pyplanpro-0.0.9/PyPlanPro/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:31.361820 pyplanpro-0.0.9/PyPlanPro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/models/resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:31.361820 pyplanpro-0.0.9/PyPlanPro/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/scheduler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/scheduler/heuristic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/scheduler/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/scheduler/scheduler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/PyPlanPro/scheduler/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:31.361820 pyplanpro-0.0.9/pyplanpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-15 07:10:31.000000 pyplanpro-0.0.9/pyplanpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 07:10:31.000000 pyplanpro-0.0.9/pyplanpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:10:31.000000 pyplanpro-0.0.9/pyplanpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 07:10:31.000000 pyplanpro-0.0.9/pyplanpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 07:10:31.000000 pyplanpro-0.0.9/pyplanpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:10:31.361820 pyplanpro-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:31.361820 pyplanpro-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:31.361820 pyplanpro-0.0.9/tests/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/tests/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/tests/scheduler/test_heuristic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:10:14.000000 pyplanpro-0.0.9/tests/scheduler/test_scheduler.py
```

### Comparing `pyplanpro-0.0.6/LICENSE` & `pyplanpro-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.6/PKG-INFO` & `pyplanpro-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.6
+Version: 0.0.9
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyplanpro-0.0.6/PyPlanPro/models/resource.py` & `pyplanpro-0.0.9/PyPlanPro/models/resource.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.6/PyPlanPro/models/resource_group.py` & `pyplanpro-0.0.9/PyPlanPro/models/resource_group.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.6/PyPlanPro/models/task.py` & `pyplanpro-0.0.9/PyPlanPro/models/task.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.6/PyPlanPro/scheduler/heuristic_solver.py` & `pyplanpro-0.0.9/PyPlanPro/scheduler/heuristic_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         resource_interval_trees = self._get_resource_interval_trees(self.resources)
 
         unscheduled_tasks = []
         for i, task_id in enumerate(task_ids_ordered):
             task = task_dict[task_id]
             # get earliest start from max predecessors end
             task_earliest_start = self._get_task_earliest_start(task_vars, task)
+            if task_earliest_start is None:
+                unscheduled_tasks.append(task.id)
+                self._update_task_vars_unscheduled(task_vars, task)
+                continue
 
             # find the resource who completes the task first
             fastest_resource = self._get_fastest_resource(task,resource_interval_trees, task_earliest_start)
             if fastest_resource is None:
                 unscheduled_tasks.append(task.id)
                 self._update_task_vars_unscheduled(task_vars, task)
                 continue
@@ -55,17 +59,28 @@
             "task_start": fastest_resource["task_start"],
             "task_end": fastest_resource["task_end"],
             "task_intervals": [(interval.begin, interval.end) for interval in sorted(fastest_resource["task_interval_tree"])]
         }
         task_vars[task.id] = task_values
 
     def _get_task_earliest_start(self, task_vars, task):
-        predecessor_max_end = max((task_vars[pred.id].get('task_end',0) for pred in task.predecessors), default=0)
-        return predecessor_max_end + task.predecessor_delay
+        # If there are no predecessors, return task.predecessor_delay
+        if not task.predecessors:
+            return 0
+
+        # find max predecessor end. If one pred is none then return none
+        max_task_end = 0
+        for pred in task.predecessors:
+            task_end = task_vars[pred.id].get('task_end')
+            if task_end is None:
+                return None
+            max_task_end = max(max_task_end, task_end)
 
+        return max_task_end + task.predecessor_delay
+ 
     def _get_task_order(self, tasks):
         """
         Returns a list of task IDs in the order required to complete them as quickly as possible while considering task priorities.
 
         :param tasks: List of tasks with durations, predecessors, and priorities.
         :return: List of task IDs in the order required to complete them as quickly as possible while considering task priorities.
         """
```

### Comparing `pyplanpro-0.0.6/PyPlanPro/scheduler/optimizer.py` & `pyplanpro-0.0.9/PyPlanPro/scheduler/optimizer.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.6/PyPlanPro/scheduler/scheduler_result.py` & `pyplanpro-0.0.9/PyPlanPro/scheduler/scheduler_result.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.6/README.md` & `pyplanpro-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.6/pyplanpro.egg-info/PKG-INFO` & `pyplanpro-0.0.9/pyplanpro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.6
+Version: 0.0.9
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyplanpro-0.0.6/pyplanpro.egg-info/SOURCES.txt` & `pyplanpro-0.0.9/pyplanpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.6/setup.py` & `pyplanpro-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
 setup(
     name='pyplanpro',
-    version='0.0.6',
+    version='0.0.9',
     author='Jacob Østergaard Nielsen',
     author_email='jaoe@oestergaard-as.dk',
     description='Task scheduler for python',
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
     url='https://github.com/Oestergaard-A-S/PyPlanPro',
     install_requires= read_requirements("requirements.txt"),
```

### Comparing `pyplanpro-0.0.6/tests/scheduler/test_heuristic_solver.py` & `pyplanpro-0.0.9/tests/scheduler/test_heuristic_solver.py`

 * *Files identical despite different names*

