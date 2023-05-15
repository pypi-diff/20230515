# Comparing `tmp/osais-1.0.42.tar.gz` & `tmp/osais-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-pyu0zaem\osais-1.0.42.tar", last modified: Fri May 12 12:48:18 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-fc5li7s8\osais-1.0.43.tar", last modified: Mon May 15 18:23:03 2023, max compression
```

## Comparing `osais-1.0.42.tar` & `osais-1.0.43.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 12:48:18.149699 osais-1.0.42/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.42/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-05-12 12:48:18.149699 osais-1.0.42/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.42/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 12:48:18.143175 osais-1.0.42/osais/
--rw-rw-rw-   0        0        0      777 2023-05-12 12:47:53.000000 osais-1.0.42/osais/__init__.py
--rw-rw-rw-   0        0        0    51840 2023-05-12 12:47:43.000000 osais-1.0.42/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:48:18.148689 osais-1.0.42/osais.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.42/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 12:48:18.149699 osais-1.0.42/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-05-12 12:47:59.000000 osais-1.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 18:23:03.843987 osais-1.0.43/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.43/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-05-15 18:23:03.842988 osais-1.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.43/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 18:23:03.836915 osais-1.0.43/osais/
+-rw-rw-rw-   0        0        0      962 2023-05-15 18:22:28.000000 osais-1.0.43/osais/__init__.py
+-rw-rw-rw-   0        0        0    52377 2023-05-15 18:22:20.000000 osais-1.0.43/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-05-15 18:23:03.841988 osais-1.0.43/osais.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.43/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 18:23:03.843987 osais-1.0.43/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-05-15 18:22:48.000000 osais-1.0.43/setup.py
```

### Comparing `osais-1.0.42/LICENSE` & `osais-1.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.42/PKG-INFO` & `osais-1.0.43/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.42
+Version: 1.0.43
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.42/osais/__init__.py` & `osais-1.0.43/osais/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.42"
+__version__="1.0.43"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
+from .osais import osais_isDebug
+from .osais import osais_isDocker
 from .osais import osais_isLocal
+from .osais import osais_isVirtualAI
 from .osais import osais_loadConfig
 from .osais import osais_getEnv
 from .osais import osais_getHarwareInfo
 from .osais import osais_getDirectoryListing
+from .osais import osais_downloadImage
 from .osais import osais_uploadeFileToS3
 from .osais import osais_getInfo
+from .osais import osais_getClientID
 from .osais import osais_resetGateway
 from .osais import osais_authenticateAI
 from .osais import osais_authenticateClient
 from .osais import osais_postRequest
 from .osais import osais_initParser
 from .osais import osais_runAI
 from .osais import osais_notify
```

### Comparing `osais-1.0.42/osais/osais.py` & `osais-1.0.43/osais/osais.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.42"
+__version__="1.0.43"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -32,16 +32,14 @@
 
 class NewFileHandler(FileSystemEventHandler):
     def __init__(self, fnOnFileCreated, _args):
         self.fnOnFileCreated = fnOnFileCreated
         self._args = _args
 
     def on_created(self, event):
-        global gS3Bucket
-        global gS3
 
         if event.is_directory:
             return
         if event.event_type == 'created':
             ## only notify if uid in the filename (otherwise we are getting notified of another AI's job !)
             if self._args["-uid"] in event.src_path:
                 self.fnOnFileCreated(os.path.dirname(event.src_path), os.path.basename(event.src_path), self._args)
@@ -49,14 +47,16 @@
                 ## also send to S3
                 osais_uploadeFileToS3(event.src_path, "output/")
 
 def start_observer_thread(path, fnOnFileCreated, _args):
 
     ## watch directory and call back if file was created
     def watch_directory(path, fnOnFileCreated, _args):    
+
+        print ("=> starting a watch on path: "+path+"\r\n")
         global gObserver
         if gObserver!=None:
             gObserver.stop()
         event_handler = NewFileHandler(fnOnFileCreated, _args)
         gObserver = Observer()
         gObserver.schedule(event_handler, path, recursive=False)
         gObserver.start()
@@ -106,19 +106,27 @@
             
 ## ------------------------------------------------------------------------
 #       System utils
 ## ------------------------------------------------------------------------
 
 def consoleLog(err): 
     msg=""
-    if hasattr(err, 'msg'):
-        msg=err.msg
-    else:
-        if err.args and err.args[0]:
-            msg=err.args[0]                      
+    try: 
+        if err["msg"]:
+            msg=err["msg"]
+    except: 
+        try: 
+            if err.msg:
+                msg=err.msg
+        except: 
+            try:
+                if err.args and err.args[0]:
+                    msg=err.args[0]         
+            except: 
+                msg="???"
     print("CRITICAL: "+msg)
 
 ## get a meaningful name for our machine
 def get_machine_name() :
     _machine=str (hex(uuid.getnode()))
     _isDocker=is_running_in_docker()
     if _isDocker:
@@ -313,31 +321,37 @@
     }
 
 ## ------------------------------------------------------------------------
 #       File / Image utils
 ## ------------------------------------------------------------------------
 
 ## downloads an image as file from external URL
-def downloadImage(url) :
+def osais_downloadImage(url) :
     import urllib.request
 
     # Determine the file name and extension of the image based on the URL.
     file_name, file_extension = os.path.splitext(url)
+    print ("will download image from "+url)
     
     # Define the local file path where the image will be saved.
     spliter='/'
     local_filename=file_name.split(spliter)[-1]
     local_file_path = f"./_input/{local_filename}{file_extension}"
-    
+
     # Download the image from the URL and save it locally.
-    urllib.request.urlretrieve(url, local_file_path)
+    response = urllib.request.urlopen(url)
+    image_data = response.read()
+    with open(local_file_path, 'wb') as f:
+        f.write(image_data)
+
     return f"{local_filename}{file_extension}"
 
 def osais_uploadeFileToS3(_filename, _dirS3): 
     global gS3
+    global gS3Bucket
 
     if gS3!=None:
         try:
             # Filename - File to upload
             # Bucket - Bucket to upload to (the top level directory under AWS S3)
             # Key - S3 object name (can contain subdirectories). If not specified then file_name is used
             gS3.meta.client.upload_file(Filename=_filename, Bucket=gS3Bucket, Key=_dirS3+os.path.basename(_filename))
@@ -362,15 +376,15 @@
 import schedule
 import json
 import sys
 import base64
 from datetime import datetime
 import argparse
 
