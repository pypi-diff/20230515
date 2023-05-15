# Comparing `tmp/trino-0.323.0.tar.gz` & `tmp/trino-0.324.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trino-0.323.0.tar", last modified: Tue May  2 09:18:30 2023, max compression
+gzip compressed data, was "trino-0.324.0.tar", last modified: Mon May 15 13:47:40 2023, max compression
```

## Comparing `trino-0.323.0.tar` & `trino-0.324.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:18:30.679182 trino-0.323.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 09:18:16.000000 trino-0.323.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-02 09:18:30.679182 trino-0.323.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-05-02 09:18:16.000000 trino-0.323.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-02 09:18:30.679182 trino-0.323.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-05-02 09:18:16.000000 trino-0.323.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:18:30.675182 trino-0.323.0/trino/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-02 09:18:19.000000 trino-0.323.0/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-02 09:18:16.000000 trino-0.323.0/trino/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    47042 2023-05-02 09:18:16.000000 trino-0.323.0/trino/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 09:18:16.000000 trino-0.323.0/trino/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    22662 2023-05-02 09:18:16.000000 trino-0.323.0/trino/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-02 09:18:16.000000 trino-0.323.0/trino/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-02 09:18:16.000000 trino-0.323.0/trino/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:18:30.679182 trino-0.323.0/trino/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-02 09:18:16.000000 trino-0.323.0/trino/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:18:30.675182 trino-0.323.0/trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:47:40.201059 trino-0.324.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-15 13:47:24.000000 trino-0.324.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 13:47:40.201059 trino-0.324.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-05-15 13:47:24.000000 trino-0.324.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 13:47:40.205060 trino-0.324.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3451 2023-05-15 13:47:24.000000 trino-0.324.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:47:40.201059 trino-0.324.0/trino/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-15 13:47:28.000000 trino-0.324.0/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-15 13:47:24.000000 trino-0.324.0/trino/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46886 2023-05-15 13:47:24.000000 trino-0.324.0/trino/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-15 13:47:24.000000 trino-0.324.0/trino/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22753 2023-05-15 13:47:24.000000 trino-0.324.0/trino/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-15 13:47:24.000000 trino-0.324.0/trino/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 13:47:24.000000 trino-0.324.0/trino/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:47:40.201059 trino-0.324.0/trino/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-15 13:47:24.000000 trino-0.324.0/trino/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:47:40.201059 trino-0.324.0/trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/top_level.txt
```

### Comparing `trino-0.323.0/LICENSE` & `trino-0.324.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/PKG-INFO` & `trino-0.324.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trino
-Version: 0.323.0
+Version: 0.324.0
 Summary: Client for the Trino distributed SQL Engine
 Home-page: https://github.com/trinodb/trino-python-client
 Author: Trino Team
 Author-email: python-client@trino.io
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trino-0.323.0/README.md` & `trino-0.324.0/README.md`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/setup.py` & `trino-0.324.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,21 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Database :: Front-Ends",
     ],
     python_requires='>=3.7',
-    install_requires=["pytz", "requests", "tzlocal"],
+    install_requires=[
+        "backports.zoneinfo;python_version<'3.9'",
+        "python-dateutil",
+        "pytz",
+        "requests",
+        "tzlocal",
+    ],
     extras_require={
         "all": all_require,
         "kerberos": kerberos_require,
         "sqlalchemy": sqlalchemy_require,
         "tests": tests_require,
         "external-authentication-token-cache": external_authentication_token_cache_require,
     },
```

### Comparing `trino-0.323.0/trino/__init__.py` & `trino-0.324.0/trino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import auth, client, constants, dbapi, exceptions, logging
 
 __all__ = ['auth', 'dbapi', 'client', 'constants', 'exceptions', 'logging']
 
-__version__ = "0.323.0"
+__version__ = "0.324.0"
```

### Comparing `trino-0.323.0/trino/auth.py` & `trino-0.324.0/trino/auth.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/client.py` & `trino-0.324.0/trino/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,29 +47,26 @@
 import warnings
 from dataclasses import dataclass
 from datetime import date, datetime, time, timedelta, timezone, tzinfo
 from decimal import Decimal
 from time import sleep
 from typing import Any, Dict, Generic, List, Optional, Tuple, TypeVar, Union
 
