# Comparing `tmp/django-rich-logging-0.2.0.tar.gz` & `tmp/django_rich_logging-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rich-logging-0.2.0.tar", max compression
+gzip compressed data, was "django_rich_logging-0.3.0.tar", max compression
```

## Comparing `django-rich-logging-0.2.0.tar` & `django_rich_logging-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2022-02-12 15:07:41.033733 django-rich-logging-0.2.0/LICENSE
--rw-r--r--   0        0        0     1493 2022-02-13 12:32:14.845790 django-rich-logging-0.2.0/README.md
--rw-r--r--   0        0        0        0 2022-02-12 15:13:16.091918 django-rich-logging-0.2.0/django_rich_logging/__init__.py
--rw-r--r--   0        0        0     3581 2022-08-15 12:25:02.165991 django-rich-logging-0.2.0/django_rich_logging/logging.py
--rw-r--r--   0        0        0     2257 2022-08-15 12:25:02.166220 django-rich-logging-0.2.0/django_rich_logging/objects.py
--rw-r--r--   0        0        0     3058 2022-08-15 12:25:21.566911 django-rich-logging-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2623 2022-08-15 12:26:07.462842 django-rich-logging-0.2.0/setup.py
--rw-r--r--   0        0        0     2930 2022-08-15 12:26:07.463020 django-rich-logging-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-02-12 15:07:41.033733 django_rich_logging-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1493 2022-02-13 12:32:14.845790 django_rich_logging-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-02-12 15:13:16.091918 django_rich_logging-0.3.0/django_rich_logging/__init__.py
+-rw-r--r--   0        0        0     3544 2022-08-16 01:52:52.638470 django_rich_logging-0.3.0/django_rich_logging/logging.py
+-rw-r--r--   0        0        0     2257 2022-08-15 12:25:02.166220 django_rich_logging-0.3.0/django_rich_logging/objects.py
+-rw-r--r--   0        0        0     3058 2023-05-15 13:53:59.924191 django_rich_logging-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 django_rich_logging-0.3.0/setup.py
+-rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 django_rich_logging-0.3.0/PKG-INFO
```

### Comparing `django-rich-logging-0.2.0/LICENSE` & `django_rich_logging-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rich-logging-0.2.0/README.md` & `django_rich_logging-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-rich-logging-0.2.0/django_rich_logging/logging.py` & `django_rich_logging-0.3.0/django_rich_logging/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,24 +82,24 @@
         Get markup based on the column's `format` and the `RequestRecord` object.
         """
 
         format = column.get("format", "")
         style = column.get("style", "%")
         date_format = column.get("datefmt")
 
+        request_record_data = request_record.get_dict(date_format=date_format)
+
         if style == "%":
-            return format % request_record.get_dict(date_format=date_format)
+            return format % request_record_data
         elif style == "{":
-            return format.format(**request_record.get_dict(date_format=date_format))
+            return format.format(**request_record_data)
         elif style == "$":
             template = Template(format)
 
-            return template.substitute(
-                **request_record.get_dict(date_format=date_format)
-            )
+            return template.substitute(**request_record_data)
         else:
             raise Exception(f"Unknown style: {style}")
 
     def emit(self, record: logging.LogRecord) -> None:
         """
         Writes the logging record. If it's a request, add the record to a live,
         updating table. If not, emit it like normal.