-## from osais_utils import getHostInfo, listDirContent, is_running_in_docker, get_external_ip, get_container_ip, get_machine_name, get_os_name, getCudaInfo, downloadImage, start_observer_thread, clearOldFiles, start_notification_thread
+##from osais import osais_initializeAI, osais_getInfo, osais_getHarwareInfo, osais_isDocker, osais_getClientID, osais_getDirectoryListing, osais_runAI, osais_authenticateAI, osais_isDebug, osais_authenticateClient, osais_postRequest, osais_downloadImage, osais_uploadeFileToS3
 
 ## ------------------------------------------------------------------------
 #       all global vars
 ## ------------------------------------------------------------------------
 
 gVersionLibOSAIS=__version__    ## version of this library (to keep it latest everywhere)
 gUsername=None                  ## user owning this AI (necessary to claim VirtAI regs)
@@ -379,49 +393,47 @@
 gVersion="0.0.0"                ## name of this AI's version (version of engine)
 gDescription=None               ## AI's quick description
 gOrigin=None                    ## where this AI came from (on internet)
 gMachineName=get_machine_name() ## the name of the machine (will change all the time if inside docker, ot keep same if running on local server)
 gLastChecked_at=datetime.utcnow()  ## when was this AI last used for processing anything
 gLastProcessStart_at=None       ## when was this AI last start event for processing anything
 
-## authenticate into OSAIS
-gAuthToken=None                 ## auth token into OSAIS for when working as virtual Ai
-gToken=None                     ## token used for authentication into OSAIS
-gSecret=None                    ## secret used for authentication into OSAIS
-gOriginOSAIS=None               ## location of OSAIS
-
-## authenticate into a local OSAIS (debug)
-gAuthTokenLocal=None            ## auth token into a local OSAIS (debug) for when working as virtual Ai
-gTokenLocal=None                ## token used for authentication into a local OSAIS (debug)
-gSecretLocal=None               ## secret used for authentication into a local OSAIS (debug)
-gOriginLocalOSAIS=None          ## location of a local OSAIS (debug)
-gClientID=None                  ## ID to authenticate as client into OSAIS (using the ai page to request AI processing)
-gClientSecret=None              ## Pwd to authenticate as client into OSAIS (using the ai page to request AI processing)
+## virtual AI / local /docker ? note: AI can act BOTH at the same time as VirtualAI and a LocalAI for a gateway
+gIsDocker=is_running_in_docker()   ## are we running in a Docker?
+gIsVirtualAI=False              ## are we working as a Virtual AI config?
+gIsLocal=False                  ## are we working locally (with a gateway)?
+gIsDebug=False                  ## are we working in debug (localhost server)? note: we cannot be PROD and DEBUG at the same time
+
+## OSAIS location
+gOriginOSAIS=None               ## location of OSAIS (Prod or debug)
+
+## authenticate into OSAIS as a VAI
+gVAIToken=None                  ## VAI token used for authentication into OSAIS
+gVAISecret=None                 ## VAI secret used for authentication into OSAIS
+gVAIAuthToken=None              ## authToken into OSAIS for when working as virtual AI
+
+## authenticate into OSAIS as a CLIENT (most likely DEMO CLIENT)
+gClientID=None                  ## ID of authenticated client into OSAIS 
 gClientAuthToken=None           ## the resulting Auth token as Client, after login
-gClientAuthTokenLocal=None      ## the resulting Auth token as Client, after login (for debug)
 
+## Gateway
 gOriginGateway=None             ## location of the local gateway for this (local) AI
 
 ## AWS related
 gS3=None
 gS3Bucket=None
 gAWSSession=None
 
 ## IP and Ports
 gExtIP=get_external_ip()        ## where this AI can be accessed from outside (IP)
 gIPLocal=get_container_ip()     ## where this AI can be accessed locally
 gPortAI=None                    ## port where this AI is accessed (will be set by AI config)
 gPortGateway=3023               ## port where the gateway can be accessed
 gPortLocalOSAIS=3022            ## port where a local OSAIS can be accessed
 
-## virtual AI / local /docker ?
-gIsDocker=is_running_in_docker()   ## are we running in a Docker?
-gIsVirtualAI=False              ## are we working as a Virtual AI config?
-gIsLocal=False                  ## are we working locally (localhost server)?
-
 ## temp cache
 gAProcessed=[]                  ## all token being sent to processing (never call twice for same)
 gIsScheduled=False              ## do we have a scheduled event running?
 
 ## run times
 gIsWarmup=False                 ## True if the request was a warmup one (not a true one from client)
 gIsBusy=False                   ## True if AI busy processing
@@ -476,144 +488,174 @@
     return _json
 
 # get the full AI config, including JSON params and hardware info
 def _getFullConfig(_name) :
     global gUsername
     global gPortAI
     global gName
-    global gToken
-    global gSecret
+    global gVAIToken
+    global gVAISecret
     global gOriginOSAIS
-    global gTokenLocal
-    global gSecretLocal
-    global gOriginLocalOSAIS
     global gIsVirtualAI
     global gIPLocal
     global gExtIP
     global gIsLocal
  
     _ip=gExtIP
-    if gIsVirtualAI==False:
+    if gIsDebug:
         _ip=gIPLocal                ## we register with local ip if we are in local gateway mode
 
     _jsonAI=_loadConfig(_name)
     _jsonBase=_loadConfig("osais")
 
     objCudaInfo=getCudaInfo()
     gpuName="no GPU"
     if objCudaInfo != 0 and "name" in objCudaInfo and objCudaInfo["name"]:
         gpuName=objCudaInfo["name"]
-    _osais="https://opensourceais.com/"
-    if gIsLocal: 
-        _osais="http://"+_ip+":3022/"
 
     return {
         "username": gUsername,
         "os": get_os_name(),
         "gpu": gpuName,
         "machine": get_machine_name(),
         "ip": _ip,
         "port": gPortAI,
-        "osais": _osais,
+        "osais": gOriginOSAIS,
         "gateway": "http://"+_ip+":3023/",
         "config_ai": _jsonAI,
         "config_base": _jsonBase
     }
 
-## PUBLIC - are we running locally?
+## PUBLIC - are we running in DEBUG mode?
+def osais_isDebug():
+    global gIsDebug
+    return gIsDebug
+
+## PUBLIC - are we running in local mode?
 def osais_isLocal():
     global gIsLocal
     return gIsLocal
 
+## PUBLIC - are we running in VAI mode?
+def osais_isVirtualAI():
+    global gIsVirtualAI
+    return gIsVirtualAI
+
 ## PUBLIC - load the config of this AI
 def osais_loadConfig(_name): 
     return _loadConfig(_name)
 
 ## PUBLIC - Get env from file (local or docker)
 def osais_getEnv(_filename):
     global gUsername
-    global gDemoID
-    global gDemoSecret
     global gIsVirtualAI
+    global gIsDebug
     global gIsLocal
     global gName
