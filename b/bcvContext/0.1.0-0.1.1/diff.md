# Comparing `tmp/bcvcontext-0.1.0.tar.gz` & `tmp/bcvcontext-0.1.1.tar.gz`

## Comparing `bcvcontext-0.1.0.tar` & `bcvcontext-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/src/bcvContext/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/src/bcvContext/bcvContext.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/README.md
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.1/src/bcvContext/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 bcvcontext-0.1.1/src/bcvContext/bcvContext.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.1/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.1/README.md
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bcvcontext-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.1/PKG-INFO
```

### Comparing `bcvcontext-0.1.0/src/bcvContext/bcvContext.py` & `bcvcontext-0.1.1/src/bcvContext/bcvContext.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 def scriptContext(filename) :
     return filename
 
 def scriptContextRawfile():
     return "../rawFile.csv"
 
 def notarizationContext(filename) :
-    notarizationPath = variables.get('notarizationPath')
+    notarizationPath = variables.get('notarization_path')
     return "../.." + notarizationPath + "/" + filename
 
 def dayContext(m, filename) :
-    notarizationPath = variables.get('notarizationPath')
+    notarizationPath = variables.get('notarization_path')
     if (m >= 0) : raise Exception("No history at J", str(m))
     day = json.load(open("../.." + notarizationPath + "/.config.json"))["day"] + m
     if (day < 0) : raise Exception("No history at J", str(day))
     lastNotarization = json.load(open("../.." + notarizationPath + "/../../Day" + str(day) + "/.dayConfig.json"))["lastNotarization"]
     return "../.." + notarizationPath + "/../../Day" + str(day) + "/Notarization" + str(lastNotarization) + "/" + filename
```

### Comparing `bcvcontext-0.1.0/.gitignore` & `bcvcontext-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.0/LICENSE` & `bcvcontext-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.0/PKG-INFO` & `bcvcontext-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcvContext
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small package to handle context path for the BCV generic workflow
 Author-email: CEA <thomas.marques@cea.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