-import pytz
+try:
+    from zoneinfo import ZoneInfo
+except ModuleNotFoundError:
+    from backports.zoneinfo import ZoneInfo
+
 import requests
-from pytz.tzinfo import BaseTzInfo
+from dateutil import tz
 from tzlocal import get_localzone_name  # type: ignore
 
 import trino.logging
 from trino import constants, exceptions
 
-try:
-    from zoneinfo import ZoneInfo  # type: ignore
-
-except ModuleNotFoundError:
-    from backports.zoneinfo import ZoneInfo  # type: ignore
-
-
 __all__ = ["ClientSession", "TrinoQuery", "TrinoRequest", "PROXIES"]
 
 logger = trino.logging.get_logger(__name__)
 
 MAX_ATTEMPTS = constants.DEFAULT_MAX_ATTEMPTS
 SOCKS_PROXY = os.environ.get("SOCKS_PROXY")
 if SOCKS_PROXY:
@@ -942,15 +939,15 @@
     if timezone_str.startswith("+") or timezone_str.startswith("-"):
         hours = timezone_str[1:3]
         minutes = timezone_str[4:6]
         if timezone_str.startswith("-"):
             return timezone(-timedelta(hours=int(hours), minutes=int(minutes)))
         return timezone(timedelta(hours=int(hours), minutes=int(minutes)))
     else:
-        return pytz.timezone(timezone_str)
+        return ZoneInfo(timezone_str)
 
 
 def _fraction_to_decimal(fractional_str: str) -> Decimal:
     return Decimal(fractional_str or 0) / POWERS_OF_TEN[len(fractional_str)]
 
 
 class TemporalType(Generic[PythonTemporalType], metaclass=abc.ABCMeta):
@@ -992,16 +989,15 @@
             This method shall be overriden to implement fraction arithmetics.
         """
         pass
 
     def normalize(self, value: PythonTemporalType) -> PythonTemporalType:
         """
             If `add_time_delta` results in value crossing DST boundaries, this method should
