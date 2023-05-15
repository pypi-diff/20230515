# Comparing `tmp/flask_management-0.1.0.tar.gz` & `tmp/flask_management-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_management-0.1.0.tar", max compression
+gzip compressed data, was "flask_management-0.1.1.tar", max compression
```

## Comparing `flask_management-0.1.0.tar` & `flask_management-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0       64 2023-05-12 10:12:39.009298 flask_management-0.1.0/README.md
--rw-r--r--   0        0        0       45 2023-05-12 09:45:33.620393 flask_management-0.1.0/flask_management/__main__.py
--rw-r--r--   0        0        0      651 2023-05-12 09:32:10.220001 flask_management-0.1.0/flask_management/constants.py
--rw-r--r--   0        0        0     1102 2023-05-12 10:07:24.682564 flask_management-0.1.0/flask_management/context.py
--rw-r--r--   0        0        0      862 2023-05-12 10:05:24.848862 flask_management-0.1.0/flask_management/generator.py
--rw-r--r--   0        0        0      557 2023-05-12 09:52:24.228376 flask_management-0.1.0/flask_management/main.py
--rw-r--r--   0        0        0        0 2023-05-12 09:10:06.479030 flask_management-0.1.0/flask_management/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 09:16:41.739753 flask_management-0.1.0/flask_management/templates/project/__init__.py
--rw-r--r--   0        0        0      344 2023-05-12 10:07:37.687255 flask_management-0.1.0/flask_management/templates/project/cookiecutter.json
--rw-r--r--   0        0        0     2058 2023-05-12 09:16:41.753980 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore
--rw-r--r--   0        0        0       25 2023-05-12 10:05:01.827494 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/README.md
--rw-r--r--   0        0        0      686 2023-05-12 10:04:03.419284 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml
--rw-r--r--   0        0        0      283 2023-05-12 09:16:41.755325 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-12 09:16:41.752694 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/tests/__init__.py
--rw-r--r--   0        0        0      372 2023-05-12 10:09:45.123747 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/__init__.py
--rw-r--r--   0        0        0      206 2023-05-12 09:38:38.791581 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/app_settings.py
--rw-r--r--   0        0        0      278 2023-05-12 10:09:59.168402 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/ext.py
--rw-r--r--   0        0        0      414 2023-05-12 10:10:04.165575 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/models.py
--rw-r--r--   0        0        0      216 2023-05-12 10:10:31.935563 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/signals.py
--rw-r--r--   0        0        0       78 2023-05-12 10:11:12.704214 flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.env }}
--rw-r--r--   0        0        0      581 2023-05-12 09:48:48.704082 flask_management-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 flask_management-0.1.0/setup.py
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 flask_management-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-05-12 10:12:39.009298 flask_management-0.1.1/README.md
+-rw-r--r--   0        0        0       45 2023-05-12 09:45:33.620393 flask_management-0.1.1/flask_management/__main__.py
+-rw-r--r--   0        0        0      659 2023-05-15 06:38:22.606321 flask_management-0.1.1/flask_management/constants.py
+-rw-r--r--   0        0        0     1102 2023-05-12 10:07:24.682564 flask_management-0.1.1/flask_management/context.py
+-rw-r--r--   0        0        0      862 2023-05-12 10:05:24.848862 flask_management-0.1.1/flask_management/generator.py
+-rw-r--r--   0        0        0      559 2023-05-15 06:38:25.266373 flask_management-0.1.1/flask_management/main.py
+-rw-r--r--   0        0        0        0 2023-05-12 09:10:06.479030 flask_management-0.1.1/flask_management/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 09:16:41.739753 flask_management-0.1.1/flask_management/templates/project/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-12 10:07:37.687255 flask_management-0.1.1/flask_management/templates/project/cookiecutter.json
+-rw-r--r--   0        0        0     2058 2023-05-12 09:16:41.753980 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore
+-rw-r--r--   0        0        0       25 2023-05-12 10:05:01.827494 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/README.md
+-rw-r--r--   0        0        0      686 2023-05-12 10:04:03.419284 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-05-12 09:16:41.755325 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-12 09:16:41.752694 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/tests/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-15 06:53:31.890127 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-12 09:38:38.791581 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/app_settings.py
+-rw-r--r--   0        0        0      162 2023-05-15 06:53:07.121983 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-15 06:52:11.622692 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/api.py
+-rw-r--r--   0        0        0      278 2023-05-12 10:09:59.168402 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/ext.py
+-rw-r--r--   0        0        0      414 2023-05-12 10:10:04.165575 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/models.py
+-rw-r--r--   0        0        0      216 2023-05-12 10:10:31.935563 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/signals.py
+-rw-r--r--   0        0        0       78 2023-05-12 10:11:12.704214 flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.env }}
+-rw-r--r--   0        0        0      581 2023-05-15 06:53:59.904948 flask_management-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 flask_management-0.1.1/setup.py
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 flask_management-0.1.1/PKG-INFO
```

### Comparing `flask_management-0.1.0/flask_management/constants.py` & `flask_management-0.1.1/flask_management/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 
 class BaseEnum(str, Enum, metaclass=BaseMetadataEnum):
     """Base enum class."""
 
 
 class PythonVersion(BaseEnum):
