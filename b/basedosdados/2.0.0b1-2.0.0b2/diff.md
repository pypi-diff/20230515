# Comparing `tmp/basedosdados-2.0.0b1.tar.gz` & `tmp/basedosdados-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basedosdados-2.0.0b1.tar", max compression
+gzip compressed data, was "basedosdados-2.0.0b2.tar", max compression
```

## Comparing `basedosdados-2.0.0b1.tar` & `basedosdados-2.0.0b2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2514 2023-05-04 15:04:40.695846 basedosdados-2.0.0b1/README.md
--rw-r--r--   0        0        0      827 2023-05-12 22:53:21.043886 basedosdados-2.0.0b1/basedosdados/__init__.py
--rw-r--r--   0        0        0      156 2023-05-10 00:48:26.910378 basedosdados-2.0.0b1/basedosdados/__main__.py
--rw-r--r--   0        0        0     8562 2023-05-11 18:29:32.124461 basedosdados-2.0.0b1/basedosdados/backend/__init__.py
--rw-r--r--   0        0        0     6737 2023-05-12 22:20:15.182110 basedosdados-2.0.0b1/basedosdados/cli/cli.py
--rw-r--r--   0        0        0      277 2023-05-10 18:22:29.189209 basedosdados-2.0.0b1/basedosdados/configs/config.toml
--rw-r--r--   0        0        0      469 2022-02-13 03:48:24.650258 basedosdados-2.0.0b1/basedosdados/configs/templates/dataset/README.md
--rw-r--r--   0        0        0      856 2022-02-13 03:48:24.650328 basedosdados-2.0.0b1/basedosdados/configs/templates/dataset/dataset_description.txt
--rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.650411 basedosdados-2.0.0b1/basedosdados/configs/templates/table/publish.sql
--rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.504177 basedosdados-2.0.0b1/basedosdados/configs/templates/table/table_description.txt
--rw-r--r--   0        0        0      895 2023-05-10 00:48:26.956830 basedosdados-2.0.0b1/basedosdados/constants.py
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650584 basedosdados-2.0.0b1/basedosdados/download/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-10 00:48:26.938508 basedosdados-2.0.0b1/basedosdados/download/base.py
--rw-r--r--   0        0        0    17788 2023-05-10 00:48:27.143327 basedosdados-2.0.0b1/basedosdados/download/download.py
--rw-r--r--   0        0        0    13689 2023-05-10 00:48:27.186769 basedosdados-2.0.0b1/basedosdados/download/metadata.py
--rw-r--r--   0        0        0     3903 2023-05-10 00:48:26.993068 basedosdados-2.0.0b1/basedosdados/exceptions.py
--rw-r--r--   0        0        0     6779 2023-05-04 15:04:40.696211 basedosdados-2.0.0b1/basedosdados/schemas/columns_schema.json
--rw-r--r--   0        0        0    65118 2023-05-04 15:04:40.696404 basedosdados-2.0.0b1/basedosdados/schemas/dataset_schema.json
--rw-r--r--   0        0        0    30753 2023-05-04 15:04:40.696511 basedosdados-2.0.0b1/basedosdados/schemas/table_schema.json
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650914 basedosdados-2.0.0b1/basedosdados/upload/__init__.py
--rw-r--r--   0        0        0    15586 2023-05-12 22:28:30.811753 basedosdados-2.0.0b1/basedosdados/upload/base.py
--rw-r--r--   0        0        0     4957 2023-05-10 01:30:14.254761 basedosdados-2.0.0b1/basedosdados/upload/connection.py
--rw-r--r--   0        0        0     8821 2023-05-12 22:28:04.742108 basedosdados-2.0.0b1/basedosdados/upload/dataset.py
--rw-r--r--   0        0        0     3228 2023-05-12 21:24:41.585549 basedosdados-2.0.0b1/basedosdados/upload/datatypes.py
--rw-r--r--   0        0        0    18917 2023-05-12 21:58:31.960998 basedosdados-2.0.0b1/basedosdados/upload/storage.py
--rw-r--r--   0        0        0    30312 2023-05-12 22:26:47.897766 basedosdados-2.0.0b1/basedosdados/upload/table.py
--rw-r--r--   0        0        0     3434 2023-05-12 22:26:30.059112 basedosdados-2.0.0b1/basedosdados/upload/utils.py
--rw-r--r--   0        0        0     1404 2023-05-12 22:53:22.557176 basedosdados-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     3901 1970-01-01 00:00:00.000000 basedosdados-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     2514 2023-05-04 15:04:40.695846 basedosdados-2.0.0b2/README.md
+-rw-r--r--   0        0        0      827 2023-05-12 22:53:21.043886 basedosdados-2.0.0b2/basedosdados/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-10 00:48:26.910378 basedosdados-2.0.0b2/basedosdados/__main__.py
+-rw-r--r--   0        0        0     8865 2023-05-15 20:52:16.710589 basedosdados-2.0.0b2/basedosdados/backend/__init__.py
+-rw-r--r--   0        0        0     6737 2023-05-12 22:20:15.182110 basedosdados-2.0.0b2/basedosdados/cli/cli.py
+-rw-r--r--   0        0        0      277 2023-05-10 18:22:29.189209 basedosdados-2.0.0b2/basedosdados/configs/config.toml
+-rw-r--r--   0        0        0      469 2022-02-13 03:48:24.650258 basedosdados-2.0.0b2/basedosdados/configs/templates/dataset/README.md
+-rw-r--r--   0        0        0      856 2022-02-13 03:48:24.650328 basedosdados-2.0.0b2/basedosdados/configs/templates/dataset/dataset_description.txt
+-rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.650411 basedosdados-2.0.0b2/basedosdados/configs/templates/table/publish.sql
+-rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.504177 basedosdados-2.0.0b2/basedosdados/configs/templates/table/table_description.txt
+-rw-r--r--   0        0        0      895 2023-05-10 00:48:26.956830 basedosdados-2.0.0b2/basedosdados/constants.py
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650584 basedosdados-2.0.0b2/basedosdados/download/__init__.py
+-rw-r--r--   0        0        0     1641 2023-05-10 00:48:26.938508 basedosdados-2.0.0b2/basedosdados/download/base.py
+-rw-r--r--   0        0        0    17788 2023-05-10 00:48:27.143327 basedosdados-2.0.0b2/basedosdados/download/download.py
+-rw-r--r--   0        0        0    13689 2023-05-10 00:48:27.186769 basedosdados-2.0.0b2/basedosdados/download/metadata.py
+-rw-r--r--   0        0        0     3903 2023-05-10 00:48:26.993068 basedosdados-2.0.0b2/basedosdados/exceptions.py
+-rw-r--r--   0        0        0     6779 2023-05-04 15:04:40.696211 basedosdados-2.0.0b2/basedosdados/schemas/columns_schema.json
+-rw-r--r--   0        0        0    65118 2023-05-04 15:04:40.696404 basedosdados-2.0.0b2/basedosdados/schemas/dataset_schema.json
+-rw-r--r--   0        0        0    30753 2023-05-04 15:04:40.696511 basedosdados-2.0.0b2/basedosdados/schemas/table_schema.json
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650914 basedosdados-2.0.0b2/basedosdados/upload/__init__.py
+-rw-r--r--   0        0        0    15586 2023-05-12 22:28:30.811753 basedosdados-2.0.0b2/basedosdados/upload/base.py
+-rw-r--r--   0        0        0     4957 2023-05-10 01:30:14.254761 basedosdados-2.0.0b2/basedosdados/upload/connection.py
+-rw-r--r--   0        0        0     9399 2023-05-15 18:47:56.098568 basedosdados-2.0.0b2/basedosdados/upload/dataset.py
+-rw-r--r--   0        0        0     3228 2023-05-12 21:24:41.585549 basedosdados-2.0.0b2/basedosdados/upload/datatypes.py
+-rw-r--r--   0        0        0    18917 2023-05-12 21:58:31.960998 basedosdados-2.0.0b2/basedosdados/upload/storage.py
+-rw-r--r--   0        0        0    30950 2023-05-15 20:52:19.557521 basedosdados-2.0.0b2/basedosdados/upload/table.py
+-rw-r--r--   0        0        0     3434 2023-05-12 22:26:30.059112 basedosdados-2.0.0b2/basedosdados/upload/utils.py
+-rw-r--r--   0        0        0     1453 2023-05-15 20:55:29.190003 basedosdados-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 basedosdados-2.0.0b2/PKG-INFO
```

### Comparing `basedosdados-2.0.0b1/README.md` & `basedosdados-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/__init__.py` & `basedosdados-2.0.0b2/basedosdados/__init__.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/backend/__init__.py` & `basedosdados-2.0.0b2/basedosdados/backend/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,39 +93,44 @@
         """
         variables = {"slug": dataset_slug}
         response = self._execute_query(query=query, variables=variables)
         r = self._simplify_graphql_response(response)
         if r["allDataset"] != []:
             return r["allDataset"][0]["_id"]
         msg = f"{dataset_slug} not found. Please create the metadata first in {self.graphql_url}"
-        raise BaseDosDadosException(msg)
+        logger.info(msg)
+        return None
 
     def _get_table_id_from_slug(self, dataset_slug, table_slug):
         query = """
             query ($dataset_Id: ID!, $table_slug: String!){
                 allTable (dataset_Id:$dataset_Id slug:$table_slug){
                     edges {
                         node {
                             _id
                         }
                     }
                 }
             }
         """
+        dataset_id = self._get_dataset_id_from_slug(dataset_slug)
 
-        variables = {
-            "dataset_Id": self._get_dataset_id_from_slug(dataset_slug),
-            "table_slug": table_slug,
-        }
-        response = self._execute_query(query=query, variables=variables)
-        r = self._simplify_graphql_response(response)
-        if r["allTable"] != []:
-            return r["allTable"][0]["_id"]
-        msg = f"No table {table_slug} found in {dataset_slug}."
-        raise BaseDosDadosException(msg)
+        if dataset_id:
+            variables = {
+                "dataset_Id": dataset_id,
+                "table_slug": table_slug,
+            }
+
+            response = self._execute_query(query=query, variables=variables)
+            r = self._simplify_graphql_response(response)
+            if r["allTable"] != []:
+                return r["allTable"][0]["_id"]
+        msg = f"No table {table_slug} found in {dataset_slug}. Please create in {self.graphql_url}"
+        logger.info(msg)
+        return None
 
     def get_dataset_config(self, dataset_id: str) -> Dict[str, Any]:
         """
         Get dataset configuration.
 
         Args:
             dataset_id (str): The ID for the dataset.
