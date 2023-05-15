# Comparing `tmp/hex_utility_pkg-0.0.1.tar.gz` & `tmp/hex_utility_pkg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hex_utility_pkg-0.0.1.tar", last modified: Sun May 14 08:31:10 2023, max compression
+gzip compressed data, was "hex_utility_pkg-0.0.2.tar", last modified: Mon May 15 05:27:29 2023, max compression
```

## Comparing `hex_utility_pkg-0.0.1.tar` & `hex_utility_pkg-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:31:10.482941 hex_utility_pkg-0.0.1/
--rw-rw-rw-   0        0        0       62 2023-05-14 08:31:10.448992 hex_utility_pkg-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-14 08:30:10.000000 hex_utility_pkg-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 08:31:10.483940 hex_utility_pkg-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 08:31:10.020164 hex_utility_pkg-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 08:31:10.098118 hex_utility_pkg-0.0.1/src/hex_utility_pkg/
--rw-rw-rw-   0        0        0        0 2023-04-27 23:02:11.000000 hex_utility_pkg-0.0.1/src/hex_utility_pkg/__init__.py
--rw-rw-rw-   0        0        0     1280 2023-04-15 01:09:03.000000 hex_utility_pkg-0.0.1/src/hex_utility_pkg/calsum.py
--rw-rw-rw-   0        0        0     1803 2023-04-30 06:39:11.000000 hex_utility_pkg-0.0.1/src/hex_utility_pkg/spilt_string.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:31:10.389243 hex_utility_pkg-0.0.1/src/hex_utility_pkg.egg-info/
--rw-rw-rw-   0        0        0       62 2023-05-14 08:31:09.000000 hex_utility_pkg-0.0.1/src/hex_utility_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-05-14 08:31:09.000000 hex_utility_pkg-0.0.1/src/hex_utility_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:31:09.000000 hex_utility_pkg-0.0.1/src/hex_utility_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-14 08:31:09.000000 hex_utility_pkg-0.0.1/src/hex_utility_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-14 08:31:09.000000 hex_utility_pkg-0.0.1/src/hex_utility_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 05:27:28.990924 hex_utility_pkg-0.0.2/
+-rw-rw-rw-   0        0        0       62 2023-05-15 05:27:28.989732 hex_utility_pkg-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-05-15 03:46:03.000000 hex_utility_pkg-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:27:28.990924 hex_utility_pkg-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 05:27:28.125880 hex_utility_pkg-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 05:27:28.456906 hex_utility_pkg-0.0.2/src/hex_utility_pkg/
+-rw-rw-rw-   0        0        0        0 2023-05-15 00:53:55.000000 hex_utility_pkg-0.0.2/src/hex_utility_pkg/__init__.py
+-rw-rw-rw-   0        0        0     1457 2023-05-15 03:34:48.000000 hex_utility_pkg-0.0.2/src/hex_utility_pkg/calsum.py
+-rw-rw-rw-   0        0        0     2100 2023-05-15 03:37:17.000000 hex_utility_pkg-0.0.2/src/hex_utility_pkg/spilt_string.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:27:28.987846 hex_utility_pkg-0.0.2/src/hex_utility_pkg.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-05-15 05:27:26.000000 hex_utility_pkg-0.0.2/src/hex_utility_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-05-15 05:27:27.000000 hex_utility_pkg-0.0.2/src/hex_utility_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:27:27.000000 hex_utility_pkg-0.0.2/src/hex_utility_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-15 05:27:27.000000 hex_utility_pkg-0.0.2/src/hex_utility_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 05:27:27.000000 hex_utility_pkg-0.0.2/src/hex_utility_pkg.egg-info/top_level.txt
```

### Comparing `hex_utility_pkg-0.0.1/pyproject.toml` & `hex_utility_pkg-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hex_utility_pkg"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
     "requests",
     'importlib-metadata; python_version>"3.8"',
 ]
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
```

### Comparing `hex_utility_pkg-0.0.1/src/hex_utility_pkg/calsum.py` & `hex_utility_pkg-0.0.2/src/hex_utility_pkg/calsum.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         self.SoureHexDataEdit =  QtWidgets.QTextEdit()
         self.SumEdit = QtWidgets.QTextEdit()
         self.layout = QtWidgets.QVBoxLayout(self)
         self.layout.addWidget(self.SoureHexDataEdit)
         self.layout.addWidget(self.SumEdit)
         self.layout.addWidget(self.button)
 
+        self.SoureHexDataEdit.setPlaceholderText("请填入16进制字符串，支持空格，\",\", \"-\"分隔符。")
+        self.SumEdit.setPlaceholderText("校验和:")
         self.button.clicked.connect(self.calculateSumBtnHandle)
 
 
     @QtCore.Slot()
     def calculateSumBtnHandle(self):
         sum = 0
         str =  self.SoureHexDataEdit.toPlainText()
```

### Comparing `hex_utility_pkg-0.0.1/src/hex_utility_pkg/spilt_string.py` & `hex_utility_pkg-0.0.2/src/hex_utility_pkg/spilt_string.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,17 @@
         self.hello = ["Hallo Welt", "Hei maailma", "Hola Mundo", "Привет мир"]
         self.button = QtWidgets.QPushButton("16进制数转ASCII字符串")
     
         self.SoureHexDataEdit =  QtWidgets.QTextEdit()
         self.StringSpiltEdit = QtWidgets.QTextEdit()
         self.ASCII_String_Edit = QtWidgets.QTextEdit()
 
+        self.SoureHexDataEdit.setPlaceholderText("16进制转字符串,请填入16进制字符串，支持空格，\",\", \"-\"分隔符。")
+        self.StringSpiltEdit.setPlaceholderText("分隔后的字符串：")
+        self.ASCII_String_Edit.setPlaceholderText("转换后的字符串:")
         self.layout = QtWidgets.QVBoxLayout(self)
         self.layout.addWidget(self.SoureHexDataEdit)
         self.layout.addWidget(self.StringSpiltEdit)
         self.layout.addWidget(self.ASCII_String_Edit)
         self.layout.addWidget(self.button)
         self.button.clicked.connect(self.calculateSumBtnHandle)
```

