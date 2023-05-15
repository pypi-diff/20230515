# Comparing `tmp/questdb-connect-0.0.45.tar.gz` & `tmp/questdb-connect-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.45.tar", last modified: Sun May 14 20:15:58 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.46.tar", last modified: Mon May 15 18:38:15 2023, max compression
```

## Comparing `questdb-connect-0.0.45.tar` & `questdb-connect-0.0.46.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.980834 questdb-connect-0.0.45/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.45/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-14 20:15:58.980706 questdb-connect-0.0.45/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.45/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-14 20:15:05.000000 questdb-connect-0.0.45/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-14 20:15:58.980867 questdb-connect-0.0.45/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.975687 questdb-connect-0.0.45/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.977707 questdb-connect-0.0.45/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.45/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.45/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.45/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2839 2023-05-14 20:08:45.000000 questdb-connect-0.0.45/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.45/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.45/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.978859 questdb-connect-0.0.45/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-14 09:35:51.000000 questdb-connect-0.0.45/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11454 2023-05-14 20:09:54.000000 questdb-connect-0.0.45/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.45/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    11867 2023-05-14 20:14:41.000000 questdb-connect-0.0.45/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.45/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.979765 questdb-connect-0.0.45/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-14 20:15:58.000000 questdb-connect-0.0.45/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 20:15:58.980435 questdb-connect-0.0.45/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9533 2023-05-14 20:06:52.000000 questdb-connect-0.0.45/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5073 2023-05-14 19:48:50.000000 questdb-connect-0.0.45/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.45/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.663355 questdb-connect-0.0.46/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.46/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-15 18:38:15.663216 questdb-connect-0.0.46/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.46/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-15 18:37:08.000000 questdb-connect-0.0.46/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-15 18:38:15.663389 questdb-connect-0.0.46/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.656682 questdb-connect-0.0.46/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.659161 questdb-connect-0.0.46/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.46/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.46/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.46/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.46/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.46/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.46/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.660814 questdb-connect-0.0.46/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-14 09:35:51.000000 questdb-connect-0.0.46/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-15 10:26:37.000000 questdb-connect-0.0.46/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.46/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13956 2023-05-15 18:37:08.000000 questdb-connect-0.0.46/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.46/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.661951 questdb-connect-0.0.46/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.662824 questdb-connect-0.0.46/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9751 2023-05-15 13:49:03.000000 questdb-connect-0.0.46/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     6270 2023-05-15 18:36:10.000000 questdb-connect-0.0.46/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.46/tests/test_types.py
```

### Comparing `questdb-connect-0.0.45/LICENSE` & `questdb-connect-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/PKG-INFO` & `questdb-connect-0.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.45
+Version: 0.0.46
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.45/README.md` & `questdb-connect-0.0.46/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/pyproject.toml` & `questdb-connect-0.0.46/pyproject.toml`

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
-version = '0.0.45'
+version = '0.0.46'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.45/src/examples/__init__.py` & `questdb-connect-0.0.46/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/src/examples/hello_world.py` & `questdb-connect-0.0.46/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.46/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/src/examples/server_utilisation.py` & `questdb-connect-0.0.46/src/examples/server_utilisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import os
 import random
 import time
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
 
 import questdb_connect.dialect as qdbc
-from sqlalchemy import Column, MetaData, create_engine, insert
+from sqlalchemy import Column, MetaData, create_engine
 from sqlalchemy.orm import Session, declarative_base
 
 
 class BaseEnum(enum.Enum):
     @classmethod
     def rand(cls):
         return cls._value2member_map_[random.randint(0, len(cls._member_map_) - 1)]
```

### Comparing `questdb-connect-0.0.45/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.46/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.46/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/src/questdb_connect/__init__.py` & `questdb-connect-0.0.46/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/src/questdb_connect/dialect.py` & `questdb-connect-0.0.46/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,24 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
 
 import sqlalchemy
 from sqlalchemy import Column, MetaData, text
-from sqlalchemy.engine.default import DefaultDialect
+from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
-from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
+from sqlalchemy.sql.compiler import (
+    DDLCompiler,
+    GenericTypeCompiler,
+    IdentifierPreparer,
+    SQLCompiler,
+)
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema
 from .types import *
 
 # ===== SQLAlchemy Dialect ======
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
@@ -43,15 +48,16 @@
 
 
 def create_engine(host: str, port: int, username: str, password: str, database: str = 'main'):
     return sqlalchemy.create_engine(
         connection_uri(host, port, username, password, database),
         future=False,
         hide_parameters=True,
-        implicit_returning=False)
+        implicit_returning=False,
+        isolation_level="REPEATABLE READ")
 
 
 # ===== QUESTDB ENGINE =====
 
 class QDBTableEngine(SchemaEventTarget, Traversible):
     def __init__(
             self,
@@ -233,21 +239,18 @@
             'persisted': True
         } for row in result_set]
 
     def get_schema_names(self):
         return ['public']
 
 