@@ -162,17 +167,21 @@
                             }
                         }
                     }
                 }
             }
         
         """
-        variables = {"dataset_id": self._get_dataset_id_from_slug(dataset_id)}
-        response = self._execute_query(query=query, variables=variables)
-        return self._simplify_graphql_response(response).get("allDataset")[0]
+        dataset_id = self._get_dataset_id_from_slug(dataset_id)
+        if dataset_id:
+            variables = {"dataset_id": dataset_id}
+            response = self._execute_query(query=query, variables=variables)
+            return self._simplify_graphql_response(response).get("allDataset")[0]
+        else:
+            return {}
 
     def get_table_config(self, dataset_id: str, table_id: str) -> Dict[str, Any]:
         """
         Get table configuration.
 
         Args:
             dataset_id (str): The ID for the dataset.
@@ -211,21 +220,24 @@
                             }
                         }
                     }
                 }
                 }
             }    
         """
-        variables = {
-            "table_id": self._get_table_id_from_slug(
-                dataset_slug=dataset_id, table_slug=table_id
-            )
-        }
-        response = self._execute_query(query=query, variables=variables)
-        return self._simplify_graphql_response(response).get("allTable")[0]
+        table_id = self._get_table_id_from_slug(
+            dataset_slug=dataset_id, table_slug=table_id
+        )
+
+        if table_id:
+            variables = {"table_id": table_id}
+            response = self._execute_query(query=query, variables=variables)
+            return self._simplify_graphql_response(response).get("allTable")[0]
+        else:
+            return {}
 
     def _simplify_graphql_response(self, response: dict) -> dict:
         """
         Simplify the graphql response
         Args:
             response: the graphql response
         Returns:
