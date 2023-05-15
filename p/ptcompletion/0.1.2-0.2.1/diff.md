# Comparing `tmp/ptcompletion-0.1.2.tar.gz` & `tmp/ptcompletion-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcompletion-0.1.2.tar", last modified: Mon May 15 02:20:35 2023, max compression
+gzip compressed data, was "ptcompletion-0.2.1.tar", last modified: Mon May 15 06:42:12 2023, max compression
```

## Comparing `ptcompletion-0.1.2.tar` & `ptcompletion-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 phantivia  (1000) phantivia  (1000)        0 2023-05-15 02:20:35.537881 ptcompletion-0.1.2/
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)     1066 2023-05-15 02:14:58.000000 ptcompletion-0.1.2/LICENSE
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      791 2023-05-15 02:20:35.537881 ptcompletion-0.1.2/PKG-INFO
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      281 2023-05-15 02:14:58.000000 ptcompletion-0.1.2/README.md
-drwxrwxr-x   0 phantivia  (1000) phantivia  (1000)        0 2023-05-15 02:20:35.537881 ptcompletion-0.1.2/ptcompletion/
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)       92 2023-05-14 11:59:06.000000 ptcompletion-0.1.2/ptcompletion/__init__.py
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)     1176 2023-05-15 02:04:34.000000 ptcompletion-0.1.2/ptcompletion/openai_task.py
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)     1632 2023-05-15 02:01:27.000000 ptcompletion-0.1.2/ptcompletion/task.py
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)     3713 2023-05-14 11:59:37.000000 ptcompletion-0.1.2/ptcompletion/task_queue.py
-drwxrwxr-x   0 phantivia  (1000) phantivia  (1000)        0 2023-05-15 02:20:35.537881 ptcompletion-0.1.2/ptcompletion.egg-info/
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      791 2023-05-15 02:20:35.000000 ptcompletion-0.1.2/ptcompletion.egg-info/PKG-INFO
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      306 2023-05-15 02:20:35.000000 ptcompletion-0.1.2/ptcompletion.egg-info/SOURCES.txt
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)        1 2023-05-15 02:20:35.000000 ptcompletion-0.1.2/ptcompletion.egg-info/dependency_links.txt
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)        7 2023-05-15 02:20:35.000000 ptcompletion-0.1.2/ptcompletion.egg-info/requires.txt
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)       13 2023-05-15 02:20:35.000000 ptcompletion-0.1.2/ptcompletion.egg-info/top_level.txt
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)       38 2023-05-15 02:20:35.537881 ptcompletion-0.1.2/setup.cfg
--rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      841 2023-05-15 02:15:30.000000 ptcompletion-0.1.2/setup.py
+drwxrwxr-x   0 phantivia  (1000) phantivia  (1000)        0 2023-05-15 06:42:12.788413 ptcompletion-0.2.1/
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)     1066 2023-05-15 02:14:58.000000 ptcompletion-0.2.1/LICENSE
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      791 2023-05-15 06:42:12.788413 ptcompletion-0.2.1/PKG-INFO
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      281 2023-05-15 02:14:58.000000 ptcompletion-0.2.1/README.md
+drwxrwxr-x   0 phantivia  (1000) phantivia  (1000)        0 2023-05-15 06:42:12.788413 ptcompletion-0.2.1/ptcompletion/
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)       92 2023-05-14 11:59:06.000000 ptcompletion-0.2.1/ptcompletion/__init__.py
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)     1176 2023-05-15 02:04:34.000000 ptcompletion-0.2.1/ptcompletion/openai_task.py
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)     1632 2023-05-15 02:01:27.000000 ptcompletion-0.2.1/ptcompletion/task.py
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)     4160 2023-05-15 06:38:26.000000 ptcompletion-0.2.1/ptcompletion/task_queue.py
+drwxrwxr-x   0 phantivia  (1000) phantivia  (1000)        0 2023-05-15 06:42:12.788413 ptcompletion-0.2.1/ptcompletion.egg-info/
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      791 2023-05-15 06:42:12.000000 ptcompletion-0.2.1/ptcompletion.egg-info/PKG-INFO
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      306 2023-05-15 06:42:12.000000 ptcompletion-0.2.1/ptcompletion.egg-info/SOURCES.txt
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)        1 2023-05-15 06:42:12.000000 ptcompletion-0.2.1/ptcompletion.egg-info/dependency_links.txt
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)        7 2023-05-15 06:42:12.000000 ptcompletion-0.2.1/ptcompletion.egg-info/requires.txt
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)       13 2023-05-15 06:42:12.000000 ptcompletion-0.2.1/ptcompletion.egg-info/top_level.txt
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)       38 2023-05-15 06:42:12.788413 ptcompletion-0.2.1/setup.cfg
+-rw-rw-r--   0 phantivia  (1000) phantivia  (1000)      841 2023-05-15 06:42:03.000000 ptcompletion-0.2.1/setup.py
```

### Comparing `ptcompletion-0.1.2/LICENSE` & `ptcompletion-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcompletion-0.1.2/PKG-INFO` & `ptcompletion-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcompletion
-Version: 0.1.2
+Version: 0.2.1
 Summary: Parallel Tasks Completion for OpenAI API, and more.
 Home-page: https://github.com/Phantivia/OpenAI_PTCompletion
 Author: Phantivia
 Author-email: phantivia@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ptcompletion-0.1.2/ptcompletion/openai_task.py` & `ptcompletion-0.2.1/ptcompletion/openai_task.py`

 * *Files identical despite different names*

### Comparing `ptcompletion-0.1.2/ptcompletion/task.py` & `ptcompletion-0.2.1/ptcompletion/task.py`

 * *Files identical despite different names*

### Comparing `ptcompletion-0.1.2/ptcompletion/task_queue.py` & `ptcompletion-0.2.1/ptcompletion/task_queue.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 import time
 from datetime import datetime
 from multiprocessing import Manager, Pool, Process, cpu_count, RLock
 from typing import Tuple
 