+    global gVAIToken
+    global gVAISecret
     global gAWSSession
     global gS3
     global gS3Bucket
+    global gOriginOSAIS
 
     AWSID=None
     AWSSecret=None
 
     ## read env from config file
-    try:
-        with open(_filename, "r") as f:
-            content = f.read()
-        print(f'Reading env vars from {_filename}')
-        variables = content.split("\n")
-        for var in variables:
-            if var!="":
-                key, value = var.split("=")
-                if key == "USERNAME":
-                    gUsername = value
-                elif key == "IS_LOCAL":
-                    gIsLocal = (value=="True")
-                elif key == "IS_VIRTUALAI":
-                    gIsVirtualAI = (value=="True")
-                elif key == "ENGINE":
-                    gName = value
-                elif key == "S3_BUCKET":
-                    gS3Bucket = value
-                elif key == "AWS_ACCESS_KEY_ID":
-                    AWSID = value
-                elif key == "AWS_ACCESS_KEY_SECRET":
-                    AWSSecret = value
-    except Exception as err: 
-        print(f'No env file {_filename}')
+    if _filename!=None:
+        try:
+            with open(_filename, "r") as f:
+                content = f.read()
+            print(f'=> Reading env vars from {_filename}')
+            variables = content.split("\n")
+            for var in variables:
+                if var!="":
+                    key, value = var.split("=")
+                    if key == "USERNAME":
+                        gUsername = value
+                    elif key == "IS_DEBUG":
+                        gIsDebug = (value=="True")
+                    elif key == "IS_LOCAL":
+                        gIsLocal = (value=="True")
+                    elif key == "IS_VIRTUALAI":
+                        gIsVirtualAI = (value=="True")
+                    elif key == "ENGINE":
+                        gName = value
+                    elif key == "S3_BUCKET":
+                        gS3Bucket = value
+                    elif key == "VAI_ID":
+                        gVAIToken = value
+                    elif key == "VAI_SECRET":
+                        gVAISecret = value
+                    elif key == "AWS_ACCESS_KEY_ID":
+                        AWSID = value
+                    elif key == "AWS_ACCESS_KEY_SECRET":
+                        AWSSecret = value
+        except Exception as err: 
+            consoleLog({"msg": f'No env file {_filename}'})
 
     # overload with env settings if any
+    print(f'=> Setting env vars from ENV...')
+    if os.environ.get('IS_DEBUG'):
+        _isDebug=(os.environ.get('IS_DEBUG')=="True")
+        if _isDebug!=gIsDebug:
+            print(f'=> is DEBUG updated to {_isDebug} from ENV var')
+            gIsDebug=_isDebug
     if os.environ.get('IS_LOCAL'):
         _isLocal=(os.environ.get('IS_LOCAL')=="True")
         if _isLocal!=gIsLocal:
-            print(f'is Local updated to {_isLocal} from ENV var')
+            print(f'=> is Local updated to {_isLocal} from ENV var')
             gIsLocal=_isLocal
     if os.environ.get('IS_VIRTUALAI'):
         _isVirtualAI=(os.environ.get('IS_VIRTUALAI')=="True")
         if _isVirtualAI!=gIsVirtualAI:
-            print(f'is Virtual updated to {_isVirtualAI} from ENV var')
+            print(f'=> is Virtual updated to {_isVirtualAI} from ENV var')
             gIsVirtualAI=_isVirtualAI
     if os.environ.get('ENGINE'):
         _name=os.environ.get('ENGINE')
         if _name!=gName:
-            print(f'Engine name updated to {_name} from ENV var')
+            print(f"=> Engine name updated to '{_name}' from ENV var")
             gName=_name
     if os.environ.get('S3_BUCKET'):
         _s3=os.environ.get('S3_BUCKET')
         if _s3!=gS3Bucket:
-            print(f'Set S3 bucket to {_s3} from ENV var')
+            print(f"=> Set S3 bucket to '{_s3}' from ENV var")
             gS3Bucket=_s3
     if os.environ.get('USERNAME') and gUsername==None:
         gUsername=os.environ.get('USERNAME')
+    if os.environ.get('VAI_ID') and gVAIToken==None:
+        gVAIToken=os.environ.get('VAI_ID')
+    if os.environ.get('VAI_SECRET') and gVAISecret==None:
+        gVAISecret=os.environ.get('VAI_SECRET')
     if os.environ.get('AWS_ACCESS_KEY_ID') and AWSID==None:
         AWSID=os.environ.get('AWS_ACCESS_KEY_ID')
     if os.environ.get('AWS_ACCESS_KEY_SECRET') and AWSSecret==None:
         AWSSecret=os.environ.get('AWS_ACCESS_KEY_SECRET')
 
     if AWSID!=None and AWSSecret!=None:
         gAWSSession = boto3.Session(
             aws_access_key_id=AWSID,
             aws_secret_access_key=AWSSecret
         )
         gS3 = gAWSSession.resource('s3')
-        print(f'Logged into AWS S3')
+        print(f'=> Logged into AWS S3')
         
+    if gIsDebug: 
+        gOriginOSAIS="http://"+gIPLocal+":3022/"
+    else:
+        gOriginOSAIS="https://opensourceais.com/"
+
     return {
+        "name": gName,
+        "osais": gOriginOSAIS,
         "username": gUsername,
         "isLocal": gIsLocal,
         "isVirtualAI": gIsVirtualAI,
-        "name": gName
+        "isDebug": gIsDebug
     }
 
 ## ------------------------------------------------------------------------
 #       cost calculation
 ## ------------------------------------------------------------------------
 
 # init the dafault cost array
@@ -642,15 +684,15 @@
 ## ------------------------------------------------------------------------
 
 # where is the output dir?
 def _getOutputDir():
     global gArgsOSAIS
     global gOutputDir
 
-    if gArgsOSAIS!=None:
+    if gArgsOSAIS!=None and  gArgsOSAIS.outdir!=None:
         return gArgsOSAIS.outdir
     return gOutputDir
 
 # receives args from request and put them in a array for processing
 def _getArgs(_args):
     aResult = []
     for key, value in _args.items():
@@ -678,14 +720,19 @@
 #       System info
 ## ------------------------------------------------------------------------
 
 def _clearDir():
     clearOldFiles(gInputDir)
     clearOldFiles(gOutputDir)
 
+## PUBLIC - running in docker?
+def osais_isDocker() :
+    global gIsDocker
+    return gIsDocker
+
 ## PUBLIC - info about harware this AI is running on
 def osais_getHarwareInfo() :
     global gName
     return getHostInfo(gName)
 
 ## PUBLIC - get list of files in a dir (check what was generated)
 def osais_getDirectoryListing(_dir) :