```

### Comparing `basedosdados-2.0.0b1/basedosdados/cli/cli.py` & `basedosdados-2.0.0b2/basedosdados/cli/cli.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/configs/templates/dataset/dataset_description.txt` & `basedosdados-2.0.0b2/basedosdados/configs/templates/dataset/dataset_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/configs/templates/table/publish.sql` & `basedosdados-2.0.0b2/basedosdados/configs/templates/table/publish.sql`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/configs/templates/table/table_description.txt` & `basedosdados-2.0.0b2/basedosdados/configs/templates/table/table_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/constants.py` & `basedosdados-2.0.0b2/basedosdados/constants.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/download/base.py` & `basedosdados-2.0.0b2/basedosdados/download/base.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/download/download.py` & `basedosdados-2.0.0b2/basedosdados/download/download.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/download/metadata.py` & `basedosdados-2.0.0b2/basedosdados/download/metadata.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/exceptions.py` & `basedosdados-2.0.0b2/basedosdados/exceptions.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/schemas/columns_schema.json` & `basedosdados-2.0.0b2/basedosdados/schemas/columns_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/schemas/dataset_schema.json` & `basedosdados-2.0.0b2/basedosdados/schemas/dataset_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/schemas/table_schema.json` & `basedosdados-2.0.0b2/basedosdados/schemas/table_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/upload/base.py` & `basedosdados-2.0.0b2/basedosdados/upload/base.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/upload/connection.py` & `basedosdados-2.0.0b2/basedosdados/upload/connection.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/upload/dataset.py` & `basedosdados-2.0.0b2/basedosdados/upload/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -115,23 +115,35 @@
                                 entity_type="iamMember",
                                 entity_id="allUsers",
                             ),
                         ]
                     )
                 dataset.access_entries = entries
             m["client"].update_dataset(dataset, ["access_entries"])
-
             logger.success(
                 " {object} {object_id}_{mode} was {action}!",
                 object_id=self.dataset_id,
                 mode=m["mode"],
                 object="Dataset",
                 action="publicized",
             )
 
+    def exists(self, mode="staging"):
+        """
+        Check if dataset exists.
+        """
+        ref_dataset_id = (
+            self.dataset_id if mode == "prod" else self.dataset_id + "_staging"
+        )
+        try:
+            ref = self.client[f"bigquery_{mode}"].get_dataset(ref_dataset_id)
+        except Exception:
+            ref = None
+        return bool(ref)
+
     def create(
         self, mode="all", if_exists="raise", dataset_is_public=True, location=None
     ):
         """Creates BigQuery datasets given `dataset_id`.
 
         It can create two datasets:
 
@@ -155,48 +167,46 @@
                 List of possible region names locations: https://cloud.google.com/bigquery/docs/locations
 
 
         Raises:
             Warning: Dataset already exists and if_exists is set to `raise`
         """
 
-        if if_exists == "replace":
-            self.delete(mode)
-        elif if_exists == "update":
-            self.update()
-            return
-
         # Set dataset_id to the ID of the dataset to create.
         for m in self._loop_modes(mode):
-            # Construct a full Dataset object to send to the API.
-            dataset_obj = self._setup_dataset_object(
-                dataset_id=m["id"], location=location, mode=m["mode"]
-            )
+            if if_exists == "replace":
+                self.delete(mode=m["mode"])
+            elif if_exists == "update":
+                self.update(mode=m["mode"])
+                continue
 
             # Send the dataset to the API for creation, with an explicit timeout.
             # Raises google.api_core.exceptions.Conflict if the Dataset already
             # exists within the project.
             try:
-                m["client"].create_dataset(dataset_obj)  # Make an API request.
-                logger.success(
-                    " {object} {object_id}_{mode} was {action}!",
-                    object_id=self.dataset_id,
-                    mode=m["mode"],
-                    object="Dataset",
-                    action="created",
-                )
-
+                if not self.exists(mode=m["mode"]):
+                    # Construct a full Dataset object to send to the API.
+                    dataset_obj = self._setup_dataset_object(
+                        dataset_id=m["id"], location=location, mode=m["mode"]
+                    )
+                    m["client"].create_dataset(dataset_obj)  # Make an API request.
+                    logger.success(
+                        " {object} {object_id}_{mode} was {action}!",
+                        object_id=self.dataset_id,
+                        mode=m["mode"],
+                        object="Dataset",
+                        action="created",
+                    )
+                    # Make prod dataset public
+                    self.publicize(dataset_is_public=dataset_is_public, mode=m["mode"])
             except Conflict as e:
                 if if_exists == "pass":
-                    return
+                    continue
                 raise Conflict(f"Dataset {self.dataset_id} already exists") from e
 
-        # Make prod dataset public
-        self.publicize(dataset_is_public=dataset_is_public)
-
     def delete(self, mode="all"):
         """Deletes dataset in BigQuery. Toogle mode to choose which dataset to delete.
 
         Args:
             mode (str): Optional.  Which dataset to delete [prod|staging|all]
         """
```

