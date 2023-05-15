# Comparing `tmp/robotframework-webservice-0.6.2.tar.gz` & `tmp/robotframework-webservice-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-webservice-0.6.2.tar", last modified: Tue May  9 20:45:05 2023, max compression
+gzip compressed data, was "robotframework-webservice-0.7.0.tar", last modified: Mon May 15 21:31:43 2023, max compression
```

## Comparing `robotframework-webservice-0.6.2.tar` & `robotframework-webservice-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/RobotFrameworkService/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/RobotFrameworkService/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/routers/robotframework.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:31:43.839557 robotframework-webservice-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-15 21:31:43.839557 robotframework-webservice-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:31:43.839557 robotframework-webservice-0.7.0/RobotFrameworkService/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/RobotFrameworkService/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/RobotFrameworkService/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/RobotFrameworkService/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/RobotFrameworkService/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:31:43.839557 robotframework-webservice-0.7.0/RobotFrameworkService/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/RobotFrameworkService/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/RobotFrameworkService/routers/robotframework.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/RobotFrameworkService/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:31:43.839557 robotframework-webservice-0.7.0/robotframework_webservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-15 21:31:43.000000 robotframework-webservice-0.7.0/robotframework_webservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-15 21:31:43.000000 robotframework-webservice-0.7.0/robotframework_webservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:31:43.000000 robotframework-webservice-0.7.0/robotframework_webservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:31:43.000000 robotframework-webservice-0.7.0/robotframework_webservice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 21:31:43.000000 robotframework-webservice-0.7.0/robotframework_webservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 21:31:43.000000 robotframework-webservice-0.7.0/robotframework_webservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:31:43.839557 robotframework-webservice-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 21:31:29.000000 robotframework-webservice-0.7.0/setup.py
```

### Comparing `robotframework-webservice-0.6.2/LICENSE` & `robotframework-webservice-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.2/PKG-INFO` & `robotframework-webservice-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-webservice
-Version: 0.6.2
+Version: 0.7.0
 Summary: Webservice for running Robot Framework tasks
 Home-page: https://github.com/MarketSquare/robotframework-webservice
 Author: Markus Stahl
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
```

### Comparing `robotframework-webservice-0.6.2/README.md` & `robotframework-webservice-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.2/RobotFrameworkService/Config.py` & `robotframework-webservice-0.7.0/RobotFrameworkService/Config.py`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.2/RobotFrameworkService/main.py` & `robotframework-webservice-0.7.0/RobotFrameworkService/main.py`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.2/RobotFrameworkService/routers/robotframework.py` & `robotframework-webservice-0.7.0/RobotFrameworkService/routers/robotframework.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,50 +7,73 @@
 from RobotFrameworkService.Config import Config as RFS_Config
 from ..constants import LOGS
 
 import robot
 
 router = APIRouter(
     prefix="/robotframework",
-    responses={404: {"description": "Not found"}},
+    responses={404: {"description": "Not found: Webservice is either busy or requested endpoint is not supported."}},
 )
 
 
 @router.get('/run/all', tags=["execution"])
 async def run(request: Request):
     """
     Run all task available.
     """
     id = request.headers["request-id"]
     result: int = _start_all_robot_tasks(id)
     if result == 0:
         result_page = 'PASS'
+        result_page += f'<p><a href="/logs/{id}/log.html">Go to log</a></p>'
         status_code = 200
     elif 250 >= result >= 1:
         result_page = f'FAIL: {result} tasks failed'
+        result_page += f'<p><a href="/logs/{id}/log.html">Go to log</a></p>'
         status_code = 400
     else:
         result_page = f'FAIL: Errorcode {result}'
         status_code = 500
-    result_page += f'<p><a href="/logs/{id}/log.html">Go to log</a></p>'
+    
     return Response(content=result_page, media_type="text/html", status_code=status_code)
 
 
 @router.get('/run/{task}', tags=["execution"])
 async def run_task(task, request: Request):
     """
     Run a given task.
     """
     id = request.headers["request-id"]
     variables = RequestHelper.parse_variables_from_query(request)
     result: int = _start_specific_robot_task(id, task, variables=variables)
     if result == 0:
         result_page = 'PASS'
+        result_page += f'<p><a href="/logs/{id}/log.html">Go to log</a></p>'
+        
     elif 250 >= result >= 1:
         result_page = f'FAIL: {result} tasks failed'
+        result_page += f'<p><a href="/logs/{id}/log.html">Go to log</a></p>'
+
+    else:
+        result_page = f'FAIL: Errorcode {result}'
+    
+    return Response(content=result_page, media_type="text/html")
+
+@router.get('/run/suite/{suite}', tags=["execution"])
+async def run_task(suite, request: Request):
+    """
+    Run a given suite.
+    """
+    id = request.headers["request-id"]
+    variables = RequestHelper.parse_variables_from_query(request)
+    result: int = _start_specific_robot_suite(id, suite, variables=variables)
+    if result == 0:
+        result_page = 'PASS'
+    elif 250 >= result >= 1:
+        result_page = f'FAIL: {result} tasks for suite {suite} failed'
     else:
         result_page = f'FAIL: Errorcode {result}'
     result_page += f'<p><a href="/logs/{id}/log.html">Go to log</a></p>'
     return Response(content=result_page, media_type="text/html")
 
 
 @router.get('/run_and_show/{task}', tags=["execution"], response_class=HTMLResponse)
@@ -124,14 +147,32 @@
         outputdir=f'logs/{id}',
         debugfile=config.debugfile,
         variable=variables,
         variablefile=variablefiles,
         consolewidth=120
     )
 
+def _start_specific_robot_suite(id: str, suite: str, variables: list=None) -> int:
+    config = RFS_Config().cmd_args
+    if variables is None:
+        variables = []
+    if config.variablefiles is None:
+        variablefiles = []
+    else:
+        variablefiles = config.variablefiles
+
+    return robot.run(
+        config.taskfolder,
+        suite=suite,
+        outputdir=f'logs/{id}',
+        debugfile=config.debugfile,
+        variable=variables,
+        variablefile=variablefiles,
+        consolewidth=120
+    )
 
 def _start_specific_robot_task(id: str, task: str, variables: list = None) -> int:
     config = RFS_Config().cmd_args
     if variables is None:
         variables = []
     if config.variablefiles is None:
         variablefiles = []
```

### Comparing `robotframework-webservice-0.6.2/robotframework_webservice.egg-info/PKG-INFO` & `robotframework-webservice-0.7.0/robotframework_webservice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-webservice
-Version: 0.6.2
+Version: 0.7.0
 Summary: Webservice for running Robot Framework tasks
 Home-page: https://github.com/MarketSquare/robotframework-webservice
 Author: Markus Stahl
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
```

### Comparing `robotframework-webservice-0.6.2/robotframework_webservice.egg-info/SOURCES.txt` & `robotframework-webservice-0.7.0/robotframework_webservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.2/setup.py` & `robotframework-webservice-0.7.0/setup.py`

 * *Files identical despite different names*