@@ -725,15 +772,15 @@
     }
 
 ## ------------------------------------------------------------------------
 #       connect to Gateway
 ## ------------------------------------------------------------------------
 
 # notify the gateway of our AI config file
-def _notifyGateway() : 
+def _connectWithGateway() : 
     global gName
     global gOriginGateway
 
     headers = {
         "Content-Type": 'application/json', 
         'Accept': 'text/plain',
     }
@@ -752,147 +799,92 @@
     return True
 
 ## PUBLIC - Reset connection to local gateway
 def osais_resetGateway(_localGateway):
     global gOriginGateway
     gOriginGateway=_localGateway
     try:
-        _notifyGateway()
+        _connectWithGateway()
     except Exception as err:
         consoleLog({"msg":"Could not reset connection to Gateway"})
         raise err
     
-    print("=> This AI is reset to talk to Gateway "+_localGateway)
     return True
 
 ## ------------------------------------------------------------------------
 #       authenticate into OSAIS as virtual AI
 ## ------------------------------------------------------------------------
 
-# Register our VAI into OSAIS
-def _registerVAI(_originOSAIS):
+# Authenticate into OSAIS as a VAI
+def _loginVAI(_originOSAIS, _token, _secret):
     global gName
-    global gToken
-    global gSecret
-    global gOriginOSAIS
-    global gTokenLocal
-    global gSecretLocal
-    global gOriginLocalOSAIS
-    global gIsLocal
 
     headers = {
-        "Content-Type": 'application/json', 
-        'Accept': 'text/plain',
+        "Content-Type": "application/json"
     }
-    objParam=_getFullConfig(gName)
-
-    ## our AI is on AWS
-    if gIsLocal==False:
-        # make it call the OSAIS that was requested to call (prod or local)
-        isProdToProd=(_originOSAIS==None)
-        if _originOSAIS==None:
-            _originOSAIS=gOriginOSAIS
-        try:
-            response = requests.post(f"{_originOSAIS}api/v1/public/virtualai/register", headers=headers, data=json.dumps(objParam))
-            objRes=response.json()["data"]
-            if objRes is None:
-                print("COULD NOT REGISTER, stopping it here")
-                sys.exit()
-
-            if isProdToProd:
-                gToken=objRes["token"]
-                gSecret=objRes["secret"]
-            else :
-                gTokenLocal=objRes["token"]
-                gSecretLocal=objRes["secret"]
-
-            print("We are REGISTERED with OSAIS Prod")
-        except Exception as err:
-            consoleLog({"msg":"Exception raised while trying to register to PROD"})
-            raise err
 
-    ## our AI is local, reg with Local OSAIS (debug)
-    else:
-        try:
-            response = requests.post(f"{gOriginLocalOSAIS}api/v1/public/virtualai/register", headers=headers, data=json.dumps(objParam))
-            objRes=response.json()["data"]
-            if objRes is None:
-                print("COULD NOT REGISTER with debug")
-
-            gTokenLocal=objRes["token"]
-            gSecretLocal=objRes["secret"]
-            print("We are REGISTERED with OSAIS Local (debug)")
-        except Exception as err:
-            consoleLog({"msg":"Exception raised while trying to register to DEBUG"})
-            raise err
+    try:
+        response = requests.post(f"{_originOSAIS}api/v1/public/virtualai/login", headers=headers, data=json.dumps({
+            "token": _token,
+            "secret": _secret
+        }))
 
-    return True
+        objRes=response.json()["data"]
+        if objRes is None:
+            consoleLog({"msg": "COULD NOT LOGIN into "+_originOSAIS+", stopping it here"})
+            sys.exit()
+        return objRes["authToken"]    
+    except Exception as err:
+        consoleLog({"msg":"Exception raised while trying to login as VAI into "+_originOSAIS})
+        raise err
 
-# Authenticate into OSAIS
-def _loginVAI(_originOSAIS):
-    global gToken
-    global gSecret
-    global gAuthToken
-    global gTokenLocal
-    global gSecretLocal
-    global gAuthTokenLocal
+## call OSAIS to update Virt AI config
+def _updateVAIConfig(): 
+    global gName
+    global gOriginOSAIS
+    global gVAIAuthToken
 
+    objParam=_getFullConfig(gName)
     headers = {
-        "Content-Type": "application/json"
+        "Content-Type": "application/json",
+        "Authorization": f"Bearer {gVAIAuthToken}"
     }
 
-    if gToken!= None:
-        try:
-            response = requests.post(f"{gOriginOSAIS}api/v1/public/virtualai/login", headers=headers, data=json.dumps({
-                "token": gToken,
-                "secret": gSecret
-            }))
-
-            objRes=response.json()["data"]
-            if objRes is None:
-                print("COULD NOT LOGIN, stopping it here")
-                sys.exit()
-            print("We got an authentication token into OSAIS")
-            gAuthToken=objRes["authToken"]    
-        except Exception as err:
-            consoleLog({"msg":"Exception raised while trying to login to PROD"})
-            raise err
-
-    if gTokenLocal!= None:
-        if _originOSAIS==None:
-            _originOSAIS=gOriginLocalOSAIS
-        try:
-            response = requests.post(f"{_originOSAIS}api/v1/public/virtualai/login", headers=headers, data=json.dumps({
-                "token": gTokenLocal,
-                "secret": gSecretLocal
-            }))
-
-            objRes=response.json()["data"]
-            if objRes is None:
-                print("COULD NOT LOGIN into OSAIS Local")
-            print("We got an authentication token into OSAIS Local (debug)")
-            gAuthTokenLocal=objRes["authToken"]    
-        except Exception as err:
-            return True
+    try:
+        response = requests.patch(f"{gOriginOSAIS}api/v1/private/virtualai/config", headers=headers, data=json.dumps({
+            "jsonEngine": objParam["config_ai"],
+        }))
 
-    return True
+        objRes=response.json()["data"]
+        if objRes is None:
+            consoleLog({"msg": "COULD NOT UPDATE CONFIG"})
+            return False
+        else:
+            print("=> We patched VAI config of OSAIS at "+gOriginOSAIS)
+        return True
+    except Exception as err:
+        consoleLog({"msg":"Exception raised while trying to update VAI config into "+gOriginOSAIS})
+        return False
 
 ## PUBLIC - Authenticate the Virtual AI into OSAIS
-def osais_authenticateAI(_originOSAIS):
+def osais_authenticateAI():
     global gIsVirtualAI
     global gOriginOSAIS
     global gIsScheduled
-    global gDemoID
-    global gDemoSecret
-    
+    global gVAIToken
+    global gVAISecret
+    global gVAIAuthToken
+
     resp={"data": None}
     if gIsVirtualAI:
         try:
-            resp= _registerVAI(_originOSAIS)
-            resp=_loginVAI(_originOSAIS)
+            ## login as VAI 
+            gVAIAuthToken=_loginVAI(gOriginOSAIS, gVAIToken, gVAISecret)
+            _updateVAIConfig()
+
         except Exception as err:
             consoleLog({"msg":"Exception raised while trying to authenticate to OSAIS"})
             raise err
         
         # Run the scheduler
         if gIsScheduled==False:
             gIsScheduled=True
@@ -900,138 +892,109 @@
 
     return resp
 
 ## ------------------------------------------------------------------------
 #       authenticate into OSAIS as Client (user)
 ## ------------------------------------------------------------------------
 
-def getClientInfo(_authToken):
+## get info about this authenticated CLIENT
+def getClientInfo():
     global gOriginOSAIS
-    global gOriginLocalOSAIS
 
     headers = {
         "Content-Type": "application/json",
-        "Authorization": f"Bearer {_authToken}"
+        "Authorization": f"Bearer {gClientAuthToken}"
     }
 
     objRes=None
-    if gIsLocal:        # if local 
-        try:
-            response = requests.get(f"{gOriginLocalOSAIS}api/v1/private/client", headers=headers)
-            objRes=response.json()["data"]            
-        except Exception as err:
-            return {"data": objRes}
-    else:    
-        try:
-            response = requests.get(f"{gOriginOSAIS}api/v1/private/client", headers=headers)
-            objRes=response.json()["data"]            
-        except Exception as err:
-            return {"data": objRes}
+    try:
+        response = requests.get(f"{gOriginOSAIS}api/v1/private/client", headers=headers)
+        objRes=response.json()["data"]            
+    except Exception as err:
+        return {"data": objRes}
 
     return {"data": objRes}
-            
-
-# Authenticate into OSAIS (as client)
-def osais_authenticateClient(_id, _secret):
-    global gOriginOSAIS
-    global gOriginLocalOSAIS
-    global gClientAuthToken
-    global gClientAuthTokenLocal
-    global gIsLocal
 
-    authToken=None
+## token of the authenticated CLIENT
+def osais_getClientID(): 
+    return gClientID
 
+## authenticate as a CLIENT
+def _authenticateClient(_route, _id, _secret):
     headers = {
         "Content-Type": "application/json"
     }
-    resp={"data": None}
-    if gIsLocal:        # if local ... log as client into debug
-        try:
-            url=f"{gOriginLocalOSAIS}api/v1/public/client/demo"      ## get a demo auth token
-            if _id!= None:
-                url=f"{gOriginLocalOSAIS}api/v1/public/client/login"
-            response = requests.post(url, headers=headers, data=json.dumps({
-                "token": _id,
-                "secret": _secret
-            }))
-
-            objRes=response.json()["data"]
-            if objRes is None:
-                print("COULD NOT LOGIN AS CLIENT into OSAIS Local")
-            print("We got a CLIENT authentication token into OSAIS Local (debug)")
-            gClientAuthTokenLocal=objRes["authToken"]
-            authToken=gClientAuthTokenLocal
-            resp={"data": {
-                "token": objRes["token"],
-                "authToken": gClientAuthTokenLocal,
-            }}
+    try:
+        url=f"{_route}api/v1/public/client/demo"      ## get a demo auth token
+        if _id!= None:
+            url=f"{_route}api/v1/public/client/login"
+        response = requests.post(url, headers=headers, data=json.dumps({
+            "token": _id,
+            "secret": _secret
+        }))
 
-        except Exception as err:
-            ## no big deal
-            gClientAuthTokenLocal=None
+        objRes=response.json()["data"]
+        if objRes is None:
+            consoleLog({"msg": "COULD NOT LOGIN AS CLIENT into "+_route})
+        resp={"data": {
+            "token": objRes["token"],
+            "authToken": objRes["authToken"],
+        }}
+        return resp
 
-    else:       # else ... log as client into prod        
-        try:
-            url=f"{gOriginOSAIS}api/v1/public/client/demo"      ## get a demo auth token
-            if _id!= None:
-                url=f"{gOriginOSAIS}api/v1/public/client/login"
-            response = requests.post(url, headers=headers, data=json.dumps({
-                "token": _id,
-                "secret": _secret
-            }))
-
-            objRes=response.json()["data"]
-            if objRes is None:
-                print("COULD NOT LOGIN AS CLIENT, stopping it here")
-                sys.exit()
-            print("We got a CLIENT authentication token into OSAIS")
-            gClientAuthToken=objRes["authToken"]    
-            authToken=gClientAuthToken
-            resp={"data": {
-                "token": objRes["token"],
-                "authToken": gClientAuthToken,
-            }}
+    except Exception as err:
+        consoleLog({"msg":"Exception raised while trying to login as CLIENT into "+_route})
+        resp={"data": {
+            "token": None,
+            "authToken": None
+        }}
 
-        except Exception as err:
-            consoleLog({"msg":"Exception raised while trying to login as CLIENT to PROD"})
-            gClientAuthToken=None
+# Authenticate into OSAIS (as client)
+def osais_authenticateClient(_id, _secret):
+    global gOriginOSAIS
+    global gClientAuthToken
+    global gClientID
+    global gIsLocal
 
-    dataClient=getClientInfo(authToken)
+    resp={"data": None}
+    
+    ## log as client into osais
+    resp=_authenticateClient(gOriginOSAIS, _id, _secret)
+    gClientAuthToken=resp["data"]["authToken"]
+    gClientID=resp["data"]["token"]
+        
+    dataClient=getClientInfo()
     resp["data"]["user"]=dataClient["data"]["user"]
     return resp 
 
+def authenticateClientAsDemo():
+    return osais_authenticateClient(None, None)
+
 ## ------------------------------------------------------------------------
 #       ask OSAIS to process a request
 ## ------------------------------------------------------------------------
 
 def osais_postRequest(objReq):
     global gClientAuthToken
-    global gClientAuthTokenLocal
-    global gIsLocal
     global gName
 
     resp={"data": None}
     _url=None
-    _authToken=None
-    if gIsLocal:
-        _authToken=gClientAuthTokenLocal
-        _url=f"{gOriginLocalOSAIS}api/v1/private/client/ai/"+objReq.gName
-    else:
-        _authToken=gClientAuthToken
-        _url=f"{gOriginOSAIS}api/v1/private/client/ai/"+objReq.gName
+    _authToken=gClientAuthToken
+    _url=f"{gOriginOSAIS}api/v1/private/client/ai/"+objReq.gName
 
     try:
         response = requests.post(_url, headers={
             "Content-Type": "application/json",
             'Accept': 'text/plain',
             "Authorization": f"Bearer {_authToken}"
         }, data=json.dumps(objReq))
         objRes=response.json()["data"]
         if objRes is None:
-            print("COULD NOT post request")
+            consoleLog({"msg": "COULD NOT post request"})
         resp={"data": objRes}
 
     except Exception as err:
         raise err
 
     return resp 
 
@@ -1058,102 +1021,120 @@
     vq_parser.add_argument("-idir", "--indir", type=str, help="input directory", default=gInputDir, dest='indir')
     vq_parser.add_argument("-local", "--islocal", type=bool, help="is local or prod?", default=False, dest='isLocal')
     vq_parser.add_argument("-cycle", "--cycle", type=int, help="cycle", default=0, dest='cycle')
     vq_parser.add_argument("-filename", "--filename", type=str, help="filename", default="default", dest='filename')
     vq_parser.add_argument("-warmup", "--warmup", type=bool, help="warmup", default=False, dest='warmup')
 
     gArgsOSAIS = vq_parser.parse_args(aArg)
-    gIsWarmup=gArgsOSAIS.warmup
+    gIsWarmup=(gArgsOSAIS.warmup==True or gArgsOSAIS.warmup=="True")
     return True
 
 ## PUBLIC - run the AI (at least try)
 def osais_runAI(*args):
     global gIsBusy
     global gAProcessed
     global gName 
     global gLastProcessStart_at
     global gOriginOSAIS
-    global gOriginLocalOSAIS
     global gIsLocal
 
     ## get args
     fn_run=args[0]
     _args=args[1]
 
     ## do not process twice same uid
     _uid=_args.get('-uid')
     if _uid in gAProcessed:
-        return  "not processing, already tried..."
-
+        consoleLog({"msg": "Not processing "+str(_uid)+", already tried!"})
+        return  None
+    
     ## where is the caller?
     _orig=None
     try: 
         if _args["-orig"]:
             _orig=_args["-orig"]
+            print("=> origin set to "+_orig)
     except:
         _orig=None
+        print("=> origin set to Default")
 
     ## start time
     gIsBusy=True
     beg_date = datetime.utcnow()
 
     ## reprocess AI args
     aArgForparserAI=_getArgs(_args)
-    args_ExclusiveOSAIS=['-orig', '-t', '-u', '-uid', '-local', '-cycle', '-warmup']
+    args_ExclusiveOSAIS=['-orig', '-t', '-u', '-uid', '-local', '-cycle', '-warmup', "-filename"]
     aArgForparserAI=_argsFromFilter(aArgForparserAI, args_ExclusiveOSAIS, False)
 
     ## process the filename passed in dir (case localhost / AI Gateway), or download file from URL (case AI running as Virtual AI)
     _input=None
-    _filename=_args.get('-filename')
-    _urlUpload=_args.get('url_upload')
+    _filename=None
+    _urlUpload=None
+    try:
+        ## the filename of the locally downloaded "url_upload" url 
+        _filename=_args.get('-filename')
+    except Exception as err:
+        consoleLog({"msg":"did not get a filename"})
+        raise err
+    
+    try:
+        _urlUpload=_args.get('url_upload')
+    except Exception as err:
+        consoleLog({"msg":"did not get an upload url"})
+        raise err
+
+    # only a urlUpload? => we need to download the file 
+    # note that lots can fail with 403 on download image from ext API, so we shall avoid this
     if not _filename and _urlUpload:
         try:
-            _input=downloadImage(_urlUpload)
+            _input=osais_downloadImage(_urlUpload)
             if _input:
                 aArgForparserAI.append("-filename")
                 aArgForparserAI.append(_input)
+                print("=> downloaded file "+_urlUpload)
             else:
                 ## min requirements
-                print("no image to process")
-                return "input required"
+                consoleLog({"msg":"no file to process"})
+                return None
         except Exception as err:
             gIsBusy=False
             consoleLog({"msg":"Could not download image"})
             raise err
-    
+
     ## Init OSAIS Params (from all args, keep only those for OSAIS)
     aArgForParserOSAIS=_getArgs(_args)
     args_ExclusiveOSAIS.append('-odir')
     args_ExclusiveOSAIS.append('-idir')
     aArgForParserOSAIS=_argsFromFilter(aArgForParserOSAIS, args_ExclusiveOSAIS, True)
     osais_initParser(aArgForParserOSAIS)
 
+    if gIsWarmup:
+        print("=> Warming up...")
+    else:
+        print("=> before run: processed args from url: "+str(aArgForparserAI)+"\r\n")
+
     ## notify OSAIS (Req received)
     CredsParam=getCredsParams()
     MorphingParam=getMorphingParams()
     StageParam=getStageParams(AI_PROGRESS_REQRECEIVED, 0)
     osais_notify(_orig, CredsParam, MorphingParam , StageParam)
 
-    if gIsWarmup:
-        print("\r\n=> Warming up... \r\n")
-    else:
-        print("\r\n=> before run: processed args from url: "+str(aArgForparserAI)+"\r\n")
-
     ## processing accepted
     gLastProcessStart_at=datetime.utcnow()
     gAProcessed.append(_uid)
 
     ## notify OSAIS (start)
     StageParam=getStageParams(AI_PROGRESS_AI_STARTED, 0)
     osais_notify(_orig, CredsParam, MorphingParam , StageParam)
 
     ## start watch file creation
     _output=_getOutputDir()
     watch_directory(_output, osais_onNotifyFileCreated, _args)
-
+    
     ## Notif OSAIS
     StageParam=getStageParams(AI_PROGRESS_INIT_IMAGE, 0)
     osais_notify(_orig, CredsParam, MorphingParam , StageParam)
 
     ## run AI
     response=None
     try:
@@ -1231,38 +1212,53 @@
     return {"stage": AI_PROGRESS_ERROR, "descr":"error"}
 
 ## ------------------------------------------------------------------------
 #       Notifications to Gateway / OSAIS
 ## ------------------------------------------------------------------------
 
 # Upload image to OSAIS 
-def _uploadImageToOSAIS(_origin, objParam, isLocal):
+def _uploadImageToOSAIS(_origin, objParam):
     if gIsVirtualAI==False:
         return None
     
-    global gAuthToken
-    global gAuthTokenLocal
+    global gVAIAuthToken
     
-    _auth=gAuthToken
-    if isLocal:
-        _auth=gAuthTokenLocal
-
     # lets go call OSAIS AI Gateway / or OSAIS itself
     headers = {
         "Content-Type": 'application/json', 
         'Accept': 'text/plain',
-        "Authorization": f"Bearer {_auth}"
+        "Authorization": f"Bearer {gVAIAuthToken}"
     }
 
     api_url=f"{_origin}api/v1/private/virtualai/upload"        
     payload = json.dumps(objParam)
     response = requests.post(api_url, headers=headers, data=payload )
     objRes=response.json()
     return objRes    
 
