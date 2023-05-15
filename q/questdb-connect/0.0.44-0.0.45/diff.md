# Comparing `tmp/questdb-connect-0.0.44.tar.gz` & `tmp/questdb-connect-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.44.tar", last modified: Sun May 14 12:46:48 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.45.tar", last modified: Sun May 14 20:15:58 2023, max compression
```

## Comparing `questdb-connect-0.0.44.tar` & `questdb-connect-0.0.45.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.919501 questdb-connect-0.0.44/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.44/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-14 12:46:48.919367 questdb-connect-0.0.44/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.44/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-14 12:44:33.000000 questdb-connect-0.0.44/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-14 12:46:48.921581 questdb-connect-0.0.44/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.913295 questdb-connect-0.0.44/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.915407 questdb-connect-0.0.44/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.44/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.44/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.44/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2839 2023-05-14 10:10:59.000000 questdb-connect-0.0.44/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.44/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.44/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.916976 questdb-connect-0.0.44/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-14 09:35:51.000000 questdb-connect-0.0.44/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.44/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.44/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    11549 2023-05-14 12:43:14.000000 questdb-connect-0.0.44/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.44/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.918223 questdb-connect-0.0.44/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.918969 questdb-connect-0.0.44/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.44/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4352 2023-05-13 17:16:29.000000 questdb-connect-0.0.44/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.44/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.980834 questdb-connect-0.0.45/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.45/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-14 20:15:58.980706 questdb-connect-0.0.45/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.45/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-14 20:15:05.000000 questdb-connect-0.0.45/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-14 20:15:58.980867 questdb-connect-0.0.45/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.975687 questdb-connect-0.0.45/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.977707 questdb-connect-0.0.45/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.45/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.45/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.45/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2839 2023-05-14 20:08:45.000000 questdb-connect-0.0.45/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.45/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.45/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.978859 questdb-connect-0.0.45/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-14 09:35:51.000000 questdb-connect-0.0.45/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11454 2023-05-14 20:09:54.000000 questdb-connect-0.0.45/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.45/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11867 2023-05-14 20:14:41.000000 questdb-connect-0.0.45/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.45/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.979765 questdb-connect-0.0.45/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.980435 questdb-connect-0.0.45/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9533 2023-05-14 20:06:52.000000 questdb-connect-0.0.45/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5073 2023-05-14 19:48:50.000000 questdb-connect-0.0.45/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.45/tests/test_types.py
```

### Comparing `questdb-connect-0.0.44/LICENSE` & `questdb-connect-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/PKG-INFO` & `questdb-connect-0.0.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.44
+Version: 0.0.45
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.44/README.md` & `questdb-connect-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/pyproject.toml` & `questdb-connect-0.0.45/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.44'
+version = '0.0.45'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.44/src/examples/__init__.py` & `questdb-connect-0.0.45/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/src/examples/hello_world.py` & `questdb-connect-0.0.45/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.45/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/src/examples/server_utilisation.py` & `questdb-connect-0.0.45/src/examples/server_utilisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     source = Column(qdbc.Symbol)  # Nodes
     attr_name = Column(qdbc.Symbol)  # Metrics
     attr_value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
 def main():
-    end_time = time.time() + 60.0
+    end_time = time.time() + 10.0
     engine = create_engine('questdb://localhost:8812/main')
     session = Session(engine)
     max_batch_size = 3000
     try:
         Base.metadata.drop_all(engine)
         Base.metadata.create_all(engine)
         batch_size = 0
```

### Comparing `questdb-connect-0.0.44/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.45/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.45/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/src/questdb_connect/__init__.py` & `questdb-connect-0.0.45/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/src/questdb_connect/dialect.py` & `questdb-connect-0.0.45/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
 
 import sqlalchemy
 from sqlalchemy import Column, MetaData, text
-from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
+from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema
@@ -43,16 +43,15 @@
 
 
 def create_engine(host: str, port: int, username: str, password: str, database: str = 'main'):
     return sqlalchemy.create_engine(
         connection_uri(host, port, username, password, database),
         future=False,
         hide_parameters=True,
-        implicit_returning=False,
-        isolation_level="REPEATABLE READ")
+        implicit_returning=False)
 
 
 # ===== QUESTDB ENGINE =====
 
 class QDBTableEngine(SchemaEventTarget, Traversible):
     def __init__(
             self,
@@ -235,18 +234,20 @@
         } for row in result_set]
 
     def get_schema_names(self):
         return ['public']
 
 
 # class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
-class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
+class QuestDBDialect(DefaultDialect, abc.ABC):
     name = 'questdb'
+    driver = "psycopg2"
     psycopg2_version = (2, 9)
     default_schema_name = 'public'