```

### Comparing `django-rich-logging-0.2.0/django_rich_logging/objects.py` & `django_rich_logging-0.3.0/django_rich_logging/objects.py`

 * *Files identical despite different names*

### Comparing `django-rich-logging-0.2.0/pyproject.toml` & `django_rich_logging-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-rich-logging"
-version = "0.2.0"
+version = "0.3.0"
 description = "A prettier way to see Django requests while developing."
 authors = ["adamghill <adam@adamghill.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "python", "static", "markdown"]
 repository = "https://github.com/adamghill/django-rich-logging/"
 homepage = "https://github.com/adamghill/django-rich-logging/"
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 "Funding" = "https://github.com/sponsors/adamghill"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 Django = ">3.0"
-rich = "^11.2.0"
+rich = ">11.2.0"
 
 # docs extras
 Sphinx = { version = "^4.3.2", optional = true }
 linkify-it-py = { version = "^1.0.3", optional = true }
 myst-parser = { version = "^0.16.1", optional = true }
 furo = { version = "^2021.11.23", optional = true }
 sphinx-copybutton = { version = "^0.4.0", optional = true }
```

### Comparing `django-rich-logging-0.2.0/setup.py` & `django_rich_logging-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 packages = \
 ['django_rich_logging']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Django>3.0', 'rich>=11.2.0,<12.0.0']
+['Django>3.0', 'rich>11.2.0']
 
 extras_require = \
 {'docs': ['Sphinx>=4.3.2,<5.0.0',
           'linkify-it-py>=1.0.3,<2.0.0',
           'myst-parser>=0.16.1,<0.17.0',
           'furo>=2021.11.23,<2022.0.0',
           'sphinx-copybutton>=0.4.0,<0.5.0',
           'sphinx-autobuild>=2021.3.14,<2022.0.0',
           'toml',
           'attrs>=21.4.0,<22.0.0']}
 
 setup_kwargs = {
     'name': 'django-rich-logging',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A prettier way to see Django requests while developing.',
     'long_description': '<p align="center">\n  <a href="https://django-rich-logging.readthedocs.io"><h1 align="center">django-rich-logging</h1></a>\n</p>\n<p align="center">A prettier way to see Django requests while developing.</p>\n\n![PyPI](https://img.shields.io/pypi/v/django-rich-logging?color=blue&style=flat-square)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/django-rich-logging?color=blue&style=flat-square)\n![GitHub Sponsors](https://img.shields.io/github/sponsors/adamghill?color=blue&style=flat-square)\n\n📖 Complete documentation: https://django-rich-logging.readthedocs.io\n\n📦 Package located at https://pypi.org/project/django-rich-logging/\n\n## ⭐ Features\n\n- live-updating table of all requests while developing\n\n![demo of django-rich-logging](https://raw.githubusercontent.com/adamghill/django-rich-logging/main/django-rich-logging.gif)\n\n## Installation\n\n`poetry add django-rich-logging` OR `pip install django-rich-logging`\n\n### Configuration\n\n```python\n# settings.py\n\n# other settings here\n\nLOGGING = {\n    "version": 1,\n    "disable_existing_loggers": False,\n    "handlers": {\n        "django_rich_logging": {\n            "class": "django_rich_logging.logging.DjangoRequestHandler",\n            "level": "INFO",\n        },\n    },\n    "loggers": {\n        "django.server": {"handlers": ["django_rich_logging"], "level": "INFO"},\n        "django.request": {"level": "CRITICAL"},\n    },\n}\n\n# other settings here\n```\n\nRead all of the documentation at https://django-rich-logging.readthedocs.io.\n',
     'author': 'adamghill',
     'author_email': 'adam@adamghill.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/adamghill/django-rich-logging/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.7,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['django_rich_logging'] package_data = \ {'': ['*']} install_requires = \
-['Django>3.0', 'rich>=11.2.0,<12.0.0'] extras_require = \ {'docs':
+['Django>3.0', 'rich>11.2.0'] extras_require = \ {'docs':
 ['Sphinx>=4.3.2,<5.0.0', 'linkify-it-py>=1.0.3,<2.0.0', 'myst-
 parser>=0.16.1,<0.17.0', 'furo>=2021.11.23,<2022.0.0', 'sphinx-
 copybutton>=0.4.0,<0.5.0', 'sphinx-autobuild>=2021.3.14,<2022.0.0', 'toml',
 'attrs>=21.4.0,<22.0.0']} setup_kwargs = { 'name': 'django-rich-logging',
-'version': '0.2.0', 'description': 'A prettier way to see Django requests while
+'version': '0.3.0', 'description': 'A prettier way to see Django requests while
 developing.', 'long_description': '
                                       \n
                        ******_django-rich-logging_******
                                       \n
 \n
             A prettier way to see Django requests while developing.
 \n\n![PyPI](https://img.shields.io/pypi/v/django-rich-
@@ -26,12 +26,12 @@
 settings.py\n\n# other settings here\n\nLOGGING = {\n "version": 1,\n
 "disable_existing_loggers": False,\n "handlers": {\n "django_rich_logging": {\n
 "class": "django_rich_logging.logging.DjangoRequestHandler",\n "level":
 "INFO",\n },\n },\n "loggers": {\n "django.server": {"handlers":
 ["django_rich_logging"], "level": "INFO"},\n "django.request": {"level":
 "CRITICAL"},\n },\n}\n\n# other settings here\n```\n\nRead all of the
 documentation at https://django-rich-logging.readthedocs.io.\n', 'author':
-'adamghill', 'author_email': 'adam@adamghill.com', 'maintainer': None,
-'maintainer_email': None, 'url': 'https://github.com/adamghill/django-rich-
+'adamghill', 'author_email': 'adam@adamghill.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'https://github.com/adamghill/django-rich-
 logging/', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'extras_require': extras_require,
 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `django-rich-logging-0.2.0/PKG-INFO` & `django_rich_logging-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: django-rich-logging
-Version: 0.2.0
+Version: 0.3.0
 Summary: A prettier way to see Django requests while developing.
 Home-page: https://github.com/adamghill/django-rich-logging/
 License: MIT
 Keywords: django,python,static,markdown
 Author: adamghill
 Author-email: adam@adamghill.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: Django (>3.0)
-Requires-Dist: Sphinx (>=4.3.2,<5.0.0); extra == "docs"
-Requires-Dist: attrs (>=21.4.0,<22.0.0); extra == "docs"
-Requires-Dist: furo (>=2021.11.23,<2022.0.0); extra == "docs"
-Requires-Dist: linkify-it-py (>=1.0.3,<2.0.0); extra == "docs"
-Requires-Dist: myst-parser (>=0.16.1,<0.17.0); extra == "docs"
-Requires-Dist: rich (>=11.2.0,<12.0.0)
-Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0); extra == "docs"
-Requires-Dist: sphinx-copybutton (>=0.4.0,<0.5.0); extra == "docs"
-Requires-Dist: toml; extra == "docs"
+Requires-Dist: Sphinx (>=4.3.2,<5.0.0) ; extra == "docs"
+Requires-Dist: attrs (>=21.4.0,<22.0.0) ; extra == "docs"
+Requires-Dist: furo (>=2021.11.23,<2022.0.0) ; extra == "docs"
+Requires-Dist: linkify-it-py (>=1.0.3,<2.0.0) ; extra == "docs"
+Requires-Dist: myst-parser (>=0.16.1,<0.17.0) ; extra == "docs"
+Requires-Dist: rich (>11.2.0)
+Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
+Requires-Dist: sphinx-copybutton (>=0.4.0,<0.5.0) ; extra == "docs"
+Requires-Dist: toml ; extra == "docs"
 Project-URL: Documentation, https://django-rich-logging.readthedocs.io/
 Project-URL: Funding, https://github.com/sponsors/adamghill
 Project-URL: Repository, https://github.com/adamghill/django-rich-logging/
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://django-rich-logging.readthedocs.io"><h1 align="center">django-rich-logging</h1></a>
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: django-rich-logging Version: 0.2.0 Summary: A
+Metadata-Version: 2.1 Name: django-rich-logging Version: 0.3.0 Summary: A
 prettier way to see Django requests while developing. Home-page: https://
 github.com/adamghill/django-rich-logging/ License: MIT Keywords:
 django,python,static,markdown Author: adamghill Author-email:
 adam@adamghill.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Provides-Extra: docs
-Requires-Dist: Django (>3.0) Requires-Dist: Sphinx (>=4.3.2,<5.0.0); extra ==
-"docs" Requires-Dist: attrs (>=21.4.0,<22.0.0); extra == "docs" Requires-Dist:
-furo (>=2021.11.23,<2022.0.0); extra == "docs" Requires-Dist: linkify-it-py
-(>=1.0.3,<2.0.0); extra == "docs" Requires-Dist: myst-parser
-(>=0.16.1,<0.17.0); extra == "docs" Requires-Dist: rich (>=11.2.0,<12.0.0)
-Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0); extra == "docs"
-Requires-Dist: sphinx-copybutton (>=0.4.0,<0.5.0); extra == "docs" Requires-
-Dist: toml; extra == "docs" Project-URL: Documentation, https://django-rich-
+Language :: Python :: 3.11 Provides-Extra: docs Requires-Dist: Django (>3.0)
+Requires-Dist: Sphinx (>=4.3.2,<5.0.0) ; extra == "docs" Requires-Dist: attrs
+(>=21.4.0,<22.0.0) ; extra == "docs" Requires-Dist: furo
+(>=2021.11.23,<2022.0.0) ; extra == "docs" Requires-Dist: linkify-it-py
+(>=1.0.3,<2.0.0) ; extra == "docs" Requires-Dist: myst-parser
+(>=0.16.1,<0.17.0) ; extra == "docs" Requires-Dist: rich (>11.2.0) Requires-
+Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs" Requires-Dist:
+sphinx-copybutton (>=0.4.0,<0.5.0) ; extra == "docs" Requires-Dist: toml ;
+extra == "docs" Project-URL: Documentation, https://django-rich-
 logging.readthedocs.io/ Project-URL: Funding, https://github.com/sponsors/
 adamghill Project-URL: Repository, https://github.com/adamghill/django-rich-
 logging/ Description-Content-Type: text/markdown
                        ******_django-rich-logging_******
             A prettier way to see Django requests while developing.
 ![PyPI](https://img.shields.io/pypi/v/django-rich-
 logging?color=blue&style=flat-square) ![PyPI - Downloads](https://
```

