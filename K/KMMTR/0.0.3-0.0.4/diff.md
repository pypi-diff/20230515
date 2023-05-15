# Comparing `tmp/KMMTR-0.0.3.tar.gz` & `tmp/KMMTR-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMMTR-0.0.3.tar", last modified: Sun May  7 13:25:47 2023, max compression
+gzip compressed data, was "KMMTR-0.0.4.tar", last modified: Mon May 15 09:04:50 2023, max compression
```

## Comparing `KMMTR-0.0.3.tar` & `KMMTR-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-07 13:25:47.133951 KMMTR-0.0.3/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-07 13:25:47.133015 KMMTR-0.0.3/KMMTR/
--rwxr-xr-x   0 jacob      (501) staff       (20)     6562 2023-05-07 13:24:43.000000 KMMTR-0.0.3/KMMTR/KMM.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     6511 2023-05-03 02:58:16.000000 KMMTR-0.0.3/KMMTR/KMMTR.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-0.0.3/KMMTR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-07 13:25:47.133646 KMMTR-0.0.3/KMMTR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-07 13:25:47.000000 KMMTR-0.0.3/KMMTR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-07 13:25:47.000000 KMMTR-0.0.3/KMMTR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-07 13:25:47.000000 KMMTR-0.0.3/KMMTR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-07 13:25:47.000000 KMMTR-0.0.3/KMMTR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-07 13:25:47.000000 KMMTR-0.0.3/KMMTR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-07 13:25:47.133822 KMMTR-0.0.3/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-0.0.3/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-07 13:25:47.133988 KMMTR-0.0.3/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-07 13:25:18.000000 KMMTR-0.0.3/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 09:04:50.280830 KMMTR-0.0.4/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 09:04:50.279948 KMMTR-0.0.4/KMMTR/
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6614 2023-05-15 09:03:46.000000 KMMTR-0.0.4/KMMTR/KMM.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6511 2023-05-03 02:58:16.000000 KMMTR-0.0.4/KMMTR/KMMTR.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-0.0.4/KMMTR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 09:04:50.280525 KMMTR-0.0.4/KMMTR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-15 09:04:50.000000 KMMTR-0.0.4/KMMTR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-15 09:04:50.000000 KMMTR-0.0.4/KMMTR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-15 09:04:50.000000 KMMTR-0.0.4/KMMTR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-15 09:04:50.000000 KMMTR-0.0.4/KMMTR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-15 09:04:50.000000 KMMTR-0.0.4/KMMTR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-15 09:04:50.280690 KMMTR-0.0.4/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-0.0.4/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-15 09:04:50.280871 KMMTR-0.0.4/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-15 09:04:11.000000 KMMTR-0.0.4/setup.py
```

### Comparing `KMMTR-0.0.3/KMMTR/KMM.py` & `KMMTR-0.0.4/KMMTR/KMM.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             An instantiated kernel function object.
         """
         Xtrain = np.array(self.target_data)
         Ytrain = np.array(self.target_response)
         ker = self.call_kernel()
         noise_ker = WhiteKernel(noise_level_bounds=(0.01,100))
         # cal the data nosie by maximazing the likelihood 
-        GPr = GPR(kernel=ker+noise_ker).fit(Xtrain,Ytrain)
+        GPr = GPR(kernel=ker+noise_ker).fit(Xtrain[:,:-int(0.8*len(Xtrain))],Ytrain[:,:-int(0.8*len(Xtrain))])
         noise_level = np.exp(GPr.kernel_.theta[1])
 
         GPr_fit = GPR(kernel=ker, alpha = noise_level).fit(Xtrain,Ytrain)
         print('Trained Kernel Function :', GPr_fit.kernel_)
         para = np.exp(GPr_fit.kernel_.theta)
 
         Inst_kernel = self.call_kernel(para)
```

### Comparing `KMMTR-0.0.3/KMMTR/KMMTR.py` & `KMMTR-0.0.4/KMMTR/KMMTR.py`

 * *Files identical despite different names*

### Comparing `KMMTR-0.0.3/KMMTR.egg-info/PKG-INFO` & `KMMTR-0.0.4/KMMTR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 0.0.3
+Version: 0.0.4
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-0.0.3/PKG-INFO` & `KMMTR-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 0.0.3
+Version: 0.0.4
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-0.0.3/README.md` & `KMMTR-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `KMMTR-0.0.3/setup.py` & `KMMTR-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='KMMTR',  # 包名
-    version='0.0.3',  # 版本
+    version='0.0.4',  # 版本
     description="a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

