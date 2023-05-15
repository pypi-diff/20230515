# Comparing `tmp/dymoval-0.8.6.tar.gz` & `tmp/dymoval-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dymoval-0.8.6.tar", last modified: Sun May 14 15:24:24 2023, max compression
+gzip compressed data, was "dymoval-0.8.7.tar", last modified: Mon May 15 10:40:52 2023, max compression
```

## Comparing `dymoval-0.8.6.tar` & `dymoval-0.8.7.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0     1550 2023-05-10 21:22:23.170383 dymoval-0.8.6/LICENSE
--rw-r--r--   0        0        0     4351 2023-05-14 08:33:05.019391 dymoval-0.8.6/README.md
--rw-r--r--   0        0        0     1922 2023-05-14 15:24:24.825849 dymoval-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-13 20:32:04.228974 dymoval-0.8.6/src/dymoval/.DS_Store
--rw-r--r--   0        0        0    53248 2023-05-09 13:04:13.533127 dymoval-0.8.6/src/dymoval/.coverage
--rw-r--r--   0        0        0      125 2022-09-25 19:29:24.323833 dymoval-0.8.6/src/dymoval/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-14 07:27:20.556641 dymoval-0.8.6/src/dymoval/config.py
--rw-r--r--   0        0        0   112805 2023-05-14 07:27:20.557127 dymoval-0.8.6/src/dymoval/dataset.py
--rw-r--r--   0        0        0     2589 2023-05-14 07:27:20.557259 dymoval-0.8.6/src/dymoval/utils.py
--rw-r--r--   0        0        0    32835 2023-05-10 20:59:33.498732 dymoval-0.8.6/src/dymoval/validation.py
--rw-r--r--   0        0        0    65913 2023-05-14 07:27:20.557505 dymoval-0.8.6/src/tutorial/DCMotor.fmu
--rw-r--r--   0        0        0  1136010 2023-05-14 07:27:20.562813 dymoval-0.8.6/src/tutorial/DCMotor.svg
--rw-r--r--   0        0        0   963816 2023-05-14 07:27:20.566908 dymoval-0.8.6/src/tutorial/DCMotorLogs.h5
--rw-r--r--   0        0        0      798 2023-05-14 07:27:20.567056 dymoval-0.8.6/src/tutorial/DCMotorModel.py
--rw-r--r--   0        0        0        0 2023-05-14 07:27:20.567078 dymoval-0.8.6/src/tutorial/__init__.py
--rw-r--r--   0        0        0    34918 2023-05-14 07:27:20.567355 dymoval-0.8.6/src/tutorial/tutorial.ipynb
--rw-r--r--   0        0        0        0 2022-09-25 19:29:24.324754 dymoval-0.8.6/tests/__init__.py
--rw-r--r--   0        0        0    12028 2023-05-14 07:27:20.567500 dymoval-0.8.6/tests/fixture_data.py
--rw-r--r--   0        0        0    54384 2023-05-14 07:27:20.567721 dymoval-0.8.6/tests/test_dataset.py
--rw-r--r--   0        0        0    12437 2022-12-07 10:38:33.080813 dymoval-0.8.6/tests/test_initializers.py
--rw-r--r--   0        0        0     3216 2022-12-07 10:38:33.080903 dymoval-0.8.6/tests/test_utils.py
--rw-r--r--   0        0        0    26580 2023-05-10 20:59:33.499045 dymoval-0.8.6/tests/test_validation.py
--rw-r--r--   0        0        0     7396 1970-01-01 00:00:00.000000 dymoval-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1550 2023-05-14 20:41:41.375087 dymoval-0.8.7/LICENSE
+-rw-r--r--   0        0        0     4475 2023-05-15 07:01:30.761752 dymoval-0.8.7/README.md
+-rw-r--r--   0        0        0     1922 2023-05-15 10:40:52.930861 dymoval-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-05-14 20:41:41.380658 dymoval-0.8.7/src/dymoval/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-15 08:02:53.628954 dymoval-0.8.7/src/dymoval/config.py
+-rw-r--r--   0        0        0   112805 2023-05-14 20:41:41.381154 dymoval-0.8.7/src/dymoval/dataset.py
+-rw-r--r--   0        0        0     2543 2023-05-15 10:15:47.636362 dymoval-0.8.7/src/dymoval/utils.py
+-rw-r--r--   0        0        0    32835 2023-05-14 20:41:41.381401 dymoval-0.8.7/src/dymoval/validation.py
+-rw-r--r--   0        0        0    65913 2023-05-14 20:41:41.381658 dymoval-0.8.7/src/tutorial/DCMotor.fmu
+-rw-r--r--   0        0        0  1136010 2023-05-14 20:41:41.386937 dymoval-0.8.7/src/tutorial/DCMotor.svg
+-rw-r--r--   0        0        0   963816 2023-05-14 20:41:41.391006 dymoval-0.8.7/src/tutorial/DCMotorLogs.h5
+-rw-r--r--   0        0        0      798 2023-05-14 20:41:41.391222 dymoval-0.8.7/src/tutorial/DCMotorModel.py
+-rw-r--r--   0        0        0        0 2023-05-14 20:41:41.391250 dymoval-0.8.7/src/tutorial/__init__.py
+-rw-r--r--   0        0        0    34918 2023-05-14 20:41:41.391446 dymoval-0.8.7/src/tutorial/tutorial.ipynb
+-rw-r--r--   0        0        0        0 2023-05-14 20:41:41.391484 dymoval-0.8.7/tests/__init__.py
+-rw-r--r--   0        0        0    12028 2023-05-14 20:41:41.391579 dymoval-0.8.7/tests/fixture_data.py
+-rw-r--r--   0        0        0    54384 2023-05-14 20:41:41.391755 dymoval-0.8.7/tests/test_dataset.py
+-rw-r--r--   0        0        0    12437 2023-05-14 20:41:41.391860 dymoval-0.8.7/tests/test_initializers.py
+-rw-r--r--   0        0        0     3216 2023-05-14 20:41:41.391927 dymoval-0.8.7/tests/test_utils.py
+-rw-r--r--   0        0        0    26580 2023-05-14 20:41:41.392032 dymoval-0.8.7/tests/test_validation.py
+-rw-r--r--   0        0        0     7517 1970-01-01 00:00:00.000000 dymoval-0.8.7/PKG-INFO
```

### Comparing `dymoval-0.8.6/LICENSE` & `dymoval-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/README.md` & `dymoval-0.8.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -99,11 +99,14 @@
 
 
 This will copy the `dymoval_tutorial.ipynb` Jupyter notebook from your installation folder to your `home` folder.
 
 For more info on what is model validation and what is implemented in *dymoval* along with the *dymoval* complete API, you can check the [docs](https://volvogroup.github.io/dymoval/).
 
 > **Note**
-> If your tutorial won't start, you can manually download the tutorial Jupyter notebook from this repo.
+> If your system don't have a default app for opening `.ipynb` files, then the
+> tutorial won't automatically open.
+> However, you have a copy of it in your
+> `home` folder that you can manually open with your preferred app.
 
 ## License
 Dymoval is licensed under [BSD 3](https://github.com/VolvoGroup/dymoval/blob/main/LICENSE) license.
```

### Comparing `dymoval-0.8.6/pyproject.toml` & `dymoval-0.8.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "dymoval"
-version = "0.8.6"
+version = "0.8.7"
 requires-python = ">=3.10"
 dependencies = [
     "pandas",
     "matplotlib",
     "scipy",
     "control",
     "pathlib",
@@ -66,15 +66,15 @@
 target-version = [
     "py310",
 ]
 line-length = 80
 exclude = "/(manual_tests|docs)/"
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 disallow_untyped_defs = true
 show_error_codes = true
 no_implicit_optional = true
 warn_return_any = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 disable_error_code = [
```

### Comparing `dymoval-0.8.6/src/dymoval/config.py` & `dymoval-0.8.7/src/dymoval/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 }
 
 # TODO If you remove python 3.10 remove the dependency (also from pyproject) from tomli as tomlib is
 # part of the standard python package starting from 3.11
 try:
     import tomllib
 except ModuleNotFoundError:
-    import tomli as tomllib
+    import tomli as tomllib  # type: ignore
 
 try:
     with open(
         pathlib.Path.home().joinpath(".dymoval/config.toml"), mode="rb"
     ) as fp:
         data = tomllib.load(fp)
     for k, val in data.items():
```

### Comparing `dymoval-0.8.6/src/dymoval/dataset.py` & `dymoval-0.8.7/src/dymoval/dataset.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/src/dymoval/utils.py` & `dymoval-0.8.7/src/dymoval/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,19 +76,18 @@
     If a dymoval_tutorial.ipynb file already exists in your home
     folder, it will be overwritten.
     """
 
     filename = str(_get_tutorial())
     home = str(Path.home())
     if sys.platform == "win32":
-        # TODO Find a way to remove shell = True
         destination = shutil.copyfile(
             filename, home + "\\dymoval_tutorial.ipynb"
         )
-        shell_process = subprocess.Popen(destination, shell=True)
+        shell_process = subprocess.run(["explorer.exe", destination])
     else:
         destination = shutil.copyfile(
             filename, home + "/dymoval_tutorial.ipynb"
         )
         opener = "open" if sys.platform == "darwin" else "xdg-open"
         shell_process = subprocess.run([opener, destination])
```

### Comparing `dymoval-0.8.6/src/dymoval/validation.py` & `dymoval-0.8.7/src/dymoval/validation.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/src/tutorial/DCMotor.fmu` & `dymoval-0.8.7/src/tutorial/DCMotor.fmu`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/src/tutorial/DCMotor.svg` & `dymoval-0.8.7/src/tutorial/DCMotor.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/src/tutorial/DCMotorLogs.h5` & `dymoval-0.8.7/src/tutorial/DCMotorLogs.h5`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/src/tutorial/DCMotorModel.py` & `dymoval-0.8.7/src/tutorial/DCMotorModel.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/src/tutorial/tutorial.ipynb` & `dymoval-0.8.7/src/tutorial/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/tests/fixture_data.py` & `dymoval-0.8.7/tests/fixture_data.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/tests/test_dataset.py` & `dymoval-0.8.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/tests/test_initializers.py` & `dymoval-0.8.7/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/tests/test_utils.py` & `dymoval-0.8.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/tests/test_validation.py` & `dymoval-0.8.7/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.6/PKG-INFO` & `dymoval-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymoval
-Version: 0.8.6
+Version: 0.8.7
 Summary: Dymoval is a Python package for validating models and analyzing datasets.
 Keywords: data-analysis modeling model validation dataset data
 Author-Email: Ubaldo Tiberi <ubaldo.tiberi@volvo.com>, Ubaldo Tiberi <ubaldo.tiberi@gmail.com>
 License: BSD 3-Clause License
         
         Author: Ubaldo Tiberi.
         Copyright (c) 2018, Volvo Autonomous Solutions.
@@ -165,11 +165,14 @@
 
 
 This will copy the `dymoval_tutorial.ipynb` Jupyter notebook from your installation folder to your `home` folder.
 
 For more info on what is model validation and what is implemented in *dymoval* along with the *dymoval* complete API, you can check the [docs](https://volvogroup.github.io/dymoval/).
 
 > **Note**
-> If your tutorial won't start, you can manually download the tutorial Jupyter notebook from this repo.
+> If your system don't have a default app for opening `.ipynb` files, then the
+> tutorial won't automatically open.
+> However, you have a copy of it in your
+> `home` folder that you can manually open with your preferred app.
 
 ## License
 Dymoval is licensed under [BSD 3](https://github.com/VolvoGroup/dymoval/blob/main/LICENSE) license.
```

