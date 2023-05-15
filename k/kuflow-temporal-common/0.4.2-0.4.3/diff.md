# Comparing `tmp/kuflow_temporal_common-0.4.2.tar.gz` & `tmp/kuflow_temporal_common-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_common-0.4.2.tar", max compression
+gzip compressed data, was "kuflow_temporal_common-0.4.3.tar", max compression
```

## Comparing `kuflow_temporal_common-0.4.2.tar` & `kuflow_temporal_common-0.4.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      789 2023-03-22 13:32:42.999843 kuflow_temporal_common-0.4.2/README.md
--rw-r--r--   0        0        0        6 2023-03-22 13:32:42.999843 kuflow_temporal_common-0.4.2/VERSION
--rw-r--r--   0        0        0     1182 2023-03-22 13:32:42.999843 kuflow_temporal_common-0.4.2/kuflow_temporal_common/__init__.py
--rw-r--r--   0        0        0     1346 2023-03-22 13:32:42.999843 kuflow_temporal_common-0.4.2/kuflow_temporal_common/activity_utils.py
--rw-r--r--   0        0        0     4006 2023-03-22 13:32:42.999843 kuflow_temporal_common-0.4.2/kuflow_temporal_common/authentication.py
--rw-r--r--   0        0        0      777 2023-03-22 13:32:42.999843 kuflow_temporal_common-0.4.2/kuflow_temporal_common/exceptions.py
--rw-r--r--   0        0        0      832 2023-03-22 13:33:52.355017 kuflow_temporal_common-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 kuflow_temporal_common-0.4.2/setup.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 kuflow_temporal_common-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      789 2023-05-15 10:43:31.536858 kuflow_temporal_common-0.4.3/README.md
+-rw-r--r--   0        0        0        6 2023-05-15 10:43:31.540859 kuflow_temporal_common-0.4.3/VERSION
+-rw-r--r--   0        0        0     1182 2023-05-15 10:43:31.540859 kuflow_temporal_common-0.4.3/kuflow_temporal_common/__init__.py
+-rw-r--r--   0        0        0     1346 2023-05-15 10:43:31.540859 kuflow_temporal_common-0.4.3/kuflow_temporal_common/activity_utils.py
+-rw-r--r--   0        0        0     4006 2023-05-15 10:43:31.540859 kuflow_temporal_common-0.4.3/kuflow_temporal_common/authentication.py
+-rw-r--r--   0        0        0      777 2023-05-15 10:43:31.540859 kuflow_temporal_common-0.4.3/kuflow_temporal_common/exceptions.py
+-rw-r--r--   0        0        0      832 2023-05-15 10:44:35.822359 kuflow_temporal_common-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 kuflow_temporal_common-0.4.3/setup.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 kuflow_temporal_common-0.4.3/PKG-INFO
```

### Comparing `kuflow_temporal_common-0.4.2/README.md` & `kuflow_temporal_common-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-0.4.2/kuflow_temporal_common/__init__.py` & `kuflow_temporal_common-0.4.3/kuflow_temporal_common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 # __all__ = ["KuFlowPayloadConverter"]
-__version__ = "0.4.2"
+__version__ = "0.4.3"
```

### Comparing `kuflow_temporal_common-0.4.2/kuflow_temporal_common/activity_utils.py` & `kuflow_temporal_common-0.4.3/kuflow_temporal_common/activity_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-0.4.2/kuflow_temporal_common/authentication.py` & `kuflow_temporal_common-0.4.3/kuflow_temporal_common/authentication.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-0.4.2/kuflow_temporal_common/exceptions.py` & `kuflow_temporal_common-0.4.3/kuflow_temporal_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-0.4.2/pyproject.toml` & `kuflow_temporal_common-0.4.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-common"
-version = "0.4.2"
+version = "0.4.3"
 description = "KuFlow utilities to use Temporal.io"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-rest = "^0.4.2"
+kuflow-rest = "^0.4.3"
 azure-core = "^1.26.3"
 isodate = "^0.6.1"
 temporalio = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "0.910"
 flake8 = "4.0.1"
```

### Comparing `kuflow_temporal_common-0.4.2/PKG-INFO` & `kuflow_temporal_common-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-common
-Version: 0.4.2
+Version: 0.4.3
 Summary: KuFlow utilities to use Temporal.io
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-core (>=1.26.3,<2.0.0)
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
-Requires-Dist: kuflow-rest (>=0.4.2,<0.5.0)
+Requires-Dist: kuflow-rest (>=0.4.3,<0.5.0)
 Requires-Dist: temporalio (>=1.1.0,<2.0.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-common.svg)](https://pypi.org/project/kuflow-temporal-common)
```

