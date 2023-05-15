# Comparing `tmp/ansar-encode-0.1.71.tar.gz` & `tmp/ansar-encode-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.71.tar", last modified: Sat Apr 29 21:25:25 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.74.tar", last modified: Mon May 15 01:55:31 2023, max compression
```

## Comparing `ansar-encode-0.1.71.tar` & `ansar-encode-0.1.74.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4913 2023-04-29 21:25:22.000000 ansar-encode-0.1.71/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19829 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.71/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4913 2023-05-15 01:55:27.000000 ansar-encode-0.1.74/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19829 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.74/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.71/LICENSE` & `ansar-encode-0.1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/PKG-INFO` & `ansar-encode-0.1.74/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.71
+Version: 0.1.74
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.71/README.md` & `ansar-encode-0.1.74/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/setup.py` & `ansar-encode-0.1.74/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/command/show_release.py` & `ansar-encode-0.1.74/src/ansar/command/show_release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/__init__.py` & `ansar-encode-0.1.74/src/ansar/encode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
 Repo: git@github.com:mr-ansar/ansar-encode.git
 Branch: main
-Commit: f414395799da108c69abeb2ec79fcc978eccde59
-Version: 0.1.70 (2023-04-30@09:25:22+NZST)
+Commit: f759a0972aee86bb1dabe3eae1dabaa975e97f76
+Version: 0.1.73 (2023-05-15@13:55:27+NZST)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
```

### Comparing `ansar-encode-0.1.71/src/ansar/encode/codec.py` & `ansar-encode-0.1.74/src/ansar/encode/codec.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/convert.py` & `ansar-encode-0.1.74/src/ansar/encode/convert.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/file.py` & `ansar-encode-0.1.74/src/ansar/encode/file.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/folder.py` & `ansar-encode-0.1.74/src/ansar/encode/folder.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/json.py` & `ansar-encode-0.1.74/src/ansar/encode/json.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/message.py` & `ansar-encode-0.1.74/src/ansar/encode/message.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/portable.py` & `ansar-encode-0.1.74/src/ansar/encode/portable.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/release.py` & `ansar-encode-0.1.74/src/ansar/encode/release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/runtime.py` & `ansar-encode-0.1.74/src/ansar/encode/runtime.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/version.py` & `ansar-encode-0.1.74/src/ansar/encode/version.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar/encode/xml.py` & `ansar-encode-0.1.74/src/ansar/encode/xml.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.71/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.74/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.71
+Version: 0.1.74
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.71/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.74/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

