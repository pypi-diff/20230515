# Comparing `tmp/pibrary-0.2.0a1.tar.gz` & `tmp/pibrary-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibrary-0.2.0a1.tar", max compression
+gzip compressed data, was "pibrary-0.2.0a2.tar", max compression
```

## Comparing `pibrary-0.2.0a1.tar` & `pibrary-0.2.0a2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-05-08 15:05:56.342612 pibrary-0.2.0a1/LICENSE
--rw-r--r--   0        0        0     1750 2023-05-15 03:36:38.146800 pibrary-0.2.0a1/README.md
--rw-r--r--   0        0        0        0 2023-05-09 06:39:08.627636 pibrary-0.2.0a1/pibrary/__init__.py
--rw-r--r--   0        0        0     4446 2023-05-12 02:16:45.133836 pibrary-0.2.0a1/pibrary/file.py
--rw-r--r--   0        0        0      939 2023-05-08 15:05:56.343483 pibrary-0.2.0a1/pibrary/logger.py
--rw-r--r--   0        0        0     1435 2023-05-14 14:59:23.553176 pibrary-0.2.0a1/pibrary/string.py
--rw-r--r--   0        0        0      487 2023-05-15 03:47:16.612269 pibrary-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     2497 1970-01-01 00:00:00.000000 pibrary-0.2.0a1/setup.py
--rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 pibrary-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-15 09:02:08.712683 pibrary-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0     1750 2023-05-15 09:02:08.712683 pibrary-0.2.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 09:02:08.712683 pibrary-0.2.0a2/pibrary/__init__.py
+-rw-r--r--   0        0        0     4446 2023-05-15 09:02:08.712683 pibrary-0.2.0a2/pibrary/file.py
+-rw-r--r--   0        0        0      939 2023-05-15 09:02:08.712683 pibrary-0.2.0a2/pibrary/logger.py
+-rw-r--r--   0        0        0     1435 2023-05-15 09:02:08.712683 pibrary-0.2.0a2/pibrary/string.py
+-rw-r--r--   0        0        0      487 2023-05-15 09:02:08.716683 pibrary-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 pibrary-0.2.0a2/PKG-INFO
```

### Comparing `pibrary-0.2.0a1/LICENSE` & `pibrary-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a1/README.md` & `pibrary-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a1/pibrary/file.py` & `pibrary-0.2.0a2/pibrary/file.py`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a1/pibrary/logger.py` & `pibrary-0.2.0a2/pibrary/logger.py`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a1/pibrary/string.py` & `pibrary-0.2.0a2/pibrary/string.py`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a1/setup.py` & `pibrary-0.2.0a2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,77 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pibrary
+Version: 0.2.0a2
+Summary: A package for reusable code for ML projects.
+License: MIT
+Author: Prakash Chaudhary
+Author-email: connectwithprakash@gmail.com
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Description-Content-Type: text/markdown
+
+# Pibrary
+
+<p align="center">
+    <em>Pibrary framework: A package for reusable code for ML projects</em>
+</p>
+<p align="center">
+    <a href="https://github.com/connectwithprakash/pibrary/actions?query=workflow%3ATest+event%3Apush+branch%3Amain" target="_blank">
+        <img src="https://github.com/connectwithprakash/pibrary/workflows/Test/badge.svg?event=push&branch=main" alt="Test">
+    </a>
+    <a href="https://pypi.org/project/pibrary" target="_blank">
+        <img src="https://img.shields.io/pypi/v/pibrary?color=%2334D058&label=pypi%20package" alt="Package version">
+    </a>
+    <a href="https://pypi.org/project/pibrary" target="_blank">
+        <img src="https://img.shields.io/pypi/pyversions/pibrary.svg?color=%2334D058" alt="Supported Python versions">
+    </a>
+    <a href="https://opensource.org/licenses/MIT" target="_blank">
+        <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT">
+    </a>
+</p>
+
+## Installation
+
+```bash
+pip install pibrary
+```
+
+## Usage
+```python
+from pibrary.file import File
+from pibrary.logger import timeit
+from pibrary.string import String
+
+# File Class
+dataframe = File(file_path).read().csv()
+File(file_path).write(dataframe).csv()
+
+json_data = File(file_path).read().json()
+File(file_path).write(json_data).csv()
+
+pickle_data = File(file_path).read().pickle()
+File(file_path).write(pickle_data).csv()
+
+# Logger
+@timeit
+def some_function(...):
+    ...
+
+# String Class
+new_text = String(text).lower().remove_digits().remove_punctuation().strip()
+```
 
-packages = \
-['pibrary']
+## Contributing
+Contributions are welcome! Please read [CONTRIBUTING](CONTRIBUTING) for details on how to contribute to this project.
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['joblib>=1.2.0,<2.0.0', 'loguru>=0.7.0,<0.8.0', 'pandas>=2.0.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'pibrary',
-    'version': '0.2.0a1',
-    'description': 'A package for reusable code for ML projects.',
-    'long_description': '# Pibrary\n\n<p align="center">\n    <em>Pibrary framework: A package for reusable code for ML projects</em>\n</p>\n<p align="center">\n    <a href="https://github.com/connectwithprakash/pibrary/actions?query=workflow%3ATest+event%3Apush+branch%3Amain" target="_blank">\n        <img src="https://github.com/connectwithprakash/pibrary/workflows/Test/badge.svg?event=push&branch=main" alt="Test">\n    </a>\n    <a href="https://pypi.org/project/pibrary" target="_blank">\n        <img src="https://img.shields.io/pypi/v/pibrary?color=%2334D058&label=pypi%20package" alt="Package version">\n    </a>\n    <a href="https://pypi.org/project/pibrary" target="_blank">\n        <img src="https://img.shields.io/pypi/pyversions/pibrary.svg?color=%2334D058" alt="Supported Python versions">\n    </a>\n    <a href="https://opensource.org/licenses/MIT" target="_blank">\n        <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT">\n    </a>\n</p>\n\n## Installation\n\n```bash\npip install pibrary\n```\n\n## Usage\n```python\nfrom pibrary.file import File\nfrom pibrary.logger import timeit\nfrom pibrary.string import String\n\n# File Class\ndataframe = File(file_path).read().csv()\nFile(file_path).write(dataframe).csv()\n\njson_data = File(file_path).read().json()\nFile(file_path).write(json_data).csv()\n\npickle_data = File(file_path).read().pickle()\nFile(file_path).write(pickle_data).csv()\n\n# Logger\n@timeit\ndef some_function(...):\n    ...\n\n# String Class\nnew_text = String(text).lower().remove_digits().remove_punctuation().strip()\n```\n\n## Contributing\nContributions are welcome! Please read [CONTRIBUTING](CONTRIBUTING) for details on how to contribute to this project.\n\n\n# License\nThis project is licensed under the terms of the [MIT license](LICENSE).\n',
-    'author': 'Prakash Chaudhary',
-    'author_email': 'connectwithprakash@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8',
-}
+# License
+This project is licensed under the terms of the [MIT license](LICENSE).
 
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,25 +1,22 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['pibrary']
-package_data = \ {'': ['*']} install_requires = \ ['joblib>=1.2.0,<2.0.0',
-'loguru>=0.7.0,<0.8.0', 'pandas>=2.0.1,<3.0.0'] setup_kwargs = { 'name':
-'pibrary', 'version': '0.2.0a1', 'description': 'A package for reusable code
-for ML projects.', 'long_description': '# Pibrary\n\n
-      \n Pibrary framework: A package for reusable code for ML projects\n
-\n
-\n \n_[Test]\n\n \n_[Package_version]\n\n \n_[Supported_Python_versions]\n\n \n
-                              [License:_MIT]\n\n
-\n\n## Installation\n\n```bash\npip install pibrary\n```\n\n##
-Usage\n```python\nfrom pibrary.file import File\nfrom pibrary.logger import
-timeit\nfrom pibrary.string import String\n\n# File Class\ndataframe = File
-(file_path).read().csv()\nFile(file_path).write(dataframe).csv()\n\njson_data =
-File(file_path).read().json()\nFile(file_path).write(json_data).csv
-()\n\npickle_data = File(file_path).read().pickle()\nFile(file_path).write
-(pickle_data).csv()\n\n# Logger\n@timeit\ndef some_function(...):\n ...\n\n#
-String Class\nnew_text = String(text).lower().remove_digits
-().remove_punctuation().strip()\n```\n\n## Contributing\nContributions are
-welcome! Please read [CONTRIBUTING](CONTRIBUTING) for details on how to
-contribute to this project.\n\n\n# License\nThis project is licensed under the
-terms of the [MIT license](LICENSE).\n', 'author': 'Prakash Chaudhary',
-'author_email': 'connectwithprakash@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: pibrary Version: 0.2.0a2 Summary: A package for
+reusable code for ML projects. License: MIT Author: Prakash Chaudhary Author-
+email: connectwithprakash@gmail.com Requires-Python: >=3.8 Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: joblib
+(>=1.2.0,<2.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: pandas
+(>=2.0.1,<3.0.0) Description-Content-Type: text/markdown # Pibrary
+        Pibrary framework: A package for reusable code for ML projects
+      [Test] [Package_version] [Supported_Python_versions] [License:_MIT]
+## Installation ```bash pip install pibrary ``` ## Usage ```python from
+pibrary.file import File from pibrary.logger import timeit from pibrary.string
+import String # File Class dataframe = File(file_path).read().csv() File
+(file_path).write(dataframe).csv() json_data = File(file_path).read().json()
+File(file_path).write(json_data).csv() pickle_data = File(file_path).read
+().pickle() File(file_path).write(pickle_data).csv() # Logger @timeit def
+some_function(...): ... # String Class new_text = String(text).lower
+().remove_digits().remove_punctuation().strip() ``` ## Contributing
+Contributions are welcome! Please read [CONTRIBUTING](CONTRIBUTING) for details
+on how to contribute to this project. # License This project is licensed under
+the terms of the [MIT license](LICENSE).
```

