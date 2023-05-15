# Comparing `tmp/databricks_common-0.1.2.tar.gz` & `tmp/databricks_common-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_common-0.1.2.tar", max compression
+gzip compressed data, was "databricks_common-0.1.3.tar", max compression
```

## Comparing `databricks_common-0.1.2.tar` & `databricks_common-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       29 2023-05-14 05:57:38.692660 databricks_common-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-05-14 06:13:24.562535 databricks_common-0.1.2/databricks_common/__init__.py
--rw-r--r--   0        0        0    10886 2023-05-14 06:10:06.703054 databricks_common-0.1.2/databricks_common/common.py
--rw-r--r--   0        0        0      195 2023-04-28 06:19:11.070881 databricks_common-0.1.2/databricks_common/main.py
--rwxr-xr-x   0        0        0      327 2023-05-14 05:35:02.723163 databricks_common-0.1.2/databricks_common/utils/get_spark.py
--rw-r--r--   0        0        0        0 2023-04-28 04:54:58.752421 databricks_common-0.1.2/databricks_common/utils/get_spark_local.py
--rw-r--r--   0        0        0      745 2023-04-28 04:34:36.232896 databricks_common-0.1.2/databricks_common/utils/logger_utils.py
--rw-r--r--   0        0        0      462 2023-05-14 06:13:29.850083 databricks_common-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-15 11:54:03.421548 databricks_common-0.1.3/databricks_common/__init__.py
+-rw-r--r--   0        0        0     8846 2023-05-15 11:42:32.515474 databricks_common-0.1.3/databricks_common/common.py
+-rw-r--r--   0        0        0      195 2023-05-15 10:35:58.597274 databricks_common-0.1.3/databricks_common/main.py
+-rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.3/databricks_common/utils/get_spark.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.3/databricks_common/utils/get_spark_local.py
+-rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.3/databricks_common/utils/logger_utils.py
+-rw-r--r--   0        0        0      740 2023-05-15 11:53:52.114143 databricks_common-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.3/PKG-INFO
```

### Comparing `databricks_common-0.1.2/databricks_common/common.py` & `databricks_common-0.1.3/databricks_common/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,21 +42,19 @@
         return cls(cat, schema, table)
 
     def check_exists(self) -> bool:
         MetastoreCatalog(self.catalog).set()
         return spark.catalog.tableExists(self.short_ref)
 
     def drop(self) -> None:
-        try:
-            spark.sql(f"DROP TABLE {self.ref}")
-            print(f"NOTE: Dropped table '{self.ref}' from Unity Metastore\n-----")
-        except Exception as e:
-            print(
-                f"NOTE: Could not drop table '{self.ref}' from Unity Metastore\n-----"
-            )
+        spark.sql(f"DROP TABLE {self.ref}")
+
+    def drop_if_exists(self) -> None:
+        if self.check_exists():
+            self.drop()
 
     def _create_basic_table(self, comment: str = "") -> None:
         """
         Function to create a basic table at self.ref
         """
         spark.sql(
             f"""
@@ -136,132 +134,89 @@
     - Describing a catalog in extended format
     - Dropping a catalog
     - Showing the available schemas in a catalog
     - For demo purposes, creating a catalog in a managed location
     """
 
     def __init__(self, name) -> None:
-        """
-        Parameters
-        ----------
-        name : str
-            Name of the catalog
-        """
         self.name = name
 
     def check_exists(self) -> bool:
-        """
-        Function to check if a catalog exists in Unity Metastore.
-        """
         try:
             spark.sql(f"DESC CATALOG {self.name}")
             return True
         except (
             Exception
         ) as e:  # TODO: Choose specific exception in case there is a specific error
             return False
 
+    def create(self, comment: str = "") -> None:
+        spark.sql(f"CREATE CATALOG {self.name} COMMENT '{comment}'")
+
     def create_if_not_exists(self, comment: str = "") -> None:
-        """
-        Function to create a catalog in Unity Metastore.
-        """
-        if self.check_exists():
-            _logger.warn(f"Catalog '{self.name}' already exists")
-            return
-        else:
-            _logger.info(f"Creating catalog '{self.name}'")
-            spark.sql(f"CREATE CATALOG {self.name} COMMENT '{comment}'")
+        spark.sql(f"CREATE CATALOG IF NOT EXISTS {self.name} COMMENT '{comment}'")
 
     def create_schema(self, schema_name: str, comment: str = "") -> None:
-        """
-        Function to create a schema in the catalog.
-        """
         self.set()
-        _logger.info(f"Creating schema '{schema_name}' in catalog '{self.name}'")
         spark.sql(f"CREATE SCHEMA {schema_name} COMMENT '{comment}'")
 
-    def create_managed_external(
+    def create_catalog_in_managed_location(
         self, container_uri: str = None, container_dir: str = None, comment: str = ""
     ) -> None:
-        """
-        Function to create a catalog in a managed location in Unity Metastore.
-        """
-        if self.check_exists():
-            _logger.info(f"Catalog '{self.name}' already exists")
-            return
-        else:
-            _logger.info(
-                f"Creating catalog '{self.name}' in managed location '{container_uri}/{container_dir}' with comment '{comment}'"
-            )
-
-            spark.sql(
-                f"""
-                CREATE CATALOG IF NOT EXISTS {self.name}
-                MANAGED LOCATION '{container_uri}/{container_dir}/'
-                COMMENT '{comment}' 
-                """
-            )
+        spark.sql(
+            f"""
+            CREATE CATALOG {self.name}
+            MANAGED LOCATION '{container_uri}/{container_dir}/'
+            COMMENT '{comment}' 
+            """
+        )
 
     def demo_create_managed_external_catalog(self) -> None:  # TODO: Convert to test
         """
         Function for demo purposes.
         """
-        self.create_managed_external(
+        self.create_catalog_in_managed_location(
             container_uri="abfss://xavierarmitage-container@oneenvadls.dfs.core.windows.net",
             container_dir="lake23",
             comment="Demo comment",
         )
 
     def describe(self) -> None:
-        """
-        Function to describe a catalog in Unity Metastore.
-        """
         spark.sql(f"DESC CATALOG {self.name}").display()
 
     def describe_extended(self) -> None:
-        """
-        Function to describe a catalog in Unity Metastore.
-        """
         spark.sql(f"DESC CATALOG EXTENDED {self.name}").display()
 
-    def drop(self) -> None:
-        """
-        Function to drop a catalog in Unity Catalog.
-        """
-        _logger.info(f"Dropping catalog '{self.name}'")
-        spark.sql(f"DROP CATALOG IF EXISTS {self.name}")
+    def drop(self, cascade=False) -> None:
+        if cascade:
+            spark.sql(f"DROP CATALOG {self.name} CASCADE")
+        else:
+            spark.sql(f"DROP CATALOG {self.name}")
+
+    def drop_if_exists(self, cascade=False) -> None:
+        if cascade:
+            spark.sql(f"DROP CATALOG IF EXISTS {self.name} CASCADE")
+        else:
+            spark.sql(f"DROP CATALOG IF EXISTS {self.name}")
 
     def drop_cascade(self) -> None:
-        """
-        Function to drop a catalog in Unity Catalog.
-        """
-        _logger.info(f"Dropping catalog '{self.name}'")
         self.drop(cascade=True)
 
     def drop_schema(self, cascade: bool = False):
-        """
-        Function to drop a schema in the catalog.
-        """
         self.set()
         _logger.info(f"Dropping schema '{self.name}'")
         if cascade:
             spark.sql(f"DROP SCHEMA IF EXISTS {self.name} CASCADE")
         else:
             spark.sql(f"DROP SCHEMA IF EXISTS {self.name}")
 
     def set(self) -> None:
-        """
-        Function to set the current catalog.
-        """
         spark.sql(f"SET CATALOG {self.name}")
 
     def show_schemas(self) -> None:
-        """
-        Function to show schemas in catalog.
-        """
         self.set()
         spark.sql("SHOW SCHEMAS").display()
 
 
 class MetastoreSchema:
     """
     Class to represent a schema in Unity Metastore.
@@ -282,68 +237,45 @@
         MetastoreCatalog(self.catalog).set()
 
     def check_exists(self) -> bool:
         """
         Function to check if a schema exists in Unity Metastore.
         """
         # TODO: There might be a more direct way to do this
-        self._set_catalog()
         try:
-            spark.sql(f"DESC SCHEMA {self.name}")
+            spark.sql(f"DESC SCHEMA {self.catalog}.{self.name}")
             return True
         except Exception as e:
             return False
 
+    def create(self, comment: str = "") -> None:
+        spark.sql(f"CREATE SCHEMA {self.ref} COMMENT '{comment}'")
+
     def create_if_not_exists(self, comment: str = "") -> None:
-        """
-        Function to create a schema in Unity Metastore.
-        """
-        self._set_catalog()
-        if self.check_exists():
-            _logger.warn(f"Schema '{self.name}' already exists")
-            return
-        else:
-            _logger.info(f"Creating schema '{self.name}'")
-            spark.sql(f"CREATE SCHEMA {self.name} COMMENT '{comment}'")
+        spark.sql(f"CREATE SCHEMA IF NOT EXISTS {self.ref} COMMENT '{comment}'")
 
     def describe(self) -> None:
-        """
-        Function to describe a schema in Unity Metastore.
-        """
-        self._set_catalog()
-        spark.sql(f"DESC SCHEMA {self.name}").display()
+        spark.sql(f"DESC SCHEMA {self.ref}").display()
 
     def describe_extended(self) -> None:
-        """
-        Function to describe a schema in Unity Metastore.
-        """
-        self._set_catalog()
-        spark.sql(f"DESC SCHEMA EXTENDED {self.name}").display()
+        spark.sql(f"DESC SCHEMA EXTENDED {self.ref}").display()
 
     def drop(self, cascade: bool = False) -> None:
-        """
-        Function to drop a schema in Unity Metastore.
-        """
-        self._set_catalog()
-        _logger.info(f"Dropping schema '{self.name}'")
         if cascade:
-            spark.sql(f"DROP SCHEMA IF EXISTS {self.name} CASCADE")
+            spark.sql(f"DROP SCHEMA {self.ref} CASCADE")
         else:
-            spark.sql(f"DROP SCHEMA IF EXISTS {self.name}")
+            spark.sql(f"DROP SCHEMA {self.ref}")
+
+    def drop_if_exists(self, cascade: bool = False) -> None:
+        if cascade:
+            spark.sql(f"DROP SCHEMA IF EXISTS {self.ref} CASCADE")
+        else:
+            spark.sql(f"DROP SCHEMA IF EXISTS {self.ref}")
 
     def show_tables(self) -> None:
-        """
-        Function to show tables in schema.
-        """
-        self._set_catalog()
-        spark.sql(f"SHOW TABLES IN {self.name}").display()
+        spark.sql(f"SHOW TABLES IN {self.ref}").display()
 
     def set(self) -> None:
-        """
-        Function to set the current schema.
-        """
-        self._set_catalog()
-        _logger.info(f"Setting schema '{self.name}' as current schema")
-        spark.sql(f"SET SCHEMA {self.name}")
+        spark.sql(f"SET SCHEMA {self.ref}")
 
     def _get_ref(self) -> str:
         return f"{self.catalog}.{self.name}"
```

### Comparing `databricks_common-0.1.2/databricks_common/utils/logger_utils.py` & `databricks_common-0.1.3/databricks_common/utils/logger_utils.py`

 * *Files identical despite different names*

