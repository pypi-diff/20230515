# Comparing `tmp/kuflow_robotframework-0.4.3.tar.gz` & `tmp/kuflow_robotframework-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_robotframework-0.4.3.tar", max compression
+gzip compressed data, was "kuflow_robotframework-0.4.4.tar", max compression
```

## Comparing `kuflow_robotframework-0.4.3.tar` & `kuflow_robotframework-0.4.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1337 2023-05-15 10:43:31.536858 kuflow_robotframework-0.4.3/KuFlow/__init__.py
--rw-r--r--   0        0        0    14293 2023-05-15 10:43:31.536858 kuflow_robotframework-0.4.3/KuFlow/keywords.py
--rw-r--r--   0        0        0     2025 2023-05-15 10:43:31.536858 kuflow_robotframework-0.4.3/README.md
--rw-r--r--   0        0        0        6 2023-05-15 10:43:31.536858 kuflow_robotframework-0.4.3/VERSION
--rw-r--r--   0        0        0      925 2023-05-15 10:44:34.846275 kuflow_robotframework-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 kuflow_robotframework-0.4.3/setup.py
--rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 kuflow_robotframework-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1337 2023-05-15 11:28:31.337287 kuflow_robotframework-0.4.4/KuFlow/__init__.py
+-rw-r--r--   0        0        0    14293 2023-05-15 11:28:31.337287 kuflow_robotframework-0.4.4/KuFlow/keywords.py
+-rw-r--r--   0        0        0     2025 2023-05-15 11:28:31.337287 kuflow_robotframework-0.4.4/README.md
+-rw-r--r--   0        0        0        6 2023-05-15 11:28:31.337287 kuflow_robotframework-0.4.4/VERSION
+-rw-r--r--   0        0        0      925 2023-05-15 11:30:01.845082 kuflow_robotframework-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 kuflow_robotframework-0.4.4/setup.py
+-rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 kuflow_robotframework-0.4.4/PKG-INFO
```

### Comparing `kuflow_robotframework-0.4.3/KuFlow/__init__.py` & `kuflow_robotframework-0.4.4/KuFlow/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 from .keywords import Keywords
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 __all__ = ["KuFlow"]
 
 
 class KuFlow(Keywords):
     """KuFlow: Automagic Workflows."""
 
     ROBOT_LIBRARY_VERSION = __version__
```

### Comparing `kuflow_robotframework-0.4.3/KuFlow/keywords.py` & `kuflow_robotframework-0.4.4/KuFlow/keywords.py`

 * *Files identical despite different names*

### Comparing `kuflow_robotframework-0.4.3/README.md` & `kuflow_robotframework-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_robotframework-0.4.3/pyproject.toml` & `kuflow_robotframework-0.4.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-robotframework"
-version = "0.4.3"
+version = "0.4.4"
 description = "KuFlow library for Robot Framework"
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
-kuflow-rest = "^0.4.3"
+kuflow-rest = "^0.4.4"
 robotframework = "^5.0"
 python-magic = {version = "^0.4.27", platform = "!=win32"}
 python-magic-bin = {version = "^0.4.14", platform = "win32"}
 
 [tool.poetry.group.dev.dependencies]
 mypy = "0.910"
 flake8 = "4.0.1"
```

### Comparing `kuflow_robotframework-0.4.3/setup.py` & `kuflow_robotframework-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['KuFlow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-rest>=0.4.3,<0.5.0', 'robotframework>=5.0,<6.0']
+['kuflow-rest>=0.4.4,<0.5.0', 'robotframework>=5.0,<6.0']
 
 extras_require = \
 {':sys_platform != "win32"': ['python-magic>=0.4.27,<0.5.0'],
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 setup_kwargs = {
     'name': 'kuflow-robotframework',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'KuFlow library for Robot Framework',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-robotframework.svg)](https://pypi.org/project/kuflow-robotframework)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-robotframework.svg)](https://pypi.org/project/kuflow-robotframework)\n\n# KuFlow Robot Framework\n\nThis library provides keywords to interact with the KuFlow API from a Robot Framework Robot. Its purpose is to facilitate interaction from the robot logic (RPA). Its use helps to keep the manipulation of robot results by Workflow decoupled as much as possible.\n\nList of available keywords:\n\n#### Set Client Authentication\n\n> Configure the client authentication in order to execute keywords against Rest API\n\n#### Append Log Message\n\n> Add a log entry to the task\n\n#### Claim Task\n\n> Allow to claim a task\n\n#### Retrieve Process\n\n> Allow to get a process by ID\n\n#### Retrieve Task\n\n> Allow to get a task by ID\n\n#### Save Element Document\n\n> Save a element task of type document\n\n#### Delete Element Document\n\n> Allow to delete a specific document from an element of document type using its id.\n\n#### Save Element\n\n> Save a element task\n\n#### Delete Element\n\n> Allow to delete task element by specifying the item definition code.\n\n#### Convert To Principal Item\n\n> Given an Id of a Principal user, create an item that represents a reference to the Principal.\n\n#### Convert To Document Item From Uri\n\n> Given an Id of a Document or the URI reference of a Document, create an item that represents a reference to the Document elementand can be used.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_robotframework-0.4.3/PKG-INFO` & `kuflow_robotframework-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-robotframework
-Version: 0.4.3
+Version: 0.4.4
 Summary: KuFlow library for Robot Framework
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
-Requires-Dist: kuflow-rest (>=0.4.3,<0.5.0)
+Requires-Dist: kuflow-rest (>=0.4.4,<0.5.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0) ; sys_platform != "win32"
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: robotframework (>=5.0,<6.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
```