-    THREE_DOT_SEV = "3.7"
-    THREE_DOT_EIG = "3.8"
-    THREE_DOT_NIN = "3.9"
+    THREE_DOT_SEVEN = "3.7"
+    THREE_DOT_EIGHT = "3.8"
+    THREE_DOT_NINE = "3.9"
     THREE_DOT_TEN = "3.10"
-    THREE_DOT_ELE = "3.11"
+    THREE_DOT_ELEVEN = "3.11"
 
 
 class Database(BaseEnum):
     POSTGRES = "Postgres"
     MYSQL = "MySQL"
```

### Comparing `flask_management-0.1.0/flask_management/context.py` & `flask_management-0.1.1/flask_management/context.py`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.0/flask_management/generator.py` & `flask_management-0.1.1/flask_management/generator.py`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.0/flask_management/main.py` & `flask_management-0.1.1/flask_management/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,14 @@
     name="Manage Flask",
 )
 
 
 @app.command(help="Creates a flask project.")
 def startproject(
     name: str,
-    python: PythonVersion = typer.Option(PythonVersion.THREE_DOT_EIG),
+    python: PythonVersion = typer.Option(PythonVersion.THREE_DOT_EIGHT),
 ):
     context = ProjectContext(
         name=name,
         python=python
     )
     generate_project(context)
```

### Comparing `flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore` & `flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.0/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml` & `flask_management-0.1.1/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.0/pyproject.toml` & `flask_management-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-management"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["huangsong <huangsong@leyantech.com>"]
 readme = "README.md"
 packages = [{ include = "flask_management" }]
 
 [[tool.poetry.source]]
 name = "tuna"
```

### Comparing `flask_management-0.1.0/setup.py` & `flask_management-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 packages = \
 ['flask_management',
  'flask_management.templates',
  'flask_management.templates.project',
  'flask_management.templates.project.{{ cookiecutter.folder_name }}.tests',
  'flask_management.templates.project.{{ cookiecutter.folder_name }}.{{ '
- 'cookiecutter.app_name }}']
+ 'cookiecutter.app_name }}',
+ 'flask_management.templates.project.{{ cookiecutter.folder_name }}.{{ '
+ 'cookiecutter.app_name }}.book']
 
 package_data = \
 {'': ['*'],
  'flask_management.templates.project': ['{{ cookiecutter.folder_name }}/*']}
 
 install_requires = \
 ['cookiecutter>=1.7.2', 'pydantic[email]>=1.7.2', 'typer']
 
 entry_points = \
 {'console_scripts': ['flaskapi = flask_management.main:app']}
 
 setup_kwargs = {
     'name': 'flask-management',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# flask-management\n\n## How to use :\n\nflaskapi your-project-name\n',
     'author': 'huangsong',
     'author_email': 'huangsong@leyantech.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

