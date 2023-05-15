# Comparing `tmp/alembic-autogenerate-enums-0.1.0.tar.gz` & `tmp/alembic-autogenerate-enums-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic-autogenerate-enums-0.1.0.tar", max compression
+gzip compressed data, was "alembic-autogenerate-enums-0.1.1.tar", max compression
```

## Comparing `alembic-autogenerate-enums-0.1.0.tar` & `alembic-autogenerate-enums-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-05-09 18:09:04.288080 alembic-autogenerate-enums-0.1.0/LICENSE
--rw-r--r--   0        0        0      930 2023-05-09 18:09:04.288152 alembic-autogenerate-enums-0.1.0/README.md
--rw-r--r--   0        0        0     8739 2023-05-09 18:40:41.987110 alembic-autogenerate-enums-0.1.0/alembic_autogenerate_enums/__init__.py
--rw-r--r--   0        0        0      485 2023-05-09 18:37:01.106059 alembic-autogenerate-enums-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 alembic-autogenerate-enums-0.1.0/setup.py
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 alembic-autogenerate-enums-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-09 18:09:04.288080 alembic-autogenerate-enums-0.1.1/LICENSE
+-rw-r--r--   0        0        0      930 2023-05-09 18:09:04.288152 alembic-autogenerate-enums-0.1.1/README.md
+-rw-r--r--   0        0        0     8739 2023-05-09 18:40:41.987110 alembic-autogenerate-enums-0.1.1/alembic_autogenerate_enums/__init__.py
+-rw-r--r--   0        0        0      485 2023-05-15 01:28:30.802864 alembic-autogenerate-enums-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 alembic-autogenerate-enums-0.1.1/setup.py
+-rw-r--r--   0        0        0     1540 1970-01-01 00:00:00.000000 alembic-autogenerate-enums-0.1.1/PKG-INFO
```

### Comparing `alembic-autogenerate-enums-0.1.0/LICENSE` & `alembic-autogenerate-enums-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic-autogenerate-enums-0.1.0/README.md` & `alembic-autogenerate-enums-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alembic-autogenerate-enums-0.1.0/alembic_autogenerate_enums/__init__.py` & `alembic-autogenerate-enums-0.1.1/alembic_autogenerate_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `alembic-autogenerate-enums-0.1.0/setup.py` & `alembic-autogenerate-enums-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 ['alembic_autogenerate_enums']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'alembic-autogenerate-enums',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Alembic hook that allows enums values to be upgraded and downgraded in migrations automatically',
     'long_description': '\n# alembic-autogenerate-enums\n\nThis package implements an Alembic hook that causes ``alembic revision\n--autogenerate`` to output PostgreSQL ``ALTER TYPE .. ADD VALUE`` SQL\nstatements as part of new migrations.\n\n\n## Usage\n\nAdd the line:\n\n    import alembic_autogenerate_enums\n\nTo the top of your ``env.py``.\n\n\n## Notes\n\nSince ``ALTER TYPE .. ADD VALUE`` cannot run transactionally, each\n``op.sync_enum_values()`` call creates its own temporary private DB connection.\nSee https://bitbucket.org/zzzeek/alembic/issues/123/a-way-to-run-non-transactional-ddl\n\n## Tests\n\nWe have incredibly basic tests in a [sample project](./test-harness).\n\n```\nmkvirtualenv alembic-autogenerate\n```\n\nInstall the main autogenerate package and then the test harness:\n\n```\npip install -e .\npip install -e test-harness\n```\n\n```\ncreateuser alembic-autogenerate\ncreatedb -O alembic-autogenerate alembic-autogenerate_db\n```\n\n```\ncd test-harness && pytest\n```\n',
-    'author': 'Pierce Freeman',
-    'author_email': 'pierce@freeman.vc',
+    'author': 'David Wilson',
+    'author_email': 'dw@botanicus.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `alembic-autogenerate-enums-0.1.0/PKG-INFO` & `alembic-autogenerate-enums-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: alembic-autogenerate-enums
-Version: 0.1.0
+Version: 0.1.1
 Summary: Alembic hook that allows enums values to be upgraded and downgraded in migrations automatically
 License: MIT
-Author: Pierce Freeman
-Author-email: pierce@freeman.vc
+Author: David Wilson
+Author-email: dw@botanicus.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