-from .task import Task
+from ptcompletion import Task
 
 
 class TaskQueue:
-    def __init__(self, requests_per_minute: int = 60, max_rounds: int = 3, log_file: str = "tasks.log") -> None:
+    def __init__(self, requests_per_minute: int = 60, max_rounds: int = 3, max_requests_per_proc = 16, log_file: str = "tasks.log") -> None:
         self.requests_per_minute = requests_per_minute
         manager = Manager()
-        self.token_bucket = manager.Value("i", 1)
+        self.quota_bucket = manager.Value("f", 1)
         self.max_rounds = max_rounds
         self.log_file = log_file
         self.token_mutex = manager.Lock()
         self.log_mutex = manager.Lock()
         self.token_request_queue = manager.Queue()
+        
+        self.max_requests_per_proc = max_requests_per_proc
+        
+        if self.requests_per_minute <= 60:
+            
+            self.fill_token_interval = 60 / self.requests_per_minute
+            self.add = 1.0
+        else:
+            self.fill_token_interval = 1.0
+            self.add = self.requests_per_minute / 60
 
     def fill_token_bucket(self, token_request_queue):
-        fill_token_interval = 60 / self.requests_per_minute
         while True:
             if token_request_queue.get():
                 with self.token_mutex:
-                    if self.token_bucket.get() < self.requests_per_minute:
-                        
-                        self.token_bucket.set(self.token_bucket.get() + 1)
-                        time.sleep(fill_token_interval)
+                    self.quota_bucket.set(self.quota_bucket.get() + self.add)
+                    time.sleep(self.fill_token_interval)
 
     def fill_token_bucket_process(self):
         fill_token_process = Process(target=self.fill_token_bucket, args=(self.token_request_queue,))
         fill_token_process.daemon = True
         fill_token_process.start()
 
     def get_token(self):
         with self.token_mutex:
-            if self.token_bucket.get() > 0:
-                self.token_bucket.set(self.token_bucket.get() - 1)
-                return True
+            quota = self.quota_bucket.get()
+            if quota > 1.0:
+                tokens = int(quota)
+                self.quota_bucket.set(quota - tokens)
+                return tokens
             else:
                 self.token_request_queue.put(True)
-                return False
+                return 0
 
     def start(self, tasks: list[Task]) -> None:
         
         if not tasks:
             return
         
         self.fill_token_bucket_process()
@@ -53,25 +62,27 @@
         
         all_start_time = time.time()
 
         for epoch in range(self.max_rounds):
             
             round_start_time = time.time()
 
-            with Pool(processes=cpu_count()) as pool:
+            with Pool(processes=cpu_count() * self.max_requests_per_proc) as pool:
                 round_tasks = []
 
                 while task_queue:
-                    if not self.get_token():  # Try to apply for token
+                    tokens = self.get_token()# Try to apply for token
+                    if tokens == 0:  
                         time.sleep(0.01)
-                        continue
-
-                    task = task_queue.pop(0)
-                    
-                    round_tasks.append(pool.apply_async(self.process_task, (task, )))
+                    else:
+                        for t in range(tokens):
+                            task = task_queue.pop(0)
+                            round_tasks.append(pool.apply_async(self.process_task, (task, )))
+                            if not task_queue:
+                                break
 
                 for result in round_tasks:
                     task = result.get()
 
                     if not task.completed:
                         task_queue.append(task)
                     if task.completed:
@@ -92,13 +103,12 @@
         task.run()
         self.log(f"Task {task.id} {'Completed' if task.completed else 'Failed'} in {round(time.time() - start_time, 3)} seconds.")
         
         return task
 
     def log(self, msg) -> None:
         
-        msg = f"[{datetime.now()}] " + msg 
-        print(msg)
-        
+        msg = f"[{datetime.now()}] " + msg + "\n"
         with self.log_mutex:
+            print(msg)
             with open(self.log_file, "a") as log_file:
-                log_file.write(msg + "\n")
+                log_file.write(msg)
```

### Comparing `ptcompletion-0.1.2/ptcompletion.egg-info/PKG-INFO` & `ptcompletion-0.2.1/ptcompletion.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcompletion
-Version: 0.1.2
+Version: 0.2.1
 Summary: Parallel Tasks Completion for OpenAI API, and more.
 Home-page: https://github.com/Phantivia/OpenAI_PTCompletion
 Author: Phantivia
 Author-email: phantivia@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ptcompletion-0.1.2/setup.py` & `ptcompletion-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name='ptcompletion',
-    version='0.1.2',
+    version='0.2.1',
     description='Parallel Tasks Completion for OpenAI API, and more.',
     long_description=README,
     long_description_content_type="text/markdown",
     author='Phantivia',
     author_email='phantivia@gmail.com',
     packages=find_packages(),
     url = r'https://github.com/Phantivia/OpenAI_PTCompletion',
```

