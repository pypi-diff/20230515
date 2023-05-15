# Comparing `tmp/dualopt-0.1.2.tar.gz` & `tmp/dualopt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualopt-0.1.2.tar", last modified: Mon May 15 01:33:23 2023, max compression
+gzip compressed data, was "dualopt-0.1.3.tar", last modified: Mon May 15 01:37:45 2023, max compression
```

## Comparing `dualopt-0.1.2.tar` & `dualopt-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 01:33:23.660930 dualopt-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-05-15 01:05:45.000000 dualopt-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      772 2023-05-15 01:33:23.659933 dualopt-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-05-15 01:16:51.000000 dualopt-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 01:33:23.585957 dualopt-0.1.2/dualopt/
--rw-rw-rw-   0        0        0       49 2023-05-15 01:14:55.000000 dualopt-0.1.2/dualopt/__init__.py
--rw-rw-rw-   0        0        0     6069 2023-05-15 01:33:14.000000 dualopt-0.1.2/dualopt/classification.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:33:23.656933 dualopt-0.1.2/dualopt.egg-info/
--rw-rw-rw-   0        0        0      772 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 01:33:23.660930 dualopt-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-05-15 01:33:16.000000 dualopt-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:37:45.471140 dualopt-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-15 01:05:45.000000 dualopt-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      772 2023-05-15 01:37:45.464145 dualopt-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2023-05-15 01:16:51.000000 dualopt-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 01:37:45.419139 dualopt-0.1.3/dualopt/
+-rw-rw-rw-   0        0        0       49 2023-05-15 01:14:55.000000 dualopt-0.1.3/dualopt/__init__.py
+-rw-rw-rw-   0        0        0     6051 2023-05-15 01:37:25.000000 dualopt-0.1.3/dualopt/classification.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:37:45.460141 dualopt-0.1.3/dualopt.egg-info/
+-rw-rw-rw-   0        0        0      772 2023-05-15 01:37:45.000000 dualopt-0.1.3/dualopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-15 01:37:45.000000 dualopt-0.1.3/dualopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 01:37:45.000000 dualopt-0.1.3/dualopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-15 01:37:45.000000 dualopt-0.1.3/dualopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 01:37:45.000000 dualopt-0.1.3/dualopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 01:37:45.471140 dualopt-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-15 01:37:38.000000 dualopt-0.1.3/setup.py
```

### Comparing `dualopt-0.1.2/LICENSE` & `dualopt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.2/PKG-INFO` & `dualopt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.2/dualopt/classification.py` & `dualopt-0.1.3/dualopt/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
           print(1)
           counter = 0
 
 
 def train(model, trainloader, criterion, scaler, optimizer, epoch, device):
   epoch_accuracy = 0
   epoch_loss = 0
-  running_loss = 0.0
+  
   model.train()
   with tqdm(trainloader, unit="batch") as tepoch:
           tepoch.set_description(f"Epoch {epoch+1}")
 
           for data in tepoch:
     
             inputs, labels = data[0].to(device), data[1].to(device)
```

### Comparing `dualopt-0.1.2/dualopt.egg-info/PKG-INFO` & `dualopt-0.1.3/dualopt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.2/setup.py` & `dualopt-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'dualopt',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.2',
+  version = '0.1.3',
   license='MIT',
   description = 'Dual Optimizer Training',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/DualOpt',
```