### Comparing `basedosdados-2.0.0b1/basedosdados/upload/datatypes.py` & `basedosdados-2.0.0b2/basedosdados/upload/datatypes.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/upload/storage.py` & `basedosdados-2.0.0b2/basedosdados/upload/storage.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/basedosdados/upload/table.py` & `basedosdados-2.0.0b2/basedosdados/upload/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,22 +30,19 @@
     """
 
     def __init__(self, dataset_id, table_id, **kwargs):
         super().__init__(**kwargs)
 
         self.table_id = table_id.replace("-", "_")
         self.dataset_id = dataset_id.replace("-", "_")
-        # self.dataset_folder = Path(self.metadata_path / self.dataset_id)
-        # self.table_folder = self.dataset_folder / table_id
         self.table_full_name = dict(
             prod=f"{self.client['bigquery_prod'].project}.{self.dataset_id}.{self.table_id}",
             staging=f"{self.client['bigquery_staging'].project}.{self.dataset_id}_staging.{self.table_id}",
         )
         self.table_full_name.update(dict(all=deepcopy(self.table_full_name)))
-        # self.metadata = Metadata(self.dataset_id, self.table_id, **kwargs)
 
     @property
     @lru_cache(256)
     def table_config(self):
         """
         Load table config
         """
@@ -71,49 +68,51 @@
 
         return bool(table_columns.get("partition_columns", []))
 
     def _load_schema_from_json(
         self,
         columns=None,
     ):
-        return [
+        schema = []
+
+        for col in columns:
             ## ref: https://cloud.google.com/python/docs/reference/bigquery/latest/google.cloud.bigquery.schema.SchemaField
-            SchemaField(
-                name=col.get("name"),
-                field_type=col.get("type"),
-                description=col.get("description", None),
+            if col.get("name") is None:
+                msg = "Columns must have a name! Check your data files for columns without name"
+                raise BaseDosDadosException(msg)
+
+            schema.append(
+                SchemaField(
+                    name=col.get("name"),
+                    field_type=col.get("type"),
+                    description=col.get("description", None),
+                )
             )
-            for col in columns
-        ]
+        return schema
 
     def _load_staging_schema_from_data(
         self, data_sample_path=None, source_format="csv"
     ):
         """
         Generate schema from columns metadata in data sample
         """
 
         if self.table_exists(mode="staging"):
             logger.warning(
                 " {object} {object_id} allready exists, replacing schema!",
                 object_id=self.table_id,
                 object="Table",
             )
-            # table_columns = [
-            #     {"name": c.name, "type": c.field_type}
-            #     for c in self._get_table_obj(mode="staging").schema
-            # ]
+
         table_columns = self._get_columns_from_data(
             data_sample_path=data_sample_path,
             source_format=source_format,
             mode="staging",
         )
-        # table_columns = table_columns.get("partition_columns") + table_columns.get(
-        #     "columns"
-        # )
+
         return self._load_schema_from_json(columns=table_columns.get("columns"))
 
     def _load_schema_from_bq(self, mode="staging"):
         """Load schema from table config
 
         Args:
             mode (bool): Which dataset to create [prod|staging].