-# class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
-class QuestDBDialect(DefaultDialect, abc.ABC):
+class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
     name = 'questdb'
-    driver = "psycopg2"
     psycopg2_version = (2, 9)
     default_schema_name = 'public'
-    default_paramstyle = 'pyformat'
     statement_compiler = QDBSQLCompiler
     ddl_compiler = QDBDDLCompiler
     type_compiler = GenericTypeCompiler
     inspector = QDBInspector
     preparer = QDBIdentifierPreparer
     supports_schemas = False
     supports_statement_cache = False
```

### Comparing `questdb-connect-0.0.45/src/questdb_connect/function_names.py` & `questdb-connect-0.0.46/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.46/src/questdb_connect/superset_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
 import sqlparse
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
-from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType, TimeGrain
+from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
 
 from . import remove_public_schema, types
 from .function_names import FUNCTION_NAMES
@@ -268,7 +268,46 @@
     def get_function_names(cls, database) -> List[str]:
         """Get a list of function names that are able to be called on the database.
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
         :return: A list of function names usable in the database
         """
         return FUNCTION_NAMES
+
+    @classmethod
+    def parse_sql(cls, sql: str) -> List[str]:
+        parsed_sql_text = []
+        for parsed_sql in sqlparse.parse(sql):
+            if parsed_sql.get_type() == 'SELECT':
+                # remove timestamp column from any group by
+                ts_col_name = None
+                has_group_by = False
+                for tok in parsed_sql.tokens:
+                    if not ts_col_name and isinstance(tok, sqlparse.sql.IdentifierList):
+                        for select_tok in tok.tokens:
+                            if isinstance(select_tok, sqlparse.sql.Identifier):
+                                if '__timestamp' in select_tok.value:
+                                    ts_col_name = select_tok.normalized
+                                    break
+                    elif ts_col_name and tok.value.lower() == 'group by':
+                        has_group_by = True
+                    elif ts_col_name and has_group_by and isinstance(tok, sqlparse.sql.IdentifierList):
+                        remove_idx = None
+                        comma_idxs = []
+                        for idx, group_tok in enumerate(tok.tokens):
+                            if group_tok.normalized == ',':
+                                comma_idxs.append(idx)
+                            elif group_tok.normalized == ts_col_name:
+                                remove_idx = idx
+                        if remove_idx is not None:
+                            tok.tokens.pop(remove_idx)
+                            if remove_idx == 0:
+                                tok.tokens.pop(comma_idxs[0] - 1)
+                            else:
+                                remove_comma_idx = -1
+                                for i, c_i in enumerate(comma_idxs):
+                                    if c_i > remove_idx:
+                                        remove_comma_idx = i - 1
+                                        break
+                                tok.tokens.pop(comma_idxs[remove_comma_idx])
+            parsed_sql_text.append(str(parsed_sql).strip(' ;'))
+        return parsed_sql_text
```

### Comparing `questdb-connect-0.0.45/src/questdb_connect/types.py` & `questdb-connect-0.0.46/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.46/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.45
+Version: 0.0.46
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.45/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.46/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.45/tests/test_dialect.py` & `questdb-connect-0.0.46/tests/test_dialect.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,25 +31,23 @@
 
 def test_insert(test_engine, test_model):
     with test_engine.connect() as conn:
         assert test_engine.dialect.has_table(conn, TEST_TABLE_NAME)
         assert not test_engine.dialect.has_table(conn, 'scorchio')
         now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
         now_date = now.date()
