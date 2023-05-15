# Comparing `tmp/lognflow-0.6.8.tar.gz` & `tmp/lognflow-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.6.8.tar", last modified: Fri May  5 00:43:21 2023, max compression
+gzip compressed data, was "lognflow-0.7.0.tar", last modified: Mon May 15 01:23:53 2023, max compression
```

## Comparing `lognflow-0.6.8.tar` & `lognflow-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.962096 lognflow-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-05 00:42:57.000000 lognflow-0.6.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-05 00:42:57.000000 lognflow-0.6.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-05 00:42:57.000000 lognflow-0.6.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-05 00:42:57.000000 lognflow-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 00:42:57.000000 lognflow-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-05 00:43:21.962096 lognflow-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-05 00:42:57.000000 lognflow-0.6.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.958096 lognflow-0.6.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.962096 lognflow-0.6.8/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 00:42:57.000000 lognflow-0.6.8/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69466 2023-05-05 00:42:57.000000 lognflow-0.6.8/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-05 00:42:57.000000 lognflow-0.6.8/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-05 00:42:57.000000 lognflow-0.6.8/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.962096 lognflow-0.6.8/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-05 00:43:21.962096 lognflow-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-05 00:42:57.000000 lognflow-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.962096 lognflow-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-05 00:42:57.000000 lognflow-0.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-05 00:42:57.000000 lognflow-0.6.8/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-05 00:42:57.000000 lognflow-0.6.8/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-05 00:42:57.000000 lognflow-0.6.8/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.990351 lognflow-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 01:23:31.000000 lognflow-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-15 01:23:31.000000 lognflow-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-15 01:23:31.000000 lognflow-0.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-15 01:23:31.000000 lognflow-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-15 01:23:31.000000 lognflow-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-15 01:23:53.990351 lognflow-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-15 01:23:31.000000 lognflow-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.986351 lognflow-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.986351 lognflow-0.7.0/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 01:23:31.000000 lognflow-0.7.0/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70856 2023-05-15 01:23:31.000000 lognflow-0.7.0/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-05-15 01:23:31.000000 lognflow-0.7.0/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-15 01:23:31.000000 lognflow-0.7.0/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.986351 lognflow-0.7.0/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-15 01:23:53.990351 lognflow-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-15 01:23:31.000000 lognflow-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.986351 lognflow-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 01:23:31.000000 lognflow-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-15 01:23:31.000000 lognflow-0.7.0/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-15 01:23:31.000000 lognflow-0.7.0/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-15 01:23:31.000000 lognflow-0.7.0/tests/test_printprogress.py
```

### Comparing `lognflow-0.6.8/CONTRIBUTING.rst` & `lognflow-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/HISTORY.rst` & `lognflow-0.7.0/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -75,12 +75,11 @@
 * A bug in tifffile support was fixed
 
 0.6.8 (2023-05-04)
 ------------------
 * Fixing readme for PyPI.
 * removed marker from log_plot. user marker and linestyle keyword arguments.
 * printprogress returns proper ETA every time if print_function is set to None::
-    pBar = printprogress(N, print_function = None)
-    for _ in range(N):
-        ETA = pBar()
-        print(f'ETA: {ETA}')
 
+0.7.0 (2023-05-15)
+------------------
+* logviewer returns data by log_sigle if the full name is mentioned.
```

### Comparing `lognflow-0.6.8/LICENSE` & `lognflow-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/PKG-INFO` & `lognflow-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.8
+Version: 0.7.0
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -167,12 +167,11 @@
 * A bug in tifffile support was fixed
 
 0.6.8 (2023-05-04)
 ------------------
 * Fixing readme for PyPI.
 * removed marker from log_plot. user marker and linestyle keyword arguments.
 * printprogress returns proper ETA every time if print_function is set to None::
-    pBar = printprogress(N, print_function = None)
-    for _ in range(N):
-        ETA = pBar()
-        print(f'ETA: {ETA}')
 