@@ -180,41 +179,36 @@
                 ][0]
 
                 partition_columns = [
                     k.split("=")[0]
                     for k in data_sample_path.as_posix().split("/")
                     if "=" in k
                 ]
-
-            columns = Datatype(source_format).header(data_sample_path)
+            columns = Datatype(source_format=source_format).header(
+                data_sample_path=data_sample_path
+            )
 
         return {
             "columns": [{"name": col, "type": "STRING"} for col in columns],
             "partition_columns": [
                 {"name": col, "type": "STRING"} for col in partition_columns
             ],
         }
 
     def _get_columns_metadata_from_api(
         self,
     ):
         """
         Get columns and partition columns from API.
         """
-
-        columns = [
-            col
-            for col in self.table_config.get("columns")
-            if col.get("isPartition") is False
-        ]
+        table_columns = self.table_config.get("columns", {})
+        columns = [col for col in table_columns if col.get("isPartition", {}) is False]
 
         partition_columns = [
-            col
-            for col in self.table_config.get("columns")
-            if col.get("isPartition") is True
+            col for col in table_columns if col.get("isPartition", {}) is True
         ]
 
         return {
             "columns": [
                 {
                     "name": col.get("name"),
                     "type": col.get("bigqueryType").get("name"),
@@ -241,32 +235,39 @@
             return
         blobs = (
             self.client["storage_staging"]
             .bucket(self.bucket_name)
             .list_blobs(prefix=f"staging/{self.dataset_id}/{self.table_id}/")
         )
         partitions_dict = {}
+        ## only needs the first bloob
         for blob in blobs:
             for folder in blob.name.split("/"):
                 if "=" in folder:
                     key = folder.split("=")[0]
-                    value = folder.split("=")[1]
+                    value = folder.split("=")
                     try:
                         partitions_dict[key].append(value)
                     except KeyError:
                         partitions_dict[key] = [value]
-        return partitions_dict
+            return partitions_dict
 
     def _get_columns_from_bq(self, mode="staging"):
-        if mode == "staging" and self.table_exists(mode="staging"):
-            schema = self._get_table_obj(mode="staging").schema
-        if mode == "prod" and self.table_exists(mode="prod"):
-            schema = self._get_table_obj(mode="prod").schema
+        if not self.table_exists(mode=mode):
+            msg = f"Table {self.dataset_id}.{self.table_id} does not exist in {mode}, please create first!"
+            raise logger.error(msg)
+        else:
+            schema = self._get_table_obj(mode=mode).schema
+
+        partition_dict = self._parser_blobs_to_partition_dict()
 
-        partition_columns = list(self._parser_blobs_to_partition_dict().keys())
+        if partition_dict:
+            partition_columns = list(partition_dict.keys())
+        else:
+            partition_columns = []
 
         return {
             "columns": [
                 {
                     "name": col.name,
                     "type": col.field_type,
                     "description": col.description,
@@ -281,14 +282,29 @@
                     "description": col.description,
                 }
                 for col in schema
                 if col.name in partition_columns
             ],
         }
 
+    def _get_cross_columns_from_bq_api(self):
+        bq = self._get_columns_from_bq(mode="staging")
+        bq_columns = bq.get("partition_columns") + bq.get("columns")
+
+        api = self._get_columns_metadata_from_api()
+        api_columns = api.get("partition_columns") + api.get("columns")
+        if api_columns != []:
+            for bq_col in bq_columns:
+                for api_col in api_columns:
+                    if bq_col.get("name") == api_col.get("name"):
+                        bq_col["type"] = api_col.get("type")
+                        bq_col["description"] = api_col.get("description")
+
+        return bq_columns
+
     def _make_publish_sql(self):
         """Create publish.sql with columns and bigquery_type"""
 
         ### publish.sql header and instructions
         publish_txt = """
         /*
         Query para publicar a tabela.
@@ -306,16 +322,17 @@
         TIPOS:
             - Para modificar tipos de colunas, basta substituir STRING por outro tipo válido.
             - Exemplo: `SAFE_CAST(column_name AS NUMERIC) column_name`
             - Mais detalhes: https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types
         */
         """
 
-        table_columns = self._get_columns_from_bq(mode="staging")
-        columns = table_columns.get("partition_columns") + table_columns.get("columns")
+        # table_columns = self._get_columns_from_api(mode="staging")
+
+        columns = self._get_cross_columns_from_bq_api()
 
         # remove triple quotes extra space
         publish_txt = inspect.cleandoc(publish_txt)
         publish_txt = textwrap.dedent(publish_txt)
 
         # add create table statement
         project_id_prod = self.client["bigquery_prod"].project
@@ -640,15 +657,17 @@
 
         table = self._get_table_obj(mode)
 
         table.description = self._get_table_description()
 
         # when mode is staging the table schema already exists
         if mode == "prod" and custom_schema is None:
-            table.schema = self._load_schema_from_bq()
+            table.schema = self._load_schema_from_json(
+                columns=self._get_cross_columns_from_bq_api()
+            )
         if mode == "prod" and custom_schema is not None:
             table.schema = self._load_schema_from_json(custom_schema)
 
         fields = ["description", "schema"]
 
         self.client[f"bigquery_prod"].update_table(table, fields=fields)
 
@@ -684,20 +703,21 @@
 
             * Check if all required fields are filled
         """
         # TODO: review this method
 
         if if_exists == "replace" and self.table_exists(mode="prod"):
             self.delete(mode="prod")
+
         publish_sql = self._make_publish_sql()
 
         ## create view using API metadata
         if custon_publish_sql is None:
             self.client["bigquery_prod"].query(publish_sql).result()
-            self.update()
+            self.update(mode="prod")
 
         ## create view using custon query
         if custon_publish_sql is not None:
             self.client["bigquery_prod"].query(custon_publish_sql).result()
             ## update schema using a custom schema
             if custom_schema is not None:
                 self.update(custom_schema=custom_schema)
```

### Comparing `basedosdados-2.0.0b1/basedosdados/upload/utils.py` & `basedosdados-2.0.0b2/basedosdados/upload/utils.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b1/pyproject.toml` & `basedosdados-2.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 license = "MIT"
 name = "basedosdados"
 packages = [
   {include = "basedosdados"},
 ]
 readme = "README.md"
 repository = "https://github.com/base-dos-dados/bases"
-version = "2.0.0-beta.1"
+version = "2.0.0-beta.2"
 
 [tool.poetry.scripts]
 basedosdados = 'basedosdados.cli.cli:cli'
 
 [tool.poetry.dependencies]
 google-api-python-client = "^2.86.0"
 google-cloud-bigquery = "^3.10.0"
@@ -27,15 +27,17 @@
 gql = "^3.4.1"
 loguru = "^0.7.0"
 pandas = "^2.0.1"
 pandas-gbq = "^0.19.2"
 pandavro = "^1.7.2"
 pydata-google-auth = "^1.8.0"
 python = ">=3.8, <3.11"
+requests-toolbelt = "^1.0.0"
 tqdm = "^4.65.0"
+tomlkit = "^0.11.8"
 
 [tool.black]
 # Use the more relaxed max line length permitted in PEP8.
 exclude = '''
 /(
     \.eggs
   | \.git
```

### Comparing `basedosdados-2.0.0b1/PKG-INFO` & `basedosdados-2.0.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basedosdados
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Organizar e facilitar o acesso a dados brasileiros através de tabelas públicas no BigQuery.
 Home-page: https://github.com/base-dos-dados/bases
 License: MIT
 Author: Joao Carabetta
 Author-email: joao.carabetta@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
 Requires-Dist: gql (>=3.4.1,<4.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pandas-gbq (>=0.19.2,<0.20.0)
 Requires-Dist: pandavro (>=1.7.2,<2.0.0)
 Requires-Dist: pydata-google-auth (>=1.8.0,<2.0.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
+Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/base-dos-dados/bases
 Description-Content-Type: text/markdown
 
 # Python Package
 
 ## Desenvolvimento Linux e Mac:
```

