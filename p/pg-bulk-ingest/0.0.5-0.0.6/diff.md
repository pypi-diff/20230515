# Comparing `tmp/pg_bulk_ingest-0.0.5.tar.gz` & `tmp/pg_bulk_ingest-0.0.6.tar.gz`

## Comparing `pg_bulk_ingest-0.0.5.tar` & `pg_bulk_ingest-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/pg_bulk_ingest.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/LICENSE
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/pg_bulk_ingest.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.6/PKG-INFO
```

### Comparing `pg_bulk_ingest-0.0.5/.gitignore` & `pg_bulk_ingest-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.5/LICENSE` & `pg_bulk_ingest-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.5/README.md` & `pg_bulk_ingest-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 # pg-bulk-ingest
 
 A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking
 
 > Work-in-progress. This README serves as a rough design spec
 
 
+## Installation
+
+`pg-bulk-ingest` can be installed from  PyPI using `pip`. `psycopg2` or `psycopg` (Psycopg 3) must also be explicitly installed.
+
+```
+pip install pg-bulk-ingest psycopg
+```
+
+
 ## Usage
 
 The API is made of 3 functions:
 
 - `replace` - replaces all the existing rows in the table with the incoming rows
 - `insert` - inserts the incoming rows into the table, leaving existing rows alone
 - `upsert` - inserts the incoming rows into the table, but if a primary key matches an existing row, updates the existing row
 
-In each case:
+In each case under hood:
 
-- Ingestion happens in a transaction - it is all ingested or none at all
-- Tables are migrated to match the definitions, using techniques to avoid exclusively locking the table to allow parallel SELECT queries
-- If there is no known technique for a migration without an exclusive lock, then an intermediate table is used, swapped with the live table at the end of the ingest. This does require an exclusive lock, but only for a short time. Backends that hold locks that conflict with this lock are forcably terminated after a delay.
 - Ingestion is done exclusively with `COPY FROM`.
+- Ingestion happens in a transaction - it is all ingested or none at all
+- The transaction is managed by client code, allowing other transactional changes such as updating metadata tables
+- Tables are migrated to match the definitions, using techniques to avoid exclusively locking the table to allow parallel SELECT queries.
+- For `upsert`, data is ingested into an intermediate table, and an `INSERT ... ON CONFICT(...) DO UPDATE` is performed to copy rows from this intermediate table to the existing table. This doesn't involve an exclusive lock on the live table, unless a migration requires it as follows.
+- For all 3 functions, if there is no known technique for a migration without a long-running exclusive lock, then an intermediate table is used, swapped with the live table at the end of the ingest. This swap does require an exclusive lock, but only for a short time. Backends that hold locks that conflict with this lock are forcably terminated after a delay.
 
 For example to `upsert`:
 
 ```python
 import sqlalchemy as sa
 from pg_bulk_ingest import upsert
 
@@ -34,18 +45,28 @@
 rows = (
     (3, 'd'),
     (4, 'a'),
     (5, 'q'),
 )
 
 # Collection of SQLAlchemy table definitions - a "Metadata"
-metadata_obj = sa.MetaData()
+metadata = sa.MetaData()
 my_table = sa.Table(
     "my_table",
-    metadata_obj,
+    metadata,
     sa.Column("id", sa.Integer, primary_key=True),
     sa.Column("value", sa.String(16), nullable=False),
     schema="my_schema",
 )
 with engine.begin() as conn:
-    upsert(conn, metadata_obj, ((row, my_table) for row in rows))
+    upsert(conn, metadata, ((row, my_table) for row in rows))
 ```
+
+
+## Compatibility
+
+- Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
+- psycopg2 >= 2.9.2 or Psycopg 3 >= 3.1.4
+- SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
+- PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, and 15.0)
+
+Note that SQLAlchemy < 2 does not support Psycopg 3.
```

### Comparing `pg_bulk_ingest-0.0.5/pyproject.toml` & `pg_bulk_ingest-0.0.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-bulk-ingest"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "sqlalchemy>=1.4.0,<2.0.0", 
+    "sqlalchemy>=1.4.24", 
 ]
 
 [project.optional-dependencies]
 dev = [
+    "psycopg>=3.1.4",
+    "psycopg2>=2.9.2",
     "pytest>=7.2.1",
-    "psycopg2-binary>=2.8.6",
+]
+ci = [
+    "pytest==7.2.1",
+]
+ci-psycopg2-sqlalchemy1 = [
+    "psycopg2==2.9.2",
+    "sqlalchemy==1.4.24",
+]
+ci-psycopg2-sqlalchemy2 = [
+    "psycopg2==2.9.2",
+    "sqlalchemy==2.0.0",
+]
+ci-psycopg3-sqlalchemy2 = [
+    "psycopg==3.1.4",
+    "sqlalchemy==2.0.0",
 ]
 
 [project.urls]
 "Source" = "https://github.com/uktrade/pg-bulk-ingest"
 
 [tool.hatch.build]
 include = [
```