+0.7.0 (2023-05-15)
+------------------
+* logviewer returns data by log_sigle if the full name is mentioned.
```

### Comparing `lognflow-0.6.8/README.rst` & `lognflow-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/docs/Makefile` & `lognflow-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/docs/conf.py` & `lognflow-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/docs/installation.rst` & `lognflow-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/docs/make.bat` & `lognflow-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/lognflow/lognflow.py` & `lognflow-0.7.0/lognflow/lognflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,19 @@
         :type log_dir: pathlib.Path
     
         :param log_prefix:
             this string will be put before the time tag for log_dir, when
             only logs_root is given.
         :type log_prefix: str
         
+        :param log_suffix:
+            if given, time tag will not be used and this string will be 
+            put at the end of the log_dir name.
+        :type log_prefix: str
+        
         :param print_text: 
             If True, everything that is logged as text will be printed as well
         :type print_text: bool
         
         :param main_log_name: 
             main log file name, by default: 'main_log'
         :type main_log_name: str
@@ -120,40 +125,45 @@
             log_... functions.
         :type time_tag: bool
     """
     
     def __init__(self, 
                  logs_root        : pathlib.Path = None,
                  log_dir          : pathlib.Path = None,
-                 log_prefix       : str          = None,
+                 log_dir_prefix   : str          = None,
+                 log_dir_suffix   : str          = None,
                  print_text       : bool         = True,
                  main_log_name    : str          = 'main_log',
                  log_flush_period : int          = 10,
                  time_tag         : bool         = True):
         self._init_time = time.time()
         self.time_tag = time_tag
-
+        self.log_dir_prefix = log_dir_prefix
+        self.log_dir_suffix = log_dir_suffix
+        
         if(log_dir is None):
             if(logs_root is None):
                 from tempfile import gettempdir
                 logs_root = gettempdir()
                 try:
                     logs_root = select_directory(logs_root)
                 except:
                     pass
-            
             new_log_dir_found = False
             while(not new_log_dir_found):
                 log_dir_name = ''
-                if(log_prefix is not None):
-                    log_dir_name = str(log_prefix)
-                    if len(log_dir_name) > 0:
-                        if log_dir_name[-1] != '_':
-                            log_dir_name += '_'
-                log_dir_name += f'{self._init_time}/'
+                if(log_dir_prefix is not None):
+                    log_dir_name = str(log_dir_prefix)
+                if len(log_dir_name) > 0:
+                    if log_dir_name[-1] != '_':
+                        log_dir_name += '_'
+                if(log_dir_suffix is None):
+                    log_dir_name += f'{self._init_time}'
+                else:
+                    log_dir_name += f'{log_dir_suffix}'
                 self.log_dir = \
                     pathlib.Path(logs_root) / log_dir_name
                 if(not self.log_dir.is_dir()):
                     new_log_dir_found = True
                 else:
                     self._init_time = time.time()
         else:
@@ -167,34 +177,60 @@
         self._loggers_dict = {}
         self._vars_dict = {}
         self._single_var_call_cnt = 0
 
         self.log_name = main_log_name
         self.log_flush_period = log_flush_period
     
+    @property
+    def time_stamp(self):
+        return time.time() - self._init_time
+    
     def rename(self, new_name:str, append: bool = False):
         """ renaming the log directory
             It is possible to rename the log directory while logging is going
             on. This is particulary useful when at the end of an experiment,
             it is necessary to put some variables in the name of the directory,
             which is very realistic in the eyes of an experimentalist.
             
             There is only one input and that is the new name of the directory.
 
             :param new_name: The new name of the directory (without parent path)
             :type new_name: str
             