+    default_paramstyle = 'pyformat'
     statement_compiler = QDBSQLCompiler
     ddl_compiler = QDBDDLCompiler
     type_compiler = GenericTypeCompiler
     inspector = QDBInspector
     preparer = QDBIdentifierPreparer
     supports_schemas = False
     supports_statement_cache = False
```

### Comparing `questdb-connect-0.0.44/src/questdb_connect/function_names.py` & `questdb-connect-0.0.45/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.45/src/questdb_connect/superset_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
+import sqlparse
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType, TimeGrain
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
@@ -209,14 +210,20 @@
     @classmethod
     def get_column_spec(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
             source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
     ) -> Optional[utils.ColumnSpec]:
+        """Get generic type related specs regarding a native column type.
+        :param native_type: Native database type
+        :param db_extra: The database extra object
+        :param source: Type coming from the database table or cursor description
+        :return: ColumnSpec object
+        """
         if not native_type:
             return None
         sqla_type = types.resolve_type_from_name(native_type)
         name_u = sqla_type.__visit_name__
         generic_type = None
         if name_u == 'BOOLEAN':
             generic_type = GenericDataType.BOOLEAN
```

### Comparing `questdb-connect-0.0.44/src/questdb_connect/types.py` & `questdb-connect-0.0.45/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.45/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.44
+Version: 0.0.45
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.44/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.45/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.44/tests/test_dialect.py` & `questdb-connect-0.0.45/tests/test_dialect.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,24 @@
 
 def test_insert(test_engine, test_model):
     with test_engine.connect() as conn:
         assert test_engine.dialect.has_table(conn, TEST_TABLE_NAME)
         assert not test_engine.dialect.has_table(conn, 'scorchio')
         now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
         now_date = now.date()
-        expected = ("(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-                    "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                    "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-                    "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-                    "(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-                    "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                    "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-                    "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
+        expected = (
+            "(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+            "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
+            "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+            "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+            "(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+            "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
+            "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+            "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')"
+        )
         stmt1 = sqla.insert(test_model).values(
             col_boolean=True,
             col_byte=8,
             col_short=12,
             col_int=13,
             col_long=14,
             col_float=15.234,
@@ -132,26 +134,28 @@
 
 
 def test_multiple_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
-    expected = ("(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-                "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-                "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
+    expected = (
+        "(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
+        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+        "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
+        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+        "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
+        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')"
+    )
     try:
         for idx in range(num_rows):
             session.add(test_model(
                 col_boolean=True,
                 col_byte=8,
                 col_short=12,
                 col_int=idx,
@@ -176,26 +180,28 @@
 
 
 def test_bulk_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
-    expected = ("(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-                "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-                "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
+    expected = (
+        "(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
+        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+        "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
+        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+        "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
+        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')"
+    )
     models = [
         test_model(
             col_boolean=True,
             col_byte=8,
             col_short=12,
             col_int=idx,
             col_long=14,
```

### Comparing `questdb-connect-0.0.44/tests/test_superset.py` & `questdb-connect-0.0.45/tests/test_superset.py`

 * *Files 17% similar despite different names*

```diff
@@ -111,7 +111,25 @@
     assert str(expr.compile(None, dialect=QuestDBDialect())) == "date_trunc('year', col_ts * 1000000)"
 
 
 def test_time_exp_highr_col_micro_1y():
     col = sqla.Column('col_ts', types.Timestamp, primary_key=True)
     expr = QDBEngineSpec.get_timestamp_expr(col, "epoch_ms", "P1Y")
     assert str(expr.compile(None, dialect=QuestDBDialect())) == "date_trunc('year', (col_ts/1000) * 1000000)"
+
+
+def test_sqlparse():
+    # TODO
+    select_stmt = 'SELECT ts AS __timestamp,'
+    select_stmt += ' attr_name AS attr_name,'
+    select_stmt += ' source AS source,'
+    select_stmt += ' max(attr_value) AS "MAX(attr_value)",'
+    select_stmt += ' AVG(attr_value) AS "AVG(attr_value)",'
+    select_stmt += ' count(attr_value) AS "COUNT(attr_value)"'
+    select_stmt += ' FROM node_metrics'
+    select_stmt += " WHERE ts >= '2023-05-07 00:00:00.000000'"
+    select_stmt += " AND ts < '2023-05-14 00:00:00.000000'"
+    select_stmt += ' GROUP BY attr_name, source, ts'
+    select_stmt += ' ORDER BY "MAX(attr_value)" DESC'
+    select_stmt += ' LIMIT 10000;'
+    parsed = QDBEngineSpec.parse_sql(select_stmt)
+    print(parsed)
```

### Comparing `questdb-connect-0.0.44/tests/test_types.py` & `questdb-connect-0.0.45/tests/test_types.py`

 * *Files identical despite different names*

