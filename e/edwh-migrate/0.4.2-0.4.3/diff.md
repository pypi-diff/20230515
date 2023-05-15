# Comparing `tmp/edwh_migrate-0.4.2.tar.gz` & `tmp/edwh_migrate-0.4.3.tar.gz`

## Comparing `edwh_migrate-0.4.2.tar` & `edwh_migrate-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/migrations.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/requirements.txt
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/src/edwh_migrate/__about__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/src/edwh_migrate/__init__.py
--rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/src/edwh_migrate/migrate.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/test_basics.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/sqlite_empty/empty_sqlite.db
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/sqlite_empty/just_implemented_features.db
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/sqlite_empty/just_implemented_features.sql
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/README.md
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/migrations.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/requirements.txt
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/src/edwh_migrate/__about__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/src/edwh_migrate/__init__.py
+-rw-r--r--   0        0        0    19223 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/src/edwh_migrate/migrate.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/test_basics.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/sqlite_empty/empty_sqlite.db
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/sqlite_empty/just_implemented_features.db
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/sqlite_empty/just_implemented_features.sql
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/LICENSE.txt
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/README.md
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/PKG-INFO
```

### Comparing `edwh_migrate-0.4.2/CHANGELOG.md` & `edwh_migrate-0.4.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.3 (2023-05-15)
+### Fix
+* BaseExceptionGroup does not exist in 3.10 yet ([`3433a4f`](https://github.com/educationwarehouse/migrate/commit/3433a4fda0d6ebfb2a551d9f5c3feb4f51e6afc0))
+
 ## v0.4.2 (2023-05-04)
 ### Documentation
 * **migrate:** Changed package name from '-' to edwh-migrate and added extra's dev dependencies ([`ae3eef6`](https://github.com/educationwarehouse/migrate/commit/ae3eef6a1e2db47d03fcd60a57d768d79b7f4a32))
 
 ## v0.4.1 (2023-05-04)
 ### Fix
 * Better troubleshooting support for the sys.argv[1] argument ([`8a21505`](https://github.com/educationwarehouse/migrate/commit/8a21505307618a45d993b772f1ea40e0c4b3343f))
```

### Comparing `edwh_migrate-0.4.2/migrations.py` & `edwh_migrate-0.4.3/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/requirements.txt` & `edwh_migrate-0.4.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/src/edwh_migrate/__init__.py` & `edwh_migrate-0.4.3/src/edwh_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/src/edwh_migrate/migrate.py` & `edwh_migrate-0.4.3/src/edwh_migrate/migrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
                 yield
             except MigrationFailed:
                 # remove the lock file, so that the migration can be retried.
                 print("ERROR: migration failed, removing the lock file.\n"
                       "Check the ewh_implemented_features table for details.")
                 lock_file.unlink()
 
-            except BaseExceptionGroup:
+            except Exception:
                 # since another exception was raised, reraise it for the stack trace.
                 lock_file.unlink()
                 raise
 
 
 def console_hook():
     """
```

### Comparing `edwh_migrate-0.4.2/tests/test_basics.py` & `edwh_migrate-0.4.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/tests/sqlite_empty/empty_sqlite.db` & `edwh_migrate-0.4.3/tests/sqlite_empty/empty_sqlite.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/tests/sqlite_empty/just_implemented_features.db` & `edwh_migrate-0.4.3/tests/sqlite_empty/just_implemented_features.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/.gitignore` & `edwh_migrate-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/LICENSE.txt` & `edwh_migrate-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/README.md` & `edwh_migrate-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/pyproject.toml` & `edwh_migrate-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.2/PKG-INFO` & `edwh_migrate-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-migrate
-Version: 0.4.2
+Version: 0.4.3
 Summary: Helps migrating database schema changes using pydal. 
 Project-URL: Documentation, https://github.com/educationwarehouse/migrate#readme
 Project-URL: Issues, https://github.com/educationwarehouse/migrate/issues
 Project-URL: Source, https://github.com/educationwarehouse/migrate
 Author-email: Remco <remco@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