-        expected = (
-            "(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-            "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
-            "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-            "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-            "(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-            "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
-            "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-            "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')"
-        )
-        stmt1 = sqla.insert(test_model).values(
+        expected = ("(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                    "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
+                    "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+                    "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+                    "(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                    "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
+                    "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+                    "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
+        insert_stmt = sqla.insert(test_model).values(
             col_boolean=True,
             col_byte=8,
             col_short=12,
             col_int=13,
             col_long=14,
             col_float=15.234,
             col_double=16.88993244,
@@ -58,16 +56,15 @@
             col_char='C',
             col_uuid='6d5eb038-63d1-4971-8484-30c16e13de5b',
             col_date=now_date,
             col_ts=now,
             col_geohash='dfvgsj2vptwu',
             col_long256='0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a'
         )
-        stmt1.compile()
-        conn.execute(stmt1)
+        conn.execute(insert_stmt)
         conn.execute(sqla.insert(test_model), {
             'col_boolean': True,
             'col_byte': 8,
             'col_short': 12,
             'col_int': 13,
             'col_long': 14,
             'col_float': 15.234,
@@ -134,28 +131,26 @@
 
 
 def test_multiple_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
-    expected = (
-        "(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
-        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-        "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
-        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-        "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
-        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')"
-    )
+    expected = ("(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+                "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+                "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
     try:
         for idx in range(num_rows):
             session.add(test_model(
                 col_boolean=True,
                 col_byte=8,
                 col_short=12,
                 col_int=idx,
@@ -180,28 +175,26 @@
 
 
 def test_bulk_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
-    expected = (
-        "(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
-        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-        "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
-        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-        "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
-        "'6d5eb038-63d1-4971-8484-30c16e13de5b', datetime.datetime(2023, 4, 12, 0, "
-        "0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
-        "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')"
-    )
+    expected = ("(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+                "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
+                "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
+                "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
     models = [
         test_model(
             col_boolean=True,
             col_byte=8,
             col_short=12,
             col_int=idx,
             col_long=14,
```

### Comparing `questdb-connect-0.0.45/tests/test_superset.py` & `questdb-connect-0.0.46/tests/test_superset.py`

 * *Files 20% similar despite different names*

```diff
@@ -113,23 +113,40 @@
 
 def test_time_exp_highr_col_micro_1y():
     col = sqla.Column('col_ts', types.Timestamp, primary_key=True)
     expr = QDBEngineSpec.get_timestamp_expr(col, "epoch_ms", "P1Y")
     assert str(expr.compile(None, dialect=QuestDBDialect())) == "date_trunc('year', (col_ts/1000) * 1000000)"
 
 
-def test_sqlparse():
-    # TODO
+def test_parse_sql_removes_timestamp_from_group_by():
     select_stmt = 'SELECT ts AS __timestamp,'
-    select_stmt += ' attr_name AS attr_name,'
-    select_stmt += ' source AS source,'
-    select_stmt += ' max(attr_value) AS "MAX(attr_value)",'
-    select_stmt += ' AVG(attr_value) AS "AVG(attr_value)",'
-    select_stmt += ' count(attr_value) AS "COUNT(attr_value)"'
-    select_stmt += ' FROM node_metrics'
-    select_stmt += " WHERE ts >= '2023-05-07 00:00:00.000000'"
-    select_stmt += " AND ts < '2023-05-14 00:00:00.000000'"
-    select_stmt += ' GROUP BY attr_name, source, ts'
-    select_stmt += ' ORDER BY "MAX(attr_value)" DESC'
-    select_stmt += ' LIMIT 10000;'
-    parsed = QDBEngineSpec.parse_sql(select_stmt)
-    print(parsed)
+    select_stmt += '    attr_name AS attr_name,'
+    select_stmt += '    max(attr_value) AS "MAX(attr_value)",'
+    select_stmt += '    AVG(attr_value) AS "AVG(attr_value)",'
+    select_stmt += '    sum(attr_value) AS "SUM(attr_value)"'
+    select_stmt += '  FROM node_metrics'
+    select_stmt += '  JOIN'
+    select_stmt += '(SELECT attr_name AS attr_name__,'
+    select_stmt += '    max(attr_value) AS mme_inner__'
+    select_stmt += '  FROM node_metrics'
+    select_stmt += "  WHERE ts >= '2023-05-08 00:00:00.000000'"
+    select_stmt += "    AND ts < '2023-05-15 00:00:00.000000'"
+    select_stmt += '  GROUP BY attr_name'
+    select_stmt += '  ORDER BY mme_inner__ DESC'
+    select_stmt += '  LIMIT 500) AS anon_1 ON attr_name = attr_name__'
+    select_stmt += " WHERE ts >= '2023-05-08 00:00:00.000000'"
+    select_stmt += "   AND ts < '2023-05-15 00:00:00.000000'"
+    select_stmt += ' GROUP BY attr_name,'
+    select_stmt += '          ts'
+    select_stmt += '  ORDER BY "MAX(attr_value)" DESC'
+    select_stmt += '  LIMIT 10000'
+    assert QDBEngineSpec.parse_sql(select_stmt) == [
+        'SELECT ts AS __timestamp,    attr_name AS attr_name,    max(attr_value) AS '
+        '"MAX(attr_value)",    AVG(attr_value) AS "AVG(attr_value)",    '
+        'sum(attr_value) AS "SUM(attr_value)"  FROM node_metrics  JOIN(SELECT '
+        'attr_name AS attr_name__,    max(attr_value) AS mme_inner__  FROM '
+        "node_metrics  WHERE ts >= '2023-05-08 00:00:00.000000'    AND ts < "
+        "'2023-05-15 00:00:00.000000'  GROUP BY attr_name  ORDER BY mme_inner__ DESC  "
+        "LIMIT 500) AS anon_1 ON attr_name = attr_name__ WHERE ts >= '2023-05-08 "
+        "00:00:00.000000'   AND ts < '2023-05-15 00:00:00.000000' GROUP BY "
+        'attr_name            ORDER BY "MAX(attr_value)" DESC  LIMIT 10000'
+    ]
```

### Comparing `questdb-connect-0.0.45/tests/test_types.py` & `questdb-connect-0.0.46/tests/test_types.py`

 * *Files identical despite different names*

