# Comparing `tmp/cognite_extractor_manager-0.8.1.tar.gz` & `tmp/cognite_extractor_manager-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_manager-0.8.1.tar", max compression
+gzip compressed data, was "cognite_extractor_manager-0.8.2.tar", max compression
```

## Comparing `cognite_extractor_manager-0.8.1.tar` & `cognite_extractor_manager-0.8.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10173 2023-05-12 13:01:10.008816 cognite_extractor_manager-0.8.1/LICENSE
--rw-r--r--   0        0        0     3816 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/README.md
--rw-r--r--   0        0        0      607 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/__init__.py
--rw-r--r--   0        0        0     3049 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/__main__.py
--rw-r--r--   0        0        0      294 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/_common.py
--rw-r--r--   0        0        0     5303 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/build.py
--rw-r--r--   0        0        0     4701 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/docker.py
--rw-r--r--   0        0        0    10553 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/initialize.py
--rw-r--r--   0        0        0     1830 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/io.py
--rw-r--r--   0        0        0     2334 2023-05-12 13:01:10.012816 cognite_extractor_manager-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4532 1970-01-01 00:00:00.000000 cognite_extractor_manager-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/LICENSE
+-rw-r--r--   0        0        0     3816 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/README.md
+-rw-r--r--   0        0        0      607 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/__init__.py
+-rw-r--r--   0        0        0     3049 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/__main__.py
+-rw-r--r--   0        0        0      294 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/_common.py
+-rw-r--r--   0        0        0     5298 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/build.py
+-rw-r--r--   0        0        0     4701 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/docker.py
+-rw-r--r--   0        0        0    10553 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/initialize.py
+-rw-r--r--   0        0        0     1830 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/io.py
+-rw-r--r--   0        0        0     2334 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4532 1970-01-01 00:00:00.000000 cognite_extractor_manager-0.8.2/PKG-INFO
```

### Comparing `cognite_extractor_manager-0.8.1/LICENSE` & `cognite_extractor_manager-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.1/README.md` & `cognite_extractor_manager-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/__init__.py` & `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
```

### Comparing `cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/__main__.py` & `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/__main__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/build.py` & `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 def update_version(initfile: str) -> None:
     print(f"Updating {initfile}")
 
     init_version_search = re.search(r'^__version__\s*=\s*"(.*)"', open(initfile).read(), re.M)
     if init_version_search is None:
         print("No __version__ found")
-        sys.exit(1)
+        return
 
     init_version = init_version_search.group(1)
     print(f"Version in {initfile}: {init_version}")
 
     poetry_version = get_pyproject()["tool"]["poetry"]["version"]
     print(f"Version in pyproject.toml: {poetry_version}")
```

### Comparing `cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/docker.py` & `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/docker.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/initialize.py` & `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/initialize.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.1/cognite/extractorutils/cogex/io.py` & `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/io.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.1/pyproject.toml` & `cognite_extractor_manager-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-manager"
-version = "0.8.1"
+version = "0.8.2"
 description = "A project manager for Python based extractors"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include="cognite", from="." },
```

### Comparing `cognite_extractor_manager-0.8.1/PKG-INFO` & `cognite_extractor_manager-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-manager
-Version: 0.8.1
+Version: 0.8.2
 Summary: A project manager for Python based extractors
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

