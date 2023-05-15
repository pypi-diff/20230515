# Comparing `tmp/dualopt-0.1.4.tar.gz` & `tmp/dualopt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualopt-0.1.4.tar", last modified: Mon May 15 01:41:20 2023, max compression
+gzip compressed data, was "dualopt-0.1.5.tar", last modified: Mon May 15 01:48:20 2023, max compression
```

## Comparing `dualopt-0.1.4.tar` & `dualopt-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 01:41:20.422940 dualopt-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-05-15 01:40:42.000000 dualopt-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      772 2023-05-15 01:41:20.421933 dualopt-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-05-15 01:40:40.000000 dualopt-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 01:41:20.372999 dualopt-0.1.4/dualopt/
--rw-rw-rw-   0        0        0       49 2023-05-15 01:40:35.000000 dualopt-0.1.4/dualopt/__init__.py
--rw-rw-rw-   0        0        0     6051 2023-05-15 01:41:04.000000 dualopt-0.1.4/dualopt/classification.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:41:20.419940 dualopt-0.1.4/dualopt.egg-info/
--rw-rw-rw-   0        0        0      772 2023-05-15 01:41:20.000000 dualopt-0.1.4/dualopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-15 01:41:20.000000 dualopt-0.1.4/dualopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 01:41:20.000000 dualopt-0.1.4/dualopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-15 01:41:20.000000 dualopt-0.1.4/dualopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 01:41:20.000000 dualopt-0.1.4/dualopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 01:41:20.422940 dualopt-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-05-15 01:41:09.000000 dualopt-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:48:20.580465 dualopt-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-05-15 01:40:42.000000 dualopt-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      772 2023-05-15 01:48:20.573465 dualopt-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2023-05-15 01:40:40.000000 dualopt-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 01:48:20.430483 dualopt-0.1.5/dualopt/
+-rw-rw-rw-   0        0        0       49 2023-05-15 01:40:35.000000 dualopt-0.1.5/dualopt/__init__.py
+-rw-rw-rw-   0        0        0     6067 2023-05-15 01:47:53.000000 dualopt-0.1.5/dualopt/classification.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:48:20.571461 dualopt-0.1.5/dualopt.egg-info/
+-rw-rw-rw-   0        0        0      772 2023-05-15 01:48:19.000000 dualopt-0.1.5/dualopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-15 01:48:19.000000 dualopt-0.1.5/dualopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 01:48:19.000000 dualopt-0.1.5/dualopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-15 01:48:19.000000 dualopt-0.1.5/dualopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 01:48:19.000000 dualopt-0.1.5/dualopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 01:48:20.581461 dualopt-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-15 01:48:00.000000 dualopt-0.1.5/setup.py
```

### Comparing `dualopt-0.1.4/LICENSE` & `dualopt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.4/PKG-INFO` & `dualopt-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.4
+Version: 0.1.5
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.4/dualopt/classification.py` & `dualopt-0.1.5/dualopt/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
   epoch = 0
   counter = 0
   while counter < set_counter:   #Counter sets the number of epochs of non improvement before stopping
 
       t0 = time.time()
 
-      train(model, trainloader, criterion, scaler, optimizer, epoch)
+      train(model, trainloader, device, criterion, scaler, optimizer, epoch)
 
       correct_1=0
       correct_5=0
       c = 0
       model.eval()
       t1 = time.time()
       with torch.no_grad():
@@ -49,15 +49,15 @@
       epoch += 1
       if float(correct_1*100/c) >= float(max(top1)):
           torch.save(model.state_dict(), PATH)
           print(1)
           counter = 0
 
 
-def train(model, trainloader, criterion, scaler, optimizer, epoch, device):
+def train(model, trainloader, device, criterion, scaler, optimizer, epoch):
   epoch_accuracy = 0
   epoch_loss = 0
   
   model.train()
   with tqdm(trainloader, unit="batch") as tepoch:
           tepoch.set_description(f"Epoch {epoch+1}")
 
@@ -104,15 +104,15 @@
     model.load_state_dict(torch.load(PATH))
 
   epoch = 0
   while counter < set_counter:   #Counter sets the number of epochs of non improvement before stopping
 
       t0 = time.time()
 
-      train(model, trainloader, criterion, scaler, optimizer, epoch, device)
+      train(model, trainloader, device, criterion, scaler, optimizer, epoch)
 
       correct_1=0
       correct_5=0
       c = 0
       model.eval()
 
       t1 = time.time()
@@ -145,15 +145,15 @@
 
   epoch = 0
   counter = 0
   while counter < set_counter:   #Counter sets the number of epochs of non improvement before stopping
 
       t0 = time.time()
 
-      train(model, trainloader, criterion, scaler, optimizer, epoch)
+      train(model, trainloader, device, criterion, scaler, optimizer, epoch)
 
       correct_1=0
       correct_5=0
       c = 0
       model.eval()
       t1 = time.time()
       with torch.no_grad():
```

### Comparing `dualopt-0.1.4/dualopt.egg-info/PKG-INFO` & `dualopt-0.1.5/dualopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.4
+Version: 0.1.5
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.4/setup.py` & `dualopt-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'dualopt',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.4',
+  version = '0.1.5',
   license='MIT',
   description = 'Dual Optimizer Training',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/DualOpt',
```