+# Upload image to a local gateway
+def _uploadImageToGateway(_origin, objParam):
+    if gIsVirtualAI==False:
+        return None
+    
+    global gVAIAuthToken
+    
+    # lets go call OSAIS AI Gateway / or OSAIS itself
+    headers = {
+        "Content-Type": 'application/json', 
+        'Accept': 'text/plain',
+        "Authorization": f"Bearer {gVAIAuthToken}"
+    }
+
+    api_url=f"{_origin}api/v1/public/upload"        
+    payload = json.dumps(objParam)
+    response = requests.post(api_url, headers=headers, data=payload )
+    objRes=response.json()
+    return objRes    
+
 def osais_onNotifyFileCreated(_dir, _filename, _args):
     ## where is the caller?
     _orig=None
     try: 
         if _args["-orig"]:
             _orig=_args["-orig"]
     except:
@@ -1272,60 +1268,65 @@
     gArgsOSAIS.filename=_filename
     _stageParam=getStageParams(AI_PROGRESS_DONE_IMAGE, 0)
     _morphingParam=getMorphingParams()
     _credsParam=getCredsParams()
     osais_notify(_orig, _credsParam, _morphingParam, _stageParam)            # OSAIS Notification
     return True
 
+def _notifyGateway(_origin, objParam):
+    headers = {
+        "Content-Type": "application/json"
+    }
+    api_url=f"{_origin}api/v1/public/notify"
+    try: 
+        response = requests.post(api_url, headers=headers, data=json.dumps(objParam))
+        objRes=response.json()
+        return objRes
+    except Exception as err:
+            raise err
+
+def _notifyOSAIS(objParam):
+    global gOriginOSAIS
+    headers = {
+        "Content-Type": "application/json",
+        "Authorization": f"Bearer {gVAIAuthToken}"
+    }
+    api_url=f"{gOriginOSAIS}api/v1/private/virtualai/notify"
+    try: 
+        response = requests.post(api_url, headers=headers, data=json.dumps(objParam))
+        objRes=response.json()
+        return objRes
+    except Exception as err:
+            raise err
+
 # Direct Notify OSAIS 
 def osais_notify(_origin, CredParam, MorphingParam, StageParam):
     global gIPLocal
     global gPortGateway
     global gIsVirtualAI
-    global gAuthToken
-    global gAuthTokenLocal
+    global gIsLocal
+    global gVAIAuthToken
     global gLastChecked_at
     global gIsWarmup
 
     ## no notification of warmup or unknown caller
     if gIsWarmup or _origin==None:
         return None
     
     gLastChecked_at = datetime.utcnow()
 
     # notification console log
     merged = dict()
     merged.update(CredParam)
     merged.update(MorphingParam)
-    print("NotifyOSAIS ("+str(StageParam["stage"])+"/ "+StageParam["descr"]+"): "+str(merged))
-    print("\r\n")
 
     _filename=""
     if MorphingParam["filename"]!="":
         _filename=MorphingParam["filename"]
 
-    # lets go call OSAIS AI Gateway / or OSAIS itself
-    headers = {
-        "Content-Type": "application/json"
-    }
-
-    ## config for calling gateway
-    api_url = f"{_origin}api/v1/public/notify"
-
-    ## config for calling OSAIS (no gateway)
-    if gIsVirtualAI:
-        _auth=gAuthToken
-
-        if CredParam["isLocal"]:
-            _auth=gAuthTokenLocal
-
-        if gIsVirtualAI==True:
-            headers["Authorization"]= f"Bearer {_auth}"
-            api_url=f"{_origin}api/v1/private/virtualai/notify"
-
     objParam={
         "response": {
             "token": CredParam["tokenAI"],
             "uid": str(MorphingParam["uid"]),
             "stage": str(StageParam["stage"]),
             "cycle": str(MorphingParam["cycle"]),
             "engine": CredParam["engine"],
@@ -1333,17 +1334,32 @@
             "descr": StageParam["descr"],
             "filename": _filename
         }
     }
 
     if "cost" in StageParam:
         objParam["response"]["cost"]= str(StageParam["cost"])
-    
-    response = requests.post(api_url, headers=headers, data=json.dumps(objParam) )
-    objRes=response.json()
+
+    ## Notify OSAIS (as Virtual AI)
+    if gIsVirtualAI:
+        try: 
+            objRes=_notifyOSAIS(objParam)
+            _at=objRes["data"]["notified_at"]
+            print("\r\n ["+_at+"] => Notified OSAIS ("+str(StageParam["stage"])+"/ "+StageParam["descr"]+"): "+str(merged)+ " on: "+api_url)
+        except:
+            consoleLog({"msg": "Failed to notify stage ("+str(StageParam["stage"])+ " to OSAIS"})
+
+    ## Notify Gateway (as Local AI)
+    if gIsLocal:
+        try: 
+            objRes=_notifyGateway(_origin, objParam)
+            _at=objRes["data"]["notified_at"]
+            print("\r\n ["+_at+"] => Notified Gateway ("+str(StageParam["stage"])+"/ "+StageParam["descr"]+"): "+str(merged)+ " on: "+api_url)
+        except:
+            consoleLog({"msg": "Failed to notify stage ("+str(StageParam["stage"])+ " to local Gateway "+_origin})
 
     if StageParam["stage"]==AI_PROGRESS_DONE_IMAGE:
         if gIsVirtualAI==True:
             _dir=MorphingParam["odir"]
             if _dir==None:
                 _dir=gOutputDir
             _dirImage=_dir+_filename
@@ -1354,122 +1370,135 @@
             im_b64 = base64.b64encode(image_data).decode("utf8")
             param={
                 "image": im_b64,
                 "uid": str(MorphingParam["uid"]),
                 "cycle": str(MorphingParam["cycle"]),
                 "engine": CredParam["engine"],
             }            
-            _uploadImageToOSAIS(_origin, param, CredParam["isLocal"])
+            if CredParam["isLocal"]:
+                _uploadImageToGateway(_origin, param)
+            else:
+                _uploadImageToOSAIS(_origin, param)
     return objRes
 
 ## ------------------------------------------------------------------------
 #       Init processing
 ## ------------------------------------------------------------------------
 
 ## PUBLIC - resetting who this AI is talking to (OSAIS prod and dbg)
-def osais_resetOSAIS(_locationProd, _localtionDebug):
+def osais_resetOSAIS(_location):
     global gOriginOSAIS
