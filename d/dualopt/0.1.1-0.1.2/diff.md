# Comparing `tmp/dualopt-0.1.1.tar.gz` & `tmp/dualopt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualopt-0.1.1.tar", last modified: Mon May 15 01:30:41 2023, max compression
+gzip compressed data, was "dualopt-0.1.2.tar", last modified: Mon May 15 01:33:23 2023, max compression
```

## Comparing `dualopt-0.1.1.tar` & `dualopt-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 01:30:41.526289 dualopt-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-05-15 01:05:45.000000 dualopt-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      772 2023-05-15 01:30:41.526289 dualopt-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-05-15 01:16:51.000000 dualopt-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 01:30:41.510660 dualopt-0.1.1/dualopt/
--rw-rw-rw-   0        0        0       49 2023-05-15 01:14:55.000000 dualopt-0.1.1/dualopt/__init__.py
--rw-rw-rw-   0        0        0     6035 2023-05-15 01:16:17.000000 dualopt-0.1.1/dualopt/classification.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:30:41.526289 dualopt-0.1.1/dualopt.egg-info/
--rw-rw-rw-   0        0        0      772 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 01:30:41.526289 dualopt-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-05-15 01:30:02.000000 dualopt-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:33:23.660930 dualopt-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-15 01:05:45.000000 dualopt-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      772 2023-05-15 01:33:23.659933 dualopt-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2023-05-15 01:16:51.000000 dualopt-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 01:33:23.585957 dualopt-0.1.2/dualopt/
+-rw-rw-rw-   0        0        0       49 2023-05-15 01:14:55.000000 dualopt-0.1.2/dualopt/__init__.py
+-rw-rw-rw-   0        0        0     6069 2023-05-15 01:33:14.000000 dualopt-0.1.2/dualopt/classification.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:33:23.656933 dualopt-0.1.2/dualopt.egg-info/
+-rw-rw-rw-   0        0        0      772 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 01:33:23.000000 dualopt-0.1.2/dualopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 01:33:23.660930 dualopt-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-15 01:33:16.000000 dualopt-0.1.2/setup.py
```

### Comparing `dualopt-0.1.1/LICENSE` & `dualopt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.1/PKG-INFO` & `dualopt-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.1/dualopt/classification.py` & `dualopt-0.1.2/dualopt/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
       epoch += 1
       if float(correct_1*100/c) >= float(max(top1)):
           torch.save(model.state_dict(), PATH)
           print(1)
           counter = 0
 
 
-def train(model, trainloader, criterion, scaler, optimizer, epoch):
+def train(model, trainloader, criterion, scaler, optimizer, epoch, device):
   epoch_accuracy = 0
   epoch_loss = 0
   running_loss = 0.0
   model.train()
   with tqdm(trainloader, unit="batch") as tepoch:
           tepoch.set_description(f"Epoch {epoch+1}")
 
@@ -80,16 +80,16 @@
 
 def classification(model, trainloader, testloader, device, PATH, top1, top5, traintime, testtime, num_classes, opt1 = 'adamw', pretrained = False, set_counter = 20):
 
   criterion = nn.CrossEntropyLoss()
 
   scaler = torch.cuda.amp.GradScaler()
 
-  top1_acc = Accuracy(task="multiclass", num_classes=10).to(device)
-  top5_acc = Accuracy(task="multiclass", num_classes=10, top_k=5).to(device)
+  top1_acc = Accuracy(task="multiclass", num_classes=num_classes).to(device)
+  top5_acc = Accuracy(task="multiclass", num_classes=num_classes, top_k=5).to(device)
 
 
   counter = 0
 
   if opt1 == 'lion':
     optimizer = Lion(model.parameters(), lr=1e-4, weight_decay=1e-2)
     print("Training with Lion")
@@ -104,15 +104,15 @@
     model.load_state_dict(torch.load(PATH))
 
   epoch = 0
   while counter < set_counter:   #Counter sets the number of epochs of non improvement before stopping
 
       t0 = time.time()
 
-      train(model, trainloader, criterion, scaler, optimizer, epoch)
+      train(model, trainloader, criterion, scaler, optimizer, epoch, device)
 
       correct_1=0
       correct_5=0
       c = 0
       model.eval()
 
       t1 = time.time()
```

### Comparing `dualopt-0.1.1/dualopt.egg-info/PKG-INFO` & `dualopt-0.1.2/dualopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.1/setup.py` & `dualopt-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'dualopt',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.1',
+  version = '0.1.2',
   license='MIT',
   description = 'Dual Optimizer Training',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/DualOpt',
```