-            :param append: keep the time tag for the folder. Default: False.
+            :param append: keep the time tag for the folder and 
+                append it to the right side of the new name. Default: False.
             :type append: bool
             
         """
         self.flush_all()
         if(append):
-            new_name += '_' + self.log_dir.name
-        new_dir = self.log_dir.parent / new_name
+            log_dir_name = ''
+            if(self.log_dir_prefix is not None):
+                log_dir_name = str(self.log_dir_prefix)
+            if len(log_dir_name) > 0:
+                if log_dir_name[-1] != '_':
+                    log_dir_name += '_'
+            if(self.log_dir_suffix is None):
+                log_dir_name_with_suffix = log_dir_name + f'{self._init_time}'
+            else:
+                log_dir_name_with_suffix = log_dir_name + f'{self.log_dir_suffix}'
+            if self.log_dir.name == log_dir_name_with_suffix:
+                log_dir_name += new_name
+                if log_dir_name[-1] != '_':
+                    log_dir_name += '_'
+                if(self.log_dir_suffix is None):
+                    log_dir_name += f'{self._init_time}'
+                else:
+                    log_dir_name += f'{self.log_dir_suffix}'
+            else:
+                log_dir_name = self.log_dir.name + '_' + new_name
+        else:
+            log_dir_name = new_name        
+        new_dir = self.log_dir.parent / log_dir_name
         try:
             self.log_dir = self.log_dir.rename(new_dir)
             for log_name in list(self._loggers_dict):
                 curr_textinlog = self._loggers_dict[log_name]
                 curr_textinlog.log_fpath = \
                     self.log_dir /curr_textinlog.log_fpath.name
         except:
@@ -237,27 +273,26 @@
                           f'Creating directory: {param_dir.absolute()}')
             param_dir.mkdir(parents = True, exist_ok = True)
         return(param_dir, param_name)
 
     def _get_fpath(self, param_dir: pathlib.Path, param_name: str, 
                    save_as: str, time_tag: bool = None) -> pathlib.Path:
         
-        time_time = time.time() - self._init_time
         time_tag = self.time_tag if (time_tag is None) else time_tag
         
         if(save_as == 'mat'):
             if(len(param_name) == 0):
                 param_name = param_dir.name
         
         if(len(param_name) > 0):
             fname = f'{param_name}'
             if(time_tag):
-                fname += f'_{time_time:>6.6f}'
+                fname += f'_{self.time_stamp:>6.6f}'
         else:
-            fname = f'{time_time:>6.6f}'
+            fname = f'{self.time_stamp:>6.6f}'
             
         return(param_dir / f'{fname}.{save_as}')
         
     def _log_text_handler(self, log_name = None, 
                          log_size_limit: int = int(1e+7),
                          time_tag: bool = None,
                          log_flush_period = None):
@@ -285,28 +320,26 @@
             while.
             In later versions, a timer will be used to call it automatically.
             :param flush:
                 force the flush regardless of when the last time was.
                 default: False
             :type flush: bool
         """
-        time_time = time.time() - self._init_time
-
         log_name = self.log_name if (log_name is None) else log_name
         curr_textinlog = self._loggers_dict[log_name]
         