-    global gOriginLocalOSAIS
-    gOriginOSAIS=_locationProd
-    gOriginLocalOSAIS=_localtionDebug
-    if _locationProd!=None:
-        print("=> This AI is reset to talk to PROD "+gOriginOSAIS)
-    if _localtionDebug!=None:
-        print("=> This AI is reset to talk to DEBUG "+gOriginLocalOSAIS+"\r\n")
+    gOriginOSAIS=_location
     return True
 
 ## PUBLIC - Init the Virtual AI
-def osais_initializeAI():
+def osais_initializeAI(_envFile):
     global gIsDocker
+    global gIsDebug
     global gIsLocal
     global gIsVirtualAI
     global gUsername
     global gName
     global gPortAI
     global gVersion
     global gPortGateway
     global gPortLocalOSAIS
     global gIPLocal
     global gExtIP
     global gOriginGateway
-    global gAuthToken
-    global gAuthTokenLocal
+    global gVAIAuthToken
     global gOriginOSAIS
-    global gOriginLocalOSAIS
+    global gClientAuthToken
 
     ## load env 
-    _envFile="env_local"
-    if gIsDocker:
-        _envFile="env_docker"
-        print("\r\n=> in Docker\r\n")
-    else:
-        print("\r\n=> NOT in Docker\r\n")        
     obj=osais_getEnv(_envFile)
     gIsLocal=obj["isLocal"]
     gIsVirtualAI=obj["isVirtualAI"]
     gUsername=obj["username"]
     gName=obj["name"]
 
     ## from env, load AI config
     gConfig=osais_loadConfig(gName)
     gPortAI = gConfig["port"]
     gVersion = gConfig["version"]
 
-    print("\r\n===== Config =====")
-    print("engine: "+str(gName) + " v"+str(gVersion))
-    print("is Local: "+str(gIsLocal))
-    print("is Virtual: "+str(gIsVirtualAI))
-    print("username: "+str(gUsername))
-    if gIsLocal:
-        print("location (local): "+str(gIPLocal)+":"+str(gPortAI))
-    else: 
-        print("location (external): "+str(gExtIP)+":"+str(gPortAI))
-    print("===== /Config =====\r\n")
 
     ## make sure we have a config file
     _loadConfig(gName)
 
     ## where is OSAIS for us then?
     gOriginGateway=f"http://{gIPLocal}:{gPortGateway}/"         ## config for local gateway (local and not virtual)
 
     ## we set OSAIS location in all cases (even if in gateway) because this AI can generate it s own page for sending reqs (needs a client logged into OSAIS)
-    if gIsLocal:
-        osais_resetOSAIS(None, f"http://{gIPLocal}:{gPortLocalOSAIS}/")
+    if gIsDebug:
+        osais_resetOSAIS(f"http://{gIPLocal}:{gPortLocalOSAIS}/")
     else:
-        osais_resetOSAIS("https://opensourceais.com/", None)
+        osais_resetOSAIS("https://opensourceais.com/")
     if gIsVirtualAI:
         try:
-            osais_authenticateAI(None)
+            osais_authenticateAI()
         except Exception as err:
             print("=> CRITICAL: Could not connect virtual AI "+gName+ " to OSAIS")
             return None
-
-        if gAuthToken!=None:
-            print("=> Running "+gName+" AI as a virtual AI connected to: "+gOriginOSAIS)
-        if gAuthTokenLocal!=None:
-            print("=> Running "+gName+" AI as a virtual AI connected to: "+gOriginLocalOSAIS)
-    else:
+    
+    if gIsLocal:
         try:
             osais_resetGateway(gOriginGateway)
-            print("=> Running "+gName+" AI as a server connected to local Gateway "+gOriginGateway)
-        
         except Exception as err:
             print("CRITICAL: could not notify Gateway at "+gOriginGateway)
             return None
 
+    dataClient=authenticateClientAsDemo()
+
     ## init default cost
     _initializeCost()
 
-    print("\r\n")
-    return gName
+    ## output the config we are runing on
+    print("\r\n<===== Config =====>\r\n")
+    print("=> engine:                  "+str(gName) + " v"+str(gVersion))
+    if gIsDocker:
+        print("=> in Docker:               True")
+    else:
+        print("=> in Docker:               False")
+    print("=> is Debug:                "+str(gIsDebug))
+    print("\r\n=> is Local:                "+str(gIsLocal))
+    if gIsLocal:
+        print(" > gateway:                 "+gOriginGateway)
+        print(" > local AI location:       "+str(gIPLocal)+":"+str(gPortAI))
+    print("\r\n=> is Virtual:              "+str(gIsVirtualAI))
+    if gIsVirtualAI:
+        print(" > virtAI location (ext.):  "+str(gExtIP)+":"+str(gPortAI))
+        print(" > OSAIS location:          "+gOriginOSAIS)
+        if gVAIAuthToken!=None:
+            print(" > is connected to OSAIS:   True")
+        else:
+            print(" > is connected to OSAIS:   False")
+    if gClientAuthToken!=None:
+        print("\r\n=> is connected as Client:  True")
+        print(" > client ID:               "+dataClient["data"]["token"])
+    else:
+        print("\r\n=> is connected as Client:  False")
+    print("\r\n=> Pay to owner:            "+str(gUsername))
+    print("\r\n<===== /Config =====>\r\n")
+
+    return {
+        "engine":gName,
+        "client": dataClient["data"]
+    }
 
 ## ------------------------------------------------------------------------
 #       Starting point of Lib
 ## ------------------------------------------------------------------------
 
 # Multithreading for observers
 watch_directory=start_observer_thread(_getOutputDir(), osais_onNotifyFileCreated, None)     
 
 #cleaning dir every 10min
 schedule.every(10).minutes.do(_clearDir)
 
-print("\r\nPython OSAIS Lib is loaded...")
+#login into OSAIS as client every 24h
+schedule.every(3600).minutes.do(authenticateClientAsDemo)
+
+#login as VAI every 24h +1min
+schedule.every(3601).minutes.do(osais_authenticateAI)
+
+print("\r\n=> Python OSAIS Lib is loaded...")
```

### Comparing `osais-1.0.42/osais.egg-info/PKG-INFO` & `osais-1.0.43/osais.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.42
+Version: 1.0.43
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.42/setup.py` & `osais-1.0.43/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.42',
+    version='1.0.43',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
     packages=["osais"],
     package_data={'src': ['osais.json']},
     install_requires=[
         'requests >=2.25.1',
         "schedule ==1.1.0",
         "watchdog ==2.1.9",
-        "Werkzeug ==2.2.2"
+        "Werkzeug ==2.2.2",
+        "Jinja2 ==3.1.2",
+        "boto3 ==1.26.130"
     ],
     python_requires='>=3',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