-            return a normalized version of the value to account for it, for example,
-            using `pytz.timezone.normalize`.
+            return a normalized version of the value to account for it.
         """
         return value
 
 
 class Time(TemporalType[time]):
     def new_instance(self, value: time, fraction: Decimal) -> TemporalType[time]:
         return Time(value, fraction)
@@ -1037,15 +1033,15 @@
 
 
 class TimestampWithTimeZone(Timestamp, TemporalType[datetime]):
     def new_instance(self, value: datetime, fraction: Decimal) -> TimestampWithTimeZone:
         return TimestampWithTimeZone(value, fraction)
 
     def normalize(self, value: datetime) -> datetime:
-        if isinstance(self._whole_python_temporal_value.tzinfo, BaseTzInfo):
+        if tz.datetime_ambiguous(value):
             return self._whole_python_temporal_value.tzinfo.normalize(value)
         return value
 
 
 class TimeValueMapper(ValueMapper[time]):
     def __init__(self, precision):
         self.time_default_size = 8  # size of 'HH:MM:SS'
```

### Comparing `trino-0.323.0/trino/constants.py` & `trino-0.324.0/trino/constants.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/dbapi.py` & `trino-0.324.0/trino/dbapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 import datetime
 import math
 import uuid
 from decimal import Decimal
 from typing import Any, Dict, List, NamedTuple, Optional  # NOQA for mypy types
 from urllib.parse import urlparse
 
-import pytz
+try:
+    from zoneinfo import ZoneInfo
+except ModuleNotFoundError:
+    from backports.zoneinfo import ZoneInfo
 
 import trino.client
 import trino.exceptions
 import trino.logging
 from trino import constants
 from trino.constants import LENGTH_TYPES, PRECISION_TYPES, SCALE_TYPES
 from trino.exceptions import (
@@ -421,29 +424,29 @@
         if isinstance(param, datetime.datetime) and param.tzinfo is None:
             datetime_str = param.strftime("%Y-%m-%d %H:%M:%S.%f")
             return "TIMESTAMP '%s'" % datetime_str
 
         if isinstance(param, datetime.datetime) and param.tzinfo is not None:
             datetime_str = param.strftime("%Y-%m-%d %H:%M:%S.%f")
             # named timezones
-            if hasattr(param.tzinfo, 'zone'):
-                return "TIMESTAMP '%s %s'" % (datetime_str, param.tzinfo.zone)
+            if isinstance(param.tzinfo, ZoneInfo):
+                return "TIMESTAMP '%s %s'" % (datetime_str, param.tzinfo.key)
             # offset-based timezones
             return "TIMESTAMP '%s %s'" % (datetime_str, param.tzinfo.tzname(param))
 
         # We can't calculate the offset for a time without a point in time
         if isinstance(param, datetime.time) and param.tzinfo is None:
             time_str = param.strftime("%H:%M:%S.%f")
             return "TIME '%s'" % time_str
 
         if isinstance(param, datetime.time) and param.tzinfo is not None:
             time_str = param.strftime("%H:%M:%S.%f")
             # named timezones
-            if hasattr(param.tzinfo, 'zone'):
-                utc_offset = datetime.datetime.now(pytz.timezone(param.tzinfo.zone)).strftime('%z')
+            if isinstance(param.tzinfo, ZoneInfo):
+                utc_offset = datetime.datetime.now(tz=param.tzinfo).strftime('%z')
                 return "TIME '%s %s:%s'" % (time_str, utc_offset[:3], utc_offset[3:])
             # offset-based timezones
             return "TIME '%s %s'" % (time_str, param.strftime('%Z')[3:])
 
         if isinstance(param, datetime.date):
             date_str = param.strftime("%Y-%m-%d")
             return "DATE '%s'" % date_str
```

### Comparing `trino-0.323.0/trino/exceptions.py` & `trino-0.324.0/trino/exceptions.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/logging.py` & `trino-0.324.0/trino/logging.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/sqlalchemy/__init__.py` & `trino-0.324.0/trino/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/sqlalchemy/compiler.py` & `trino-0.324.0/trino/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/sqlalchemy/datatype.py` & `trino-0.324.0/trino/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/sqlalchemy/dialect.py` & `trino-0.324.0/trino/sqlalchemy/dialect.py`

 * *Files 3% similar despite different names*

```diff
@@ -332,23 +332,28 @@
         res = connection.execute(sql.text(query), {"schema": schema, "table": table_name})
         return res.first() is not None
 
     def has_sequence(self, connection: Connection, sequence_name: str, schema: str = None, **kw) -> bool:
         """Trino has no support for sequence. Returns False indicate that given sequence does not exists."""
         return False
 
-    def _get_server_version_info(self, connection: Connection) -> Any:
-        query = "SELECT version()"
-        try:
-            res = connection.execute(sql.text(query))
-            version = res.scalar()
-            return tuple([version])
-        except exc.ProgrammingError as e:
-            logger.debug(f"Failed to get server version: {e.orig.message}")
-            return None
+    @classmethod
+    def _get_server_version_info(cls, connection: Connection) -> Any:
+        def get_server_version_info(_):
+            query = "SELECT version()"
+            try:
+                res = connection.execute(sql.text(query))
+                version = res.scalar()
+                return tuple([version])
+            except exc.ProgrammingError as e:
+                logger.debug(f"Failed to get server version: {e.orig.message}")
+                return None
+
+        # Make server_version_info lazy in order to only make HTTP calls if user explicitly requests it.
+        cls.server_version_info = property(get_server_version_info, lambda instance, value: None)
 
     def _raw_connection(self, connection: Union[Engine, Connection]) -> trino_dbapi.Connection:
         if isinstance(connection, Engine):
             return connection.raw_connection()
         return connection.connection
 
     def _get_default_catalog_name(self, connection: Connection) -> Optional[str]:
```

### Comparing `trino-0.323.0/trino/sqlalchemy/error.py` & `trino-0.324.0/trino/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/sqlalchemy/util.py` & `trino-0.324.0/trino/sqlalchemy/util.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino/transaction.py` & `trino-0.324.0/trino/transaction.py`

 * *Files identical despite different names*

### Comparing `trino-0.323.0/trino.egg-info/PKG-INFO` & `trino-0.324.0/trino.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trino
-Version: 0.323.0
+Version: 0.324.0
 Summary: Client for the Trino distributed SQL Engine
 Home-page: https://github.com/trinodb/trino-python-client
 Author: Trino Team
 Author-email: python-client@trino.io
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trino-0.323.0/trino.egg-info/SOURCES.txt` & `trino-0.324.0/trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

