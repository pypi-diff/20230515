# Comparing `tmp/ansar-encode-0.1.74.tar.gz` & `tmp/ansar-encode-0.1.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.74.tar", last modified: Mon May 15 01:55:31 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.75.tar", last modified: Mon May 15 02:16:43 2023, max compression
```

## Comparing `ansar-encode-0.1.74.tar` & `ansar-encode-0.1.75.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4913 2023-05-15 01:55:27.000000 ansar-encode-0.1.74/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19829 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.74/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.74/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 01:55:31.366666 ansar-encode-0.1.74/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-05-15 01:55:31.000000 ansar-encode-0.1.74/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4913 2023-05-15 02:16:40.000000 ansar-encode-0.1.75/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    18929 2023-05-15 02:16:28.000000 ansar-encode-0.1.75/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.75/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.74/LICENSE` & `ansar-encode-0.1.75/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/PKG-INFO` & `ansar-encode-0.1.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.74
+Version: 0.1.75
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.74/README.md` & `ansar-encode-0.1.75/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/setup.py` & `ansar-encode-0.1.75/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/command/show_release.py` & `ansar-encode-0.1.75/src/ansar/command/show_release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/__init__.py` & `ansar-encode-0.1.75/src/ansar/encode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
 Repo: git@github.com:mr-ansar/ansar-encode.git
 Branch: main
-Commit: f759a0972aee86bb1dabe3eae1dabaa975e97f76
-Version: 0.1.73 (2023-05-15@13:55:27+NZST)
+Commit: 07d41b16fec830c88b0ff5f8fee6a80e17bde747
+Version: 0.1.74 (2023-05-15@14:16:40+NZST)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
```

### Comparing `ansar-encode-0.1.74/src/ansar/encode/codec.py` & `ansar-encode-0.1.75/src/ansar/encode/codec.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/convert.py` & `ansar-encode-0.1.75/src/ansar/encode/convert.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/file.py` & `ansar-encode-0.1.75/src/ansar/encode/file.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/folder.py` & `ansar-encode-0.1.75/src/ansar/encode/folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,37 +66,25 @@
     try:
         for f in os.listdir(path):
             p = os.path.join(path, f)
             if os.path.isdir(p):
                 remove_folder(p)
             elif os.path.isfile(p):
                 os.remove(p)
-    except OSError as e:
-        if e.errno == errno.ENOENT:
-            raise FileNotFound(REMOVE_FOLDER, p, 'name does not exist', e.errno)
-        elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(REMOVE_FOLDER, p, 'access or permissions', e.errno)
-        elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(REMOVE_FOLDER, p, 'name in path is not a folder', e.errno)
-        raise FileFailure(REMOVE_FOLDER, p, 'unexpected platform code', code=0)
+    except FileNotFoundError:
+        pass
 #
 #
 def remove_folder(path):
     """Delete everything under the given folder, and then the folder."""
     try:
         remove_contents(path)
         os.rmdir(path)
-    except OSError as e:
-        if e.errno == errno.ENOENT:
-            raise FileNotFound(REMOVE_FOLDER, path, 'name does not exist', e.errno)
-        elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(REMOVE_FOLDER, path, 'access or permissions', e.errno)
-        elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(REMOVE_FOLDER, path, 'name in path is not a folder', e.errno)
-        raise FileFailure(REMOVE_FOLDER, path, 'unexpected platform code', code=0)
+    except FileNotFoundError:
+        pass
 #
 #
 def shape_of_folder(path):
     """Walk the given folder, acumulating folders, files and bytes (3-tuple)."""
     folders, files, bytes = 0, 0, 0
     try:
         for f in os.listdir(path):
```

### Comparing `ansar-encode-0.1.74/src/ansar/encode/json.py` & `ansar-encode-0.1.75/src/ansar/encode/json.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/message.py` & `ansar-encode-0.1.75/src/ansar/encode/message.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/portable.py` & `ansar-encode-0.1.75/src/ansar/encode/portable.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/release.py` & `ansar-encode-0.1.75/src/ansar/encode/release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/runtime.py` & `ansar-encode-0.1.75/src/ansar/encode/runtime.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/version.py` & `ansar-encode-0.1.75/src/ansar/encode/version.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar/encode/xml.py` & `ansar-encode-0.1.75/src/ansar/encode/xml.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.74/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.75/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.74
+Version: 0.1.75
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.74/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.75/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*
