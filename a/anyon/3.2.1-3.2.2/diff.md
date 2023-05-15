# Comparing `tmp/anyon-3.2.1-cp311-cp311-win_amd64.whl.zip` & `tmp/anyon-3.2.2-cp311-cp311-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 365957 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-09 03:16 anyon-3.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1192 b- defN 23-May-09 03:16 anyon-3.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-09 03:16 anyon-3.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-09 03:16 anyon-3.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      376 b- defN 23-May-09 03:16 anyon-3.2.1.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20480 b- defN 23-May-09 03:16 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    76288 b- defN 23-May-09 03:16 anyon/loader.pyd
--rw-rw-rw-  2.0 fat    99840 b- defN 23-May-09 03:16 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   179200 b- defN 23-May-09 03:16 anyon/server.pyd
--rw-rw-rw-  2.0 fat    20992 b- defN 23-May-09 03:16 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat    92672 b- defN 23-May-09 03:16 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   134144 b- defN 23-May-09 03:16 anyon/stage/compiler.pyd
--rw-rw-rw-  2.0 fat    61952 b- defN 23-May-09 03:16 anyon/stage/demodulator.pyd
--rw-rw-rw-  2.0 fat   114176 b- defN 23-May-09 03:16 anyon/stage/device.pyd
-14 files, 802495 bytes uncompressed, 364195 bytes compressed:  54.6%
+Zip file size: 2339544 bytes, number of entries: 14
+-rwxrwxrwx  2.0 unx     1080 b- defN 23-May-15 06:42 anyon-3.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1160 b- defN 23-May-15 06:42 anyon-3.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-15 06:42 anyon-3.2.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        1 b- defN 23-May-15 06:42 anyon-3.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      376 b- defN 23-May-15 06:42 anyon-3.2.2.dist-info/RECORD
+-rwxr-xr-x  2.0 unx    73384 b- defN 23-May-15 06:42 anyon/__init__.so
+-rwxr-xr-x  2.0 unx   453736 b- defN 23-May-15 06:42 anyon/loader.so
+-rwxr-xr-x  2.0 unx   709192 b- defN 23-May-15 06:42 anyon/remote.so
+-rwxr-xr-x  2.0 unx  1381136 b- defN 23-May-15 06:42 anyon/server.so
+-rwxr-xr-x  2.0 unx    75128 b- defN 23-May-15 06:42 anyon/stage/__init__.so
+-rwxr-xr-x  2.0 unx   725680 b- defN 23-May-15 06:42 anyon/stage/calculator.so
+-rwxr-xr-x  2.0 unx   960384 b- defN 23-May-15 06:42 anyon/stage/compiler.so
+-rwxr-xr-x  2.0 unx   412480 b- defN 23-May-15 06:42 anyon/stage/demodulator.so
+-rwxr-xr-x  2.0 unx   868376 b- defN 23-May-15 06:42 anyon/stage/device.so
+14 files, 5662223 bytes uncompressed, 2337800 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
-Filename: anyon-3.2.1.dist-info/LICENSE
+Filename: anyon-3.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-3.2.1.dist-info/METADATA
+Filename: anyon-3.2.2.dist-info/METADATA
 Comment: 
 
-Filename: anyon-3.2.1.dist-info/WHEEL
+Filename: anyon-3.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-3.2.1.dist-info/top_level.txt
+Filename: anyon-3.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-3.2.1.dist-info/RECORD
+Filename: anyon-3.2.2.dist-info/RECORD
 Comment: 
 
-Filename: anyon/__init__.pyd
+Filename: anyon/__init__.so
 Comment: 
 
-Filename: anyon/loader.pyd
+Filename: anyon/loader.so
 Comment: 
 
-Filename: anyon/remote.pyd
+Filename: anyon/remote.so
 Comment: 
 
-Filename: anyon/server.pyd
+Filename: anyon/server.so
 Comment: 
 
-Filename: anyon/stage/__init__.pyd
+Filename: anyon/stage/__init__.so
 Comment: 
 
-Filename: anyon/stage/calculator.pyd
+Filename: anyon/stage/calculator.so
 Comment: 
 
-Filename: anyon/stage/compiler.pyd
+Filename: anyon/stage/compiler.so
 Comment: 
 
-Filename: anyon/stage/demodulator.pyd
+Filename: anyon/stage/demodulator.so
 Comment: 
 
-Filename: anyon/stage/device.pyd
+Filename: anyon/stage/device.so
 Comment: 
 
 Zip file comment:
```

## Comparing `anyon-3.2.1.dist-info/LICENSE` & `anyon-3.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anyon-3.2.1.dist-info/METADATA` & `anyon-3.2.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-Metadata-Version: 2.1
-Name: anyon
-Version: 3.2.1
-Summary: Dream It Possible!
-Home-page: https://gitee.com/
-Author: YL Feng
-Author-email: fengyulong@pku.edu.cn
-License: MIT
-Project-URL: source, https://gitee.com
-Keywords: Hello,World!
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: axion (>=3.2.29)
-Requires-Dist: srpc (>=4.2.8)
-Requires-Dist: zee (>=0.0.2)
-Requires-Dist: requests (>=2.28.0)
-
-#### 介绍
-
-
-#### 软件架构
-
-
-#### 安装教程
-
-
-#### 使用说明
-
-
-#### 参与贡献
-
-
-#### 特技
-
-
-
-
-
+Metadata-Version: 2.1
+Name: anyon
+Version: 3.2.2
+Summary: Dream It Possible!
+Home-page: https://gitee.com/
+Author: YL Feng
+Author-email: fengyulong@pku.edu.cn
+License: MIT
+Project-URL: source, https://gitee.com
+Keywords: Hello,World!
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: axion (>=3.3.1)
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: requests (>=2.28.0)
+Requires-Dist: srpc (>=4.2.8)
+Requires-Dist: zee (>=0.0.2)
+
+#### 介绍
+
+
+#### 软件架构
+
+
+#### 安装教程
+
+
+#### 使用说明
+
+
+#### 参与贡献
+
+
+#### 特技
+
+
+
+
+
+
+
```