-        if((time_time - curr_textinlog.last_log_flush_time \
+        if((self.time_stamp - curr_textinlog.last_log_flush_time \
                                            > curr_textinlog.log_flush_period)
            | flush):
             
             with open(curr_textinlog.log_fpath, 'a+') as f:
                 f.writelines(curr_textinlog.to_be_logged)
                 f.flush()
             curr_textinlog.to_be_logged = []
-            curr_textinlog.last_log_flush_time = time_time
+            curr_textinlog.last_log_flush_time = self.time_stamp
 
     def log_text(self, 
                  log_name: str = None,
                  to_be_logged = '', 
                  log_time_stamp = True,
                  print_text = None,
                  log_size_limit: int = int(1e+7),
@@ -346,37 +379,35 @@
             :param end: str
                    The last charachter for this call.
             :param new_file: bool
                    if a new file is needed. If time_tag is True, it will make
                    a new file with a new name that has a time tag. If False,
                    it closees the current text file and overwrites on it.
         """
-        time_time = time.time() - self._init_time
-
         time_tag = self.time_tag if (time_tag is None) else time_tag
         log_flush_period = self.log_flush_period \
             if (log_flush_period is None) else log_flush_period
         log_name = self.log_name if (log_name is None) else log_name
 
         if((print_text is None) | (print_text is True)):
             print_text = self._print_text
         if(print_text):
             if(log_time_stamp):
-                print(f'T:{time_time:>6.6f}| ', end='')
+                print(f'T:{self.time_stamp:>6.6f}| ', end='')
             print(to_be_logged)
                 
         if ( (not (log_name in self._loggers_dict)) or new_file):
             self._log_text_handler(log_name, 
                                    log_size_limit = log_size_limit,
                                    time_tag = time_tag)
 
         curr_textinlog = self._loggers_dict[log_name]
         _logger = []
         if(log_time_stamp):
-            _time_str = f'T:{time_time:>6.6f}| '
+            _time_str = f'T:{self.time_stamp:>6.6f}| '
             _logger.append(_time_str)
         if(isinstance(to_be_logged, list)):
             for _ in to_be_logged:
                 _tolog = str(_)
                 _logger.append(_tolog)
         else:
             _tolog = str(to_be_logged)
@@ -425,17 +456,14 @@
                     An np array whose size doesn't change
             :param save_as: str
                     can be 'npz' or 'txt' which will save it as text.
             :param log_size_limit: int
                     log_size_limit in bytes, default: 1e+7.
                     
         """
-        
-        time_time = time.time() - self._init_time
-        
         try:
             _ = parameter_value.shape
         except:
             parameter_value = np.array([parameter_value])
         
         log_counter_limit = self._get_log_counter_limit(\
             parameter_value, log_size_limit)
@@ -444,29 +472,29 @@
             _var = self._vars_dict[parameter_name]
             data_array, time_array, curr_index, \
                 file_start_time, save_as, log_counter_limit = \
                 (_var.data_array, _var.time_array, _var.curr_index, \
                     _var.file_start_time, _var.save_as, _var.log_counter_limit)
             curr_index += 1
         else:
-            file_start_time = time.time()
+            file_start_time = self.time_stamp
             curr_index = 0
 
         if(curr_index >= log_counter_limit):
             self.log_var_flush(parameter_name)
-            file_start_time = time.time()
+            file_start_time = self.time_stamp
             curr_index = 0
 
         if(curr_index == 0):
             data_array = np.zeros((log_counter_limit, ) + parameter_value.shape,
                                   dtype = parameter_value.dtype)
             time_array = np.zeros(log_counter_limit)
         
         try:
-            time_array[curr_index] = time_time
+            time_array[curr_index] = self.time_stamp
         except:
             self.log_text(
                 self.log_name,
                 f'current index {curr_index} cannot be used in the logger')
         if(parameter_value.shape == data_array[curr_index].shape):
             data_array[curr_index] = parameter_value
         else:
@@ -1565,15 +1593,15 @@
                           for common_stem in common_stems]
 
         return(flist_A_new, flist_B_new)
     
     def replace_time_with_index(self, var_name):
         """ index in file names
             lognflow uses time stamps to make new log files for a variable.
-            That is done by putting _time_stamp after the name of the variable.
+            That is done by putting time stamp after the name of the variable.
             This function changes all of the time stamps, sorted ascendingly,
             by indices.
             
             :param var_name:
                 variable name
         """
         var_dir = self.log_dir / var_name
```

### Comparing `lognflow-0.6.8/lognflow/logviewer.py` & `lognflow-0.7.0/lognflow/logviewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 pass
         else:
             self.logger(f'{var_name} not found.')
             return
     
     def get_stack_of_files(self, 
         var_name = None, flist = [], suffix = None,
-        return_data = False, return_flist = True,
+        return_data = False, return_flist = True, read_func = None,
         verbose = True):
         
         """ Get list or data of all files in a directory
         
             This function gives the list of paths of all files in a directory
             for a single variable. 
 
@@ -187,22 +187,23 @@
                 It returns a tuple, (dataset, flist),
                 dataset will be a numpy array in case all files produce same
                 shape numpy arrays.
                 flist is type pathlib.Path
             
         """
         if suffix is None:
-            if len(var_name.split('.')) > 1:
-                suffix = var_name.split('.')[-1]
-                name_before_suffix = var_name.split('.')[:-1]
+            var_name_split = var_name.split('.')
+            if len(var_name_split) > 1:
+                suffix = var_name_split[-1]
+                name_before_suffix = var_name_split[:-1]
                 if((len(name_before_suffix) == 1) & 
                    (name_before_suffix[0] == '')):
                     var_name = '*'
                 else:
-                    var_name = ('.').join(var_name.split('.')[:-1])
+                    var_name = ('.').join(var_name_split[:-1])
             else:
                 suffix = '*'
 
         suffix = suffix.strip('.')
         if not flist:
             assert var_name is not None, \
                 ' The file list is empty. Please provide the ' \
@@ -219,48 +220,47 @@
                     patt = patt.replace('**', '*')
                 flist = list(var_dir.glob(patt))
         if flist:
             flist.sort()
             n_files = len(flist)
             if((not return_data) & return_flist):
                 return(flist)
-            data_type = None
-            if(data_type is None):
+            
+            ######### asked for data ########
+            if(read_func is None):
                 try:
                     fdata = np.load(flist[0])
-                    data_type = 'numpy'
+                    read_func = np.load
                 except:
                     pass
-            if(data_type is None):
+            if(read_func is None):
                 try:
                     from matplotlib.pyplot import imread
                     fdata = imread(flist[0])
-                    data_type = 'image'
+                    read_func = plt.imread
                 except:
                     pass
-            if(data_type is not None):
+            if(read_func is not None):
+                fdata = read_func(flist[0])
                 dataset = np.zeros((n_files, ) + fdata.shape, 
                                    dtype=fdata.dtype)
                 for fcnt, fpath in enumerate(flist):
-                    if(data_type == 'numpy'):
-                        dataset[fcnt] = np.load(fpath)
-                    elif(data_type == 'image'):
-                        dataset[fcnt] = imread(fpath)
+                    dataset[fcnt] = read_func(fpath)
                 if(verbose):
                     self.logger(f'logviewer: Reading dataset from {var_dir}'
                                 f', the shape would be: {dataset.shape}')
                 if(return_flist):
                     return(dataset, flist)
                 else:
                     return(dataset)
             else:
                 if(verbose):
                     self.logger(f'File {flist[0].name} cannot be opened by '\
-                          + r'np.load() or plt.imread()')
-            
+                          + r'np.load() or plt.imread(), provide read_func.')
+
     def get_common_files(self, var_name_A, var_name_B):
         """ get common files in two directories
         
             It happens often in ML that there are two directories, A and B,
             and we are interested to get the flist in both that is common 
             between them. returns a tuple of two lists of files.
```

### Comparing `lognflow-0.6.8/lognflow/printprogress.py` & `lognflow-0.7.0/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/lognflow.egg-info/PKG-INFO` & `lognflow-0.7.0/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.8
+Version: 0.7.0
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -167,12 +167,11 @@
 * A bug in tifffile support was fixed
 
 0.6.8 (2023-05-04)
 ------------------
 * Fixing readme for PyPI.
 * removed marker from log_plot. user marker and linestyle keyword arguments.
 * printprogress returns proper ETA every time if print_function is set to None::
-    pBar = printprogress(N, print_function = None)
-    for _ in range(N):
-        ETA = pBar()
-        print(f'ETA: {ETA}')
 
+0.7.0 (2023-05-15)
+------------------
+* logviewer returns data by log_sigle if the full name is mentioned.
```

### Comparing `lognflow-0.6.8/lognflow.egg-info/SOURCES.txt` & `lognflow-0.7.0/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/setup.py` & `lognflow-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.6.8'
+__version__ = '0.7.0'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.6.8/tests/test_lognflow.py` & `lognflow-0.7.0/tests/test_lognflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,15 @@
 if __name__ == '__main__':
     
     #-----IF RUN BY PYTHON------#
     temp_dir = select_directory()
     #---------------------------#
     
     test_log_text()
+    exit()
     test_log_single_text()
     test_log_surface()
     test_log_single()
     test_lognflow_conflict_in_names()
     test_rename()
     test_log_plot()
     test_prepare_stack_of_images()
```

### Comparing `lognflow-0.6.8/tests/test_logviewer.py` & `lognflow-0.7.0/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.8/tests/test_printprogress.py` & `lognflow-0.7.0/tests/test_printprogress.py`

 * *Files identical despite different names*

